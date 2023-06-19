# Comparing `tmp/pyload-ng-0.5.0b3.dev71.tar.gz` & `tmp/pyload-ng-0.5.0b3.dev72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyload-ng-0.5.0b3.dev71.tar", last modified: Mon May 22 19:53:33 2023, max compression
+gzip compressed data, was "pyload-ng-0.5.0b3.dev72.tar", last modified: Mon Jun 19 08:45:02 2023, max compression
```

## Comparing `pyload-ng-0.5.0b3.dev71.tar` & `pyload-ng-0.5.0b3.dev72.tar`

### file list

```diff
@@ -1,865 +1,861 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.151840 pyload-ng-0.5.0b3.dev71/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-05-22 19:53:33.151840 pyload-ng-0.5.0b3.dev71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/babel_v2.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/babel_v3.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/poetry.toml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-22 19:53:33.151840 pyload-ng-0.5.0b3.dev71/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/core/
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/core/api/
--rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/config/default.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/config/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/core/database/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14019 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/database/file_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/database/storage_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/database/user_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/pyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/pypackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/log_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/addon_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/captcha_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19441 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18965 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/thread_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/cookie_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/http_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/http_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/request_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.091839 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/xdcc/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/xdcc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/network/xdcc/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.095839 pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/addon_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/clicknload_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/database_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/decrypter_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/download_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/info_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/plugin_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.095839 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.095839 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/old/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/old/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/old/packagetools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/purge.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/seconds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.095839 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.095839 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/purge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.095839 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.103839 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/AccioDebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/AlldebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/AniStreamCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/ArchiveOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/BackinNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/CloudsharesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/CloudsixMe.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/CloudzillaTo.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/CramitIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/CzshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DatoidCz.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DdownloadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DebridItaliaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DebridlinkFr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DebridplanetCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DepositfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DownsterNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/EasybytezCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/EuroshareEu.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/ExashareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/ExtmatrixCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FastixRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FastshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/File4SafeCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FileStoreTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FileboomMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilecloudIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilefactoryCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilejokerNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FileomCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilerNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilerioCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilesMailRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FourSharedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FshareVn.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/Ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/GetTwentyFourOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/HellshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/HighWayMe.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/Http.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/HugefilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/HundredEightyUploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/IronfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/JunkyvideoCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/JunocloudMe.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/KatfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/Keep2ShareCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/LinkifierCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/LinksnappyCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegaCoNz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegaDebridEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegaRapidCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegaRapidoNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegasharesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MovReelCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MultihostersCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MultishareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MyfastfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NitrobitNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NitroflareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NoPremiumPl.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NosuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NovafileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NowVideoSx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/OneFichierCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/OpenloadCo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/OverLoadMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/PorntrexCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/PremiumTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/PremiumizeMe.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/PutdriveCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/QuickshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RPNetBiz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RapideoPl.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RapidfileshareNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RapidgatorNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RapiduNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RarefileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RealdebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RehostTo.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SafesharingEu.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SecureUploadEu.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SendmywayCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SharebeastCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SimplyPremiumCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SimplydebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SmoozedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/StreamcloudEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TbSevenPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TenluaVn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TurbobitNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TusfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TwojlimitPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UlozTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UpleaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UploadcCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UploadgigCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UploadheroCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UpstoreNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UptoboxCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/VidPlayNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/WebshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/WorldbytezCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/WrzucajplikiPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/YibaishiwuCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/ZeveraCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.107839 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AndroidPhoneNotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AntiCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AntiStandby.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AntiVirus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AppriseNotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/BypassCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/Captcha9Kw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/Checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ClickNLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/CloudFlareDdos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/DeathByCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/DeleteFinished.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/DiscordNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/DownloadScheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ExpertDecoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ExternalScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ExtractArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/HotFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/IRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ImageTyperz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/JustPremium.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/LinkFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/LogMarker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/MergeFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/MultiHome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/PushBullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/PushOver.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/RestartFailed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/SkipRev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/TORRENT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/TransmissionRPC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/UnSkipOnFail.py
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/UpdateManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/UserAgentSwitcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/WindowsPhoneNotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/XFileSharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/XMPP.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.107839 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/
--rw-r--r--   0 runner    (1001) docker     (123)    30497 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/CircleCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/CoinHive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/HCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)    17858 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/ReCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/SolveMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/UlozTo.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.107839 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/captcha_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/chat_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/dead_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/dead_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/hoster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/multi_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/multi_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/multi_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/simple_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/simple_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/xfs_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/xfs_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/xfs_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.107839 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/CCF.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/DLC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/RSDF.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/TORRENT.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/TXT.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.115839 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/AlldebridComTorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/ArchiveOrgFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/ChipDe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CloudMailRuFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CloudzillaToFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CriptTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CryptCat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CzshareComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DailymotionComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DataHuFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DepositfilesComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/Dereferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DevhostStFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DlProtectCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/EasybytezComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/EmbeduploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilecloudIoFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilecryptCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilefactoryComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilerNetFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilestubeCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FiletramCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FourChanOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FreakhareComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FreetexthostCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FshareVnFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FurLy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/Go4UpCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/GofileIoFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/GooGl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/GoogledriveComDereferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/GoogledriveComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/HearthisAtFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/HflixIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/HoerbuchIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/ImgurCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/JDlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/LixIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MediafireComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MegaCoNzFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MegaRapidCzFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MegadyskPlFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MirrorcreatorCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MultiUpOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MultiloadCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/NitroflareComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/NosvideoCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/PastebinCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/PastedCo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/QuickshareCzFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/RealdebridComTorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/SafelinkingNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/SexuriaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/ShSt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TenluaVnFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TinyurlCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TnyCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TurbobitNetFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TusfilesNetFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/UlozToFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/XFileSharingFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/XupPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/YoutubeComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.127839 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AccioDebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AlfafileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AlldebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AndroidfilehostCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AnonfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ArchiveOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/BasketbuildCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/BayfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/BezvadataCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ClicknuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CloudMailRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CloudzillaTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CosmoboxOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CramitIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CzshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DailymotionCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DailyuploadsNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DataHu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DataportCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DatoidCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DdownloadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DebridItaliaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DebridlinkFr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DebridplanetCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DefaultPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DepositfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DevhostSt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DlFreeFr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DownsterNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DropDownload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DropboxCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/EasybytezCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/EasyuploadIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/EdiskCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/EuroshareEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ExashareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ExtmatrixCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FastixRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FastshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FikperCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileAl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileSharkPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileStoreTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileboomMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilecloudIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FiledropperCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilefactoryCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilefoxCc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilejokerNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileomCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilepupNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilerNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilerioCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilesMailRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileuploadNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FiregetCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FistfastNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FlyFilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FourSharedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FshareVn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/Ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GamefrontCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GetTwentyFourOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GigapetaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GofileIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GooIm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GoogledriveCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HearthisAt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HellshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HighWayMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HitfileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HostujeNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HotlinkCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/Http.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HugefilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HundredEightyUploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/IfolderRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/IronfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/JumbofilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/JunocloudMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/KatfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/Keep2ShareCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/KingfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/KrakenfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LetsuploadCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LetsuploadCo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LibgenIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LinkifierCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LinksnappyCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LinksnappyComTorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LoadTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MediafireCom.py
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaCoNz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaDebridEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaRapidCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaRapidoNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegacrypterCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegadyskPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegasharesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaupNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MovReelCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MultihostersCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MultishareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MyfastfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MystoreTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NarodRu.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NippyshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NitrobitNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NitroflareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NoPremiumPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NofileIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NosuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NovafileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NowVideoSx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/OneFichierCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/OnlineTvRecorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/OpenloadIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/OverLoadMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PixeldrainCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PornhostCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PornhubCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PornovkaCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PorntrexCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PremiumTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PremiumizeMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PromptfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PutdriveCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/QuickshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RPNetBiz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RapideoPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RapidfileshareNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RapidgatorNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RapiduNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RarefileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RealdebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RedtubeCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RehostTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RemixshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RgHostNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SafesharingEu.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SecureUploadEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SenditCloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SendspaceCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/Share4WebCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ShareplaceCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SimplyPremiumCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SimplydebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SizedriveCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SmoozedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SmuleCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SolidfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SoundcloudCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SpeedyshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/StreamCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/StreamcloudEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SuprafilesMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TbSevenPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TenluaVn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TurbobitNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TusfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TwoSharedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TwojlimitPl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UlozTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UloziskoSk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UnibytesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UpfileVn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UpleaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UploadgigCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UploadheroCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UploadrocketNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UploadshipCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UpstoreNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UptoboxCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UserscloudCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UseruploadNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VeehdCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VeohCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VidPlayNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VimeoCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VkCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/WebshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/WetransferCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/WrzucTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/WrzucajplikiPl.py
--rw-r--r--   0 runner    (1001) docker     (123)    36323 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XDCC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XFileSharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XHamsterCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XVideosCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XdadevelopersCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YadiSk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YesPornPleaseCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YibaishiwuCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YoupornCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YourfilesTo.py
--rw-r--r--   0 runner    (1001) docker     (123)    55150 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YoutubeCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ZDF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ZbigzCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ZeveraCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ZippyshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.131840 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/HjSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/SevenZip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/UnRar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/UnTar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/UnZip.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/plugins/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.131840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.131840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.131840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/api_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/app_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/cnl_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/json_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.131840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/css/logs.css
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/css/pathchooser.css
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/css/window.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.135840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/add_folder.png
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/arrow-refresh.png
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/button.png
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/cog.png
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-add-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-add.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-cancel-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-cancel.png
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-pause-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-pause.png
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-play-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-play.png
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-stop-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-stop.png
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/dialog-close.png
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/dialog-question.png
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/error.png
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/folder.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-bg.png
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-login.png
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-collector.png
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-config.png
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-development.png
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-download.png
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-home.png
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-index.png
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-news.png
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-queue.png
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-recent.png
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-wiki.png
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-search-noshadow.png
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/images.png
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/notice.png
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/package-go.png
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/page-tools-backlinks.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/page-tools-edit.png
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/page-tools-revisions.png
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/parse-uri.png
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/pencil.png
--rw-r--r--   0 runner    (1001) docker     (123)    39315 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/pyload-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/reconnect.png
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-downloading.png
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-failed.png
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-finished.png
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-none.png
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-offline.png
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-proc.png
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-queue.png
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-waiting.png
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/success.png
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/tab-background.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/tabs-border-bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/user-actions-logout.png
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/user-actions-profile.png
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/user-info.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.135840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/js/captcha-interactive.user.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.135840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.135840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Error.js
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.135840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.135840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css
--rw-r--r--   0 runner    (1001) docker     (123)    89614 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   251703 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/Purr/
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/TinyTab/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/captcha.html
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/filemanager.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/folder.html
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/base.js
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/filemanager.js
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/info.js
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/packages.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/pathchooser.js
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/pathchooser.html
--rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/settings_item.html
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/window.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/dashboard.css
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/info.css
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/login.css
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/logout.css
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/logs.css
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/pathchooser.css
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/settings.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   117150 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    35452 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.139840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    73908 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    86659 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/captcha.html
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/base.js
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/info.js
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/packages.js
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/pathchooser.html
--rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/settings_item.html
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/window.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/dashboard.css
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/info.css
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/login.css
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/logout.css
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/logs.css
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/settings.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.143840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   117202 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    35452 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    73908 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    86659 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.087839 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/captcha.html
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/base.js
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/info.js
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/packages.js
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/settings_item.html
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/window.html
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/src/pyload/webui/webserver_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.147840 pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-05-22 19:53:33.000000 pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37100 2023-05-22 19:53:33.000000 pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:53:33.000000 pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-22 19:53:33.000000 pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:53:33.000000 pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-22 19:53:33.000000 pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 19:53:33.000000 pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:53:33.151840 pyload-ng-0.5.0b3.dev71/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/tests/api_exerciser.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/tests/system_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 19:53:29.000000 pyload-ng-0.5.0b3.dev71/tests/test_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.279785 pyload-ng-0.5.0b3.dev72/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-06-19 08:45:02.279785 pyload-ng-0.5.0b3.dev72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/babel_v2.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/babel_v3.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/poetry.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-19 08:45:02.279785 pyload-ng-0.5.0b3.dev72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/core/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/config/default.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/config/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/core/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14019 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/database/file_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/database/storage_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/database/user_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/pyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/pypackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/log_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/addon_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/captcha_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19441 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18965 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/thread_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/cookie_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/http_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/http_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/request_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/xdcc/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/xdcc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/network/xdcc/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/addon_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/clicknload_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/database_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/decrypter_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/download_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/info_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/plugin_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/old/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/old/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/old/packagetools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/purge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/seconds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/purge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.223784 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.231784 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/AccioDebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/AlldebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/AniStreamCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/ArchiveOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/BackinNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/CloudsharesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/CloudsixMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/CloudzillaTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/CramitIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/CzshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DatoidCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DdownloadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DebridItaliaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DebridlinkFr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DebridplanetCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DepositfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DownsterNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/EasybytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/EuroshareEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/ExashareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/ExtmatrixCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FastixRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FastshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/File4SafeCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FileStoreTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FileboomMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilecloudIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilefactoryCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilejokerNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FileomCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilerNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilerioCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilesMailRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FiregetCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FourSharedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FshareVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/Ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/GetTwentyFourOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/HellshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/HighWayMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/Http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/HugefilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/HundredEightyUploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/IronfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/JunkyvideoCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/JunocloudMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/KatfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/Keep2ShareCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/LinkifierCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/LinksnappyCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegaCoNz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegaDebridEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegaRapidCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegaRapidoNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegasharesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MovReelCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MultihostersCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MultishareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MyfastfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NitrobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NitroflareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NoPremiumPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NosuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NovafileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NowVideoSx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/OneFichierCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/OverLoadMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/PorntrexCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/PremiumTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/PremiumizeMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/PutdriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/QuickshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RPNetBiz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RapideoPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RapidfileshareNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RapidgatorNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RapiduNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RarefileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RealdebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RehostTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SafesharingEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SecureUploadEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SendmywayCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SharebeastCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SimplyPremiumCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SimplydebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SmoozedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/StreamcloudEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TbSevenPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TenluaVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TurbobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TusfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TwojlimitPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UlozTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UpleaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UploadcCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UploadgigCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UpstoreNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UptoboxCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/VidPlayNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/WebshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/WorldbytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/WrzucajplikiPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/YibaishiwuCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/ZeveraCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.235784 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AndroidPhoneNotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AntiCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AntiStandby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AntiVirus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AppriseNotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/BypassCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/Captcha9Kw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/Checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ClickNLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/CloudFlareDdos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/DeathByCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/DeleteFinished.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/DiscordNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/DownloadScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ExpertDecoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ExternalScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ExtractArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/HotFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/IRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ImageTyperz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/JustPremium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/LinkFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/LogMarker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/MergeFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/MultiHome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/PushBullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/PushOver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/RestartFailed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/SkipRev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/TORRENT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/TransmissionRPC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/UnSkipOnFail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/UpdateManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/UserAgentSwitcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/WindowsPhoneNotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/XFileSharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/XMPP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.235784 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/
+-rw-r--r--   0 runner    (1001) docker     (123)    30497 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/CircleCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/CoinHive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/HCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17858 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/ReCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/SolveMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/UlozTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.239784 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/captcha_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/chat_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/dead_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/dead_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/hoster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/multi_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/multi_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/multi_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/simple_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/simple_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/xfs_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/xfs_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/xfs_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.239784 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/CCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/DLC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/RSDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/TORRENT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/TXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.243784 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/AlldebridComTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/ArchiveOrgFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/ChipDe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/CloudMailRuFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/CloudzillaToFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/CriptTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/CzshareComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DailymotionComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DataHuFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DepositfilesComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/Dereferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DevhostStFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/EasybytezComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/EmbeduploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilecloudIoFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilecryptCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilefactoryComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilerNetFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilestubeCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FiletramCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FourChanOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FreakhareComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FreetexthostCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FshareVnFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FurLy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/Go4UpCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/GofileIoFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/GooGl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/GoogledriveComDereferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/GoogledriveComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/HearthisAtFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/HflixIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/HoerbuchIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/ImgurCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/JDlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/LixIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MediafireComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MegaCoNzFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MegaRapidCzFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MegadyskPlFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MirrorcreatorCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MultiUpOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MultiloadCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/NitroflareComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/NosvideoCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/PastebinCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/PastedCo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/QuickshareCzFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/RealdebridComTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/SafelinkingNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/SexuriaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/ShSt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TenluaVnFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TinyurlCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TnyCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TurbobitNetFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TusfilesNetFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/UlozToFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/WetransferComDereferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/XFileSharingFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/XupPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/YoutubeComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.259784 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AccioDebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AlfafileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AlldebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AndroidfilehostCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AnonfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ArchiveOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/BasketbuildCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/BayfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/BezvadataCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ClicknuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CloudMailRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CloudzillaTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CosmoboxOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CramitIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CzshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DailymotionCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DailyuploadsNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DataHu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DataportCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DatoidCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DdownloadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DebridItaliaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DebridlinkFr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DebridplanetCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DefaultPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DepositfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DevhostSt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DlFreeFr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DownsterNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DropDownload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DropboxCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/EasybytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/EasyuploadIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/EdiskCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/EuroshareEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ExashareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ExtmatrixCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FastixRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FastshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FikperCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileAl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileSharkPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileStoreTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileboomMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilecloudIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilefactoryCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilefoxCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilejokerNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileomCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilepupNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilerNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilericeCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilerioCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilesMailRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileuploadNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FiregetCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FistfastNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FlyFilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FourSharedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FshareVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/Ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GamefrontCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GetTwentyFourOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GigapetaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GofileIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GooIm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GoogledriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HearthisAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HellshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HighWayMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HitfileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HostujeNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HotlinkCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/Http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HugefilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HundredEightyUploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/IfolderRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/IronfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/JumbofilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/JunocloudMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/KatfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/Keep2ShareCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/KingfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/KrakenfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LetsuploadCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LetsuploadCo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LibgenIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LinkifierCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LinksnappyCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LinksnappyComTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LoadTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MediafireCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaCoNz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaDebridEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaRapidCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaRapidoNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegacrypterCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegadyskPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegasharesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaupNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MexaSh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MovReelCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MultihostersCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MultishareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MyfastfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MystoreTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NarodRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NippyshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NitrobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NitroflareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NoPremiumPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NofileIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NosuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NovafileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NowVideoSx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/OneFichierCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/OnlineTvRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/OverLoadMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PixeldrainCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PornhostCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PornhubCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PornovkaCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PorntrexCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PremiumTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PremiumizeMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PromptfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PutdriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/QuickshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RPNetBiz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RapideoPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RapidfileshareNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RapidgatorNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RapiduNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RarefileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RealdebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RedtubeCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RehostTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RemixshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RgHostNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SafesharingEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SecureUploadEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SenditCloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SendspaceCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/Share4WebCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ShareplaceCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SimplyPremiumCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SimplydebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SizedriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SmoozedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SmuleCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SolidfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SoundcloudCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SpeedyshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/StreamCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/StreamcloudEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SuprafilesMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TbSevenPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TenluaVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TurbobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TusfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TwoSharedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TwojlimitPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UlozTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UloziskoSk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UnibytesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UpfileVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UpleaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UploadgigCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UploadrocketNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UploadshipCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UpstoreNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UptoboxCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UserscloudCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UseruploadNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VeehdCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VeohCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VidPlayNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VimeoCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VkCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/WebshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/WetransferCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/WrzucTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/WrzucajplikiPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36323 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XDCC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XFileSharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XHamsterCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XVideosCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XdadevelopersCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YadiSk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YesPornPleaseCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YibaishiwuCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YoupornCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YourfilesTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55150 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YoutubeCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ZDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ZbigzCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ZeveraCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.259784 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/HjSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/SevenZip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/UnRar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/UnTar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/UnZip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/plugins/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.259784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.259784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.259784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/api_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/app_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/cnl_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/json_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.215784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.259784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/css/logs.css
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/css/pathchooser.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/css/window.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.263784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/add_folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/arrow-refresh.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/button.png
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/cog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-add-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-add.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-cancel-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-cancel.png
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-pause-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-pause.png
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-play-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-play.png
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-stop-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-stop.png
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/dialog-close.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/dialog-question.png
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-bg.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-login.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-collector.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-config.png
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-development.png
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-download.png
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-home.png
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-index.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-news.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-queue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-recent.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-wiki.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-search-noshadow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/images.png
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/notice.png
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/package-go.png
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/page-tools-backlinks.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/page-tools-edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/page-tools-revisions.png
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/parse-uri.png
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/pencil.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39315 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/pyload-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/reconnect.png
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-downloading.png
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-failed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-finished.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-none.png
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-offline.png
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-proc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-queue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-waiting.png
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/success.png
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/tab-background.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/tabs-border-bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/user-actions-logout.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/user-actions-profile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/user-info.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.263784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/js/captcha-interactive.user.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.215784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.263784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.263784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Error.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.263784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css
+-rw-r--r--   0 runner    (1001) docker     (123)    89614 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   251703 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/Purr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/TinyTab/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/captcha.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/filemanager.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/folder.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/filemanager.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/info.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/packages.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/pathchooser.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/pathchooser.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/settings_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/window.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.215784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/info.css
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/login.css
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/logout.css
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/logs.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/pathchooser.css
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/settings.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.215784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.215784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   117150 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.267784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    35452 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    73908 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86659 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/captcha.html
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/info.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/packages.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/pathchooser.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/settings_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/window.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/info.css
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/login.css
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/logout.css
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/logs.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/settings.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.271784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   117202 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    35452 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    73908 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86659 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.219784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/captcha.html
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/info.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/packages.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/settings_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/window.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/src/pyload/webui/webserver_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.275784 pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-06-19 08:45:02.000000 pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-06-19 08:45:02.000000 pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:45:02.000000 pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 08:45:02.000000 pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:45:02.000000 pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-19 08:45:02.000000 pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 08:45:02.000000 pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:45:02.279785 pyload-ng-0.5.0b3.dev72/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/tests/api_exerciser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/tests/system_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-19 08:44:58.000000 pyload-ng-0.5.0b3.dev72/tests/test_skeleton.py
```

### Comparing `pyload-ng-0.5.0b3.dev71/AUTHORS.md` & `pyload-ng-0.5.0b3.dev72/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/CODE_OF_CONDUCT.md` & `pyload-ng-0.5.0b3.dev72/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/CONTRIBUTING.md` & `pyload-ng-0.5.0b3.dev72/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/LICENSE.md` & `pyload-ng-0.5.0b3.dev72/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/PKG-INFO` & `pyload-ng-0.5.0b3.dev72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyload-ng
-Version: 0.5.0b3.dev71
+Version: 0.5.0b3.dev72
 Summary: The free and open-source Download Manager written in pure Python
 Home-page: https://pyload.net
 Download-URL: https://github.com/pyload/pyload/releases
 Author: pyLoad team
 Author-email: support@pyload.net
 Maintainer: Walter Purcaro
 Maintainer-email: vuolter@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyload-ng Version: 0.5.0b3.dev71 Summary: The free
+Metadata-Version: 2.1 Name: pyload-ng Version: 0.5.0b3.dev72 Summary: The free
 and open-source Download Manager written in pure Python Home-page: https://
 pyload.net Download-URL: https://github.com/pyload/pyload/releases Author:
 pyLoad team Author-email: support@pyload.net Maintainer: Walter Purcaro
 Maintainer-email: vuolter@gmail.com License: agpl3 Project-URL: Source Code
 (mirror), https://gitlab.com/pyload/pyload Project-URL: Source Code, https://
 github.com/pyload/pyload Project-URL: Bug Tracker, https://github.com/pyload/
 pyload/issues Project-URL: Documentation, https://github.com/pyload/pyload/wiki
```

### Comparing `pyload-ng-0.5.0b3.dev71/README.md` & `pyload-ng-0.5.0b3.dev72/README.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/SECURITY.md` & `pyload-ng-0.5.0b3.dev72/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/pyproject.toml` & `pyload-ng-0.5.0b3.dev72/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/setup.cfg` & `pyload-ng-0.5.0b3.dev72/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/setup.py` & `pyload-ng-0.5.0b3.dev72/setup.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/__init__.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/__main__.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/__main__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/__init__.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/api/__init__.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/config/default.cfg` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/config/default.cfg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/config/parser.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/config/parser.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/database/__init__.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/database/file_database.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/database/file_database.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/database/storage_database.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/database/storage_database.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/database/user_database.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/database/user_database.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/data.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/data.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/enums.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/enums.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/exceptions.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/pyfile.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/pyfile.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/datatypes/pypackage.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/datatypes/pypackage.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/log_factory.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/log_factory.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/account_manager.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/account_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/addon_manager.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/addon_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/captcha_manager.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/captcha_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/event_manager.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/event_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/file_manager.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/file_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/plugin_manager.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/managers/thread_manager.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/managers/thread_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/network/browser.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/network/browser.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/network/bucket.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/network/bucket.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/network/cookie_jar.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/network/cookie_jar.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/exceptions.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/http_chunk.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/http_chunk.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/http_download.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/http_download.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/network/http/http_request.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/network/http/http_request.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/network/request_factory.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/network/request_factory.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/network/xdcc/request.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/network/xdcc/request.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/scheduler.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/addon_thread.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/addon_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/clicknload_thread.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/clicknload_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/database_thread.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/database_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/decrypter_thread.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/decrypter_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/download_thread.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/download_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/info_thread.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/info_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/threads/plugin_thread.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/threads/plugin_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/check.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/check.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/convert.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/debug.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/debug.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/format.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/format.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/fs.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/misc.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/old/__init__.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/old/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/old/packagetools.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/old/packagetools.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/parse.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/parse.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/purge.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/purge.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/seconds.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/seconds.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/base.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/base.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/info.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/info.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/lock.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/lock.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/struct/style.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/struct/style.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/system.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/system.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/check.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/check.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/convert.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/convert.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/format.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/format.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/parse.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/parse.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/core/utils/web/purge.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/core/utils/web/purge.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/AccioDebridCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/AccioDebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/AlldebridCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/AlldebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/ArchiveOrg.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/ArchiveOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/CloudzillaTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/CloudzillaTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/CzshareCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/CzshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DatoidCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DatoidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DdownloadCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DdownloadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DebridItaliaCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DebridItaliaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DebridlinkFr.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DebridlinkFr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DebridplanetCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DebridplanetCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DepositfilesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DepositfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/DownsterNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/DownsterNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/EuroshareEu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/EuroshareEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/ExtmatrixCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/ExtmatrixCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FastixRu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FastixRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FastshareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FastshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FileStoreTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FileStoreTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FileboomMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FileboomMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilecloudIo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilecloudIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilefactoryCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilefactoryCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilejokerNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilejokerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilerNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FilesMailRu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FilesMailRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FourSharedCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FourSharedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/FshareVn.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/FshareVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/GetTwentyFourOrg.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/GetTwentyFourOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/HellshareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/HellshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/HighWayMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/HighWayMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/IronfilesNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/IronfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/KatfileCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/KatfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/Keep2ShareCc.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/Keep2ShareCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/LinkifierCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/LinkifierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/LinksnappyCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/LinksnappyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegaCoNz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegaCoNz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegaDebridEu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegaDebridEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegaRapidCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegaRapidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegaRapidoNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegaRapidoNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MegasharesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MegasharesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MultishareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MultishareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/MyfastfileCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/MyfastfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NitrobitNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NitrobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NitroflareCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NitroflareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NoPremiumPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NoPremiumPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/NowVideoSx.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/NowVideoSx.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/OneFichierCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/OneFichierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/OverLoadMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/OverLoadMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/PorntrexCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/PorntrexCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/PremiumTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/PremiumTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/PremiumizeMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/PremiumizeMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/QuickshareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/QuickshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RPNetBiz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RPNetBiz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RapideoPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RapideoPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RapidfileshareNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RapidfileshareNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RapidgatorNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RapidgatorNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RapiduNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RapiduNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RealdebridCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RealdebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/RehostTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/RehostTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SimplyPremiumCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SimplyPremiumCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SimplydebridCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SimplydebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/SmoozedCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/SmoozedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TbSevenPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TbSevenPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TenluaVn.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TenluaVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TurbobitNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TurbobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TusfilesNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TusfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/TwojlimitPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/TwojlimitPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UlozTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UlozTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UpleaCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UpleaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UploadgigCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UploadgigCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UpstoreNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UpstoreNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/UptoboxCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/UptoboxCom.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 from ..base.xfs_account import XFSAccount
 
 
 class UptoboxCom(XFSAccount):
     __name__ = "UptoboxCom"
     __type__ = "account"
-    __version__ = "0.25"
+    __version__ = "0.26"
     __status__ = "testing"
 
     __description__ = """Uptobox.com account plugin"""
     __license__ = "GPLv3"
     __authors__ = [
         ("benbox69", "dev@tollet.me"),
         ("GammaC0de", "nitzo2001[AT]yahoo[DOT]com"),
     ]
 
-    PLUGIN_DOMAIN = "uptobox.com"
+    PLUGIN_DOMAIN = "uptobox.eu"
 
-    LOGIN_URL = "https://uptobox.com/login"
-    LOGIN_SKIP_PATTERN = r"https://uptobox\.com/logout"
+    LOGIN_URL = "https://uptobox.eu/login"
+    LOGIN_SKIP_PATTERN = r"https://uptobox\.eu/logout"
 
     PREMIUM_PATTERN = r"Premium member"
 
     VALID_UNTIL_PATTERN = r"class='expiration-date .+?'>(\d{1,2} [\w^_]+ \d{4})"
 
     def signin(self, user, password, data):
         html = self.load(self.LOGIN_URL, cookies=self.COOKIES)
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/WebshareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/WebshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/WrzucajplikiPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/WrzucajplikiPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/YibaishiwuCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/YibaishiwuCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/accounts/ZeveraCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/accounts/ZeveraCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AndroidPhoneNotify.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AndroidPhoneNotify.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AntiCaptcha.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AntiCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AntiStandby.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AntiStandby.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AntiVirus.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AntiVirus.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/AppriseNotify.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/AppriseNotify.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/BypassCaptcha.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/BypassCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/Captcha9Kw.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/Captcha9Kw.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/Checksum.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/Checksum.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ClickNLoad.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ClickNLoad.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/CloudFlareDdos.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/CloudFlareDdos.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/DeathByCaptcha.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/DeathByCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/DeleteFinished.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/DeleteFinished.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/DiscordNotifier.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/DiscordNotifier.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/DownloadScheduler.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/DownloadScheduler.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ExpertDecoders.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ExpertDecoders.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ExternalScripts.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ExternalScripts.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ExtractArchive.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ExtractArchive.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/HotFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/HotFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/IRC.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/IRC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/ImageTyperz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/ImageTyperz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/JustPremium.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/JustPremium.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/LinkFilter.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/LinkFilter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/LogMarker.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/LogMarker.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/MergeFiles.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/MergeFiles.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/MultiHome.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/MultiHome.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/PushBullet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/PushBullet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/PushOver.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/PushOver.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/RestartFailed.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/RestartFailed.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/SkipRev.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/SkipRev.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/TORRENT.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/TORRENT.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/TransmissionRPC.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/TransmissionRPC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/UnSkipOnFail.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/UnSkipOnFail.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/UpdateManager.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/UpdateManager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/UserAgentSwitcher.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/UserAgentSwitcher.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/WindowsPhoneNotify.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/WindowsPhoneNotify.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/XFileSharing.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/XFileSharing.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/addons/XMPP.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/addons/XMPP.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/CircleCaptcha.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/CircleCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/CoinHive.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/CoinHive.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/HCaptcha.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/HCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/ReCaptcha.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/ReCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/SolveMedia.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/SolveMedia.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/anticaptchas/UlozTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/anticaptchas/UlozTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/account.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/account.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/addon.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/addon.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/captcha.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/captcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/captcha_service.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/captcha_service.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/chat_bot.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/chat_bot.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/container.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/container.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/dead_decrypter.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/dead_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/dead_downloader.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/dead_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/decrypter.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/downloader.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/extractor.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/extractor.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/hoster.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/hoster.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/multi_account.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/multi_account.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/multi_decrypter.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/multi_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/multi_downloader.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/multi_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/notifier.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/notifier.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/ocr.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/ocr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/plugin.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/plugin.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/simple_decrypter.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/simple_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/simple_downloader.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/simple_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/xfs_account.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/xfs_account.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/xfs_decrypter.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/xfs_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/base/xfs_downloader.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/base/xfs_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/CCF.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/CCF.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/DLC.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/DLC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/RSDF.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/RSDF.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/TORRENT.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/TORRENT.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/containers/TXT.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/containers/TXT.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/AlldebridComTorrent.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/AlldebridComTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/ArchiveOrgFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/ArchiveOrgFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/ChipDe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/ChipDe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CloudMailRuFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/CloudMailRuFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CloudzillaToFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/CloudzillaToFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CriptTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/CriptTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CryptCat.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DataHuFolder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,48 @@
 # -*- coding: utf-8 -*-
-import re
+
 
 from ..base.simple_decrypter import SimpleDecrypter
 
 
-class CryptCat(SimpleDecrypter):
-    __name__ = "CryptCat"
+class DataHuFolder(SimpleDecrypter):
+    __name__ = "DataHuFolder"
     __type__ = "decrypter"
-    __version__ = "0.04"
+    __version__ = "0.13"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?crypt\.cat/\w+"
+    __pattern__ = r"http://(?:www\.)?data\.hu/dir/\w+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         (
             "folder_per_package",
             "Default;Yes;No",
             "Create folder for each package",
             "Default",
         ),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Crypt.cat decrypter plugin"""
+    __description__ = """Data.hu folder decrypter plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
-
-    OFFLINE_PATTERN = r"Folder not available!"
+    __authors__ = [("crash", None), ("stickell", "l.stickell@yahoo.it")]
 
-    LINK_PATTERN = r'<input .+?readonly="" value="\s*(.+?)" type="text">'
+    LINK_PATTERN = r"<a href=\'(http://data\.hu/get/.+)\' target=\'_blank\'>\1</a>"
+    NAME_PATTERN = r"<title>(?P<N>.+?) Let\xf6lt\xe9se</title>"
 
-    def get_links(self):
-        baseurl = self.req.http.last_effective_url
-        url, inputs = self.parse_html_form()
+    def _prepare(self):
+        SimpleDecrypter._prepare(self)
 
-        if ">Enter your password.<" in self.data:
+        if "K\xe9rlek add meg a jelsz\xf3t" in self.data:  #: Password protected
             password = self.get_password()
             if not password:
                 self.fail(self._("Password required"))
 
-            inputs["Pass1"] = password
-
-        elif "Enter Captcha" in self.data:
-            m = re.search(r'<img src="(.+?)"', self.data)
-            if m is not None:
-                captcha_code = self.captcha.decrypt(m.group(1), input_type="jpeg")
-                inputs["security_code"] = captcha_code
-
-            else:
-                return []
-
-        else:
-            return []
-
-        self.data = self.load(baseurl, post=inputs, ref=baseurl)
-
-        if "You have entered an incorrect password." in self.data:
-            self.fail(self._("Wrong password"))
+            self.log_debug(
+                "The folder is password protected', 'Using password: " + password
+            )
 
-        elif "Your filled the captcha wrongly!" in self.data:
-            self.retry_captcha()
+            self.data = self.load(self.pyfile.url, post={"mappa_pass": password})
 
-        return re.findall(self.LINK_PATTERN, self.data)
+            if "Hib\xe1s jelsz\xf3" in self.data:  #: Wrong password
+                self.fail(self._("Wrong password"))
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/CzshareComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/CzshareComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DailymotionComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DailymotionComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DataHuFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,39 @@
 # -*- coding: utf-8 -*-
 
-
 from ..base.simple_decrypter import SimpleDecrypter
 
 
-class DataHuFolder(SimpleDecrypter):
-    __name__ = "DataHuFolder"
+class TNTVillageScambioeticoOrg(SimpleDecrypter):
+    __name__ = "TNTVillageScambioeticoOrg"
     __type__ = "decrypter"
-    __version__ = "0.13"
+    __version__ = "0.07"
     __status__ = "testing"
 
-    __pattern__ = r"http://(?:www\.)?data\.hu/dir/\w+"
+    __pattern__ = r"http://(?:www\.)?forum\.tntvillage\.scambioetico\.org/index\.php\?.*showtopic=\d+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         (
             "folder_per_package",
             "Default;Yes;No",
             "Create folder for each package",
             "Default",
         ),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Data.hu folder decrypter plugin"""
+    __description__ = """TNTVillage.scambioetico.org decrypter plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("crash", None), ("stickell", "l.stickell@yahoo.it")]
-
-    LINK_PATTERN = r"<a href=\'(http://data\.hu/get/.+)\' target=\'_blank\'>\1</a>"
-    NAME_PATTERN = r"<title>(?P<N>.+?) Let\xf6lt\xe9se</title>"
-
-    def _prepare(self):
-        SimpleDecrypter._prepare(self)
+    __authors__ = [("Walter Purcaro", "vuolter@gmail.com")]
 
-        if "K\xe9rlek add meg a jelsz\xf3t" in self.data:  #: Password protected
-            password = self.get_password()
-            if not password:
-                self.fail(self._("Password required"))
-
-            self.log_debug(
-                "The folder is password protected', 'Using password: " + password
-            )
-
-            self.data = self.load(self.pyfile.url, post={"mappa_pass": password})
+    LINK_PATTERNS = [
+        r'<th class="titlemedium"><a href=\'(.+?)\'',
+        r"<a href='(\./index\.php\?act.+?)'",
+    ]
 
-            if "Hib\xe1s jelsz\xf3" in self.data:  #: Wrong password
-                self.fail(self._("Wrong password"))
+    def get_links(self):
+        for p in self.LINK_PATTERNS:
+            self.LINK_PATTERN = p
+            links = SimpleDecrypter.get_links(self)
+            if links:
+                return links
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DepositfilesComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DepositfilesComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/Dereferer.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/Dereferer.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DevhostStFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/DevhostStFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/DlProtectCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/HearthisAtFolder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 # -*- coding: utf-8 -*-
-
 import re
 import urllib.parse
 
-from ..base.simple_decrypter import SimpleDecrypter
+from ..base.decrypter import BaseDecrypter
 
 
-class DlProtectCom(SimpleDecrypter):
-    __name__ = "DlProtectCom"
+class HearthisAtFolder(BaseDecrypter):
+    __name__ = "HearthisAtFolder"
     __type__ = "decrypter"
-    __version__ = "0.13"
+    __version__ = "0.01"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?dl-protect1\.com/\w+"
+    __pattern__ = r"https?://(?:www\.)?hearthis\.at/.*(?<!#pyload)$"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         (
             "folder_per_package",
             "Default;Yes;No",
             "Create folder for each package",
             "Default",
         ),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
+        ("dl_subfolders", "bool", "Download subfolders", False),
+        ("package_subfolder", "bool", "Subfolder as a separate package", False),
     ]
 
-    __description__ = """Dl-protect.com decrypter plugin"""
+    __description__ = """Hearthis.at folder decrypter plugin"""
     __license__ = "GPLv3"
-    __authors__ = [
-        ("Walter Purcaro", "vuolter@gmail.com"),
-        ("GammaC0de", "nitzo2001[AT]yahoo[DOT]com"),
-    ]
+    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
+
+    def decrypt(self, pyfile):
+        self.data = self.load(pyfile.url)
+
+        m = re.search(r"intTrackId = (\d+);", self.data)
+        if m is not None:
+            #: Single track
+            self.packages = [
+                (pyfile.package().name, pyfile.url + "#pyload", pyfile.package().folder)
+            ]
+
+        else:
+            #: Playlist
+            m = re.search(r"intInternalId = (\d+);", self.data)
+            if m is None:
+                self.fail(self._("Internal Id not found"))
 
-    def get_links(self):
-        if "Cliquez sur continuer pour voir le(s) lien" in self.data:
-            self.data = self.load(self.pyfile.url, post={"submit": "Continuer"})
-
-        if 'img src="captcha.php' in self.data:
-            captcha_code = self.captcha.decrypt(
-                urllib.parse.urljoin(self.pyfile.url, "/captcha.php"), input_type="jpeg"
-            )
             self.data = self.load(
-                self.pyfile.url, post={"captchaCode": captcha_code, "submit": ""}
+                "https://hearthis.at/user_ajax_more.php",
+                post={"user": m.group(1), "min": 0, "max": 200},
             )
 
-            if "Le code de sécurité est incorrect" in self.data:
-                self.retry_captcha()
-
-        return re.findall(r'<a href="(?P<id>[^/].+?)">(?P=id)</a>', self.data)
+            links = [
+                urllib.parse.urljoin(pyfile.url, x) + "#pyload"
+                for x in re.findall(
+                    r'<a class="player-link".+?href="(.+?)".+?</a>', self.data, re.S
+                )
+            ]
+            self.packages = [(pyfile.package().name, links, pyfile.package().folder)]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/EasybytezComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/EasybytezComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/EmbeduploadCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/EmbeduploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilecloudIoFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilecloudIoFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilecryptCc.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilecryptCc.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from ..base.decrypter import BaseDecrypter
 from ..helpers import replace_patterns
 
 
 class FilecryptCc(BaseDecrypter):
     __name__ = "FilecryptCc"
     __type__ = "decrypter"
-    __version__ = "0.48"
+    __version__ = "0.49"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?filecrypt\.(?:cc|co)/Container/\w+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("handle_mirror_pages", "bool", "Handle Mirror Pages", True),
     ]
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilefactoryComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilefactoryComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilerNetFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilerNetFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FilestubeCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FilestubeCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FiletramCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FiletramCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FourChanOrg.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FourChanOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FreakhareComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FreakhareComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FreetexthostCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FreetexthostCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FshareVnFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FshareVnFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/FurLy.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/FurLy.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/Go4UpCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/Go4UpCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/GofileIoFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/GofileIoFolder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # -*- coding: utf-8 -*-
 
 import base64
 import json
 
+from pyload.core.network.http.exceptions import BadHeader
+
 from ..base.decrypter import BaseDecrypter
 
 
 class GofileIoFolder(BaseDecrypter):
     __name__ = "GofileIoFolder"
     __type__ = "decrypter"
-    __version__ = "0.01"
+    __version__ = "0.02"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?gofile\.io/d/(?P<ID>\w+)"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         (
@@ -30,15 +32,19 @@
     __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
     URL_REPLACEMENTS = [("http://", "https://")]
 
     API_URL = "https://api.gofile.io/"
 
     def api_request(self, method, **kwargs):
-        json_data = self.load(self.API_URL + method, get=kwargs)
+        try:
+            json_data = self.load(self.API_URL + method, get=kwargs)
+        except BadHeader as exc:
+            json_data = exc.content
+
         return json.loads(json_data)
 
     def decrypt(self, pyfile):
         api_data = self.api_request("createAccount")
         if api_data["status"] != "ok":
             self.fail(
                 self._("createAccount API failed | {}").format(api_data["status"])
@@ -78,9 +84,12 @@
 
             else:
                 self.offline()
 
         elif status == "error-notFound":
             self.offline()
 
+        elif status == "error-notPremium":
+            self.fail(self._("File can be downloaded by premium users only"))
+
         else:
-            self.fail("getContent API failed | {}".format(status))
+            self.fail(self._("getContent API failed | {}").format(status))
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/GooGl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/GooGl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/GoogledriveComDereferer.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/GoogledriveComDereferer.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/GoogledriveComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/GoogledriveComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/HearthisAtFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MyfastfileCom.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,45 @@
 # -*- coding: utf-8 -*-
-import re
-import urllib.parse
+import json
 
-from ..base.decrypter import BaseDecrypter
+from ..base.multi_downloader import MultiDownloader
 
 
-class HearthisAtFolder(BaseDecrypter):
-    __name__ = "HearthisAtFolder"
-    __type__ = "decrypter"
-    __version__ = "0.01"
+class MyfastfileCom(MultiDownloader):
+    __name__ = "MyfastfileCom"
+    __type__ = "downloader"
+    __version__ = "0.16"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?hearthis\.at/.*(?<!#pyload)$"
+    __pattern__ = r"http://\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}/dl/"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
-        (
-            "folder_per_package",
-            "Default;Yes;No",
-            "Create folder for each package",
-            "Default",
-        ),
+        ("fallback", "bool", "Fallback to free download if premium fails", False),
+        ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
-        ("dl_subfolders", "bool", "Download subfolders", False),
-        ("package_subfolder", "bool", "Subfolder as a separate package", False),
+        ("revert_failed", "bool", "Revert to standard download if fails", True),
     ]
 
-    __description__ = """Hearthis.at folder decrypter plugin"""
+    __description__ = """Myfastfile.com multi-downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
+    __authors__ = [("stickell", "l.stickell@yahoo.it")]
 
-    def decrypt(self, pyfile):
-        self.data = self.load(pyfile.url)
+    def setup(self):
+        self.chunk_limit = -1
 
-        m = re.search(r"intTrackId = (\d+);", self.data)
-        if m is not None:
-            #: Single track
-            self.packages = [
-                (pyfile.package().name, pyfile.url + "#pyload", pyfile.package().folder)
-            ]
-
-        else:
-            #: Playlist
-            m = re.search(r"intInternalId = (\d+);", self.data)
-            if m is None:
-                self.fail(self._("Internal Id not found"))
-
-            self.data = self.load(
-                "https://hearthis.at/user_ajax_more.php",
-                post={"user": m.group(1), "min": 0, "max": 200},
-            )
-
-            links = [
-                urllib.parse.urljoin(pyfile.url, x) + "#pyload"
-                for x in re.findall(
-                    r'<a class="player-link".+?href="(.+?)".+?</a>', self.data, re.S
-                )
-            ]
-            self.packages = [(pyfile.package().name, links, pyfile.package().folder)]
+    def handle_premium(self, pyfile):
+        self.data = self.load(
+            "http://myfastfile.com/api.php",
+            get={
+                "user": self.account.user,
+                "pass": self.account.get_login("password"),
+                "link": pyfile.url,
+            },
+        )
+        self.log_debug("JSON data: " + self.data)
+
+        self.data = json.loads(self.data)
+        if self.data["status"] != "ok":
+            self.fail(self._("Unable to unrestrict link"))
+
+        self.link = self.data["link"]
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/HflixIn.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/HflixIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/HoerbuchIn.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/HoerbuchIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/ImgurCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/ImgurCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/JDlist.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/JDlist.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/LixIn.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/LixIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MediafireComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MediafireComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MegaCoNzFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MegaCoNzFolder.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..base.decrypter import BaseDecrypter
 from ..downloaders.MegaCoNz import MegaClient, MegaCrypto
 
 
 class MegaCoNzFolder(BaseDecrypter):
     __name__ = "MegaCoNzFolder"
     __type__ = "decrypter"
-    __version__ = "0.25"
+    __version__ = "0.26"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?mega(?:\.co)?\.nz/folder/(?P<ID>[\w^_]+)#(?P<KEY>[\w,\-=]+)/?$"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         (
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MegaRapidCzFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MegaRapidCzFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MegadyskPlFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MegadyskPlFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MirrorcreatorCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MirrorcreatorCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MultiUpOrg.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MultiUpOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/MultiloadCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/MultiloadCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/NitroflareComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/NitroflareComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/NosvideoCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/NosvideoCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/PastebinCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/PastebinCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/PastedCo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/PastedCo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/QuickshareCzFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/QuickshareCzFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/RealdebridComTorrent.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/RealdebridComTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/SafelinkingNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/SafelinkingNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/SexuriaCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/SexuriaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/ShSt.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/ShSt.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TinyurlCom.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 # -*- coding: utf-8 -*-
 
 from ..base.simple_decrypter import SimpleDecrypter
 
 
-class TNTVillageScambioeticoOrg(SimpleDecrypter):
-    __name__ = "TNTVillageScambioeticoOrg"
+class TinyurlCom(SimpleDecrypter):
+    __name__ = "TinyurlCom"
     __type__ = "decrypter"
     __version__ = "0.07"
     __status__ = "testing"
 
-    __pattern__ = r"http://(?:www\.)?forum\.tntvillage\.scambioetico\.org/index\.php\?.*showtopic=\d+"
+    __pattern__ = r"https?://(?:www\.)?(preview\.)?tinyurl\.com/[\w\-]+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         (
             "folder_per_package",
             "Default;Yes;No",
             "Create folder for each package",
             "Default",
         ),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """TNTVillage.scambioetico.org decrypter plugin"""
+    __description__ = """Tinyurl.com decrypter plugin"""
     __license__ = "GPLv3"
     __authors__ = [("Walter Purcaro", "vuolter@gmail.com")]
 
-    LINK_PATTERNS = [
-        r'<th class="titlemedium"><a href=\'(.+?)\'',
-        r"<a href='(\./index\.php\?act.+?)'",
-    ]
+    URL_REPLACEMENTS = [(r"preview\.", r"")]
 
-    def get_links(self):
-        for p in self.LINK_PATTERNS:
-            self.LINK_PATTERN = p
-            links = SimpleDecrypter.get_links(self)
-            if links:
-                return links
+    OFFLINE_PATTERN = r">Error: Unable to find site's URL to redirect to"
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TenluaVnFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TenluaVnFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TinyurlCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TnyCz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
 
+import re
+
 from ..base.simple_decrypter import SimpleDecrypter
 
 
-class TinyurlCom(SimpleDecrypter):
-    __name__ = "TinyurlCom"
+class TnyCz(SimpleDecrypter):
+    __name__ = "TnyCz"
     __type__ = "decrypter"
-    __version__ = "0.07"
+    __version__ = "0.09"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?(preview\.)?tinyurl\.com/[\w\-]+"
+    __pattern__ = r"http://(?:www\.)?tny\.cz/\w+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         (
             "folder_per_package",
             "Default;Yes;No",
             "Create folder for each package",
             "Default",
         ),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Tinyurl.com decrypter plugin"""
+    __description__ = """Tny.cz decrypter plugin"""
     __license__ = "GPLv3"
     __authors__ = [("Walter Purcaro", "vuolter@gmail.com")]
 
-    URL_REPLACEMENTS = [(r"preview\.", r"")]
+    NAME_PATTERN = r"<title>(?P<N>.+?) - .+</title>"
 
-    OFFLINE_PATTERN = r">Error: Unable to find site's URL to redirect to"
+    def get_links(self):
+        m = re.search(r'<a id=\'save_paste\' href="(.+save\.php\?hash=.+)">', self.data)
+        return re.findall(".+", self.load(m.group(1))) if m else None
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TnyCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/WetransferComDereferer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-# -*- coding: utf-8 -*-
+# -*- coding: utf-8 -*
 
-import re
+from ..base.decrypter import BaseDecrypter
 
-from ..base.simple_decrypter import SimpleDecrypter
 
-
-class TnyCz(SimpleDecrypter):
-    __name__ = "TnyCz"
+class WetransferComDereferer(BaseDecrypter):
+    __name__ = "WetransferComDereferer"
     __type__ = "decrypter"
-    __version__ = "0.09"
+    __version__ = "0.01"
     __status__ = "testing"
 
-    __pattern__ = r"http://(?:www\.)?tny\.cz/\w+"
+    __pattern__ = r"https?://we\.tl/[\-\w]{12}"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         (
             "folder_per_package",
             "Default;Yes;No",
             "Create folder for each package",
             "Default",
         ),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Tny.cz decrypter plugin"""
+    __description__ = """we.tl dereferer plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("Walter Purcaro", "vuolter@gmail.com")]
-
-    NAME_PATTERN = r"<title>(?P<N>.+?) - .+</title>"
+    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
-    def get_links(self):
-        m = re.search(r'<a id=\'save_paste\' href="(.+save\.php\?hash=.+)">', self.data)
-        return re.findall(".+", self.load(m.group(1))) if m else None
+    def decrypt(self, pyfile):
+        headers = self.load(pyfile.url, just_header=True)
+        link = headers.get("location")
+        if link is not None:
+            self.packages = [(pyfile.package().folder, [link], pyfile.package().name)]
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TurbobitNetFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TurbobitNetFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/TusfilesNetFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/TusfilesNetFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/UlozToFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/UlozToFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/XFileSharingFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/XFileSharingFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/XupPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/XupPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/decrypters/YoutubeComFolder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/decrypters/YoutubeComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AccioDebridCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AccioDebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AlfafileNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AlfafileNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AlldebridCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AlldebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AndroidfilehostCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AndroidfilehostCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/AnonfilesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/AnonfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ArchiveOrg.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ArchiveOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/BasketbuildCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/BasketbuildCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/BayfilesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/BayfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/BezvadataCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/BezvadataCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ClicknuploadCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ClicknuploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CloudMailRu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CloudMailRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CloudzillaTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CloudzillaTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CosmoboxOrg.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CosmoboxOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CramitIn.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CramitIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/CzshareCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/CzshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DailymotionCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DailymotionCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DailyuploadsNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DailyuploadsNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DataHu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DataHu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DataportCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DataportCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DatoidCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DatoidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DdownloadCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DdownloadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DebridItaliaCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DebridItaliaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DebridlinkFr.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DebridlinkFr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DebridplanetCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DebridplanetCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DefaultPlugin.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DefaultPlugin.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DepositfilesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DepositfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DevhostSt.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DevhostSt.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DlFreeFr.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DlFreeFr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DownsterNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DownsterNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DropDownload.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DropDownload.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/DropboxCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/DropboxCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/EasybytezCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/EasybytezCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/EasyuploadIo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/EasyuploadIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/EdiskCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/EdiskCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/EuroshareEu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/EuroshareEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ExashareCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ExashareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ExtmatrixCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ExtmatrixCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FastixRu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FastixRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FastshareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FastshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FikperCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FikperCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileAl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileAl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileSharkPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileSharkPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileStoreTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileStoreTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileboomMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileboomMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilecloudIo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilecloudIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FiledropperCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilepupNet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 # -*- coding: utf-8 -*-
+
+#
+# Test links:
+# http://www.filepup.net/files/k5w4ZVoF1410184283.html
+# http://www.filepup.net/files/R4GBq9XH1410186553.html
+
 import re
-import urllib.parse
 
 from ..base.simple_downloader import SimpleDownloader
 
 
-class FiledropperCom(SimpleDownloader):
-    __name__ = "FiledropperCom"
+class FilepupNet(SimpleDownloader):
+    __name__ = "FilepupNet"
     __type__ = "downloader"
-    __version__ = "0.06"
+    __version__ = "0.08"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?filedropper\.com/\w+"
+    __pattern__ = r"http://(?:www\.)?filepup\.net/files/\w+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Filedropper.com downloader plugin"""
+    __description__ = """Filepup.net downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("zapp-brannigan", "fuerst.reinje@web.de")]
+    __authors__ = [
+        ("zapp-brannigan", "fuerst.reinje@web.de"),
+        ("Walter Purcaro", "vuolter@gmail.com"),
+    ]
+
+    NAME_PATTERN = r">(?P<N>.+?)</h1>"
+    SIZE_PATTERN = r'class="fa fa-archive"></i> \((?P<S>[\d.,]+) (?P<U>[\w^_]+)'
 
-    NAME_PATTERN = r"Filename: (?P<N>.+?) <"
-    # NOTE: Website says always 0 KiB
-    SIZE_PATTERN = r"Size: (?P<S>[\d.,]+) (?P<U>[\w^_]+),"
-    OFFLINE_PATTERN = r'value="a\.swf"'
+    OFFLINE_PATTERN = r">This file has been deleted"
+
+    LINK_FREE_PATTERN = r"(http://www\.filepup\.net/get/.+?)\'"
 
     def setup(self):
         self.multi_dl = False
         self.chunk_limit = 1
 
     def handle_free(self, pyfile):
-        m = re.search(r'img id="img" src="(.+?)"', self.data)
-        if m is None:
-            self.fail(self._("Captcha not found"))
-
-        captcha_code = self.captcha.decrypt(f"http://www.filedropper.com/{m.group(1)}")
-
-        m = re.search(r'method="post" action="(.+?)"', self.data)
+        m = re.search(self.LINK_FREE_PATTERN, self.data)
         if m is not None:
-            self.download(
-                urllib.parse.urljoin("http://www.filedropper.com/", m.group(1)),
-                post={"code": captcha_code},
-            )
+            dl_link = m.group(1)
+            self.download(dl_link, post={"task": "download"})
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilefactoryCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilefactoryCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilefoxCc.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilefoxCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilejokerNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilejokerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileomCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileomCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilepupNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VkCom.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 # -*- coding: utf-8 -*-
 
 #
 # Test links:
-# http://www.filepup.net/files/k5w4ZVoF1410184283.html
-# http://www.filepup.net/files/R4GBq9XH1410186553.html
+#   http://vk.com/video_ext.php?oid=166335015&id=162608895&hash=b55affa83774504b&hd=1
 
 import re
 
 from ..base.simple_downloader import SimpleDownloader
 
 
-class FilepupNet(SimpleDownloader):
-    __name__ = "FilepupNet"
+class VkCom(SimpleDownloader):
+    __name__ = "VkCom"
     __type__ = "downloader"
-    __version__ = "0.08"
+    __version__ = "0.06"
     __status__ = "testing"
 
-    __pattern__ = r"http://(?:www\.)?filepup\.net/files/\w+"
+    __pattern__ = r"https?://(?:www\.)?vk\.com/video_ext\.php/\?.+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Filepup.net downloader plugin"""
+    __description__ = """Vk.com downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [
-        ("zapp-brannigan", "fuerst.reinje@web.de"),
-        ("Walter Purcaro", "vuolter@gmail.com"),
-    ]
-
-    NAME_PATTERN = r">(?P<N>.+?)</h1>"
-    SIZE_PATTERN = r'class="fa fa-archive"></i> \((?P<S>[\d.,]+) (?P<U>[\w^_]+)'
-
-    OFFLINE_PATTERN = r">This file has been deleted"
+    __authors__ = [("Walter Purcaro", "vuolter@gmail.com")]
 
-    LINK_FREE_PATTERN = r"(http://www\.filepup\.net/get/.+?)\'"
+    NAME_PATTERN = r'"md_title":"(?P<N>.+?)"'
+    OFFLINE_PATTERN = r'<div id="video_ext_msg">'
 
-    def setup(self):
-        self.multi_dl = False
-        self.chunk_limit = 1
+    LINK_FREE_PATTERN = r'url\d+":"(.+?)"'
 
     def handle_free(self, pyfile):
-        m = re.search(self.LINK_FREE_PATTERN, self.data)
-        if m is not None:
-            dl_link = m.group(1)
-            self.download(dl_link, post={"task": "download"})
+        self.link = re.findall(self.LINK_FREE_PATTERN, self.data)[
+            0 if self.config.get("quality") == "Low" else -1
+        ]
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilerNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilerioCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilerioCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FilesMailRu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilesMailRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileuploadCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileuploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FileuploadNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FileuploadNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FiregetCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FiregetCom.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from ..base.xfs_downloader import XFSDownloader
 
 
 class FiregetCom(XFSDownloader):
     __name__ = "FiregetCom"
     __type__ = "downloader"
-    __version__ = "0.04"
+    __version__ = "0.05"
     __status__ = "testing"
 
-    __pattern__ = r"http://(?:www\.)?fireget\.com/(?P<ID>\w{12})/.+"
+    __pattern__ = r"https?://(?:www\.)?fireget\.com/(?P<ID>\w{12})/.+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FistfastNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FistfastNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FlyFilesNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FlyFilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FourSharedCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FourSharedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/FshareVn.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FshareVn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 import json
 import re
 import urllib.parse
 
 import pycurl
+from pyload.core.network.cookie_jar import CookieJar
 from pyload.core.network.http.exceptions import BadHeader
+from pyload.core.network.http.http_request import HTTPRequest
 
 from ..base.simple_downloader import SimpleDownloader
 
 
 class FshareVn(SimpleDownloader):
     __name__ = "FshareVn"
     __type__ = "downloader"
-    __version__ = "0.37"
+    __version__ = "0.40"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?fshare\.vn/file/(?P<ID>\w+)"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
@@ -28,14 +30,15 @@
     __license__ = "GPLv3"
     __authors__ = [
         ("zoidberg", "zoidberg@mujmail.cz"),
         ("GammaC0de", "nitzo2001[AT]yahoo[DOT]com"),
     ]
 
     OFFLINE_PATTERN = r"Tập tin của bạn yêu cầu không tồn tại"
+    TEMP_OFFLINE_PATTERN = r"^unmatchable$"
 
     URL_REPLACEMENTS = [("http://", "https://")]
 
     API_KEY = "dMnqMMZMUnN5YpvKENaEhdQQ5jxDqddt"
     API_URL = "https://api.fshare.vn/api/"
 
     # See https://www.fshare.vn/api-doc
@@ -87,14 +90,26 @@
                     "size": file_info["current"]["size"],
                     "status": 2,
                 }
             )
 
         return info
 
+    def setup(self):
+        try:
+            self.req.http.close()
+        except Exception:
+            pass
+
+        self.req.http = HTTPRequest(
+            cookies=CookieJar(None),
+            options=self.pyload.request_factory.get_options(),
+            limit=5_000_000,
+        )
+
     def handle_free(self, pyfile):
         action, inputs = self.parse_html_form('class="password-form"')
         if action is not None:
             password = self.get_password()
             if password:
                 inputs["DownloadPasswordForm[password]"] = password
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/Ftp.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/Ftp.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GamefrontCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GamefrontCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GetTwentyFourOrg.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GetTwentyFourOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GigapetaCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GigapetaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GofileIo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GofileIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GooIm.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GooIm.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/GoogledriveCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/GoogledriveCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HearthisAt.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HearthisAt.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HellshareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HellshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HighWayMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HighWayMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HitfileNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HitfileNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HostujeNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HostujeNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HotlinkCc.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HotlinkCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/Http.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/Http.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HugefilesNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HugefilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/HundredEightyUploadCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/HundredEightyUploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/IfolderRu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/IfolderRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/IronfilesNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/IronfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/JumbofilesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/JumbofilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/JunocloudMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/JunocloudMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/KatfileCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/KatfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/Keep2ShareCc.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/Keep2ShareCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/KingfilesNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/KingfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/KrakenfilesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/KrakenfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LetsuploadCc.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LetsuploadCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LetsuploadCo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LetsuploadCo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LibgenIo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LibgenIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LinkifierCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LinkifierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LinksnappyCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LinksnappyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LinksnappyComTorrent.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LinksnappyComTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/LoadTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/LoadTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MediafireCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MediafireCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaCoNz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaCoNz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaDebridEu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaDebridEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaRapidCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaRapidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaRapidoNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaRapidoNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegacrypterCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegacrypterCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegadyskPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegadyskPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegasharesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegasharesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MegaupNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MegaupNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MovReelCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MovReelCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MultihostersCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MultihostersCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MultishareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MultishareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MyfastfileCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PremiumTo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,66 @@
 # -*- coding: utf-8 -*-
+
 import json
+import re
 
 from ..base.multi_downloader import MultiDownloader
 
 
-class MyfastfileCom(MultiDownloader):
-    __name__ = "MyfastfileCom"
+class PremiumTo(MultiDownloader):
+    __name__ = "PremiumTo"
     __type__ = "downloader"
-    __version__ = "0.16"
+    __version__ = "0.36"
     __status__ = "testing"
 
-    __pattern__ = r"http://\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}/dl/"
+    __pattern__ = r"^unmatchable$"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", False),
+        ("revert_failed", "bool", "Revert to standard download if fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
-        ("revert_failed", "bool", "Revert to standard download if fails", True),
     ]
 
-    __description__ = """Myfastfile.com multi-downloader plugin"""
+    __description__ = """Premium.to multi-downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("stickell", "l.stickell@yahoo.it")]
+    __authors__ = [
+        ("RaNaN", "RaNaN@pyload.net"),
+        ("zoidberg", "zoidberg@mujmail.cz"),
+        ("stickell", "l.stickell@yahoo.it"),
+        ("GammaC0de", "nitzo2001[AT]yahoo[DOT]com"),
+    ]
+
+    CHECK_TRAFFIC = True
 
-    def setup(self):
-        self.chunk_limit = -1
+    # See https://premium.to/API.html
+    API_URL = "http://api.premium.to/api/2/"
 
     def handle_premium(self, pyfile):
-        self.data = self.load(
-            "http://myfastfile.com/api.php",
+        self.download(
+            self.API_URL + "getfile.php",
             get={
-                "user": self.account.user,
-                "pass": self.account.get_login("password"),
+                "userid": self.account.user,
+                "apikey": self.account.info["login"]["password"],
                 "link": pyfile.url,
             },
+            disposition=True,
         )
-        self.log_debug("JSON data: " + self.data)
 
-        self.data = json.loads(self.data)
-        if self.data["status"] != "ok":
-            self.fail(self._("Unable to unrestrict link"))
+    def check_download(self):
+        if self.scan_download(
+            {
+                "json": re.compile(
+                    rb'\A{["\']code["\']:\d+,["\']message["\']:(["\']).+?\1}\Z'
+                )
+            }
+        ):
+            with open(self.last_download, "r") as fp:
+                json_data = json.loads(fp.read())
+
+            self.remove(self.last_download)
+            self.fail(
+                self._("API error {} - {}").format(json_data["code"], json_data["message"])
+            )
 
-        self.link = self.data["link"]
+        return super().check_download()
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/MystoreTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MystoreTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NarodRu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NarodRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NippyshareCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NippyshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NitrobitNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NitrobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NitroflareCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NitroflareCom.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..anticaptchas.ReCaptcha import ReCaptcha
 from ..base.simple_downloader import SimpleDownloader
 
 
 class NitroflareCom(SimpleDownloader):
     __name__ = "NitroflareCom"
     __type__ = "downloader"
-    __version__ = "0.40"
+    __version__ = "0.41"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?(?:nitro\.download|nitroflare\.com)/view/(?P<ID>[\w^_]+)"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
@@ -34,14 +34,15 @@
 
     INFO_PATTERN = r'title="(?P<N>.+?)".+>(?P<S>[\d.,]+) (?P<U>[\w^_]+)'
     OFFLINE_PATTERN = r">File doesn\'t exist"
 
     LINK_PATTERN = r'(https?://[\w\-]+\.nitroflare\.com/.+?)"'
 
     DIRECT_LINK = False
+    DISPOSITION = False
 
     PREMIUM_ONLY_PATTERN = r"This file is available with Premium only"
     DL_LIMIT_PATTERN = r"You have to wait \d+ minutes to download your next file."
 
     URL_REPLACEMENTS = [(r"nitro\.download", "nitroflare.com")]
 
     # See https://nitroflare.com/member?s=general-api
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NoPremiumPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NoPremiumPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NofileIo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NofileIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NosuploadCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NosuploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NovafileCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NovafileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/NowVideoSx.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/NowVideoSx.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/OneFichierCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/OneFichierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/OnlineTvRecorder.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/OnlineTvRecorder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/OpenloadIo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RPNetBiz.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,93 @@
 # -*- coding: utf-8 -*-
-
 import json
-import re
 
-from ..base.simple_downloader import SimpleDownloader
+from ..base.multi_downloader import MultiDownloader
 
 
-class OpenloadIo(SimpleDownloader):
-    __name__ = "OpenloadIo"
+class RPNetBiz(MultiDownloader):
+    __name__ = "RPNetBiz"
     __type__ = "downloader"
-    __version__ = "0.21"
+    __version__ = "0.22"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?openload\.(co|io)/(f|embed)/(?P<ID>[\w\-]+)"
+    __pattern__ = r"https?://.+rpnet\.biz"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
-        ("fallback", "bool", "Fallback to free download if premium fails", True),
+        ("fallback", "bool", "Fallback to free download if premium fails", False),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
+        ("revert_failed", "bool", "Revert to standard download if fails", True),
     ]
 
-    __description__ = """Openload.co downloader plugin"""
+    __description__ = """RPNet.biz multi-downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [(None, None)]
-
-    OFFLINE_PATTERN = r">We are sorry"
-
-    # The API reference, that this implementation uses is available at
-    # https://openload.co/api
-    API_URL = "https://api.openload.co/1"
-
-    def api_request(self, file_id, method, **kwargs):
-        kwargs["file"] = file_id
-        return json.loads(self.load(self.API_URL + "/file/" + method, get=kwargs))
-
-    def api_info(self, url):
-        file_id = re.match(self.__pattern__, url).group("ID")
-        info_json = self.api_request(file_id, "info")
-        file_info = info_json["result"][file_id]
-
-        return {"name": file_info["name"], "size": file_info["size"]}
+    __authors__ = [("Dman", "dmanugm@gmail.com")]
 
     def setup(self):
-        self.multi_dl = True
-        self.chunk_limit = 1
-
-    def handle_free(self, pyfile):
-        file_id = self.info["pattern"]["ID"]
-
-        ticket_json = self.api_request(file_id, "dlticket")
+        self.chunk_limit = -1
 
-        if ticket_json["status"] != 200:
-            self.log_error(ticket_json["msg"])
+    def handle_premium(self, pyfile):
+        user, info = self.account.select()
 
-        if ticket_json["status"] == 404:
-            self.offline(ticket_json["msg"])
-
-        elif ticket_json["status"] == 509:
-            self.temp_offline(ticket_json["msg"])
-
-        elif ticket_json["status"] != 200:
-            self.fail(ticket_json["msg"])
-
-        self.wait(ticket_json["result"]["wait_time"])
-
-        # check if a captcha is required for this download
-        captcha_response = ""
-        if (
-            "captcha_url" in ticket_json["result"]
-            and ticket_json["result"]["captcha_url"]
-        ):
-            captcha_url = ticket_json["result"]["captcha_url"]
-            self.log_debug(f"This download requires a captcha solution: {captcha_url}")
-            captcha_response = self.captcha.decrypt(captcha_url)
-
-        ticket = ticket_json["result"]["ticket"]
-
-        download_json = self.api_request(
-            file_id, "dl", ticket=ticket, captcha_response=captcha_response
+        res = self.load(
+            "https://premium.rpnet.biz/client_api.php",
+            get={
+                "username": user,
+                "password": info["login"]["password"],
+                "action": "generate",
+                "links": pyfile.url,
+            },
         )
 
-        # check download link request result status
-        if download_json["status"] == 403:
-            # wrong captcha, get new captcha and try again
-            self.retry_captcha()
-
-        elif download_json["status"] == 200:
-            self.link = download_json["result"]["url"]
-
+        self.log_debug(f"JSON data: {res}")
+        #: Get the first link... since we only queried one
+        link_status = json.loads(res)["links"][0]
+
+        #: Check if we only have an id as a HDD link
+        if "id" in link_status:
+            self.log_debug("Need to wait at least 30 seconds before requery")
+            self.wait(30)  #: Wait for 30 seconds
+            #: Lets query the server again asking for the status on the link,
+            #: We need to keep doing this until we reach 100
+            attempts = 30
+            my_try = 0
+            while my_try <= attempts:
+                self.log_debug(f"Try: {my_try}; Max Tries: {attempts}")
+                res = self.load(
+                    "https://premium.rpnet.biz/client_api.php",
+                    get={
+                        "username": user,
+                        "password": info["login"]["password"],
+                        "action": "downloadInformation",
+                        "id": link_status["id"],
+                    },
+                )
+                self.log_debug(f"JSON data hdd query: {res}")
+                download_status = json.loads(res)["download"]
+
+                dl_status = download_status["status"]
+                if dl_status == "100":
+                    lk_status = link_status["generated"] = download_status["rpnet_link"]
+                    self.log_debug(f"Successfully downloaded to rpnet HDD: {lk_status}")
+                    break
+                else:
+                    self.log_debug(f"At {dl_status}% for the file download")
+
+                self.wait(30)
+                my_try += 1
+
+            if my_try > attempts:  #: We went over the limit!
+                self.fail(
+                    self._(
+                        "Waited for about 15 minutes for download to finish but failed"
+                    )
+                )
+
+        if "generated" in link_status:
+            self.link = link_status["generated"]
+            return
+        elif "error" in link_status:
+            self.fail(link_status["error"])
         else:
-            # no status 403 or 200 means getting the download url failed, abort
-            self.fail(download_json["msg"])
+            self.fail(self._("Something went wrong, not supposed to enter here"))
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/OverLoadMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/OverLoadMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PixeldrainCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PixeldrainCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PornhostCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PornhostCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PornhubCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PornhubCom.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..base.simple_downloader import SimpleDownloader
 
 
 class PornhubCom(SimpleDownloader):
     __name__ = "PornhubCom"
     __type__ = "downloader"
-    __version__ = "0.61"
+    __version__ = "0.62"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?pornhub\.com/view_video\.php\?viewkey=\w+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PornovkaCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PornovkaCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PorntrexCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PorntrexCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PremiumTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TbSevenPl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,57 @@
 # -*- coding: utf-8 -*-
 
-import json
 import re
 
+from pyload.core.utils import parse
+
 from ..base.multi_downloader import MultiDownloader
 
 
-class PremiumTo(MultiDownloader):
-    __name__ = "PremiumTo"
+class TbSevenPl(MultiDownloader):
+    __name__ = "TbSevenPl"
     __type__ = "downloader"
-    __version__ = "0.36"
+    __version__ = "0.02"
     __status__ = "testing"
 
     __pattern__ = r"^unmatchable$"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", False),
-        ("revert_failed", "bool", "Revert to standard download if fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
+        ("revert_failed", "bool", "Revert to standard download if fails", True),
     ]
 
-    __description__ = """Premium.to multi-downloader plugin"""
+    __description__ = """Tb7.pl multi-downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [
-        ("RaNaN", "RaNaN@pyload.net"),
-        ("zoidberg", "zoidberg@mujmail.cz"),
-        ("stickell", "l.stickell@yahoo.it"),
-        ("GammaC0de", "nitzo2001[AT]yahoo[DOT]com"),
-    ]
+    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
-    CHECK_TRAFFIC = True
+    NAME_PATTERN = r'<div class="name">(?P<N>.+?)<'
+    SIZE_PATTERN = r'Rozmiar: <span class="type red">(?P<S>[\d.,]+) (?P<U>[\w_^]+)<'
 
-    # See https://premium.to/API.html
-    API_URL = "http://api.premium.to/api/2/"
+    LINK_PATTERN = r'<a href="(.+?)" target="_blank">Pobierz</a>'
 
     def handle_premium(self, pyfile):
-        self.download(
-            self.API_URL + "getfile.php",
-            get={
-                "userid": self.account.user,
-                "apikey": self.account.info["login"]["password"],
-                "link": pyfile.url,
-            },
-            disposition=True,
+        self.data = self.load(
+            "https://tb7.pl/mojekonto/sciagaj", post={"step": 1, "content": pyfile.url}
+        )
+
+        m = re.search(self.NAME_PATTERN, self.data)
+        if m is not None:
+            pyfile.name = m.group("N")
+
+        m = re.search(self.SIZE_PATTERN, self.data)
+        if m is not None:
+            pyfile.size = parse.bytesize(m.group("S"), m.group("U"))
+
+        self.data = self.load(
+            "https://tb7.pl/mojekonto/sciagaj", post={"step": 2, "0": "on"}
         )
 
-    def check_download(self):
-        if self.scan_download(
-            {
-                "json": re.compile(
-                    rb'\A{["\']code["\']:\d+,["\']message["\']:(["\']).+?\1}\Z'
-                )
-            }
-        ):
-            with open(self.last_download, "r") as fp:
-                json_data = json.loads(fp.read())
-
-            self.remove(self.last_download)
-            self.fail(
-                self._("API error {} - {}").format(json_data["code"], json_data["message"])
-            )
+        if "Nieaktywne linki" in self.data:
+            self.temp_offline()
 
-        return super().check_download()
+        m = re.search(self.LINK_PATTERN, self.data)
+        if m is not None:
+            self.link = m.group(1)
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PremiumizeMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PremiumizeMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PromptfileCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PromptfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/PutdriveCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/PutdriveCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/QuickshareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/QuickshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RPNetBiz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RapideoPl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,112 @@
 # -*- coding: utf-8 -*-
 import json
 
 from ..base.multi_downloader import MultiDownloader
 
 
-class RPNetBiz(MultiDownloader):
-    __name__ = "RPNetBiz"
+class RapideoPl(MultiDownloader):
+    __name__ = "RapideoPl"
     __type__ = "downloader"
-    __version__ = "0.22"
+    __version__ = "0.14"
     __status__ = "testing"
 
-    __pattern__ = r"https?://.+rpnet\.biz"
+    __pattern__ = r"^unmatchable$"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", False),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
         ("revert_failed", "bool", "Revert to standard download if fails", True),
     ]
 
-    __description__ = """RPNet.biz multi-downloader plugin"""
+    __description__ = """Rapideo.pl multi-downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("Dman", "dmanugm@gmail.com")]
+    __authors__ = [("goddie", "dev@rapideo.pl")]
 
-    def setup(self):
-        self.chunk_limit = -1
+    API_URL = "http://enc.rapideo.pl"
 
-    def handle_premium(self, pyfile):
-        user, info = self.account.select()
+    API_QUERY = {
+        "site": "newrd",
+        "output": "json",
+        "username": "",
+        "password": "",
+        "url": "",
+    }
 
-        res = self.load(
-            "https://premium.rpnet.biz/client_api.php",
-            get={
-                "username": user,
-                "password": info["login"]["password"],
-                "action": "generate",
-                "links": pyfile.url,
-            },
-        )
-
-        self.log_debug(f"JSON data: {res}")
-        #: Get the first link... since we only queried one
-        link_status = json.loads(res)["links"][0]
-
-        #: Check if we only have an id as a HDD link
-        if "id" in link_status:
-            self.log_debug("Need to wait at least 30 seconds before requery")
-            self.wait(30)  #: Wait for 30 seconds
-            #: Lets query the server again asking for the status on the link,
-            #: We need to keep doing this until we reach 100
-            attempts = 30
-            my_try = 0
-            while my_try <= attempts:
-                self.log_debug(f"Try: {my_try}; Max Tries: {attempts}")
-                res = self.load(
-                    "https://premium.rpnet.biz/client_api.php",
-                    get={
-                        "username": user,
-                        "password": info["login"]["password"],
-                        "action": "downloadInformation",
-                        "id": link_status["id"],
-                    },
-                )
-                self.log_debug(f"JSON data hdd query: {res}")
-                download_status = json.loads(res)["download"]
+    ERROR_CODES = {
+        0: "Incorrect login credentials",
+        1: "Not enough transfer to download - top-up your account",
+        2: "Incorrect / dead link",
+        3: "Error connecting to hosting, try again later",
+        9: "Premium account has expired",
+        15: "Hosting no longer supported",
+        80: "Too many incorrect login attempts, account blocked for 24h",
+    }
+
+    def _prepare(self):
+        MultiDownloader._prepare(self)
+
+        data = self.account.get_data()
+
+        self.usr = data["usr"]
+        self.pwd = data["pwd"]
+
+    def run_file_query(self, url, mode=None):
+        query = self.API_QUERY.copy()
+
+        query["username"] = self.usr
+        query["password"] = self.pwd
+        query["url"] = url
+
+        if mode == "fileinfo":
+            query["check"] = 2
+            query["loc"] = 1
+
+        self.log_debug(query)
+
+        return self.load(self.API_URL, post=query)
 
-                dl_status = download_status["status"]
-                if dl_status == "100":
-                    lk_status = link_status["generated"] = download_status["rpnet_link"]
-                    self.log_debug(f"Successfully downloaded to rpnet HDD: {lk_status}")
-                    break
-                else:
-                    self.log_debug(f"At {dl_status}% for the file download")
+    def handle_free(self, pyfile):
+        try:
+            data = self.run_file_query(pyfile.url, "fileinfo")
 
-                self.wait(30)
-                my_try += 1
+        except Exception:
+            self.temp_offline("Query error #1")
 
-            if my_try > attempts:  #: We went over the limit!
+        try:
+            parsed = json.loads(data)
+
+        except Exception:
+            self.temp_offline("Data not found")
+
+        self.log_debug(parsed)
+
+        if "errno" in parsed.keys():
+            if parsed["errno"] in self.ERROR_CODES:
+                #: Error code in known
+                self.fail(self.ERROR_CODES[parsed["errno"]])
+            else:
+                #: Error code isn't yet added to plugin
+                self.fail(
+                    parsed["errstring"]
+                    or self._("Unknown error (code: {})").format(parsed["errno"])
+                )
+
+        if "sdownload" in parsed:
+            if parsed["sdownload"] == "1":
                 self.fail(
                     self._(
-                        "Waited for about 15 minutes for download to finish but failed"
-                    )
+                        "Download from {} is possible only using Rapideo.pl website \
+                    directly"
+                    ).format(parsed["hosting"])
                 )
 
-        if "generated" in link_status:
-            self.link = link_status["generated"]
-            return
-        elif "error" in link_status:
-            self.fail(link_status["error"])
-        else:
-            self.fail(self._("Something went wrong, not supposed to enter here"))
+        pyfile.name = parsed["filename"]
+        pyfile.size = parsed["filesize"]
+
+        try:
+            self.link = self.run_file_query(pyfile.url, "filedownload")
+
+        except Exception:
+            self.temp_offline("Query error #2")
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RapideoPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TwojlimitPl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 import json
 
 from ..base.multi_downloader import MultiDownloader
 
 
-class RapideoPl(MultiDownloader):
-    __name__ = "RapideoPl"
+class TwojlimitPl(MultiDownloader):
+    __name__ = "TwojlimitPl"
     __type__ = "downloader"
-    __version__ = "0.14"
+    __version__ = "0.02"
     __status__ = "testing"
 
     __pattern__ = r"^unmatchable$"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", False),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
         ("revert_failed", "bool", "Revert to standard download if fails", True),
     ]
 
-    __description__ = """Rapideo.pl multi-downloader plugin"""
+    __description__ = """Twojlimit.pl multi-downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("goddie", "dev@rapideo.pl")]
+    __authors__ = [("synweap15", "pawel@twojlimit.pl")]
 
-    API_URL = "http://enc.rapideo.pl"
+    API_URL = "https://crypt.twojlimit.pl"
 
     API_QUERY = {
-        "site": "newrd",
+        "site": "newtl",
         "output": "json",
         "username": "",
         "password": "",
         "url": "",
     }
 
     ERROR_CODES = {
@@ -40,73 +40,68 @@
         2: "Incorrect / dead link",
         3: "Error connecting to hosting, try again later",
         9: "Premium account has expired",
         15: "Hosting no longer supported",
         80: "Too many incorrect login attempts, account blocked for 24h",
     }
 
-    def _prepare(self):
-        MultiDownloader._prepare(self)
-
-        data = self.account.get_data()
-
-        self.usr = data["usr"]
-        self.pwd = data["pwd"]
-
-    def run_file_query(self, url, mode=None):
-        query = self.API_QUERY.copy()
-
-        query["username"] = self.usr
-        query["password"] = self.pwd
-        query["url"] = url
-
-        if mode == "fileinfo":
-            query["check"] = 2
-            query["loc"] = 1
-
-        self.log_debug(query)
-
-        return self.load(self.API_URL, post=query)
+    def setup(self):
+        self.multi_dl = True
+        self.resume_download = True
+        self.chunk_limit = -1
 
     def handle_free(self, pyfile):
         try:
             data = self.run_file_query(pyfile.url, "fileinfo")
 
-        except Exception:
+        except Exception as exc:
+            self.log_error(exc)
             self.temp_offline("Query error #1")
 
         try:
-            parsed = json.loads(data)
+            json_data = json.loads(data)
 
         except Exception:
             self.temp_offline("Data not found")
 
-        self.log_debug(parsed)
-
-        if "errno" in parsed.keys():
-            if parsed["errno"] in self.ERROR_CODES:
+        if "errno" in json_data:
+            if json_data["errno"] in self.ERROR_CODES:
                 #: Error code in known
-                self.fail(self.ERROR_CODES[parsed["errno"]])
+                self.fail(self.ERROR_CODES[json_data["errno"]])
+
             else:
                 #: Error code isn't yet added to plugin
                 self.fail(
-                    parsed["errstring"]
-                    or self._("Unknown error (code: {})").format(parsed["errno"])
+                    json_data["errstring"]
+                    or self._("Unknown error (code: {})").format(json_data["errno"])
                 )
 
-        if "sdownload" in parsed:
-            if parsed["sdownload"] == "1":
+        if "sdownload" in json_data:
+            if json_data["sdownload"] == "1":
                 self.fail(
                     self._(
-                        "Download from {} is possible only using Rapideo.pl website \
-                    directly"
-                    ).format(parsed["hosting"])
+                        "Download from {} is possible only using TwojLimit.pl website directly"
+                    ).format(json_data["hosting"])
                 )
 
-        pyfile.name = parsed["filename"]
-        pyfile.size = parsed["filesize"]
+        pyfile.name = json_data["filename"]
+        pyfile.size = json_data["filesize"]
 
         try:
-            self.link = self.run_file_query(pyfile.url, "filedownload")
+            self.download(self.run_file_query(pyfile.url, "filedownload"))
 
-        except Exception:
+        except Exception as exc:
+            self.log_error(exc)
             self.temp_offline("Query error #2")
+
+    def run_file_query(self, url, mode=None):
+        query = self.API_QUERY.copy()
+
+        query["username"] = self.account.user
+        query["password"] = self.account.info["data"]["hash_password"]
+        query["url"] = url
+
+        if mode == "fileinfo":
+            query["check"] = 2
+            query["loc"] = 1
+
+        return self.load(self.API_URL, post=query, redirect=20)
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RapidfileshareNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RapidfileshareNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RapidgatorNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RapidgatorNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RapiduNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RapiduNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RarefileNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RarefileNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RealdebridCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RealdebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RedtubeCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RedtubeCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RehostTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RehostTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RemixshareCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RemixshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/RgHostNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/RgHostNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SafesharingEu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SafesharingEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SecureUploadEu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SecureUploadEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SenditCloud.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SenditCloud.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SendspaceCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SendspaceCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ShareplaceCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ShareplaceCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SimplyPremiumCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SimplyPremiumCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SimplydebridCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SimplydebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SizedriveCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SizedriveCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SmoozedCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SmoozedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SmuleCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SmuleCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SolidfilesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SolidfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SoundcloudCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SoundcloudCom.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # -*- coding: utf-8 -*-
 import json
 import re
 
+from pyload.core.network.cookie_jar import CookieJar
+from pyload.core.network.http.http_request import HTTPRequest
+
 from ..base.simple_downloader import SimpleDownloader
 
 
 class SoundcloudCom(SimpleDownloader):
     __name__ = "SoundcloudCom"
     __type__ = "downloader"
-    __version__ = "0.19"
+    __version__ = "0.21"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?soundcloud\.com/[\w\-]+/[\w\-]+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
@@ -26,15 +29,25 @@
         ("Walter Purcaro", "vuolter@gmail.com"),
         ("GammaC0de", "nitzo2001[AT]yahoo[DOT]com"),
     ]
 
     NAME_PATTERN = r'title" content="(?P<N>.+?)"'
     OFFLINE_PATTERN = r'<title>"SoundCloud - Hear the world’s sounds"</title>'
 
-    CLIENT_ID = "wuM9g7pMB4mU13fW6SuRfQeJNRYNIX9O"
+    def setup(self):
+        try:
+            self.req.http.close()
+        except Exception:
+            pass
+
+        self.req.http = HTTPRequest(
+            cookies=CookieJar(None),
+            options=self.pyload.request_factory.get_options(),
+            limit=5_000_000,
+        )
 
     def get_info(self, url="", html=""):
         info = super(SoundcloudCom, self).get_info(url, html)
         # Unfortunately, NAME_PATTERN does not include file extension, so we add '.mp3' as an extension.
         if "name" in info:
             info["name"] += ".mp3"
 
@@ -45,14 +58,26 @@
             json_data = re.search(
                 r"<script>window\.__sc_hydration = (.+?);</script>", self.data
             ).group(1)
 
         except (AttributeError, IndexError):
             self.fail("Failed to retrieve json_data")
 
+        try:
+            js_url = re.findall(r'script crossorigin src="(.+?)"></script>', self.data)[-1]
+        except IndexError:
+            self.fail(self._("Failed to find js_url"))
+
+        js_data = self.load(js_url)
+        m = re.search(r'[ ,]client_id:"(.+?)"', js_data)
+        if m is None:
+            self.fail(self._("client_id not found"))
+
+        client_id = m.group(1)
+
         hydra_table = {
             table["hydratable"]: table["data"] for table in json.loads(json_data)
         }
         streams = [
             s["url"]
             for s in hydra_table["sound"]["media"]["transcodings"]
             if s["format"]["protocol"] == "progressive"
@@ -60,12 +85,12 @@
         ]
         track_authorization = hydra_table["sound"]["track_authorization"]
 
         if streams:
             json_data = self.load(
                 streams[0],
                 get={
-                    "client_id": self.CLIENT_ID,
+                    "client_id": client_id,
                     "track_authorization": track_authorization,
                 },
             )
             self.link = json.loads(json_data).get("url")
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SpeedyshareCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SpeedyshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/StreamCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/StreamCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/StreamcloudEu.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/StreamcloudEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/SuprafilesMe.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/SuprafilesMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TbSevenPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UseruploadNet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 # -*- coding: utf-8 -*-
 
 import re
 
-from pyload.core.utils import parse
+from ..base.xfs_downloader import XFSDownloader
 
-from ..base.multi_downloader import MultiDownloader
 
-
-class TbSevenPl(MultiDownloader):
-    __name__ = "TbSevenPl"
+class UseruploadNet(XFSDownloader):
+    __name__ = "UseruploadNet"
     __type__ = "downloader"
     __version__ = "0.02"
     __status__ = "testing"
 
-    __pattern__ = r"^unmatchable$"
+    __pattern__ = r"https?://(?:www\.)?userupload\.net/\w{12}"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
-        ("fallback", "bool", "Fallback to free download if premium fails", False),
+        ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
-        ("revert_failed", "bool", "Revert to standard download if fails", True),
     ]
 
-    __description__ = """Tb7.pl multi-downloader plugin"""
+    __description__ = """Userupload.net downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
+    __authors__ = [("OzzieIsaacs", "ozzie.fernandez.isaacs@gmail.com")]
 
-    NAME_PATTERN = r'<div class="name">(?P<N>.+?)<'
-    SIZE_PATTERN = r'Rozmiar: <span class="type red">(?P<S>[\d.,]+) (?P<U>[\w_^]+)<'
+    PLUGIN_DOMAIN = "userupload.net"
 
-    LINK_PATTERN = r'<a href="(.+?)" target="_blank">Pobierz</a>'
+    NAME_PATTERN = r"<title>Download (?P<N>.+?)</title>"
+    SIZE_PATTERN = r"<span>File Size : (?P<S>[\d.,]+) (?P<U>[\w^_]+)</span>"
 
-    def handle_premium(self, pyfile):
-        self.data = self.load(
-            "https://tb7.pl/mojekonto/sciagaj", post={"step": 1, "content": pyfile.url}
-        )
+    LINK_PATTERN = r'<a href="(.+?)" type="button" class="btn btn-primary btn-block mb-4">'
 
-        m = re.search(self.NAME_PATTERN, self.data)
-        if m is not None:
-            pyfile.name = m.group("N")
-
-        m = re.search(self.SIZE_PATTERN, self.data)
-        if m is not None:
-            pyfile.size = parse.bytesize(m.group("S"), m.group("U"))
+    def handle_free(self, pyfile):
+        self.check_errors()
 
         self.data = self.load(
-            "https://tb7.pl/mojekonto/sciagaj", post={"step": 2, "0": "on"}
+            pyfile.url,
+            post=self._post_parameters(),
+            ref=self.pyfile.url,
+            redirect=False,
         )
 
-        if "Nieaktywne linki" in self.data:
-            self.temp_offline()
-
         m = re.search(self.LINK_PATTERN, self.data)
         if m is not None:
             self.link = m.group(1)
+            pyfile.name = self.link.split("/")[-1]
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TenluaVn.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TenluaVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TurbobitNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TurbobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TusfilesNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TusfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/TwoSharedCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/TwoSharedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UlozTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UlozTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UloziskoSk.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UloziskoSk.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UnibytesCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UnibytesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UpfileVn.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UpfileVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UpleaCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UpleaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UploadgigCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UploadgigCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UploadrocketNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UploadrocketNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UploadshipCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UploadshipCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UpstoreNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UpstoreNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UptoboxCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UptoboxCom.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 from ..base.simple_downloader import SimpleDownloader
 
 
 class UptoboxCom(SimpleDownloader):
     __name__ = "UptoboxCom"
     __type__ = "downloader"
-    __version__ = "0.38"
+    __version__ = "0.39"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?(uptobox|uptostream)\.com/\w{12}"
+    __pattern__ = r"https?://(?:www\.)?(uptobox|uptostream)\.(?:com|eu)/(?P<ID>\w{12})"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
@@ -23,28 +23,29 @@
     __description__ = """Uptobox.com downloader plugin"""
     __license__ = "GPLv3"
     __authors__ = [
         ("Walter Purcaro", "vuolter@gmail.com"),
         ("GammaC0de", "nitzo2001[AT]yahoo[DOT]com"),
     ]
 
-    PLUGIN_DOMAIN = "uptobox.com"
+    PLUGIN_DOMAIN = "uptobox.eu"
 
     INFO_PATTERN = (
         r"""(?:"para_title">|<h1(?: .*)?>)(?P<N>.+) \((?P<S>[\d.,]+) (?P<U>[\w^_]+)\)"""
     )
     OFFLINE_PATTERN = r"""(File not found|Access Denied|404 Not Found)"""
     TEMP_OFFLINE_PATTERN = r""">Service Unavailable"""
     WAIT_PATTERN = r"""data-remaining-time=["'](\d+)["']"""
     LINK_PATTERN = (
-        r"""["'](https?://(?:obwp\d+\.uptobox\.com|\w+\.uptobox\.com/dl?)/.*?)["']"""
+        r"""['"](https?://(?:obwp\d+\.uptobox\.(?:com|eu)|\w+\.uptobox\.(?:com|eu)/dl?)/.+?)['"]"""
     )
+    DIRECT_LINK = False
 
     DL_LIMIT_PATTERN = r"""or you can wait (.+) to launch a new download"""
-    URL_REPLACEMENTS = [("http://", "https://")]
+    URL_REPLACEMENTS = [(__pattern__ + ".*", r"https://uptobox.eu/\g<ID>")]
 
     def setup(self):
         self.multi_dl = self.premium
         self.chunk_limit = 1
         self.resume_download = True
 
     def handle_free(self, pyfile):
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UserscloudCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/UserscloudCom.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..base.xfs_downloader import XFSDownloader
 
 
 class UserscloudCom(XFSDownloader):
     __name__ = "UserscloudCom"
     __type__ = "downloader"
-    __version__ = "0.10"
+    __version__ = "0.11"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?userscloud\.com/(?P<ID>\w{12})"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/UseruploadNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/MexaSh.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 # -*- coding: utf-8 -*-
 
-import re
-
 from ..base.xfs_downloader import XFSDownloader
 
 
-class UseruploadNet(XFSDownloader):
-    __name__ = "UseruploadNet"
+class MexaSh(XFSDownloader):
+    __name__ = "MexaSh"
     __type__ = "downloader"
-    __version__ = "0.02"
+    __version__ = "0.01"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?userupload\.net/\w{12}"
+    __pattern__ = r"https?://(?:www\.)?(?:mexa\.sh|mexashare\.com)/(?P<ID>\w{12})"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Userupload.net downloader plugin"""
+    __description__ = """Mexa.sh downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("OzzieIsaacs", "ozzie.fernandez.isaacs@gmail.com")]
-
-    PLUGIN_DOMAIN = "userupload.net"
+    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
-    NAME_PATTERN = r"<title>Download (?P<N>.+?)</title>"
-    SIZE_PATTERN = r"<span>File Size : (?P<S>[\d.,]+) (?P<U>[\w^_]+)</span>"
+    PLUGIN_DOMAIN = "mexa.sh"
 
-    LINK_PATTERN = r'<a href="(.+?)" type="button" class="btn btn-primary btn-block mb-4">'
+    URL_REPLACEMENTS = [(__pattern__ + ".*", "https://mexa.sh/\g<ID>")]
 
-    def handle_free(self, pyfile):
-        self.check_errors()
+    NAME_PATTERN = r">You have requested the file.+?>(?P<N>.+?)</a>"
+    SIZE_PATTERN = r">\sFile Size\s: (?P<S>[\d.,]+)\s*(?P<U>[\w^_]+)"
 
-        self.data = self.load(
-            pyfile.url,
-            post=self._post_parameters(),
-            ref=self.pyfile.url,
-            redirect=False,
-        )
+    WAIT_PATTERN = r'class="seconds">(\d+)<'
+    DL_LIMIT_PATTERN = r"you can download this file after :.+?<a style='background.+?>(.+?)</a>"
 
-        m = re.search(self.LINK_PATTERN, self.data)
-        if m is not None:
-            self.link = m.group(1)
-            pyfile.name = self.link.split("/")[-1]
+    LINK_PATTERN = r"document.location = '(https://srv\d+.mexa.sh.+?)'"
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VeehdCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VeehdCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VeohCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VeohCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VidPlayNet.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VidPlayNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VimeoCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/VimeoCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/VkCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/WrzucajplikiPl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # -*- coding: utf-8 -*-
 
-#
-# Test links:
-#   http://vk.com/video_ext.php?oid=166335015&id=162608895&hash=b55affa83774504b&hd=1
-
 import re
 
-from ..base.simple_downloader import SimpleDownloader
+from ..base.xfs_downloader import XFSDownloader
 
 
-class VkCom(SimpleDownloader):
-    __name__ = "VkCom"
+class WrzucajplikiPl(XFSDownloader):
+    __name__ = "WrzucajplikiPl"
     __type__ = "downloader"
-    __version__ = "0.06"
+    __version__ = "0.03"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?vk\.com/video_ext\.php/\?.+"
+    __pattern__ = r"https?://(?:www\.)?wrzucajpliki\.pl/(?P<ID>\w{12})"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Vk.com downloader plugin"""
+    __description__ = """Wrzucajpliki.pl downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("Walter Purcaro", "vuolter@gmail.com")]
+    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
+
+    NAME_PATTERN = r'name="fname" value="(?P<N>.+?)"'
+    SIZE_PATTERN = r">You have requested .+?> \((?P<S>[\d.,]+) (?P<U>[\w^_]+)\)"
 
-    NAME_PATTERN = r'"md_title":"(?P<N>.+?)"'
-    OFFLINE_PATTERN = r'<div id="video_ext_msg">'
+    WAIT_PATTERN = r'<span class="seconds">(\d+)</span>'
+    DL_LIMIT_PATTERN = r">You have to wait (.+?) till next download<"
 
-    LINK_FREE_PATTERN = r'url\d+":"(.+?)"'
+    OFFLINE_PATTERN = r"File Not Found|No such file with this filename"
+    TEMP_OFFLINE_PATTERN = (
+        r"Connection limit reached|Server error|You have reached the download limit"
+    )
 
-    def handle_free(self, pyfile):
-        self.link = re.findall(self.LINK_FREE_PATTERN, self.data)[
-            0 if self.config.get("quality") == "Low" else -1
-        ]
+    PLUGIN_DOMAIN = "wrzucajpliki.pl"
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/WebshareCz.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/WebshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/WetransferCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/WetransferCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/WrzucTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/WrzucTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/WrzucajplikiPl.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/FilericeCom.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # -*- coding: utf-8 -*-
 
-import re
-
 from ..base.xfs_downloader import XFSDownloader
 
 
-class WrzucajplikiPl(XFSDownloader):
-    __name__ = "WrzucajplikiPl"
+class FilericeCom(XFSDownloader):
+    __name__ = "FilericeCom"
     __type__ = "downloader"
-    __version__ = "0.03"
+    __version__ = "0.01"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?wrzucajpliki\.pl/(?P<ID>\w{12})"
+    __pattern__ = r"https?://(?:www\.)?filerice\.com/(?P<ID>\w{12})"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Wrzucajpliki.pl downloader plugin"""
+    __description__ = """Filerice.com downloader plugin"""
     __license__ = "GPLv3"
     __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
-    NAME_PATTERN = r'name="fname" value="(?P<N>.+?)"'
-    SIZE_PATTERN = r">You have requested .+?> \((?P<S>[\d.,]+) (?P<U>[\w^_]+)\)"
+    NAME_PATTERN = r'<div class="name">[^>]*>(?P<N>.+?)<'
+    SIZE_PATTERN = r"<span>Size (?P<S>[\d.,]+) (?P<U>[\w^_]+)<"
 
     WAIT_PATTERN = r'<span class="seconds">(\d+)</span>'
     DL_LIMIT_PATTERN = r">You have to wait (.+?) till next download<"
 
-    OFFLINE_PATTERN = r"File Not Found|No such file with this filename"
-    TEMP_OFFLINE_PATTERN = (
-        r"Connection limit reached|Server error|You have reached the download limit"
-    )
-
-    PLUGIN_DOMAIN = "wrzucajpliki.pl"
+    PLUGIN_DOMAIN = "filerice.com"
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XDCC.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XDCC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XFileSharing.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XFileSharing.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XHamsterCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XHamsterCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XVideosCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XVideosCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/XdadevelopersCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/XdadevelopersCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YadiSk.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YadiSk.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YesPornPleaseCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YesPornPleaseCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YibaishiwuCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YibaishiwuCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YoupornCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YoupornCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YourfilesTo.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YourfilesTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/YoutubeCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/YoutubeCom.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
         return to_str(last_line)  #: Last line may contain error message
 
 
 class YoutubeCom(BaseDownloader):
     __name__ = "YoutubeCom"
     __type__ = "downloader"
-    __version__ = "0.87"
+    __version__ = "0.88"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:[^/]*\.)?(?:youtu\.be/|youtube\.com/watch\?(?:.*&)?v=)[\w\-]+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         (
             "quality",
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ZDF.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ZDF.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ZbigzCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ZbigzCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/downloaders/ZeveraCom.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/downloaders/ZeveraCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/HjSplit.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/HjSplit.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/SevenZip.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/SevenZip.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/UnRar.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/UnRar.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/UnTar.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/UnTar.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/extractors/UnZip.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/extractors/UnZip.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/plugins/helpers.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/plugins/helpers.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/__init__.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/__init__.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/api_blueprint.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/api_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/app_blueprint.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/app_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/cnl_blueprint.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/cnl_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/blueprints/json_blueprint.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/blueprints/json_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/config.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/config.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/extensions.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/extensions.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/filters.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/filters.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/handlers.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/handlers.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/helpers.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/helpers.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/processors.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/processors.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/css/base.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/css/logs.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/css/logs.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/css/pathchooser.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/css/pathchooser.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/css/window.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/css/window.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/add_folder.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/add_folder.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/arrow-refresh.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/arrow-refresh.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/cog.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/cog.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-add-blue.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-add-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-cancel-blue.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-cancel-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-cancel.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-cancel.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-pause-blue.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-pause-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-pause.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-pause.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-play-blue.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-play-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-play.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-play.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/control-stop-blue.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/control-stop-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/delete.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/delete.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/dialog-close.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/dialog-close.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/dialog-question.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/dialog-question.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/error.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/error.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/favicon.ico` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/folder.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/folder.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-login.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-login.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-collector.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-collector.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-config.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-config.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-development.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-development.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-download.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-download.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-home.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-home.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-news.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-news.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-queue.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-queue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-recent.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-recent.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-menu-wiki.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-menu-wiki.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/head-search-noshadow.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/head-search-noshadow.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/images.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/images.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/notice.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/notice.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/package-go.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/package-go.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/page-tools-backlinks.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/page-tools-backlinks.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/page-tools-edit.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/page-tools-edit.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/page-tools-revisions.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/page-tools-revisions.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/parse-uri.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/parse-uri.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/pyload-logo.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/pyload-logo.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/reconnect.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/reconnect.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-downloading.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-downloading.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-failed.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-failed.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-finished.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-finished.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-none.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-none.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-offline.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-offline.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-proc.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-proc.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-queue.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-queue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/status-waiting.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/status-waiting.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/success.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/success.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/user-actions-logout.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/user-actions-logout.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/user-actions-profile.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/user-actions-profile.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/img/user-info.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/img/user-info.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/js/captcha-interactive.user.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/js/captcha-interactive.user.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/base.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/captcha.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/captcha.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/dashboard.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/filemanager.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/filemanager.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/files.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/files.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/folder.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/folder.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/info.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/info.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/base.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/base.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/dashboard.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/filemanager.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/filemanager.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/packages.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/packages.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/js/settings.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/login.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/login.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/logs.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/logs.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/packages.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/packages.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/pathchooser.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/pathchooser.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/settings.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/settings.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/settings_item.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/settings_item.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/templates/window.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/templates/window.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/base.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/logs.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/logs.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/pathchooser.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/pathchooser.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/css/settings.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/css/settings.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/favicon.ico` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/base.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/captcha.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/captcha.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/dashboard.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/files.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/files.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/info.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/info.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/base.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/base.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -390,14 +390,15 @@
     params = JSON.parse(a.params);
     $("#cap_id").val(a.id);
     if (a.result_type === "textual") {
         $("#cap_textual_img").attr("src", params.src);
         $("#cap_submit").css("display", "inline");
         $("#cap_box #cap_title").text("");
         $("#cap_textual").css("display", "block");
+        $("#cap_result").focus();
     } else if (a.result_type === "positional") {
         $("#cap_positional_img").attr("src", params.src);
         $("#cap_box #cap_title").text("{{_('Please click on the right captcha position.')}}");
         $("#cap_positional").css("display", "block");
     } else if (a.result_type === "interactive") {
         $("#cap_box #cap_title").text("");
         if (interactiveCaptchaHandlerInstance == null) {
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/dashboard.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/info.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/info.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/packages.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/packages.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/js/settings.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/login.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/login.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/logs.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/logs.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/packages.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/packages.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/pathchooser.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/pathchooser.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/settings.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/settings.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/settings_item.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/settings_item.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/modern/templates/window.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/modern/templates/window.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/base.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/logs.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/logs.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/css/settings.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/css/settings.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/base.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/captcha.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/captcha.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/dashboard.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/files.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/files.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/info.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/info.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/base.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/base.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -390,14 +390,15 @@
     params = JSON.parse(a.params);
     $("#cap_id").val(a.id);
     if (a.result_type === "textual") {
         $("#cap_textual_img").attr("src", params.src);
         $("#cap_submit").css("display", "inline");
         $("#cap_box #cap_title").text("");
         $("#cap_textual").css("display", "block");
+        $("#cap_result").focus();
     } else if (a.result_type === "positional") {
         $("#cap_positional_img").attr("src", params.src);
         $("#cap_box #cap_title").text("{{_('Please click on the right captcha position.')}}");
         $("#cap_positional").css("display", "block");
     } else if (a.result_type === "interactive") {
         $("#cap_box #cap_title").text("");
         if (interactiveCaptchaHandlerInstance == null) {
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/info.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/info.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/packages.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/packages.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/js/settings.js` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/login.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/login.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/logs.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/logs.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/packages.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/packages.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/settings.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/settings.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/settings_item.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/settings_item.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/app/themes/pyplex/templates/window.html` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/app/themes/pyplex/templates/window.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload/webui/webserver_thread.py` & `pyload-ng-0.5.0b3.dev72/src/pyload/webui/webserver_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/PKG-INFO` & `pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyload-ng
-Version: 0.5.0b3.dev71
+Version: 0.5.0b3.dev72
 Summary: The free and open-source Download Manager written in pure Python
 Home-page: https://pyload.net
 Download-URL: https://github.com/pyload/pyload/releases
 Author: pyLoad team
 Author-email: support@pyload.net
 Maintainer: Walter Purcaro
 Maintainer-email: vuolter@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyload-ng Version: 0.5.0b3.dev71 Summary: The free
+Metadata-Version: 2.1 Name: pyload-ng Version: 0.5.0b3.dev72 Summary: The free
 and open-source Download Manager written in pure Python Home-page: https://
 pyload.net Download-URL: https://github.com/pyload/pyload/releases Author:
 pyLoad team Author-email: support@pyload.net Maintainer: Walter Purcaro
 Maintainer-email: vuolter@gmail.com License: agpl3 Project-URL: Source Code
 (mirror), https://gitlab.com/pyload/pyload Project-URL: Source Code, https://
 github.com/pyload/pyload Project-URL: Bug Tracker, https://github.com/pyload/
 pyload/issues Project-URL: Documentation, https://github.com/pyload/pyload/wiki
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/SOURCES.txt` & `pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 src/pyload/plugins/accounts/FilecloudIo.py
 src/pyload/plugins/accounts/FilefactoryCom.py
 src/pyload/plugins/accounts/FilejokerNet.py
 src/pyload/plugins/accounts/FileomCom.py
 src/pyload/plugins/accounts/FilerNet.py
 src/pyload/plugins/accounts/FilerioCom.py
 src/pyload/plugins/accounts/FilesMailRu.py
+src/pyload/plugins/accounts/FiregetCom.py
 src/pyload/plugins/accounts/FourSharedCom.py
 src/pyload/plugins/accounts/FshareVn.py
 src/pyload/plugins/accounts/Ftp.py
 src/pyload/plugins/accounts/GetTwentyFourOrg.py
 src/pyload/plugins/accounts/HellshareCz.py
 src/pyload/plugins/accounts/HighWayMe.py
 src/pyload/plugins/accounts/Http.py
@@ -149,15 +150,14 @@
 src/pyload/plugins/accounts/NitrobitNet.py
 src/pyload/plugins/accounts/NitroflareCom.py
 src/pyload/plugins/accounts/NoPremiumPl.py
 src/pyload/plugins/accounts/NosuploadCom.py
 src/pyload/plugins/accounts/NovafileCom.py
 src/pyload/plugins/accounts/NowVideoSx.py
 src/pyload/plugins/accounts/OneFichierCom.py
-src/pyload/plugins/accounts/OpenloadCo.py
 src/pyload/plugins/accounts/OverLoadMe.py
 src/pyload/plugins/accounts/PorntrexCom.py
 src/pyload/plugins/accounts/PremiumTo.py
 src/pyload/plugins/accounts/PremiumizeMe.py
 src/pyload/plugins/accounts/PutdriveCom.py
 src/pyload/plugins/accounts/QuickshareCz.py
 src/pyload/plugins/accounts/RPNetBiz.py
@@ -181,15 +181,14 @@
 src/pyload/plugins/accounts/TurbobitNet.py
 src/pyload/plugins/accounts/TusfilesNet.py
 src/pyload/plugins/accounts/TwojlimitPl.py
 src/pyload/plugins/accounts/UlozTo.py
 src/pyload/plugins/accounts/UpleaCom.py
 src/pyload/plugins/accounts/UploadcCom.py
 src/pyload/plugins/accounts/UploadgigCom.py
-src/pyload/plugins/accounts/UploadheroCom.py
 src/pyload/plugins/accounts/UpstoreNet.py
 src/pyload/plugins/accounts/UptoboxCom.py
 src/pyload/plugins/accounts/VidPlayNet.py
 src/pyload/plugins/accounts/WebshareCz.py
 src/pyload/plugins/accounts/WorldbytezCom.py
 src/pyload/plugins/accounts/WrzucajplikiPl.py
 src/pyload/plugins/accounts/YibaishiwuCom.py
@@ -272,23 +271,21 @@
 src/pyload/plugins/containers/__init__.py
 src/pyload/plugins/decrypters/AlldebridComTorrent.py
 src/pyload/plugins/decrypters/ArchiveOrgFolder.py
 src/pyload/plugins/decrypters/ChipDe.py
 src/pyload/plugins/decrypters/CloudMailRuFolder.py
 src/pyload/plugins/decrypters/CloudzillaToFolder.py
 src/pyload/plugins/decrypters/CriptTo.py
-src/pyload/plugins/decrypters/CryptCat.py
 src/pyload/plugins/decrypters/CzshareComFolder.py
 src/pyload/plugins/decrypters/DailymotionComFolder.py
 src/pyload/plugins/decrypters/DataHuFolder.py
 src/pyload/plugins/decrypters/DebridlinkFrTorrent.py
 src/pyload/plugins/decrypters/DepositfilesComFolder.py
 src/pyload/plugins/decrypters/Dereferer.py
 src/pyload/plugins/decrypters/DevhostStFolder.py
-src/pyload/plugins/decrypters/DlProtectCom.py
 src/pyload/plugins/decrypters/EasybytezComFolder.py
 src/pyload/plugins/decrypters/EmbeduploadCom.py
 src/pyload/plugins/decrypters/FilecloudIoFolder.py
 src/pyload/plugins/decrypters/FilecryptCc.py
 src/pyload/plugins/decrypters/FilefactoryComFolder.py
 src/pyload/plugins/decrypters/FilerNetFolder.py
 src/pyload/plugins/decrypters/FilestubeCom.py
@@ -328,14 +325,15 @@
 src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py
 src/pyload/plugins/decrypters/TenluaVnFolder.py
 src/pyload/plugins/decrypters/TinyurlCom.py
 src/pyload/plugins/decrypters/TnyCz.py
 src/pyload/plugins/decrypters/TurbobitNetFolder.py
 src/pyload/plugins/decrypters/TusfilesNetFolder.py
 src/pyload/plugins/decrypters/UlozToFolder.py
+src/pyload/plugins/decrypters/WetransferComDereferer.py
 src/pyload/plugins/decrypters/XFileSharingFolder.py
 src/pyload/plugins/decrypters/XupPl.py
 src/pyload/plugins/decrypters/YoutubeComFolder.py
 src/pyload/plugins/decrypters/__init__.py
 src/pyload/plugins/downloaders/AccioDebridCom.py
 src/pyload/plugins/downloaders/AlfafileNet.py
 src/pyload/plugins/downloaders/AlldebridCom.py
@@ -377,21 +375,21 @@
 src/pyload/plugins/downloaders/FastshareCz.py
 src/pyload/plugins/downloaders/FikperCom.py
 src/pyload/plugins/downloaders/FileAl.py
 src/pyload/plugins/downloaders/FileSharkPl.py
 src/pyload/plugins/downloaders/FileStoreTo.py
 src/pyload/plugins/downloaders/FileboomMe.py
 src/pyload/plugins/downloaders/FilecloudIo.py
-src/pyload/plugins/downloaders/FiledropperCom.py
 src/pyload/plugins/downloaders/FilefactoryCom.py
 src/pyload/plugins/downloaders/FilefoxCc.py
 src/pyload/plugins/downloaders/FilejokerNet.py
 src/pyload/plugins/downloaders/FileomCom.py
 src/pyload/plugins/downloaders/FilepupNet.py
 src/pyload/plugins/downloaders/FilerNet.py
+src/pyload/plugins/downloaders/FilericeCom.py
 src/pyload/plugins/downloaders/FilerioCom.py
 src/pyload/plugins/downloaders/FilesMailRu.py
 src/pyload/plugins/downloaders/FileuploadCom.py
 src/pyload/plugins/downloaders/FileuploadNet.py
 src/pyload/plugins/downloaders/FiregetCom.py
 src/pyload/plugins/downloaders/FistfastNet.py
 src/pyload/plugins/downloaders/FlyFilesNet.py
@@ -434,14 +432,15 @@
 src/pyload/plugins/downloaders/MegaDebridEu.py
 src/pyload/plugins/downloaders/MegaRapidCz.py
 src/pyload/plugins/downloaders/MegaRapidoNet.py
 src/pyload/plugins/downloaders/MegacrypterCom.py
 src/pyload/plugins/downloaders/MegadyskPl.py
 src/pyload/plugins/downloaders/MegasharesCom.py
 src/pyload/plugins/downloaders/MegaupNet.py
+src/pyload/plugins/downloaders/MexaSh.py
 src/pyload/plugins/downloaders/MovReelCom.py
 src/pyload/plugins/downloaders/MultihostersCom.py
 src/pyload/plugins/downloaders/MultishareCz.py
 src/pyload/plugins/downloaders/MyfastfileCom.py
 src/pyload/plugins/downloaders/MystoreTo.py
 src/pyload/plugins/downloaders/NarodRu.py
 src/pyload/plugins/downloaders/NippyshareCom.py
@@ -450,15 +449,14 @@
 src/pyload/plugins/downloaders/NoPremiumPl.py
 src/pyload/plugins/downloaders/NofileIo.py
 src/pyload/plugins/downloaders/NosuploadCom.py
 src/pyload/plugins/downloaders/NovafileCom.py
 src/pyload/plugins/downloaders/NowVideoSx.py
 src/pyload/plugins/downloaders/OneFichierCom.py
 src/pyload/plugins/downloaders/OnlineTvRecorder.py
-src/pyload/plugins/downloaders/OpenloadIo.py
 src/pyload/plugins/downloaders/OverLoadMe.py
 src/pyload/plugins/downloaders/PixeldrainCom.py
 src/pyload/plugins/downloaders/PornhostCom.py
 src/pyload/plugins/downloaders/PornhubCom.py
 src/pyload/plugins/downloaders/PornovkaCz.py
 src/pyload/plugins/downloaders/PorntrexCom.py
 src/pyload/plugins/downloaders/PremiumTo.py
@@ -502,15 +500,14 @@
 src/pyload/plugins/downloaders/TwojlimitPl.py
 src/pyload/plugins/downloaders/UlozTo.py
 src/pyload/plugins/downloaders/UloziskoSk.py
 src/pyload/plugins/downloaders/UnibytesCom.py
 src/pyload/plugins/downloaders/UpfileVn.py
 src/pyload/plugins/downloaders/UpleaCom.py
 src/pyload/plugins/downloaders/UploadgigCom.py
-src/pyload/plugins/downloaders/UploadheroCom.py
 src/pyload/plugins/downloaders/UploadrocketNet.py
 src/pyload/plugins/downloaders/UploadshipCom.py
 src/pyload/plugins/downloaders/UpstoreNet.py
 src/pyload/plugins/downloaders/UptoboxCom.py
 src/pyload/plugins/downloaders/UserscloudCom.py
 src/pyload/plugins/downloaders/UseruploadNet.py
 src/pyload/plugins/downloaders/VeehdCom.py
@@ -532,15 +529,14 @@
 src/pyload/plugins/downloaders/YibaishiwuCom.py
 src/pyload/plugins/downloaders/YoupornCom.py
 src/pyload/plugins/downloaders/YourfilesTo.py
 src/pyload/plugins/downloaders/YoutubeCom.py
 src/pyload/plugins/downloaders/ZDF.py
 src/pyload/plugins/downloaders/ZbigzCom.py
 src/pyload/plugins/downloaders/ZeveraCom.py
-src/pyload/plugins/downloaders/ZippyshareCom.py
 src/pyload/plugins/downloaders/__init__.py
 src/pyload/plugins/extractors/HjSplit.py
 src/pyload/plugins/extractors/SevenZip.py
 src/pyload/plugins/extractors/UnRar.py
 src/pyload/plugins/extractors/UnTar.py
 src/pyload/plugins/extractors/UnZip.py
 src/pyload/plugins/extractors/__init__.py
```

### Comparing `pyload-ng-0.5.0b3.dev71/src/pyload_ng.egg-info/requires.txt` & `pyload-ng-0.5.0b3.dev72/src/pyload_ng.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/tests/api_exerciser.py` & `pyload-ng-0.5.0b3.dev72/tests/api_exerciser.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/tests/system_check.py` & `pyload-ng-0.5.0b3.dev72/tests/system_check.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev71/tests/test_json.py` & `pyload-ng-0.5.0b3.dev72/tests/test_json.py`

 * *Files identical despite different names*

