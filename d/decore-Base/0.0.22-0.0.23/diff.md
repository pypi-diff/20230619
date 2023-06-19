# Comparing `tmp/decore_Base-0.0.22.tar.gz` & `tmp/decore_Base-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decore_Base-0.0.22.tar", last modified: Fri Jun 16 13:40:35 2023, max compression
+gzip compressed data, was "decore_Base-0.0.23.tar", last modified: Mon Jun 19 13:19:09 2023, max compression
```

## Comparing `decore_Base-0.0.22.tar` & `decore_Base-0.0.23.tar`

### file list

```diff
@@ -1,236 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.317565 decore_Base-0.0.22/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.289566 decore_Base-0.0.22/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-16 13:40:27.000000 decore_Base-0.0.22/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.289566 decore_Base-0.0.22/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 13:40:27.000000 decore_Base-0.0.22/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-16 13:40:27.000000 decore_Base-0.0.22/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.293566 decore_Base-0.0.22/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-16 13:40:27.000000 decore_Base-0.0.22/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-16 13:40:27.000000 decore_Base-0.0.22/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-16 13:40:27.000000 decore_Base-0.0.22/KOFI.md
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-16 13:40:27.000000 decore_Base-0.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-16 13:40:35.317565 decore_Base-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-16 13:40:27.000000 decore_Base-0.0.22/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-06-16 13:40:27.000000 decore_Base-0.0.22/README_DE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.293566 decore_Base-0.0.22/decore_Base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-16 13:40:35.000000 decore_Base-0.0.22/decore_Base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-16 13:40:35.000000 decore_Base-0.0.22/decore_Base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:40:35.000000 decore_Base-0.0.22/decore_Base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 13:40:35.000000 decore_Base-0.0.22/decore_Base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 13:40:35.000000 decore_Base-0.0.22/decore_Base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.293566 decore_Base-0.0.22/decore_base/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.293566 decore_Base-0.0.22/decore_base/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/classes/decore_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/decore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.293566 decore_Base-0.0.22/decore_base/library/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.293566 decore_Base-0.0.22/decore_base/library/particl_market/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/particl_market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/particl_market/particl_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/powershell2.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/return_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.293566 decore_Base-0.0.22/decore_base/library/roaster/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/roaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/roaster/roaster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/roaster/roaster_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/library/roaster/roaster_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.293566 decore_Base-0.0.22/decore_base/prepare/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.293566 decore_Base-0.0.22/decore_base/prepare/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/.vscode/launch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.289566 decore_Base-0.0.22/decore_base/prepare/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.297566 decore_Base-0.0.22/decore_base/prepare/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.297566 decore_Base-0.0.22/decore_base/prepare/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/css/586.ed179a62.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.297566 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.297566 decore_Base-0.0.22/decore_base/prepare/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.301566 decore_Base-0.0.22/decore_base/prepare/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/js/586.aa14c175.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/js/app.af6cbe84.js
--rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/static/js/vendor.0902ddb5.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.301566 decore_Base-0.0.22/decore_base/prepare/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/prepare/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.301566 decore_Base-0.0.22/decore_base/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.301566 decore_Base-0.0.22/decore_base/sample/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.301566 decore_Base-0.0.22/decore_base/sample/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/bases/account_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/bases/company_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/bases/global_management_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/bases/information_stytem_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/bases/person_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/bases/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/language.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.301566 decore_Base-0.0.22/decore_base/sample/models/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/models/account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/models/company_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/models/person_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/models/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.289566 decore_Base-0.0.22/decore_base/sample/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.301566 decore_Base-0.0.22/decore_base/sample/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.301566 decore_Base-0.0.22/decore_base/sample/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/css/586.ed179a62.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.305565 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.305565 decore_Base-0.0.22/decore_base/sample/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.305565 decore_Base-0.0.22/decore_base/sample/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/js/586.aa14c175.js
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/js/app.af6cbe84.js
--rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/static/js/vendor.0902ddb5.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.305565 decore_Base-0.0.22/decore_base/sample/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.309565 decore_Base-0.0.22/decore_base/sample/state/
--rw-r--r--   0 runner    (1001) docker     (123)  1363968 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/state/database.db
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/sample/state/querybase.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.309565 decore_Base-0.0.22/decore_base/uniform/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/uniform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/uniform/conform_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.309565 decore_Base-0.0.22/decore_base/uniform/depricated/
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/uniform/depricated/askform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/uniform/depricated/buyform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/uniform/depricated/conform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/uniform/depricated/deform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/uniform/perform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/uniform/reform_client_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-16 13:40:27.000000 decore_Base-0.0.22/decore_base/uniform/reform_server_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.309565 decore_Base-0.0.22/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.309565 decore_Base-0.0.22/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.309565 decore_Base-0.0.22/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/_static/styles/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/config.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/decore.rst.out
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/language.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/model.rst.out
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.289566 decore_Base-0.0.22/docs/page/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.309565 decore_Base-0.0.22/docs/page/doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)    79302 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    46211 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/doctrees/index.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.309565 decore_Base-0.0.22/docs/page/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.313565 decore_Base-0.0.22/docs/page/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_sources/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.313565 decore_Base-0.0.22/docs/page/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/pygments.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.313565 decore_Base-0.0.22/docs/page/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    80813 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/scripts/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   335757 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.313565 decore_Base-0.0.22/docs/page/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   176654 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/styles/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/styles/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    63341 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/styles/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.289566 decore_Base-0.0.22/docs/page/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.289566 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.313565 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.313565 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 runner    (1001) docker     (123)   101691 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.317565 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181264 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105112 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60236 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   389948 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   154840 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    43241 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/page/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:40:35.317565 decore_Base-0.0.22/docs/state/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-16 13:40:27.000000 decore_Base-0.0.22/docs/state/querybase.db
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-16 13:40:27.000000 decore_Base-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 13:40:27.000000 decore_Base-0.0.22/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-16 13:40:35.317565 decore_Base-0.0.22/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.549661 decore_Base-0.0.23/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-19 13:18:55.000000 decore_Base-0.0.23/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-19 13:18:55.000000 decore_Base-0.0.23/KOFI.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-19 13:18:55.000000 decore_Base-0.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-06-19 13:19:09.549661 decore_Base-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-06-19 13:18:55.000000 decore_Base-0.0.23/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-06-19 13:18:55.000000 decore_Base-0.0.23/README_DE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_Base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 13:19:09.000000 decore_Base-0.0.23/decore_Base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/classes/decore_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/decore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/library/particl_market/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/particl_market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/particl_market/particl_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/powershell2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/library/roaster/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/roaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/roaster/roaster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/roaster/roaster_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/library/roaster/roaster_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/prepare/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/prepare/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/.vscode/launch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.517661 decore_Base-0.0.23/decore_base/prepare/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/prepare/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.525661 decore_Base-0.0.23/decore_base/prepare/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/css/586.ed179a62.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.529661 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.529661 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.529661 decore_Base-0.0.23/decore_base/prepare/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/js/586.aa14c175.js
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/js/app.af6cbe84.js
+-rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/static/js/vendor.0902ddb5.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.529661 decore_Base-0.0.23/decore_base/prepare/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/prepare/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/account_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/company_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/global_management_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/information_stytem_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/person_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/bases/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/language.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/models/account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/models/company_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/models/person_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/models/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/decore_base/sample/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.533661 decore_Base-0.0.23/decore_base/sample/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/css/586.ed179a62.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.537661 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.537661 decore_Base-0.0.23/decore_base/sample/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.537661 decore_Base-0.0.23/decore_base/sample/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/js/586.aa14c175.js
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/js/app.af6cbe84.js
+-rw-r--r--   0 runner    (1001) docker     (123)   376226 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/static/js/vendor.0902ddb5.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.537661 decore_Base-0.0.23/decore_base/sample/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/decore_base/sample/state/
+-rw-r--r--   0 runner    (1001) docker     (123)  1363968 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/state/database.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/state/keybase.kdbx
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/sample/state/querybase.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/decore_base/uniform/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/conform_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/decore_base/uniform/depricated/
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/depricated/askform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/depricated/buyform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/depricated/conform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/depricated/deform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/perform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/reform_client_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-19 13:18:55.000000 decore_Base-0.0.23/decore_base/uniform/reform_server_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/_static/styles/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/decore.rst.out
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/language.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/model.rst.out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/docs/page/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/page/doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)    79165 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    46074 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/page/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.541661 decore_Base-0.0.23/docs/page/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/pygments.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    80813 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   335757 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   176654 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/styles/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/styles/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    63341 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/styles/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/docs/page/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.521661 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.545661 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   101691 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.549661 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181264 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105112 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60236 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   389948 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   154840 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42879 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/page/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:19:09.549661 decore_Base-0.0.23/docs/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/state/keybase.kdbx
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-19 13:18:55.000000 decore_Base-0.0.23/docs/state/querybase.db
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 13:18:55.000000 decore_Base-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-19 13:18:55.000000 decore_Base-0.0.23/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-19 13:19:09.549661 decore_Base-0.0.23/setup.cfg
```

### Comparing `decore_Base-0.0.22/.github/FUNDING.yml` & `decore_Base-0.0.23/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/.gitignore` & `decore_Base-0.0.23/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/.vscode/launch.json` & `decore_Base-0.0.23/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/KOFI.md` & `decore_Base-0.0.23/KOFI.md`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/LICENSE` & `decore_Base-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/PKG-INFO` & `decore_Base-0.0.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore_Base
-Version: 0.0.22
+Version: 0.0.23
 Summary: decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 Home-page: https://www.decore.dev
 Author: Kemo Panzah
 Project-URL: Funding, https://ko-fi.com/decore_Base
 Project-URL: Source, https://github.com/KemoPanzah/decore_Base
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -226,22 +226,20 @@
          def first_view():
             @decore.dialog(title='Add Person', icon='mdi-plus', type='standard', display='drawer', activator='default-menu')
             def first_dialog():
                @decore.widget(title='Add Person Form', icon='mdi-account', type='form', fields=[First_model.firstname, First_model.lastname])
                def first_widget():
                   @decore.action(title='Save Person', icon='mdi-content-save', type='submit')
                   def first_action(self, data):
-                     item = First_model()
-                     item.title = data['firstname'] + ' ' + data['lastname']
-                     item.firstname = data['firstname']
-                     item.lastname = data['lastname']
+                     item = First_model(data['item'])
+                     item.title = item.firstname + ' ' + item.lastname
                      if item.save():
                         return True, item.title + ' saved successfully'
                      else:
-                        return False, item.error
+                        return False, 'Error while saving ' + item.title
 
 .. note::
    To create a record with decore Base, we need to create an instance of the model. In our case **First_model**. The instance is filled with the data from the form and then saved.
 
    The ID in the form of a UUID is generated automatically and does not have to be specified separately.
 
 .. warning::
```

### Comparing `decore_Base-0.0.22/README.rst` & `decore_Base-0.0.23/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -212,22 +212,20 @@
          def first_view():
             @decore.dialog(title='Add Person', icon='mdi-plus', type='standard', display='drawer', activator='default-menu')
             def first_dialog():
                @decore.widget(title='Add Person Form', icon='mdi-account', type='form', fields=[First_model.firstname, First_model.lastname])
                def first_widget():
                   @decore.action(title='Save Person', icon='mdi-content-save', type='submit')
                   def first_action(self, data):
-                     item = First_model()
-                     item.title = data['firstname'] + ' ' + data['lastname']
-                     item.firstname = data['firstname']
-                     item.lastname = data['lastname']
+                     item = First_model(data['item'])
+                     item.title = item.firstname + ' ' + item.lastname
                      if item.save():
                         return True, item.title + ' saved successfully'
                      else:
-                        return False, item.error
+                        return False, 'Error while saving ' + item.title
 
 .. note::
    To create a record with decore Base, we need to create an instance of the model. In our case **First_model**. The instance is filled with the data from the form and then saved.
 
    The ID in the form of a UUID is generated automatically and does not have to be specified separately.
 
 .. warning::
```

### Comparing `decore_Base-0.0.22/README_DE.rst` & `decore_Base-0.0.23/README_DE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -212,22 +212,20 @@
          def first_view():
             @decore.dialog(title='Add Person', icon='mdi-plus', type='standard', display='drawer', activator='default-menu')
             def first_dialog():
                @decore.widget(title='Add Person Form', icon='mdi-account', type='form', fields=[First_model.firstname, First_model.lastname])
                def first_widget():
                   @decore.action(title='Save Person', icon='mdi-content-save', type='submit')
                   def first_action(self, data):
-                     item = First_model()
-                     item.title = data['firstname'] + ' ' + data['lastname']
-                     item.firstname = data['firstname']
-                     item.lastname = data['lastname']
+                     item = First_model(data['item'])
+                     item.title = item.firstname + ' ' + item.lastname
                      if item.save():
                         return True, item.title + ' saved successfully'
                      else:
-                        return False, item.error
+                        return False, 'Error while saving ' + item.title
 
 .. note::
    Um mit decore Base einen Datensatz zu erzeugen, müssen wir eine Instanz vom Model erzeugen. In unserem Fall **First_model**. Die Instanz wird mit den Daten aus dem Formular befüllt und anschließend gespeichert.
 
    Die ID in Form einer UUID wird automatisch generiert und muss nicht extra angegeben werden.
 
 .. warning::
```

### Comparing `decore_Base-0.0.22/decore_Base.egg-info/PKG-INFO` & `decore_Base-0.0.23/decore_Base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore-Base
-Version: 0.0.22
+Version: 0.0.23
 Summary: decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 Home-page: https://www.decore.dev
 Author: Kemo Panzah
 Project-URL: Funding, https://ko-fi.com/decore_Base
 Project-URL: Source, https://github.com/KemoPanzah/decore_Base
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -226,22 +226,20 @@
          def first_view():
             @decore.dialog(title='Add Person', icon='mdi-plus', type='standard', display='drawer', activator='default-menu')
             def first_dialog():
                @decore.widget(title='Add Person Form', icon='mdi-account', type='form', fields=[First_model.firstname, First_model.lastname])
                def first_widget():
                   @decore.action(title='Save Person', icon='mdi-content-save', type='submit')
                   def first_action(self, data):
-                     item = First_model()
-                     item.title = data['firstname'] + ' ' + data['lastname']
-                     item.firstname = data['firstname']
-                     item.lastname = data['lastname']
+                     item = First_model(data['item'])
+                     item.title = item.firstname + ' ' + item.lastname
                      if item.save():
                         return True, item.title + ' saved successfully'
                      else:
-                        return False, item.error
+                        return False, 'Error while saving ' + item.title
 
 .. note::
    To create a record with decore Base, we need to create an instance of the model. In our case **First_model**. The instance is filled with the data from the form and then saved.
 
    The ID in the form of a UUID is generated automatically and does not have to be specified separately.
 
 .. warning::
```

### Comparing `decore_Base-0.0.22/decore_Base.egg-info/SOURCES.txt` & `decore_Base-0.0.23/decore_Base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_Base.egg-info/requires.txt` & `decore_Base-0.0.23/decore_Base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/classes/decore_base.py` & `decore_Base-0.0.23/decore_base/classes/decore_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/classes/decore_list.py` & `decore_Base-0.0.23/decore_base/classes/decore_list.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/classes/decore_model.py` & `decore_Base-0.0.23/decore_base/classes/decore_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,14 +324,15 @@
         if not t_group:
             t_group = globals.kdb.add_group(globals.kdb.root_group, self.__class__.__name__)
             globals.kdb.save()
         return t_group
 
     def validate(self):
         t_schema = self.build_schema()
+        #TODO - Schema as property and Validator as attribute in model
         t_val = Validator(t_schema, require_all=True, allow_unknown = True)
         r_value =  t_val.validate(self.__data__)
         if r_value == False:
             logging.error('%s > %s' % ('validate_model', str(t_val.errors)))
         return r_value
 
     # TODO - Wer ruft das auf? was ist damit?
```

### Comparing `decore_Base-0.0.22/decore_base/classes/decore_pool.py` & `decore_Base-0.0.23/decore_base/classes/decore_pool.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/classes/decore_prompt.py` & `decore_Base-0.0.23/decore_base/classes/decore_prompt.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/classes/decore_query.py` & `decore_Base-0.0.23/decore_base/classes/decore_query.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/classes/decore_return.py` & `decore_Base-0.0.23/decore_base/classes/decore_return.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/classes/decore_translate.py` & `decore_Base-0.0.23/decore_base/classes/decore_translate.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/classes/decore_view.py` & `decore_Base-0.0.23/decore_base/classes/decore_view.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/decore.py` & `decore_Base-0.0.23/decore_base/decore.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,23 +114,23 @@
             t_base.schema = model.build_schema()
             self.pool.register(t_base)
         return wrapper
 
     l_view_type = Literal['table']
     l_view_pag_type = Literal['client']
 
-    def view(self, parent_id=None, icon=None, title=None, desc=None, type: l_view_type = 'table', fields=[], filter_s=[], query={}, pag_type: l_view_pag_type = 'client', pag_recs=16):
+    def view(self, parent_id=None, icon=None, title=None, desc=None, type: l_view_type = 'table', fields=[], filters=[], query={}, pag_type: l_view_pag_type = 'client', pag_recs=16):
         def wrapper(func):
             t_parent_s = func.__qualname__.replace('.<locals>', '').rsplit('.')
             if not parent_id:
                 t_parent_id = t_parent_s[-2]
             else:
                 t_parent_id = parent_id
             t_source_id = t_parent_s[0]
-            self.pool.register(Decore_view(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, fields, filter_s, query, pag_type, pag_recs))
+            self.pool.register(Decore_view(func.__name__, t_parent_id, t_source_id, icon, title, desc, func.__doc__, type, fields, filters, query, pag_type, pag_recs))
             func()
         return wrapper
 
     l_dialog_type = Literal['standard', 'tabs', 'stepper']
     l_dialog_display = Literal['modal', 'drawer']
     l_dialog_activator = Literal['none', 'default-menu', 'item-menu', 'item-click']
```

### Comparing `decore_Base-0.0.22/decore_base/globals.py` & `decore_Base-0.0.23/decore_base/globals.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/library/particl_market/particl_market.py` & `decore_Base-0.0.23/decore_base/library/particl_market/particl_market.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/library/powershell.py` & `decore_Base-0.0.23/decore_base/library/powershell.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/library/powershell2.py` & `decore_Base-0.0.23/decore_base/library/powershell2.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/library/return_value.py` & `decore_Base-0.0.23/decore_base/library/return_value.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/library/roaster/roaster_client.py` & `decore_Base-0.0.23/decore_base/library/roaster/roaster_client.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/library/roaster/roaster_functions.py` & `decore_Base-0.0.23/decore_base/library/roaster/roaster_functions.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/library/roaster/roaster_server.py` & `decore_Base-0.0.23/decore_base/library/roaster/roaster_server.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/.gitignore` & `decore_Base-0.0.23/decore_base/prepare/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/.vscode/launch.json` & `decore_Base-0.0.23/decore_base/prepare/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/css/586.ed179a62.css` & `decore_Base-0.0.23/decore_base/prepare/spa/static/css/586.ed179a62.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.23/decore_base/prepare/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.23/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/favicon.ico` & `decore_Base-0.0.23/decore_base/prepare/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.23/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.23/decore_base/prepare/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/js/586.aa14c175.js` & `decore_Base-0.0.23/decore_base/prepare/spa/static/js/586.aa14c175.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.23/decore_base/prepare/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/js/app.af6cbe84.js` & `decore_Base-0.0.23/decore_base/prepare/spa/static/js/app.af6cbe84.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/static/js/vendor.0902ddb5.js` & `decore_Base-0.0.23/decore_base/prepare/spa/static/js/vendor.0902ddb5.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/prepare/spa/templates/index.html` & `decore_Base-0.0.23/decore_base/prepare/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/.gitignore` & `decore_Base-0.0.23/decore_base/sample/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/.vscode/launch.json` & `decore_Base-0.0.23/decore_base/sample/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/bases/account_base.py` & `decore_Base-0.0.23/decore_base/sample/bases/account_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from decore_base import decore
 from models.account_model import Account_model as Model
 
-@decore.base(p_title='Accounts', p_model=Model)
+@decore.base(title='Accounts', model=Model)
 class Account_base(object):
-    @decore.widget(p_parent_id='per_vi1_di1_wi1', p_title='Accounts' , p_type='table', p_active_s=[Model.title, Model.email])
+    @decore.widget(parent_id='per_vi1_di1_wi1', title='Accounts' , type='table', fields=[Model.title, Model.email])
     def per_vi1_di1_wi1_wi1():
         pass
 
-    @decore.view(p_parent_id='Information_system_base', p_title='Accounts',p_icon='mdi-account-circle-outline', p_type='table', p_active_s=Model.field_s, p_filter_s=[Model.password ,Model.person])
+    @decore.view(parent_id='Information_system_base', title='Accounts',icon='mdi-account-circle-outline', type='table', fields=Model.field_s, filters=[Model.password ,Model.person])
     def acc_vi1():
         pass
```

### Comparing `decore_Base-0.0.22/decore_base/sample/bases/global_management_base.py` & `decore_Base-0.0.23/decore_base/sample/bases/global_management_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/bases/person_base.py` & `decore_Base-0.0.23/decore_base/sample/bases/person_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 from decore_base import decore
 from decore_base.classes.decore_base import Decore_base as Base
 from models.person_model import Person_model as Model
 
-@decore.base(p_title='Person', p_model=Model)
+@decore.base(title='Person', model=Model)
 class Person_base(Base):
     
-    @decore.widget(p_parent_id='com_vi1_di1', p_title='Persons', p_type='table', p_active_s=Model.field_s)
+    @decore.widget(parent_id='com_vi1_di1', title='Persons', type='table', fields=Model.field_s)
     def com_vi1_di1_wi1():
         pass
 
-    @decore.view(p_parent_id='Global_management_base', p_title='Persons', p_icon='mdi-account-group-outline', p_type='table', p_active_s=Model.field_s, p_filter_s=[Model.academic_degree, Model.companies, Model.accounts])
+    @decore.view(parent_id='Global_management_base', title='Persons', icon='mdi-account-group-outline', type='table', fields=Model.field_s, filters=[Model.academic_degree, Model.companies, Model.accounts])
     def per_vi1():
         
-        @decore.dialog(p_title='Add person...', p_icon='mdi-plus' , p_type='standard', p_activator='default-menu')
+        @decore.dialog(title='Add person...', icon='mdi-plus' , type='standard', activator='default-menu')
         def per_vi1_di3():
-            @decore.widget(p_type='form', p_active_s=[Model.first_name, Model.last_name, Model.academic_degree, Model.age, Model.capacity])
+            @decore.widget(type='form', fields=[Model.first_name, Model.last_name, Model.academic_degree, Model.age, Model.capacity])
             def per_vi1_di3_wi1():
-                @decore.action(p_type='submit')
+                @decore.action(type='submit')
                 def per_vi1_di3_wi1_ac1(self, p_data):
+                    t_item = Model(p_data['item'])
+                    t_item.title = t_item.first_name + ' ' + t_item.last_name
                     return True, 'Success!'
         
-        @decore.action(p_title='Test action', p_icon='mdi-test-tube', p_type='standard', p_activator='default-menu')
+        @decore.action(title='Test action', icon='mdi-test-tube', type='standard', activator='default-menu')
         def per_vi1_ac1(self, p_data):
             return True, 'Success!'
 
-        @decore.dialog(p_title='Person', p_type='standard', p_display='drawer', p_activator='item-click')
+        @decore.dialog(title='Person', type='standard', display='drawer', activator='item-click')
         def per_vi1_di1():
-            @decore.widget(p_title='Informations', p_type='info', p_active_s=Model.field_s)
+            @decore.widget(title='Informations', type='info', fields=Model.field_s)
             def per_vi1_di1_wi1():
-                @decore.dialog(p_title='Edit Person', p_icon='mdi-pencil', p_type='standard', p_display='drawer', p_activator='item-menu')
+                @decore.dialog(title='Edit Person', icon='mdi-pencil', type='standard', display='drawer', activator='item-menu')
                 def per_vi1_wi1_di1():
-                    @decore.widget(p_type='form', p_active_s=[Model.first_name, Model.last_name])
+                    @decore.widget(type='form', fields=[Model.first_name, Model.last_name])
                     def per_vi1_di1_wi1_di1_wi1():
-                        @decore.action(p_type='submit')
+                        @decore.action(type='submit')
                         def per_vi1_di1_wi1_di1_wi1_ac1(self, p_data):
                             return True, 'Success!'
         
-        @decore.dialog(p_title='Edit Person', p_icon='mdi-pencil', p_type='standard', p_display='drawer', p_activator='item-menu')
+        @decore.dialog(title='Edit Person', icon='mdi-pencil', type='standard', display='drawer', activator='item-menu')
         def per_vi1_di2():
-            @decore.widget(p_type='form', p_active_s=[Model.first_name, Model.last_name])
+            @decore.widget(type='form', fields=[Model.first_name, Model.last_name])
             def per_vi1_di2_wi1():
-                @decore.action(p_type='submit')
+                @decore.action(type='submit')
                 def per_vi1_di2_wi1_ac1(self, p_data):
                     return True, 'Success!'
```

### Comparing `decore_Base-0.0.22/decore_base/sample/bases/test_base.py` & `decore_Base-0.0.23/decore_base/sample/bases/test_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from decore_base import decore
 from models.test_model import Test_model
 
-@decore.base(p_title='Test Base', p_icon='mdi-test-tube', p_model=Test_model)
+@decore.base(title='Test Base', icon='mdi-test-tube', model=Test_model)
 class Test_base:
-    @decore.view(p_title='Formtest', p_icon='mdi-test-tube', p_type='table')
+    @decore.view(title='Formtest', icon='mdi-test-tube', type='table')
     def tst_vi1():
-        @decore.dialog(p_title='Formtest', p_icon='mdi-test-tube', p_type='standard', p_display='drawer', p_activator='none')
+        @decore.dialog(title='Formtest', icon='mdi-test-tube', type='standard', display='drawer', activator='none')
         def tst_vi1_di1():
-            @decore.widget(p_title='Formtest', p_icon='mdi-test-tube', p_type='form', p_active_s=[Test_model.title,Test_model.desc, Test_model.charfield, Test_model.intfield, Test_model.textfield, Test_model.booleanfield , Test_model.passwordfield])
+            @decore.widget(title='Formtest', icon='mdi-test-tube', type='form', fields=[Test_model.title,Test_model.desc, Test_model.charfield, Test_model.intfield, Test_model.textfield, Test_model.booleanfield , Test_model.passwordfield])
             def tst_vi1_di1_wi1():
-                @decore.action(p_title='Submit', p_type='submit', p_icon='mdi-test-tube')
+                @decore.action(title='Submit', type='submit', icon='mdi-test-tube')
                 def tst_vi1_di1_wi1_ac1(self, t_data):
                     return True, 'Success'
```

### Comparing `decore_Base-0.0.22/decore_base/sample/models/person_model.py` & `decore_Base-0.0.23/decore_base/sample/models/person_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/models/test_model.py` & `decore_Base-0.0.23/decore_base/sample/models/test_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/css/586.ed179a62.css` & `decore_Base-0.0.23/decore_base/sample/spa/static/css/586.ed179a62.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.23/decore_base/sample/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.23/decore_base/sample/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/favicon.ico` & `decore_Base-0.0.23/decore_base/sample/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.23/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.23/decore_base/sample/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/js/586.aa14c175.js` & `decore_Base-0.0.23/decore_base/sample/spa/static/js/586.aa14c175.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.23/decore_base/sample/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/js/app.af6cbe84.js` & `decore_Base-0.0.23/decore_base/sample/spa/static/js/app.af6cbe84.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/static/js/vendor.0902ddb5.js` & `decore_Base-0.0.23/decore_base/sample/spa/static/js/vendor.0902ddb5.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/spa/templates/index.html` & `decore_Base-0.0.23/decore_base/sample/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/state/database.db` & `decore_Base-0.0.23/decore_base/sample/state/database.db`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/state/keybase.kdbx` & `decore_Base-0.0.23/decore_base/sample/state/keybase.kdbx`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/sample/state/querybase.db` & `decore_Base-0.0.23/decore_base/sample/state/querybase.db`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/uniform/conform_model.py` & `decore_Base-0.0.23/decore_base/uniform/conform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/uniform/depricated/askform_base.py` & `decore_Base-0.0.23/decore_base/uniform/depricated/askform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/uniform/depricated/buyform_base.py` & `decore_Base-0.0.23/decore_base/uniform/depricated/buyform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/uniform/depricated/conform_base.py` & `decore_Base-0.0.23/decore_base/uniform/depricated/conform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/uniform/depricated/deform_base.py` & `decore_Base-0.0.23/decore_base/uniform/depricated/deform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/uniform/perform_model.py` & `decore_Base-0.0.23/decore_base/uniform/perform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/uniform/reform_client_model.py` & `decore_Base-0.0.23/decore_base/uniform/reform_client_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/decore_base/uniform/reform_server_model.py` & `decore_Base-0.0.23/decore_base/uniform/reform_server_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/Makefile` & `decore_Base-0.0.23/docs/Makefile`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/_static/favicon.ico` & `decore_Base-0.0.23/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/_static/logo.png` & `decore_Base-0.0.23/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/conf.py` & `decore_Base-0.0.23/docs/conf.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/make.bat` & `decore_Base-0.0.23/docs/make.bat`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/doctrees/environment.pickle` & `decore_Base-0.0.23/docs/page/doctrees/environment.pickle`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9500 0001 0000 0000 008c 1273 7068  .............sph
+00000000: 8005 9503 0001 0000 0000 008c 1273 7068  .............sph
 00000010: 696e 782e 656e 7669 726f 6e6d 656e 7494  inx.environment.
 00000020: 8c10 4275 696c 6445 6e76 6972 6f6e 6d65  ..BuildEnvironme
 00000030: 6e74 9493 9429 8194 7d94 288c 0361 7070  nt...)..}.(..app
 00000040: 944e 8c0a 646f 6374 7265 6564 6972 948c  .N..doctreedir..
 00000050: 5443 3a5c 5573 6572 735c 726f 6861 726b  TC:\Users\rohark
 00000060: 5c44 6f63 756d 656e 7473 5c56 6973 7561  \Documents\Visua
 00000070: 6c20 5374 7564 696f 2043 6f64 655c 5072  l Studio Code\Pr
@@ -781,15 +781,15 @@
 000030c0: 944b 058c 1666 696c 655f 696e 7365 7274  .K...file_insert
 000030d0: 696f 6e5f 656e 6162 6c65 6494 888c 1373  ion_enabled....s
 000030e0: 6d61 7274 7175 6f74 6573 5f6c 6f63 616c  martquotes_local
 000030f0: 6573 945d 9468 5a68 0368 9389 8c0d 6c61  es.].hZh.h....la
 00003100: 6e67 7561 6765 5f63 6f64 6594 686a 8c0c  nguage_code.hj..
 00003110: 736d 6172 745f 7175 6f74 6573 9488 758c  smart_quotes..u.
 00003120: 0861 6c6c 5f64 6f63 7394 7d94 6acd 0200  .all_docs.}.j...
-00003130: 0047 41d9 2319 781a 653e 738c 0c64 6570  .GA.#.x.e>s..dep
+00003130: 0047 41d9 23c3 7c38 ace9 738c 0c64 6570  .GA.#.|8..s..dep
 00003140: 656e 6465 6e63 6965 7394 8c0b 636f 6c6c  endencies...coll
 00003150: 6563 7469 6f6e 7394 8c0b 6465 6661 756c  ections...defaul
 00003160: 7464 6963 7494 9394 8c08 6275 696c 7469  tdict.....builti
 00003170: 6e73 948c 0373 6574 9493 9485 9452 946a  ns...set.....R.j
 00003180: cd02 0000 8f94 288c 0d2e 2e2f 5245 4144  ......(..../READ
 00003190: 4d45 2e72 7374 9490 738c 0869 6e63 6c75  ME.rst..s..inclu
 000031a0: 6465 6494 6afb 0200 006a fe02 0000 8594  ded.j....j......
@@ -3384,15 +3384,15 @@
 0000d370: 0300 004e 7562 656a 2403 0000 7d94 286a  ...Nubej$...}.(j
 0000d380: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
 0000d390: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
 0000d3a0: 5d94 756a 3203 0000 6a5d 0300 006a 3403  ].uj2...j]...j4.
 0000d3b0: 0000 6a5c 0300 006a 3603 0000 4bca 6a23  ..j\...j6...K.j#
 0000d3c0: 0300 006a a50a 0000 6a33 0300 006a 1103  ...j....j3...j..
 0000d3d0: 0000 7562 6a24 0500 0029 8194 7d94 286a  ..ubj$...)..}.(j
-0000d3e0: 1303 0000 5857 0400 0066 726f 6d20 6465  ....XW...from de
+0000d3e0: 1303 0000 5813 0400 0066 726f 6d20 6465  ....X....from de
 0000d3f0: 636f 7265 5f62 6173 6520 696d 706f 7274  core_base import
 0000d400: 2064 6563 6f72 650a 6672 6f6d 206d 6f64   decore.from mod
 0000d410: 656c 732e 6669 7273 745f 6d6f 6465 6c20  els.first_model 
 0000d420: 696d 706f 7274 2046 6972 7374 5f6d 6f64  import First_mod
 0000d430: 656c 0a0a 4064 6563 6f72 652e 6261 7365  el..@decore.base
 0000d440: 2874 6974 6c65 3d27 4d79 2046 6972 7374  (title='My First
 0000d450: 2042 6173 6527 2c20 6963 6f6e 3d27 6d64   Base', icon='md
@@ -3433,1525 +3433,1516 @@
 0000d680: 2069 636f 6e3d 276d 6469 2d63 6f6e 7465   icon='mdi-conte
 0000d690: 6e74 2d73 6176 6527 2c20 7479 7065 3d27  nt-save', type='
 0000d6a0: 7375 626d 6974 2729 0a20 2020 2020 2020  submit').       
 0000d6b0: 2020 2020 2064 6566 2066 6972 7374 5f61       def first_a
 0000d6c0: 6374 696f 6e28 7365 6c66 2c20 6461 7461  ction(self, data
 0000d6d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
 0000d6e0: 2020 6974 656d 203d 2046 6972 7374 5f6d    item = First_m
-0000d6f0: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
-0000d700: 2020 2020 2020 6974 656d 2e74 6974 6c65        item.title
-0000d710: 203d 2064 6174 615b 2766 6972 7374 6e61   = data['firstna
-0000d720: 6d65 275d 202b 2027 2027 202b 2064 6174  me'] + ' ' + dat
-0000d730: 615b 276c 6173 746e 616d 6527 5d0a 2020  a['lastname'].  
-0000d740: 2020 2020 2020 2020 2020 2020 2069 7465               ite
-0000d750: 6d2e 6669 7273 746e 616d 6520 3d20 6461  m.firstname = da
-0000d760: 7461 5b27 6669 7273 746e 616d 6527 5d0a  ta['firstname'].
-0000d770: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d780: 7465 6d2e 6c61 7374 6e61 6d65 203d 2064  tem.lastname = d
-0000d790: 6174 615b 276c 6173 746e 616d 6527 5d0a  ata['lastname'].
-0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d7b0: 6620 6974 656d 2e73 6176 6528 293a 0a20  f item.save():. 
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7d0: 2072 6574 7572 6e20 5472 7565 2c20 6974   return True, it
-0000d7e0: 656d 2e74 6974 6c65 202b 2027 2073 6176  em.title + ' sav
-0000d7f0: 6564 2073 7563 6365 7373 6675 6c6c 7927  ed successfully'
-0000d800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d810: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000d820: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0000d830: 616c 7365 2c20 6974 656d 2e65 7272 6f72  alse, item.error
-0000d840: 946a 1403 0000 5d94 6a1e 0300 0058 5704  .j....].j....XW.
-0000d850: 0000 6672 6f6d 2064 6563 6f72 655f 6261  ..from decore_ba
-0000d860: 7365 2069 6d70 6f72 7420 6465 636f 7265  se import decore
-0000d870: 0a66 726f 6d20 6d6f 6465 6c73 2e66 6972  .from models.fir
-0000d880: 7374 5f6d 6f64 656c 2069 6d70 6f72 7420  st_model import 
-0000d890: 4669 7273 745f 6d6f 6465 6c0a 0a40 6465  First_model..@de
-0000d8a0: 636f 7265 2e62 6173 6528 7469 746c 653d  core.base(title=
-0000d8b0: 274d 7920 4669 7273 7420 4261 7365 272c  'My First Base',
-0000d8c0: 2069 636f 6e3d 276d 6469 2d68 6f6d 6527   icon='mdi-home'
-0000d8d0: 2c20 6d6f 6465 6c3d 4669 7273 745f 6d6f  , model=First_mo
-0000d8e0: 6465 6c29 0a63 6c61 7373 2046 6972 7374  del).class First
-0000d8f0: 5f62 6173 653a 0a20 2020 4064 6563 6f72  _base:.   @decor
-0000d900: 652e 7669 6577 2874 6974 6c65 3d27 5065  e.view(title='Pe
-0000d910: 7273 6f6e 272c 2069 636f 6e3d 276d 6469  rson', icon='mdi
-0000d920: 2d61 6363 6f75 6e74 272c 2074 7970 653d  -account', type=
-0000d930: 2774 6162 6c65 272c 2066 6965 6c64 733d  'table', fields=
-0000d940: 5b46 6972 7374 5f6d 6f64 656c 2e66 6972  [First_model.fir
-0000d950: 7374 6e61 6d65 2c20 4669 7273 745f 6d6f  stname, First_mo
-0000d960: 6465 6c2e 6c61 7374 6e61 6d65 5d29 0a20  del.lastname]). 
-0000d970: 2020 6465 6620 6669 7273 745f 7669 6577    def first_view
-0000d980: 2829 3a0a 2020 2020 2020 4064 6563 6f72  ():.      @decor
-0000d990: 652e 6469 616c 6f67 2874 6974 6c65 3d27  e.dialog(title='
-0000d9a0: 4164 6420 5065 7273 6f6e 272c 2069 636f  Add Person', ico
-0000d9b0: 6e3d 276d 6469 2d70 6c75 7327 2c20 7479  n='mdi-plus', ty
-0000d9c0: 7065 3d27 7374 616e 6461 7264 272c 2064  pe='standard', d
-0000d9d0: 6973 706c 6179 3d27 6472 6177 6572 272c  isplay='drawer',
-0000d9e0: 2061 6374 6976 6174 6f72 3d27 6465 6661   activator='defa
-0000d9f0: 756c 742d 6d65 6e75 2729 0a20 2020 2020  ult-menu').     
-0000da00: 2064 6566 2066 6972 7374 5f64 6961 6c6f   def first_dialo
-0000da10: 6728 293a 0a20 2020 2020 2020 2020 4064  g():.         @d
-0000da20: 6563 6f72 652e 7769 6467 6574 2874 6974  ecore.widget(tit
-0000da30: 6c65 3d27 4164 6420 5065 7273 6f6e 2046  le='Add Person F
-0000da40: 6f72 6d27 2c20 6963 6f6e 3d27 6d64 692d  orm', icon='mdi-
-0000da50: 6163 636f 756e 7427 2c20 7479 7065 3d27  account', type='
-0000da60: 666f 726d 272c 2066 6965 6c64 733d 5b46  form', fields=[F
-0000da70: 6972 7374 5f6d 6f64 656c 2e66 6972 7374  irst_model.first
-0000da80: 6e61 6d65 2c20 4669 7273 745f 6d6f 6465  name, First_mode
-0000da90: 6c2e 6c61 7374 6e61 6d65 5d29 0a20 2020  l.lastname]).   
-0000daa0: 2020 2020 2020 6465 6620 6669 7273 745f        def first_
-0000dab0: 7769 6467 6574 2829 3a0a 2020 2020 2020  widget():.      
-0000dac0: 2020 2020 2020 4064 6563 6f72 652e 6163        @decore.ac
-0000dad0: 7469 6f6e 2874 6974 6c65 3d27 5361 7665  tion(title='Save
-0000dae0: 2050 6572 736f 6e27 2c20 6963 6f6e 3d27   Person', icon='
-0000daf0: 6d64 692d 636f 6e74 656e 742d 7361 7665  mdi-content-save
-0000db00: 272c 2074 7970 653d 2773 7562 6d69 7427  ', type='submit'
-0000db10: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
-0000db20: 6620 6669 7273 745f 6163 7469 6f6e 2873  f first_action(s
-0000db30: 656c 662c 2064 6174 6129 3a0a 2020 2020  elf, data):.    
-0000db40: 2020 2020 2020 2020 2020 2069 7465 6d20             item 
-0000db50: 3d20 4669 7273 745f 6d6f 6465 6c28 290a  = First_model().
-0000db60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000db70: 7465 6d2e 7469 746c 6520 3d20 6461 7461  tem.title = data
-0000db80: 5b27 6669 7273 746e 616d 6527 5d20 2b20  ['firstname'] + 
-0000db90: 2720 2720 2b20 6461 7461 5b27 6c61 7374  ' ' + data['last
-0000dba0: 6e61 6d65 275d 0a20 2020 2020 2020 2020  name'].         
-0000dbb0: 2020 2020 2020 6974 656d 2e66 6972 7374        item.first
-0000dbc0: 6e61 6d65 203d 2064 6174 615b 2766 6972  name = data['fir
-0000dbd0: 7374 6e61 6d65 275d 0a20 2020 2020 2020  stname'].       
-0000dbe0: 2020 2020 2020 2020 6974 656d 2e6c 6173          item.las
-0000dbf0: 746e 616d 6520 3d20 6461 7461 5b27 6c61  tname = data['la
-0000dc00: 7374 6e61 6d65 275d 0a20 2020 2020 2020  stname'].       
-0000dc10: 2020 2020 2020 2020 6966 2069 7465 6d2e          if item.
-0000dc20: 7361 7665 2829 3a0a 2020 2020 2020 2020  save():.        
-0000dc30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000dc40: 2054 7275 652c 2069 7465 6d2e 7469 746c   True, item.titl
-0000dc50: 6520 2b20 2720 7361 7665 6420 7375 6363  e + ' saved succ
-0000dc60: 6573 7366 756c 6c79 270a 2020 2020 2020  essfully'.      
-0000dc70: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2072 6574 7572 6e20 4661 6c73 652c 2069   return False, i
-0000dca0: 7465 6d2e 6572 726f 7294 8594 8194 7d94  tem.error.....}.
-0000dcb0: 6a23 0300 006a 080b 0000 7362 616a 2403  j#...j....sbaj$.
-0000dcc0: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
-0000dcd0: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
-0000dce0: 946a 2e03 0000 5d94 6a30 0300 006a 3103  .j....].j0...j1.
-0000dcf0: 0000 6a33 0500 0089 6869 8c06 7079 7468  ..j3....hi..pyth
-0000dd00: 6f6e 946a 3505 0000 7d94 756a 3203 0000  on.j5...}.uj2...
-0000dd10: 6a23 0500 006a 3403 0000 6a5c 0300 006a  j#...j4...j\...j
-0000dd20: 3603 0000 4bcc 6a23 0300 006a a50a 0000  6...K.j#...j....
-0000dd30: 6a33 0300 006a 1103 0000 7562 6a53 0700  j3...j....ubjS..
-0000dd40: 0029 8194 7d94 286a 1303 0000 5817 0100  .)..}.(j....X...
-0000dd50: 0054 6f20 6372 6561 7465 2061 2072 6563  .To create a rec
-0000dd60: 6f72 6420 7769 7468 2064 6563 6f72 6520  ord with decore 
-0000dd70: 4261 7365 2c20 7765 206e 6565 6420 746f  Base, we need to
-0000dd80: 2063 7265 6174 6520 616e 2069 6e73 7461   create an insta
-0000dd90: 6e63 6520 6f66 2074 6865 206d 6f64 656c  nce of the model
-0000dda0: 2e20 496e 206f 7572 2063 6173 6520 2a2a  . In our case **
-0000ddb0: 4669 7273 745f 6d6f 6465 6c2a 2a2e 2054  First_model**. T
-0000ddc0: 6865 2069 6e73 7461 6e63 6520 6973 2066  he instance is f
-0000ddd0: 696c 6c65 6420 7769 7468 2074 6865 2064  illed with the d
-0000dde0: 6174 6120 6672 6f6d 2074 6865 2066 6f72  ata from the for
-0000ddf0: 6d20 616e 6420 7468 656e 2073 6176 6564  m and then saved
-0000de00: 2e0a 0a54 6865 2049 4420 696e 2074 6865  ...The ID in the
-0000de10: 2066 6f72 6d20 6f66 2061 2055 5549 4420   form of a UUID 
-0000de20: 6973 2067 656e 6572 6174 6564 2061 7574  is generated aut
-0000de30: 6f6d 6174 6963 616c 6c79 2061 6e64 2064  omatically and d
-0000de40: 6f65 7320 6e6f 7420 6861 7665 2074 6f20  oes not have to 
-0000de50: 6265 2073 7065 6369 6669 6564 2073 6570  be specified sep
-0000de60: 6172 6174 656c 792e 946a 1403 0000 5d94  arately..j....].
-0000de70: 286a 5e03 0000 2981 947d 9428 6a13 0300  (j^...)..}.(j...
-0000de80: 008c b054 6f20 6372 6561 7465 2061 2072  ...To create a r
-0000de90: 6563 6f72 6420 7769 7468 2064 6563 6f72  ecord with decor
-0000dea0: 6520 4261 7365 2c20 7765 206e 6565 6420  e Base, we need 
-0000deb0: 746f 2063 7265 6174 6520 616e 2069 6e73  to create an ins
-0000dec0: 7461 6e63 6520 6f66 2074 6865 206d 6f64  tance of the mod
-0000ded0: 656c 2e20 496e 206f 7572 2063 6173 6520  el. In our case 
-0000dee0: 2a2a 4669 7273 745f 6d6f 6465 6c2a 2a2e  **First_model**.
-0000def0: 2054 6865 2069 6e73 7461 6e63 6520 6973   The instance is
-0000df00: 2066 696c 6c65 6420 7769 7468 2074 6865   filled with the
-0000df10: 2064 6174 6120 6672 6f6d 2074 6865 2066   data from the f
-0000df20: 6f72 6d20 616e 6420 7468 656e 2073 6176  orm and then sav
-0000df30: 6564 2e94 6a14 0300 005d 9428 6a1e 0300  ed..j....].(j...
-0000df40: 008c 5d54 6f20 6372 6561 7465 2061 2072  ..]To create a r
-0000df50: 6563 6f72 6420 7769 7468 2064 6563 6f72  ecord with decor
-0000df60: 6520 4261 7365 2c20 7765 206e 6565 6420  e Base, we need 
-0000df70: 746f 2063 7265 6174 6520 616e 2069 6e73  to create an ins
-0000df80: 7461 6e63 6520 6f66 2074 6865 206d 6f64  tance of the mod
-0000df90: 656c 2e20 496e 206f 7572 2063 6173 6520  el. In our case 
-0000dfa0: 9485 9481 947d 9428 6a23 0300 006a 1c0b  .....}.(j#...j..
-0000dfb0: 0000 6a33 0300 006a 1103 0000 6a34 0300  ..j3...j....j4..
-0000dfc0: 004e 6a36 0300 004e 7562 6a72 0300 0029  .Nj6...Nubjr...)
-0000dfd0: 8194 7d94 286a 1303 0000 8c0f 2a2a 4669  ..}.(j......**Fi
-0000dfe0: 7273 745f 6d6f 6465 6c2a 2a94 6a14 0300  rst_model**.j...
-0000dff0: 005d 946a 1e03 0000 8c0b 4669 7273 745f  .].j......First_
-0000e000: 6d6f 6465 6c94 8594 8194 7d94 286a 2303  model.....}.(j#.
-0000e010: 0000 6a24 0b00 006a 3303 0000 6a11 0300  ..j$...j3...j...
-0000e020: 006a 3403 0000 4e6a 3603 0000 4e75 6261  .j4...Nj6...Nuba
-0000e030: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
-0000e040: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
-0000e050: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
-0000e060: 006a 7103 0000 6a23 0300 006a 1c0b 0000  .jq...j#...j....
-0000e070: 7562 6a1e 0300 008c 442e 2054 6865 2069  ubj.....D. The i
-0000e080: 6e73 7461 6e63 6520 6973 2066 696c 6c65  nstance is fille
-0000e090: 6420 7769 7468 2074 6865 2064 6174 6120  d with the data 
-0000e0a0: 6672 6f6d 2074 6865 2066 6f72 6d20 616e  from the form an
-0000e0b0: 6420 7468 656e 2073 6176 6564 2e94 8594  d then saved....
-0000e0c0: 8194 7d94 286a 2303 0000 6a1c 0b00 006a  ..}.(j#...j....j
-0000e0d0: 3303 0000 6a11 0300 006a 3403 0000 4e6a  3...j....j4...Nj
-0000e0e0: 3603 0000 4e75 6265 6a24 0300 007d 9428  6...Nubej$...}.(
-0000e0f0: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-0000e100: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-0000e110: 005d 9475 6a32 0300 006a 5d03 0000 6a34  .].uj2...j]...j4
-0000e120: 0300 006a 5c03 0000 6a36 0300 004b e56a  ...j\...j6...K.j
-0000e130: 2303 0000 6a18 0b00 0075 626a 5e03 0000  #...j....ubj^...
-0000e140: 2981 947d 9428 6a13 0300 008c 6554 6865  )..}.(j.....eThe
-0000e150: 2049 4420 696e 2074 6865 2066 6f72 6d20   ID in the form 
-0000e160: 6f66 2061 2055 5549 4420 6973 2067 656e  of a UUID is gen
-0000e170: 6572 6174 6564 2061 7574 6f6d 6174 6963  erated automatic
-0000e180: 616c 6c79 2061 6e64 2064 6f65 7320 6e6f  ally and does no
-0000e190: 7420 6861 7665 2074 6f20 6265 2073 7065  t have to be spe
-0000e1a0: 6369 6669 6564 2073 6570 6172 6174 656c  cified separatel
-0000e1b0: 792e 946a 1403 0000 5d94 6a1e 0300 008c  y..j....].j.....
-0000e1c0: 6554 6865 2049 4420 696e 2074 6865 2066  eThe ID in the f
-0000e1d0: 6f72 6d20 6f66 2061 2055 5549 4420 6973  orm of a UUID is
-0000e1e0: 2067 656e 6572 6174 6564 2061 7574 6f6d   generated autom
-0000e1f0: 6174 6963 616c 6c79 2061 6e64 2064 6f65  atically and doe
-0000e200: 7320 6e6f 7420 6861 7665 2074 6f20 6265  s not have to be
-0000e210: 2073 7065 6369 6669 6564 2073 6570 6172   specified separ
-0000e220: 6174 656c 792e 9485 9481 947d 9428 6a23  ately......}.(j#
-0000e230: 0300 006a 3c0b 0000 6a33 0300 006a 1103  ...j<...j3...j..
-0000e240: 0000 6a34 0300 004e 6a36 0300 004e 7562  ..j4...Nj6...Nub
-0000e250: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
-0000e260: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
-0000e270: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
-0000e280: 0000 6a5d 0300 006a 3403 0000 6a5c 0300  ..j]...j4...j\..
-0000e290: 006a 3603 0000 4be7 6a23 0300 006a 180b  .j6...K.j#...j..
-0000e2a0: 0000 7562 656a 2403 0000 7d94 286a 2603  ..ubej$...}.(j&.
-0000e2b0: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
-0000e2c0: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
-0000e2d0: 756a 3203 0000 6a52 0700 006a 2303 0000  uj2...jR...j#...
-0000e2e0: 6aa5 0a00 006a 3303 0000 6a11 0300 006a  j....j3...j....j
-0000e2f0: 3403 0000 6a5c 0300 006a 3603 0000 4e75  4...j\...j6...Nu
-0000e300: 626a 1e08 0000 2981 947d 9428 6a13 0300  bj....)..}.(j...
-0000e310: 008c 9954 6865 2066 6965 6c64 202a 2a74  ...The field **t
-0000e320: 6974 6c65 2a2a 2077 6173 2069 6e68 6572  itle** was inher
-0000e330: 6974 6564 2066 726f 6d20 7468 6520 636c  ited from the cl
-0000e340: 6173 7320 2a2a 4465 666f 726d 5f6d 6f64  ass **Deform_mod
-0000e350: 656c 2a2a 2061 6e64 206d 7573 7420 6265  el** and must be
-0000e360: 2075 7365 6420 666f 7220 6561 6368 2072   used for each r
-0000e370: 6563 6f72 6420 6372 6561 7469 6f6e 2e20  ecord creation. 
-0000e380: 4f74 6865 7277 6973 6520 7468 6520 6974  Otherwise the it
-0000e390: 656d 2077 696c 6c20 6661 696c 2074 6865  em will fail the
-0000e3a0: 2076 616c 6964 6174 696f 6e2e 946a 1403   validation..j..
-0000e3b0: 0000 5d94 6a5e 0300 0029 8194 7d94 286a  ..].j^...)..}.(j
-0000e3c0: 1303 0000 6a52 0b00 006a 1403 0000 5d94  ....jR...j....].
-0000e3d0: 286a 1e03 0000 8c0a 5468 6520 6669 656c  (j......The fiel
-0000e3e0: 6420 9485 9481 947d 9428 6a23 0300 006a  d .....}.(j#...j
-0000e3f0: 540b 0000 6a33 0300 006a 1103 0000 6a34  T...j3...j....j4
-0000e400: 0300 004e 6a36 0300 004e 7562 6a72 0300  ...Nj6...Nubjr..
-0000e410: 0029 8194 7d94 286a 1303 0000 8c09 2a2a  .)..}.(j......**
-0000e420: 7469 746c 652a 2a94 6a14 0300 005d 946a  title**.j....].j
-0000e430: 1e03 0000 8c05 7469 746c 6594 8594 8194  ......title.....
-0000e440: 7d94 286a 2303 0000 6a5b 0b00 006a 3303  }.(j#...j[...j3.
-0000e450: 0000 6a11 0300 006a 3403 0000 4e6a 3603  ..j....j4...Nj6.
-0000e460: 0000 4e75 6261 6a24 0300 007d 9428 6a26  ..Nubaj$...}.(j&
-0000e470: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
-0000e480: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-0000e490: 9475 6a32 0300 006a 7103 0000 6a23 0300  .uj2...jq...j#..
-0000e4a0: 006a 540b 0000 7562 6a1e 0300 008c 1e20  .jT...ubj...... 
-0000e4b0: 7761 7320 696e 6865 7269 7465 6420 6672  was inherited fr
-0000e4c0: 6f6d 2074 6865 2063 6c61 7373 2094 8594  om the class ...
-0000e4d0: 8194 7d94 286a 2303 0000 6a54 0b00 006a  ..}.(j#...jT...j
-0000e4e0: 3303 0000 6a11 0300 006a 3403 0000 4e6a  3...j....j4...Nj
-0000e4f0: 3603 0000 4e75 626a 7203 0000 2981 947d  6...Nubjr...)..}
-0000e500: 9428 6a13 0300 008c 102a 2a44 6566 6f72  .(j......**Defor
-0000e510: 6d5f 6d6f 6465 6c2a 2a94 6a14 0300 005d  m_model**.j....]
-0000e520: 946a 1e03 0000 8c0c 4465 666f 726d 5f6d  .j......Deform_m
-0000e530: 6f64 656c 9485 9481 947d 9428 6a23 0300  odel.....}.(j#..
-0000e540: 006a 6d0b 0000 6a33 0300 006a 1103 0000  .jm...j3...j....
-0000e550: 6a34 0300 004e 6a36 0300 004e 7562 616a  j4...Nj6...Nubaj
-0000e560: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
-0000e570: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
-0000e580: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
-0000e590: 6a71 0300 006a 2303 0000 6a54 0b00 0075  jq...j#...jT...u
-0000e5a0: 626a 1e03 0000 8c58 2061 6e64 206d 7573  bj.....X and mus
-0000e5b0: 7420 6265 2075 7365 6420 666f 7220 6561  t be used for ea
-0000e5c0: 6368 2072 6563 6f72 6420 6372 6561 7469  ch record creati
-0000e5d0: 6f6e 2e20 4f74 6865 7277 6973 6520 7468  on. Otherwise th
-0000e5e0: 6520 6974 656d 2077 696c 6c20 6661 696c  e item will fail
-0000e5f0: 2074 6865 2076 616c 6964 6174 696f 6e2e   the validation.
-0000e600: 9485 9481 947d 9428 6a23 0300 006a 540b  .....}.(j#...jT.
-0000e610: 0000 6a33 0300 006a 1103 0000 6a34 0300  ..j3...j....j4..
-0000e620: 004e 6a36 0300 004e 7562 656a 2403 0000  .Nj6...Nubej$...
-0000e630: 7d94 286a 2603 0000 5d94 6a28 0300 005d  }.(j&...].j(...]
-0000e640: 946a 2a03 0000 5d94 6a2c 0300 005d 946a  .j*...].j,...].j
-0000e650: 2e03 0000 5d94 756a 3203 0000 6a5d 0300  ....].uj2...j]..
-0000e660: 006a 3403 0000 6a5c 0300 006a 3603 0000  .j4...j\...j6...
-0000e670: 4bea 6a23 0300 006a 500b 0000 7562 616a  K.j#...jP...ubaj
-0000e680: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
-0000e690: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
-0000e6a0: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
-0000e6b0: 6a1d 0800 006a 2303 0000 6aa5 0a00 006a  j....j#...j....j
-0000e6c0: 3303 0000 6a11 0300 006a 3403 0000 6a5c  3...j....j4...j\
-0000e6d0: 0300 006a 3603 0000 4e75 6265 6a24 0300  ...j6...Nubej$..
-0000e6e0: 007d 9428 6a26 0300 005d 948c 0661 6374  .}.(j&...]...act
-0000e6f0: 696f 6e94 616a 2803 0000 5d94 6a2a 0300  ion.aj(...].j*..
-0000e700: 005d 948c 0661 6374 696f 6e94 616a 2c03  .]...action.aj,.
-0000e710: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
-0000e720: 0068 4e6a 2303 0000 6a2c 0600 006a 3303  .hNj#...j,...j3.
-0000e730: 0000 6a11 0300 006a 3403 0000 6a5c 0300  ..j....j4...j\..
-0000e740: 006a 3603 0000 4bc7 7562 656a 2403 0000  .j6...K.ubej$...
-0000e750: 7d94 286a 2603 0000 5d94 8c05 7573 6167  }.(j&...]...usag
-0000e760: 6594 616a 2803 0000 5d94 6a2a 0300 005d  e.aj(...].j*...]
-0000e770: 948c 0575 7361 6765 9461 6a2c 0300 005d  ...usage.aj,...]
-0000e780: 946a 2e03 0000 5d94 756a 3203 0000 684e  .j....].uj2...hN
-0000e790: 6a23 0300 006a 9e04 0000 6a33 0300 006a  j#...j....j3...j
-0000e7a0: 1103 0000 6a34 0300 006a 5c03 0000 6a36  ....j4...j\...j6
-0000e7b0: 0300 004b 3c75 626a 3703 0000 2981 947d  ...K<ubj7...)..}
-0000e7c0: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
-0000e7d0: 286a 3c03 0000 2981 947d 9428 6a13 0300  (j<...)..}.(j...
-0000e7e0: 008c 1a52 756e 2c20 4465 7665 6c6f 706d  ...Run, Developm
-0000e7f0: 656e 7420 616e 6420 4275 696c 6494 6a14  ent and Build.j.
-0000e800: 0300 005d 946a 1e03 0000 8c1a 5275 6e2c  ...].j......Run,
-0000e810: 2044 6576 656c 6f70 6d65 6e74 2061 6e64   Development and
-0000e820: 2042 7569 6c64 9485 9481 947d 9428 6a23   Build.....}.(j#
-0000e830: 0300 006a 9e0b 0000 6a33 0300 006a 1103  ...j....j3...j..
-0000e840: 0000 6a34 0300 004e 6a36 0300 004e 7562  ..j4...Nj6...Nub
-0000e850: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
-0000e860: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
-0000e870: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
-0000e880: 0000 6a3b 0300 006a 2303 0000 6a9b 0b00  ..j;...j#...j...
-0000e890: 006a 3303 0000 6a11 0300 006a 3403 0000  .j3...j....j4...
-0000e8a0: 6a5c 0300 006a 3603 0000 4bed 7562 6a5e  j\...j6...K.ubj^
-0000e8b0: 0300 0029 8194 7d94 286a 1303 0000 8c71  ...)..}.(j.....q
-0000e8c0: 546f 2073 7461 7274 206f 6e6c 7920 796f  To start only yo
-0000e8d0: 7572 2061 7070 6c69 6361 7469 6f6e 2c20  ur application, 
-0000e8e0: 7275 6e20 6060 7079 7468 6f6e 2061 7070  run ``python app
-0000e8f0: 2e70 7960 6020 696e 2079 6f75 7220 7072  .py`` in your pr
-0000e900: 6f6a 6563 7420 726f 6f74 2064 6972 6563  oject root direc
-0000e910: 746f 7279 2e20 5573 6520 7468 6520 7465  tory. Use the te
-0000e920: 726d 696e 616c 2069 6e20 7673 636f 6465  rminal in vscode
-0000e930: 2e94 6a14 0300 005d 9428 6a1e 0300 008c  ..j....].(j.....
-0000e940: 2454 6f20 7374 6172 7420 6f6e 6c79 2079  $To start only y
-0000e950: 6f75 7220 6170 706c 6963 6174 696f 6e2c  our application,
-0000e960: 2072 756e 2094 8594 8194 7d94 286a 2303   run .....}.(j#.
-0000e970: 0000 6aac 0b00 006a 3303 0000 6a11 0300  ..j....j3...j...
-0000e980: 006a 3403 0000 4e6a 3603 0000 4e75 626a  .j4...Nj6...Nubj
-0000e990: f905 0000 2981 947d 9428 6a13 0300 008c  ....)..}.(j.....
-0000e9a0: 1160 6070 7974 686f 6e20 6170 702e 7079  .``python app.py
-0000e9b0: 6060 946a 1403 0000 5d94 6a1e 0300 008c  ``.j....].j.....
-0000e9c0: 0d70 7974 686f 6e20 6170 702e 7079 9485  .python app.py..
-0000e9d0: 9481 947d 9428 6a23 0300 006a b40b 0000  ...}.(j#...j....
-0000e9e0: 6a33 0300 006a 1103 0000 6a34 0300 004e  j3...j....j4...N
-0000e9f0: 6a36 0300 004e 7562 616a 2403 0000 7d94  j6...Nubaj$...}.
-0000ea00: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-0000ea10: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-0000ea20: 0000 5d94 756a 3203 0000 6af8 0500 006a  ..].uj2...j....j
-0000ea30: 2303 0000 6aac 0b00 0075 626a 1e03 0000  #...j....ubj....
-0000ea40: 8c3c 2069 6e20 796f 7572 2070 726f 6a65  .< in your proje
-0000ea50: 6374 2072 6f6f 7420 6469 7265 6374 6f72  ct root director
-0000ea60: 792e 2055 7365 2074 6865 2074 6572 6d69  y. Use the termi
-0000ea70: 6e61 6c20 696e 2076 7363 6f64 652e 9485  nal in vscode...
-0000ea80: 9481 947d 9428 6a23 0300 006a ac0b 0000  ...}.(j#...j....
-0000ea90: 6a33 0300 006a 1103 0000 6a34 0300 004e  j3...j....j4...N
-0000eaa0: 6a36 0300 004e 7562 656a 2403 0000 7d94  j6...Nubej$...}.
-0000eab0: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-0000eac0: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-0000ead0: 0000 5d94 756a 3203 0000 6a5d 0300 006a  ..].uj2...j]...j
-0000eae0: 3403 0000 6a5c 0300 006a 3603 0000 4bee  4...j\...j6...K.
-0000eaf0: 6a23 0300 006a 9b0b 0000 6a33 0300 006a  j#...j....j3...j
-0000eb00: 1103 0000 7562 6a5e 0300 0029 8194 7d94  ....ubj^...)..}.
-0000eb10: 286a 1303 0000 8c34 4f70 656e 2074 6865  (j.....4Open the
-0000eb20: 2062 726f 7773 6572 2061 6e64 2074 7970   browser and typ
-0000eb30: 6520 6060 6874 7470 3a2f 2f6c 6f63 616c  e ``http://local
-0000eb40: 686f 7374 3a35 3535 3560 602e 946a 1403  host:5555``..j..
-0000eb50: 0000 5d94 286a 1e03 0000 8c1a 4f70 656e  ..].(j......Open
-0000eb60: 2074 6865 2062 726f 7773 6572 2061 6e64   the browser and
-0000eb70: 2074 7970 6520 9485 9481 947d 9428 6a23   type .....}.(j#
-0000eb80: 0300 006a cc0b 0000 6a33 0300 006a 1103  ...j....j3...j..
-0000eb90: 0000 6a34 0300 004e 6a36 0300 004e 7562  ..j4...Nj6...Nub
-0000eba0: 6af9 0500 0029 8194 7d94 286a 1303 0000  j....)..}.(j....
-0000ebb0: 8c19 6060 6874 7470 3a2f 2f6c 6f63 616c  ..``http://local
-0000ebc0: 686f 7374 3a35 3535 3560 6094 6a14 0300  host:5555``.j...
-0000ebd0: 005d 946a 1e03 0000 8c15 6874 7470 3a2f  .].j......http:/
-0000ebe0: 2f6c 6f63 616c 686f 7374 3a35 3535 3594  /localhost:5555.
-0000ebf0: 8594 8194 7d94 286a 2303 0000 6ad4 0b00  ....}.(j#...j...
-0000ec00: 006a 3303 0000 6a11 0300 006a 3403 0000  .j3...j....j4...
-0000ec10: 4e6a 3603 0000 4e75 6261 6a24 0300 007d  Nj6...Nubaj$...}
-0000ec20: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
-0000ec30: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
-0000ec40: 0300 005d 9475 6a32 0300 006a f805 0000  ...].uj2...j....
-0000ec50: 6a23 0300 006a cc0b 0000 7562 6a1e 0300  j#...j....ubj...
-0000ec60: 008c 012e 9485 9481 947d 9428 6a23 0300  .........}.(j#..
-0000ec70: 006a cc0b 0000 6a33 0300 006a 1103 0000  .j....j3...j....
-0000ec80: 6a34 0300 004e 6a36 0300 004e 7562 656a  j4...Nj6...Nubej
-0000ec90: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
-0000eca0: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
-0000ecb0: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
-0000ecc0: 6a5d 0300 006a 3403 0000 6a5c 0300 006a  j]...j4...j\...j
-0000ecd0: 3603 0000 4bf0 6a23 0300 006a 9b0b 0000  6...K.j#...j....
-0000ece0: 6a33 0300 006a 1103 0000 7562 6a37 0300  j3...j....ubj7..
-0000ecf0: 0029 8194 7d94 286a 1303 0000 685e 6a14  .)..}.(j....h^j.
-0000ed00: 0300 005d 9428 6a3c 0300 0029 8194 7d94  ...].(j<...)..}.
-0000ed10: 286a 1303 0000 8c0b 4465 7665 6c6f 706d  (j......Developm
-0000ed20: 656e 7494 6a14 0300 005d 946a 1e03 0000  ent.j....].j....
-0000ed30: 8c0b 4465 7665 6c6f 706d 656e 7494 8594  ..Development...
-0000ed40: 8194 7d94 286a 2303 0000 6aef 0b00 006a  ..}.(j#...j....j
-0000ed50: 3303 0000 6a11 0300 006a 3403 0000 4e6a  3...j....j4...Nj
-0000ed60: 3603 0000 4e75 6261 6a24 0300 007d 9428  6...Nubaj$...}.(
-0000ed70: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-0000ed80: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-0000ed90: 005d 9475 6a32 0300 006a 3b03 0000 6a23  .].uj2...j;...j#
-0000eda0: 0300 006a ec0b 0000 6a33 0300 006a 1103  ...j....j3...j..
-0000edb0: 0000 6a34 0300 006a 5c03 0000 6a36 0300  ..j4...j\...j6..
-0000edc0: 004b f375 626a 5e03 0000 2981 947d 9428  .K.ubj^...)..}.(
-0000edd0: 6a13 0300 008c 6c54 6f20 6465 7665 6c6f  j.....lTo develo
-0000ede0: 7020 796f 7572 2061 7070 6c69 6361 7469  p your applicati
-0000edf0: 6f6e 2c20 7573 6520 796f 7572 2064 6562  on, use your deb
-0000ee00: 7567 6765 7220 7769 7468 2074 6865 2060  ugger with the `
-0000ee10: 605b 6465 765d 2064 6563 6f72 6520 6261  `[dev] decore ba
-0000ee20: 7365 2064 6576 656c 6f70 6d65 6e74 6060  se development``
-0000ee30: 2070 726f 6669 6c65 2069 6e20 7673 636f   profile in vsco
-0000ee40: 6465 2e94 6a14 0300 005d 9428 6a1e 0300  de..j....].(j...
-0000ee50: 008c 3854 6f20 6465 7665 6c6f 7020 796f  ..8To develop yo
-0000ee60: 7572 2061 7070 6c69 6361 7469 6f6e 2c20  ur application, 
-0000ee70: 7573 6520 796f 7572 2064 6562 7567 6765  use your debugge
-0000ee80: 7220 7769 7468 2074 6865 2094 8594 8194  r with the .....
-0000ee90: 7d94 286a 2303 0000 6afd 0b00 006a 3303  }.(j#...j....j3.
-0000eea0: 0000 6a11 0300 006a 3403 0000 4e6a 3603  ..j....j4...Nj6.
-0000eeb0: 0000 4e75 626a f905 0000 2981 947d 9428  ..Nubj....)..}.(
-0000eec0: 6a13 0300 008c 2160 605b 6465 765d 2064  j.....!``[dev] d
-0000eed0: 6563 6f72 6520 6261 7365 2064 6576 656c  ecore base devel
-0000eee0: 6f70 6d65 6e74 6060 946a 1403 0000 5d94  opment``.j....].
-0000eef0: 6a1e 0300 008c 1d5b 6465 765d 2064 6563  j......[dev] dec
-0000ef00: 6f72 6520 6261 7365 2064 6576 656c 6f70  ore base develop
-0000ef10: 6d65 6e74 9485 9481 947d 9428 6a23 0300  ment.....}.(j#..
-0000ef20: 006a 050c 0000 6a33 0300 006a 1103 0000  .j....j3...j....
-0000ef30: 6a34 0300 004e 6a36 0300 004e 7562 616a  j4...Nj6...Nubaj
-0000ef40: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
-0000ef50: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
-0000ef60: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
-0000ef70: 6af8 0500 006a 2303 0000 6afd 0b00 0075  j....j#...j....u
-0000ef80: 626a 1e03 0000 8c13 2070 726f 6669 6c65  bj...... profile
-0000ef90: 2069 6e20 7673 636f 6465 2e94 8594 8194   in vscode......
-0000efa0: 7d94 286a 2303 0000 6afd 0b00 006a 3303  }.(j#...j....j3.
-0000efb0: 0000 6a11 0300 006a 3403 0000 4e6a 3603  ..j....j4...Nj6.
-0000efc0: 0000 4e75 6265 6a24 0300 007d 9428 6a26  ..Nubej$...}.(j&
-0000efd0: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
-0000efe0: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-0000eff0: 9475 6a32 0300 006a 5d03 0000 6a34 0300  .uj2...j]...j4..
-0000f000: 006a 5c03 0000 6a36 0300 004b f46a 2303  .j\...j6...K.j#.
-0000f010: 0000 6aec 0b00 006a 3303 0000 6a11 0300  ..j....j3...j...
-0000f020: 0075 626a 5e03 0000 2981 947d 9428 6a13  .ubj^...)..}.(j.
-0000f030: 0300 008c 344f 7065 6e20 7468 6520 6272  ....4Open the br
-0000f040: 6f77 7365 7220 616e 6420 7479 7065 2060  owser and type `
-0000f050: 6068 7474 703a 2f2f 6c6f 6361 6c68 6f73  `http://localhos
-0000f060: 743a 3535 3535 6060 2e94 6a14 0300 005d  t:5555``..j....]
-0000f070: 9428 6a1e 0300 008c 1a4f 7065 6e20 7468  .(j......Open th
-0000f080: 6520 6272 6f77 7365 7220 616e 6420 7479  e browser and ty
-0000f090: 7065 2094 8594 8194 7d94 286a 2303 0000  pe .....}.(j#...
-0000f0a0: 6a1d 0c00 006a 3303 0000 6a11 0300 006a  j....j3...j....j
-0000f0b0: 3403 0000 4e6a 3603 0000 4e75 626a f905  4...Nj6...Nubj..
-0000f0c0: 0000 2981 947d 9428 6a13 0300 008c 1960  ..)..}.(j......`
-0000f0d0: 6068 7474 703a 2f2f 6c6f 6361 6c68 6f73  `http://localhos
-0000f0e0: 743a 3535 3535 6060 946a 1403 0000 5d94  t:5555``.j....].
-0000f0f0: 6a1e 0300 008c 1568 7474 703a 2f2f 6c6f  j......http://lo
-0000f100: 6361 6c68 6f73 743a 3535 3535 9485 9481  calhost:5555....
-0000f110: 947d 9428 6a23 0300 006a 250c 0000 6a33  .}.(j#...j%...j3
-0000f120: 0300 006a 1103 0000 6a34 0300 004e 6a36  ...j....j4...Nj6
-0000f130: 0300 004e 7562 616a 2403 0000 7d94 286a  ...Nubaj$...}.(j
-0000f140: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
-0000f150: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
-0000f160: 5d94 756a 3203 0000 6af8 0500 006a 2303  ].uj2...j....j#.
-0000f170: 0000 6a1d 0c00 0075 626a 1e03 0000 8c01  ..j....ubj......
-0000f180: 2e94 8594 8194 7d94 286a 2303 0000 6a1d  ......}.(j#...j.
-0000f190: 0c00 006a 3303 0000 6a11 0300 006a 3403  ...j3...j....j4.
-0000f1a0: 0000 4e6a 3603 0000 4e75 6265 6a24 0300  ..Nj6...Nubej$..
-0000f1b0: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
-0000f1c0: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
-0000f1d0: 6a2e 0300 005d 9475 6a32 0300 006a 5d03  j....].uj2...j].
-0000f1e0: 0000 6a34 0300 006a 5c03 0000 6a36 0300  ..j4...j\...j6..
-0000f1f0: 004b f66a 2303 0000 6aec 0b00 006a 3303  .K.j#...j....j3.
-0000f200: 0000 6a11 0300 0075 6265 6a24 0300 007d  ..j....ubej$...}
-0000f210: 9428 6a26 0300 005d 948c 0b64 6576 656c  .(j&...]...devel
-0000f220: 6f70 6d65 6e74 9461 6a28 0300 005d 946a  opment.aj(...].j
-0000f230: 2a03 0000 5d94 8c0b 6465 7665 6c6f 706d  *...]...developm
-0000f240: 656e 7494 616a 2c03 0000 5d94 6a2e 0300  ent.aj,...].j...
-0000f250: 005d 9475 6a32 0300 0068 4e6a 2303 0000  .].uj2...hNj#...
-0000f260: 6a9b 0b00 006a 3303 0000 6a11 0300 006a  j....j3...j....j
-0000f270: 3403 0000 6a5c 0300 006a 3603 0000 4bf3  4...j\...j6...K.
-0000f280: 7562 6a37 0300 0029 8194 7d94 286a 1303  ubj7...)..}.(j..
-0000f290: 0000 685e 6a14 0300 005d 9428 6a3c 0300  ..h^j....].(j<..
-0000f2a0: 0029 8194 7d94 286a 1303 0000 8c05 4275  .)..}.(j......Bu
-0000f2b0: 696c 6494 6a14 0300 005d 946a 1e03 0000  ild.j....].j....
-0000f2c0: 8c05 4275 696c 6494 8594 8194 7d94 286a  ..Build.....}.(j
-0000f2d0: 2303 0000 6a48 0c00 006a 3303 0000 6a11  #...jH...j3...j.
-0000f2e0: 0300 006a 3403 0000 4e6a 3603 0000 4e75  ...j4...Nj6...Nu
-0000f2f0: 6261 6a24 0300 007d 9428 6a26 0300 005d  baj$...}.(j&...]
-0000f300: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
-0000f310: 2c03 0000 5d94 6a2e 0300 005d 9475 6a32  ,...].j....].uj2
-0000f320: 0300 006a 3b03 0000 6a23 0300 006a 450c  ...j;...j#...jE.
-0000f330: 0000 6a33 0300 006a 1103 0000 6a34 0300  ..j3...j....j4..
-0000f340: 006a 5c03 0000 6a36 0300 004b f975 626a  .j\...j6...K.ubj
-0000f350: 5e03 0000 2981 947d 9428 6a13 0300 008c  ^...)..}.(j.....
-0000f360: 7454 6f20 6275 696c 6420 796f 7572 2061  tTo build your a
-0000f370: 7070 6c69 6361 7469 6f6e 2c20 7275 6e20  pplication, run 
-0000f380: 6060 7079 7468 6f6e 2061 7070 2e70 7920  ``python app.py 
-0000f390: 2d2d 6275 696c 6460 6020 696e 2079 6f75  --build`` in you
-0000f3a0: 7220 7072 6f6a 6563 7420 726f 6f74 2064  r project root d
-0000f3b0: 6972 6563 746f 7279 2e20 5573 6520 7468  irectory. Use th
-0000f3c0: 6520 7465 726d 696e 616c 2069 6e20 7673  e terminal in vs
-0000f3d0: 636f 6465 2e94 6a14 0300 005d 9428 6a1e  code..j....].(j.
-0000f3e0: 0300 008c 1f54 6f20 6275 696c 6420 796f  .....To build yo
-0000f3f0: 7572 2061 7070 6c69 6361 7469 6f6e 2c20  ur application, 
-0000f400: 7275 6e20 9485 9481 947d 9428 6a23 0300  run .....}.(j#..
-0000f410: 006a 560c 0000 6a33 0300 006a 1103 0000  .jV...j3...j....
-0000f420: 6a34 0300 004e 6a36 0300 004e 7562 6af9  j4...Nj6...Nubj.
-0000f430: 0500 0029 8194 7d94 286a 1303 0000 8c19  ...)..}.(j......
-0000f440: 6060 7079 7468 6f6e 2061 7070 2e70 7920  ``python app.py 
-0000f450: 2d2d 6275 696c 6460 6094 6a14 0300 005d  --build``.j....]
-0000f460: 946a 1e03 0000 8c15 7079 7468 6f6e 2061  .j......python a
-0000f470: 7070 2e70 7920 2d2d 6275 696c 6494 8594  pp.py --build...
-0000f480: 8194 7d94 286a 2303 0000 6a5e 0c00 006a  ..}.(j#...j^...j
-0000f490: 3303 0000 6a11 0300 006a 3403 0000 4e6a  3...j....j4...Nj
-0000f4a0: 3603 0000 4e75 6261 6a24 0300 007d 9428  6...Nubaj$...}.(
-0000f4b0: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-0000f4c0: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-0000f4d0: 005d 9475 6a32 0300 006a f805 0000 6a23  .].uj2...j....j#
-0000f4e0: 0300 006a 560c 0000 7562 6a1e 0300 008c  ...jV...ubj.....
-0000f4f0: 3c20 696e 2079 6f75 7220 7072 6f6a 6563  < in your projec
-0000f500: 7420 726f 6f74 2064 6972 6563 746f 7279  t root directory
-0000f510: 2e20 5573 6520 7468 6520 7465 726d 696e  . Use the termin
-0000f520: 616c 2069 6e20 7673 636f 6465 2e94 8594  al in vscode....
-0000f530: 8194 7d94 286a 2303 0000 6a56 0c00 006a  ..}.(j#...jV...j
-0000f540: 3303 0000 6a11 0300 006a 3403 0000 4e6a  3...j....j4...Nj
-0000f550: 3603 0000 4e75 6265 6a24 0300 007d 9428  6...Nubej$...}.(
-0000f560: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-0000f570: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-0000f580: 005d 9475 6a32 0300 006a 5d03 0000 6a34  .].uj2...j]...j4
-0000f590: 0300 006a 5c03 0000 6a36 0300 004b fa6a  ...j\...j6...K.j
-0000f5a0: 2303 0000 6a45 0c00 006a 3303 0000 6a11  #...jE...j3...j.
-0000f5b0: 0300 0075 6265 6a24 0300 007d 9428 6a26  ...ubej$...}.(j&
-0000f5c0: 0300 005d 948c 0562 7569 6c64 9461 6a28  ...]...build.aj(
-0000f5d0: 0300 005d 946a 2a03 0000 5d94 8c05 6275  ...].j*...]...bu
-0000f5e0: 696c 6494 616a 2c03 0000 5d94 6a2e 0300  ild.aj,...].j...
-0000f5f0: 005d 9475 6a32 0300 0068 4e6a 2303 0000  .].uj2...hNj#...
-0000f600: 6a9b 0b00 006a 3303 0000 6a11 0300 006a  j....j3...j....j
-0000f610: 3403 0000 6a5c 0300 006a 3603 0000 4bf9  4...j\...j6...K.
-0000f620: 7562 656a 2403 0000 7d94 286a 2603 0000  ubej$...}.(j&...
-0000f630: 5d94 8c19 7275 6e2d 6465 7665 6c6f 706d  ]...run-developm
-0000f640: 656e 742d 616e 642d 6275 696c 6494 616a  ent-and-build.aj
-0000f650: 2803 0000 5d94 6a2a 0300 005d 948c 1a72  (...].j*...]...r
-0000f660: 756e 2c20 6465 7665 6c6f 706d 656e 7420  un, development 
-0000f670: 616e 6420 6275 696c 6494 616a 2c03 0000  and build.aj,...
-0000f680: 5d94 6a2e 0300 005d 9475 6a32 0300 0068  ].j....].uj2...h
-0000f690: 4e6a 2303 0000 6a9e 0400 006a 3303 0000  Nj#...j....j3...
-0000f6a0: 6a11 0300 006a 3403 0000 6a5c 0300 006a  j....j4...j\...j
-0000f6b0: 3603 0000 4bed 7562 656a 2403 0000 7d94  6...K.ubej$...}.
-0000f6c0: 286a 2603 0000 5d94 8c0b 6765 742d 7374  (j&...]...get-st
-0000f6d0: 6172 7465 6494 616a 2803 0000 5d94 6a2a  arted.aj(...].j*
-0000f6e0: 0300 005d 948c 0b67 6574 2073 7461 7274  ...]...get start
-0000f6f0: 6564 9461 6a2c 0300 005d 946a 2e03 0000  ed.aj,...].j....
-0000f700: 5d94 756a 3203 0000 684e 6a23 0300 006a  ].uj2...hNj#...j
-0000f710: 3803 0000 6a33 0300 006a 1103 0000 6a34  8...j3...j....j4
-0000f720: 0300 006a 5c03 0000 6a36 0300 004b 1a75  ...j\...j6...K.u
-0000f730: 626a 3703 0000 2981 947d 9428 6a13 0300  bj7...)..}.(j...
-0000f740: 0068 5e6a 1403 0000 5d94 286a 3c03 0000  .h^j....].(j<...
-0000f750: 2981 947d 9428 6a13 0300 008c 1253 616d  )..}.(j......Sam
-0000f760: 706c 6520 6170 706c 6963 6174 696f 6e94  ple application.
-0000f770: 6a14 0300 005d 946a 1e03 0000 8c12 5361  j....].j......Sa
-0000f780: 6d70 6c65 2061 7070 6c69 6361 7469 6f6e  mple application
-0000f790: 9485 9481 947d 9428 6a23 0300 006a 910c  .....}.(j#...j..
-0000f7a0: 0000 6a33 0300 006a 1103 0000 6a34 0300  ..j3...j....j4..
-0000f7b0: 004e 6a36 0300 004e 7562 616a 2403 0000  .Nj6...Nubaj$...
-0000f7c0: 7d94 286a 2603 0000 5d94 6a28 0300 005d  }.(j&...].j(...]
-0000f7d0: 946a 2a03 0000 5d94 6a2c 0300 005d 946a  .j*...].j,...].j
-0000f7e0: 2e03 0000 5d94 756a 3203 0000 6a3b 0300  ....].uj2...j;..
-0000f7f0: 006a 2303 0000 6a8e 0c00 006a 3303 0000  .j#...j....j3...
-0000f800: 6a11 0300 006a 3403 0000 6a5c 0300 006a  j....j4...j\...j
-0000f810: 3603 0000 4bfd 7562 6a5e 0300 0029 8194  6...K.ubj^...)..
-0000f820: 7d94 286a 1303 0000 8c9e 546f 2062 6574  }.(j......To bet
-0000f830: 7465 7220 756e 6465 7273 7461 6e64 2068  ter understand h
-0000f840: 6f77 2064 6563 6f72 6520 6261 7365 2077  ow decore base w
-0000f850: 6f72 6b73 2c20 6974 2069 7320 6265 7374  orks, it is best
-0000f860: 2074 6f20 6c6f 6f6b 2061 7420 7468 6520   to look at the 
-0000f870: 7361 6d70 6c65 2061 7070 6c69 6361 7469  sample applicati
-0000f880: 6f6e 2e20 5468 6520 6170 706c 6963 6174  on. The applicat
-0000f890: 696f 6e20 7265 7072 6573 656e 7473 206d  ion represents m
-0000f8a0: 7920 636f 6e74 696e 756f 7573 2064 6576  y continuous dev
-0000f8b0: 656c 6f70 6d65 6e74 206f 6620 6465 636f  elopment of deco
-0000f8c0: 7265 2062 6173 652e 946a 1403 0000 5d94  re base..j....].
-0000f8d0: 6a1e 0300 008c 9e54 6f20 6265 7474 6572  j......To better
-0000f8e0: 2075 6e64 6572 7374 616e 6420 686f 7720   understand how 
-0000f8f0: 6465 636f 7265 2062 6173 6520 776f 726b  decore base work
-0000f900: 732c 2069 7420 6973 2062 6573 7420 746f  s, it is best to
-0000f910: 206c 6f6f 6b20 6174 2074 6865 2073 616d   look at the sam
-0000f920: 706c 6520 6170 706c 6963 6174 696f 6e2e  ple application.
-0000f930: 2054 6865 2061 7070 6c69 6361 7469 6f6e   The application
-0000f940: 2072 6570 7265 7365 6e74 7320 6d79 2063   represents my c
-0000f950: 6f6e 7469 6e75 6f75 7320 6465 7665 6c6f  ontinuous develo
-0000f960: 706d 656e 7420 6f66 2064 6563 6f72 6520  pment of decore 
-0000f970: 6261 7365 2e94 8594 8194 7d94 286a 2303  base......}.(j#.
-0000f980: 0000 6a9f 0c00 006a 3303 0000 6a11 0300  ..j....j3...j...
-0000f990: 006a 3403 0000 4e6a 3603 0000 4e75 6261  .j4...Nj6...Nuba
-0000f9a0: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
-0000f9b0: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
-0000f9c0: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
-0000f9d0: 006a 5d03 0000 6a34 0300 006a 5c03 0000  .j]...j4...j\...
-0000f9e0: 6a36 0300 004b fe6a 2303 0000 6a8e 0c00  j6...K.j#...j...
-0000f9f0: 006a 3303 0000 6a11 0300 0075 626a 5e03  .j3...j....ubj^.
-0000fa00: 0000 2981 947d 9428 6a13 0300 008c 4868  ..)..}.(j.....Hh
-0000fa10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000fa20: 6d2f 4b65 6d6f 5061 6e7a 6168 2f64 6563  m/KemoPanzah/dec
-0000fa30: 6f72 655f 4261 7365 2f74 7265 652f 6d61  ore_Base/tree/ma
-0000fa40: 7374 6572 2f64 6563 6f72 655f 6261 7365  ster/decore_base
-0000fa50: 2f73 616d 706c 6594 6a14 0300 005d 946a  /sample.j....].j
-0000fa60: 9e03 0000 2981 947d 9428 6a13 0300 006a  ....)..}.(j....j
-0000fa70: af0c 0000 6a14 0300 005d 946a 1e03 0000  ....j....].j....
-0000fa80: 8c48 6874 7470 733a 2f2f 6769 7468 7562  .Hhttps://github
-0000fa90: 2e63 6f6d 2f4b 656d 6f50 616e 7a61 682f  .com/KemoPanzah/
-0000faa0: 6465 636f 7265 5f42 6173 652f 7472 6565  decore_Base/tree
-0000fab0: 2f6d 6173 7465 722f 6465 636f 7265 5f62  /master/decore_b
-0000fac0: 6173 652f 7361 6d70 6c65 9485 9481 947d  ase/sample.....}
-0000fad0: 9428 6a23 0300 006a b10c 0000 6a33 0300  .(j#...j....j3..
-0000fae0: 006a 1103 0000 6a34 0300 004e 6a36 0300  .j....j4...Nj6..
-0000faf0: 004e 7562 616a 2403 0000 7d94 286a 2603  .Nubaj$...}.(j&.
-0000fb00: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
-0000fb10: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
-0000fb20: 8c06 7265 6675 7269 946a af0c 0000 756a  ..refuri.j....uj
-0000fb30: 3203 0000 6a9d 0300 006a 2303 0000 6aad  2...j....j#...j.
-0000fb40: 0c00 0075 6261 6a24 0300 007d 9428 6a26  ...ubaj$...}.(j&
-0000fb50: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
-0000fb60: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-0000fb70: 9475 6a32 0300 006a 5d03 0000 6a34 0300  .uj2...j]...j4..
-0000fb80: 006a 5c03 0000 6a36 0300 004d 0001 6a23  .j\...j6...M..j#
-0000fb90: 0300 006a 8e0c 0000 6a33 0300 006a 1103  ...j....j3...j..
-0000fba0: 0000 7562 6a5e 0300 0029 8194 7d94 286a  ..ubj^...)..}.(j
-0000fbb0: 1303 0000 8cb0 546f 2073 796e 6368 726f  ......To synchro
-0000fbc0: 6e69 7a65 2074 6865 2073 616d 706c 6520  nize the sample 
-0000fbd0: 6170 706c 6963 6174 696f 6e20 7769 7468  application with
-0000fbe0: 2061 2073 7562 666f 6c64 6572 206f 6620   a subfolder of 
-0000fbf0: 7468 6520 7072 6f6a 6563 7420 726f 6f74  the project root
-0000fc00: 2064 6972 6563 746f 7279 2c20 7275 6e20   directory, run 
-0000fc10: 6060 7079 7468 6f6e 2061 7070 2e70 7920  ``python app.py 
-0000fc20: 2d2d 7361 6d70 6c65 6060 2069 6e20 796f  --sample`` in yo
-0000fc30: 7572 2070 726f 6a65 6374 2072 6f6f 7420  ur project root 
-0000fc40: 6469 7265 6374 6f72 792e 2055 7365 2074  directory. Use t
-0000fc50: 6865 2074 6572 6d69 6e61 6c20 696e 2076  he terminal in v
-0000fc60: 7363 6f64 652e 946a 1403 0000 5d94 286a  scode..j....].(j
-0000fc70: 1e03 0000 8c5a 546f 2073 796e 6368 726f  .....ZTo synchro
-0000fc80: 6e69 7a65 2074 6865 2073 616d 706c 6520  nize the sample 
-0000fc90: 6170 706c 6963 6174 696f 6e20 7769 7468  application with
-0000fca0: 2061 2073 7562 666f 6c64 6572 206f 6620   a subfolder of 
-0000fcb0: 7468 6520 7072 6f6a 6563 7420 726f 6f74  the project root
-0000fcc0: 2064 6972 6563 746f 7279 2c20 7275 6e20   directory, run 
-0000fcd0: 9485 9481 947d 9428 6a23 0300 006a c50c  .....}.(j#...j..
-0000fce0: 0000 6a33 0300 006a 1103 0000 6a34 0300  ..j3...j....j4..
-0000fcf0: 004e 6a36 0300 004e 7562 6af9 0500 0029  .Nj6...Nubj....)
-0000fd00: 8194 7d94 286a 1303 0000 8c1a 6060 7079  ..}.(j......``py
-0000fd10: 7468 6f6e 2061 7070 2e70 7920 2d2d 7361  thon app.py --sa
-0000fd20: 6d70 6c65 6060 946a 1403 0000 5d94 6a1e  mple``.j....].j.
-0000fd30: 0300 008c 1670 7974 686f 6e20 6170 702e  .....python app.
-0000fd40: 7079 202d 2d73 616d 706c 6594 8594 8194  py --sample.....
-0000fd50: 7d94 286a 2303 0000 6acd 0c00 006a 3303  }.(j#...j....j3.
-0000fd60: 0000 6a11 0300 006a 3403 0000 4e6a 3603  ..j....j4...Nj6.
-0000fd70: 0000 4e75 6261 6a24 0300 007d 9428 6a26  ..Nubaj$...}.(j&
-0000fd80: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
-0000fd90: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-0000fda0: 9475 6a32 0300 006a f805 0000 6a23 0300  .uj2...j....j#..
-0000fdb0: 006a c50c 0000 7562 6a1e 0300 008c 3c20  .j....ubj.....< 
-0000fdc0: 696e 2079 6f75 7220 7072 6f6a 6563 7420  in your project 
-0000fdd0: 726f 6f74 2064 6972 6563 746f 7279 2e20  root directory. 
-0000fde0: 5573 6520 7468 6520 7465 726d 696e 616c  Use the terminal
-0000fdf0: 2069 6e20 7673 636f 6465 2e94 8594 8194   in vscode......
-0000fe00: 7d94 286a 2303 0000 6ac5 0c00 006a 3303  }.(j#...j....j3.
-0000fe10: 0000 6a11 0300 006a 3403 0000 4e6a 3603  ..j....j4...Nj6.
-0000fe20: 0000 4e75 6265 6a24 0300 007d 9428 6a26  ..Nubej$...}.(j&
-0000fe30: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
-0000fe40: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-0000fe50: 9475 6a32 0300 006a 5d03 0000 6a34 0300  .uj2...j]...j4..
-0000fe60: 006a 5c03 0000 6a36 0300 004d 0201 6a23  .j\...j6...M..j#
-0000fe70: 0300 006a 8e0c 0000 6a33 0300 006a 1103  ...j....j3...j..
-0000fe80: 0000 7562 6a5e 0300 0029 8194 7d94 286a  ..ubj^...)..}.(j
-0000fe90: 1303 0000 8c7f 546f 2072 756e 2074 6865  ......To run the
-0000fea0: 2073 616d 706c 6520 6170 706c 6963 6174   sample applicat
-0000feb0: 696f 6e20 6166 7465 7220 7379 6e63 6872  ion after synchr
-0000fec0: 6f6e 697a 6174 696f 6e2c 2075 7365 2079  onization, use y
-0000fed0: 6f75 7220 6465 6275 6767 6572 2077 6974  our debugger wit
-0000fee0: 6820 7468 6520 6060 5b73 6d70 5d20 6465  h the ``[smp] de
-0000fef0: 636f 7265 2062 6173 6520 7361 6d70 6c65  core base sample
-0000ff00: 6060 2070 726f 6669 6c65 2069 6e20 7673  `` profile in vs
-0000ff10: 636f 6465 2e94 6a14 0300 005d 9428 6a1e  code..j....].(j.
-0000ff20: 0300 008c 5054 6f20 7275 6e20 7468 6520  ....PTo run the 
-0000ff30: 7361 6d70 6c65 2061 7070 6c69 6361 7469  sample applicati
-0000ff40: 6f6e 2061 6674 6572 2073 796e 6368 726f  on after synchro
-0000ff50: 6e69 7a61 7469 6f6e 2c20 7573 6520 796f  nization, use yo
-0000ff60: 7572 2064 6562 7567 6765 7220 7769 7468  ur debugger with
-0000ff70: 2074 6865 2094 8594 8194 7d94 286a 2303   the .....}.(j#.
-0000ff80: 0000 6ae5 0c00 006a 3303 0000 6a11 0300  ..j....j3...j...
-0000ff90: 006a 3403 0000 4e6a 3603 0000 4e75 626a  .j4...Nj6...Nubj
-0000ffa0: f905 0000 2981 947d 9428 6a13 0300 008c  ....)..}.(j.....
-0000ffb0: 1c60 605b 736d 705d 2064 6563 6f72 6520  .``[smp] decore 
-0000ffc0: 6261 7365 2073 616d 706c 6560 6094 6a14  base sample``.j.
-0000ffd0: 0300 005d 946a 1e03 0000 8c18 5b73 6d70  ...].j......[smp
-0000ffe0: 5d20 6465 636f 7265 2062 6173 6520 7361  ] decore base sa
-0000fff0: 6d70 6c65 9485 9481 947d 9428 6a23 0300  mple.....}.(j#..
-00010000: 006a ed0c 0000 6a33 0300 0095 b235 0000  .j....j3.....5..
-00010010: 0000 0000 6a11 0300 006a 3403 0000 4e6a  ....j....j4...Nj
-00010020: 3603 0000 4e75 6261 6a24 0300 007d 9428  6...Nubaj$...}.(
-00010030: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-00010040: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-00010050: 005d 9475 6a32 0300 006a f805 0000 6a23  .].uj2...j....j#
-00010060: 0300 006a e50c 0000 7562 6a1e 0300 008c  ...j....ubj.....
-00010070: 1320 7072 6f66 696c 6520 696e 2076 7363  . profile in vsc
-00010080: 6f64 652e 9485 9481 947d 9428 6a23 0300  ode......}.(j#..
-00010090: 006a e50c 0000 6a33 0300 006a 1103 0000  .j....j3...j....
-000100a0: 6a34 0300 004e 6a36 0300 004e 7562 656a  j4...Nj6...Nubej
-000100b0: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
-000100c0: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
-000100d0: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
-000100e0: 6a5d 0300 006a 3403 0000 6a5c 0300 006a  j]...j4...j\...j
-000100f0: 3603 0000 4d04 016a 2303 0000 6a8e 0c00  6...M..j#...j...
-00010100: 006a 3303 0000 6a11 0300 0075 6265 6a24  .j3...j....ubej$
-00010110: 0300 007d 9428 6a26 0300 005d 948c 1273  ...}.(j&...]...s
-00010120: 616d 706c 652d 6170 706c 6963 6174 696f  ample-applicatio
-00010130: 6e94 616a 2803 0000 5d94 6a2a 0300 005d  n.aj(...].j*...]
-00010140: 948c 1273 616d 706c 6520 6170 706c 6963  ...sample applic
-00010150: 6174 696f 6e94 616a 2c03 0000 5d94 6a2e  ation.aj,...].j.
-00010160: 0300 005d 9475 6a32 0300 0068 4e6a 2303  ...].uj2...hNj#.
-00010170: 0000 6a38 0300 006a 3303 0000 6a11 0300  ..j8...j3...j...
-00010180: 006a 3403 0000 6a5c 0300 006a 3603 0000  .j4...j\...j6...
-00010190: 4bfd 7562 6a37 0300 0029 8194 7d94 286a  K.ubj7...)..}.(j
-000101a0: 1303 0000 685e 6a14 0300 005d 9428 6a3c  ....h^j....].(j<
-000101b0: 0300 0029 8194 7d94 286a 1303 0000 8c05  ...)..}.(j......
-000101c0: 4e6f 7465 7394 6a14 0300 005d 946a 1e03  Notes.j....].j..
-000101d0: 0000 8c05 4e6f 7465 7394 8594 8194 7d94  ....Notes.....}.
-000101e0: 286a 2303 0000 6a10 0d00 006a 3303 0000  (j#...j....j3...
-000101f0: 6a11 0300 006a 3403 0000 4e6a 3603 0000  j....j4...Nj6...
-00010200: 4e75 6261 6a24 0300 007d 9428 6a26 0300  Nubaj$...}.(j&..
-00010210: 005d 946a 2803 0000 5d94 6a2a 0300 005d  .].j(...].j*...]
-00010220: 946a 2c03 0000 5d94 6a2e 0300 005d 9475  .j,...].j....].u
-00010230: 6a32 0300 006a 3b03 0000 6a23 0300 006a  j2...j;...j#...j
-00010240: 0d0d 0000 6a33 0300 006a 1103 0000 6a34  ....j3...j....j4
-00010250: 0300 006a 5c03 0000 6a36 0300 004d 0701  ...j\...j6...M..
-00010260: 7562 6a5e 0300 0029 8194 7d94 286a 1303  ubj^...)..}.(j..
-00010270: 0000 8c46 5468 6973 2064 6f63 756d 656e  ...FThis documen
-00010280: 7461 7469 6f6e 2077 6173 2074 7261 6e73  tation was trans
-00010290: 6c61 7465 6420 6672 6f6d 2047 6572 6d61  lated from Germa
-000102a0: 6e20 696e 746f 2045 6e67 6c69 7368 2077  n into English w
-000102b0: 6974 6820 4465 6570 6c2e 946a 1403 0000  ith Deepl..j....
-000102c0: 5d94 6a1e 0300 008c 4654 6869 7320 646f  ].j.....FThis do
-000102d0: 6375 6d65 6e74 6174 696f 6e20 7761 7320  cumentation was 
-000102e0: 7472 616e 736c 6174 6564 2066 726f 6d20  translated from 
-000102f0: 4765 726d 616e 2069 6e74 6f20 456e 676c  German into Engl
-00010300: 6973 6820 7769 7468 2044 6565 706c 2e94  ish with Deepl..
-00010310: 8594 8194 7d94 286a 2303 0000 6a1e 0d00  ....}.(j#...j...
-00010320: 006a 3303 0000 6a11 0300 006a 3403 0000  .j3...j....j4...
-00010330: 4e6a 3603 0000 4e75 6261 6a24 0300 007d  Nj6...Nubaj$...}
-00010340: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
-00010350: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
-00010360: 0300 005d 9475 6a32 0300 006a 5d03 0000  ...].uj2...j]...
-00010370: 6a34 0300 006a 5c03 0000 6a36 0300 004d  j4...j\...j6...M
-00010380: 0801 6a23 0300 006a 0d0d 0000 6a33 0300  ..j#...j....j3..
-00010390: 006a 1103 0000 7562 6a16 0300 008c 0863  .j....ubj......c
-000103a0: 6f6d 706f 756e 6494 9394 2981 947d 9428  ompound...)..}.(
-000103b0: 6a13 0300 0068 5e6a 1403 0000 5d94 6a0e  j....h^j....].j.
-000103c0: 0300 008c 0774 6f63 7472 6565 9493 9429  .....toctree...)
-000103d0: 8194 7d94 286a 1303 0000 685e 6a14 0300  ..}.(j....h^j...
-000103e0: 005d 946a 2403 0000 7d94 286a 2603 0000  .].j$...}.(j&...
-000103f0: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
-00010400: 6a2c 0300 005d 946a 2e03 0000 5d94 6a23  j,...].j....].j#
-00010410: 0300 006a cd02 0000 8c07 656e 7472 6965  ...j......entrie
-00010420: 7394 5d94 8c0c 696e 636c 7564 6566 696c  s.]...includefil
-00010430: 6573 945d 948c 086d 6178 6465 7074 6894  es.]...maxdepth.
-00010440: 4b02 8c07 6361 7074 696f 6e94 4e8c 0467  K...caption.N..g
-00010450: 6c6f 6294 898c 0668 6964 6465 6e94 888c  lob....hidden...
-00010460: 0d69 6e63 6c75 6465 6869 6464 656e 9489  .includehidden..
-00010470: 8c08 6e75 6d62 6572 6564 944b 008c 0a74  ..numbered.K...t
-00010480: 6974 6c65 736f 6e6c 7994 898c 0a72 6177  itlesonly....raw
-00010490: 656e 7472 6965 7394 5d94 756a 3203 0000  entries.].uj2...
-000104a0: 6a31 0d00 006a 3403 0000 6a35 0300 006a  j1...j4...j5...j
-000104b0: 3603 0000 4b0b 6a23 0300 006a 2e0d 0000  6...K.j#...j....
-000104c0: 7562 616a 2403 0000 7d94 286a 2603 0000  ubaj$...}.(j&...
-000104d0: 5d94 6a28 0300 005d 948c 0f74 6f63 7472  ].j(...]...toctr
-000104e0: 6565 2d77 7261 7070 6572 9461 6a2a 0300  ee-wrapper.aj*..
-000104f0: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-00010500: 9475 6a32 0300 006a 2c0d 0000 6a23 0300  .uj2...j,...j#..
-00010510: 006a 0d0d 0000 6a33 0300 006a 1103 0000  .j....j3...j....
-00010520: 6a34 0300 006a 3503 0000 6a36 0300 004e  j4...j5...j6...N
-00010530: 7562 6a18 0300 0029 8194 7d94 286a 1303  ubj....)..}.(j..
-00010540: 0000 8c12 496e 6469 6365 7320 616e 6420  ....Indices and 
-00010550: 7461 626c 6573 946a 1403 0000 5d94 6a1e  tables.j....].j.
-00010560: 0300 008c 1249 6e64 6963 6573 2061 6e64  .....Indices and
-00010570: 2074 6162 6c65 7394 8594 8194 7d94 6a23   tables.....}.j#
-00010580: 0300 006a 500d 0000 7362 616a 2403 0000  ...jP...sbaj$...
-00010590: 7d94 286a 2603 0000 5d94 6a28 0300 005d  }.(j&...].j(...]
-000105a0: 946a 2a03 0000 5d94 6a2c 0300 005d 946a  .j*...].j,...].j
-000105b0: 2e03 0000 5d94 6a30 0300 006a 3103 0000  ....].j0...j1...
-000105c0: 756a 3203 0000 6a17 0300 006a 2303 0000  uj2...j....j#...
-000105d0: 6a0d 0d00 006a 3303 0000 6a11 0300 006a  j....j3...j....j
-000105e0: 3403 0000 6a35 0300 006a 3603 0000 4b0f  4...j5...j6...K.
-000105f0: 7562 6a18 0300 0029 8194 7d94 286a 1303  ubj....)..}.(j..
-00010600: 0000 8c12 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ....============
-00010610: 3d3d 3d3d 3d3d 946a 1403 0000 5d94 6a1e  ======.j....].j.
-00010620: 0300 008c 123d 3d3d 3d3d 3d3d 3d3d 3d3d  .....===========
-00010630: 3d3d 3d3d 3d3d 3d94 8594 8194 7d94 6a23  =======.....}.j#
-00010640: 0300 006a 5e0d 0000 7362 616a 2403 0000  ...j^...sbaj$...
-00010650: 7d94 286a 2603 0000 5d94 6a28 0300 005d  }.(j&...].j(...]
-00010660: 946a 2a03 0000 5d94 6a2c 0300 005d 946a  .j*...].j,...].j
-00010670: 2e03 0000 5d94 6a30 0300 006a 3103 0000  ....].j0...j1...
-00010680: 756a 3203 0000 6a17 0300 006a 2303 0000  uj2...j....j#...
-00010690: 6a0d 0d00 006a 3303 0000 6a11 0300 006a  j....j3...j....j
-000106a0: 3403 0000 6a35 0300 006a 3603 0000 4b11  4...j5...j6...K.
-000106b0: 7562 6a18 0300 0029 8194 7d94 286a 1303  ubj....)..}.(j..
-000106c0: 0000 8c11 2a20 3a72 6566 3a60 6765 6e69  ....* :ref:`geni
-000106d0: 6e64 6578 6094 6a14 0300 005d 946a 1e03  ndex`.j....].j..
-000106e0: 0000 8c11 2a20 3a72 6566 3a60 6765 6e69  ....* :ref:`geni
-000106f0: 6e64 6578 6094 8594 8194 7d94 6a23 0300  ndex`.....}.j#..
-00010700: 006a 6c0d 0000 7362 616a 2403 0000 7d94  .jl...sbaj$...}.
-00010710: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-00010720: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-00010730: 0000 5d94 6a30 0300 006a 3103 0000 756a  ..].j0...j1...uj
-00010740: 3203 0000 6a17 0300 006a 2303 0000 6a0d  2...j....j#...j.
-00010750: 0d00 006a 3303 0000 6a11 0300 006a 3403  ...j3...j....j4.
-00010760: 0000 6a35 0300 006a 3603 0000 4b12 7562  ..j5...j6...K.ub
-00010770: 6a18 0300 0029 8194 7d94 286a 1303 0000  j....)..}.(j....
-00010780: 8c11 2a20 3a72 6566 3a60 6d6f 6469 6e64  ..* :ref:`modind
-00010790: 6578 6094 6a14 0300 005d 946a 1e03 0000  ex`.j....].j....
-000107a0: 8c11 2a20 3a72 6566 3a60 6d6f 6469 6e64  ..* :ref:`modind
-000107b0: 6578 6094 8594 8194 7d94 6a23 0300 006a  ex`.....}.j#...j
-000107c0: 7a0d 0000 7362 616a 2403 0000 7d94 286a  z...sbaj$...}.(j
-000107d0: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
-000107e0: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
-000107f0: 5d94 6a30 0300 006a 3103 0000 756a 3203  ].j0...j1...uj2.
-00010800: 0000 6a17 0300 006a 2303 0000 6a0d 0d00  ..j....j#...j...
-00010810: 006a 3303 0000 6a11 0300 006a 3403 0000  .j3...j....j4...
-00010820: 6a35 0300 006a 3603 0000 4b13 7562 6a18  j5...j6...K.ubj.
-00010830: 0300 0029 8194 7d94 286a 1303 0000 8c0f  ...)..}.(j......
-00010840: 2a20 3a72 6566 3a60 7365 6172 6368 6094  * :ref:`search`.
-00010850: 6a14 0300 005d 946a 1e03 0000 8c0f 2a20  j....].j......* 
-00010860: 3a72 6566 3a60 7365 6172 6368 6094 8594  :ref:`search`...
-00010870: 8194 7d94 6a23 0300 006a 880d 0000 7362  ..}.j#...j....sb
-00010880: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
-00010890: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
-000108a0: 0300 005d 946a 2e03 0000 5d94 6a30 0300  ...].j....].j0..
-000108b0: 006a 3103 0000 756a 3203 0000 6a17 0300  .j1...uj2...j...
-000108c0: 006a 2303 0000 6a0d 0d00 006a 3303 0000  .j#...j....j3...
-000108d0: 6a11 0300 006a 3403 0000 6a35 0300 006a  j....j4...j5...j
-000108e0: 3603 0000 4b14 7562 656a 2403 0000 7d94  6...K.ubej$...}.
-000108f0: 286a 2603 0000 5d94 8c05 6e6f 7465 7394  (j&...]...notes.
-00010900: 616a 2803 0000 5d94 6a2a 0300 005d 948c  aj(...].j*...]..
-00010910: 056e 6f74 6573 9461 6a2c 0300 005d 946a  .notes.aj,...].j
-00010920: 2e03 0000 5d94 756a 3203 0000 684e 6a23  ....].uj2...hNj#
-00010930: 0300 006a 3803 0000 6a33 0300 006a 1103  ...j8...j3...j..
-00010940: 0000 6a34 0300 006a 5c03 0000 6a36 0300  ..j4...j\...j6..
-00010950: 004d 0701 7562 656a 2403 0000 7d94 286a  .M..ubej$...}.(j
-00010960: 2603 0000 5d94 8c07 7765 6c63 6f6d 6594  &...]...welcome.
-00010970: 616a 2803 0000 5d94 6a2a 0300 005d 948c  aj(...].j*...]..
-00010980: 0777 656c 636f 6d65 9461 6a2c 0300 005d  .welcome.aj,...]
-00010990: 946a 2e03 0000 5d94 756a 3203 0000 684e  .j....].uj2...hN
-000109a0: 6a23 0300 006a 1103 0000 6a33 0300 006a  j#...j....j3...j
-000109b0: 1103 0000 6a34 0300 006a 3503 0000 6a36  ....j4...j5...j6
-000109c0: 0300 004b 0775 6265 6a24 0300 007d 9428  ...K.ubej$...}.(
-000109d0: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-000109e0: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-000109f0: 005d 948c 0673 6f75 7263 6594 6a35 0300  .]...source.j5..
-00010a00: 0075 6a32 0300 006a 0f03 0000 8c0e 6375  .uj2...j......cu
-00010a10: 7272 656e 745f 736f 7572 6365 944e 8c0c  rrent_source.N..
-00010a20: 6375 7272 656e 745f 6c69 6e65 944e 6ade  current_line.Nj.
-00010a30: 0200 008c 1164 6f63 7574 696c 732e 6672  .....docutils.fr
-00010a40: 6f6e 7465 6e64 948c 0656 616c 7565 7394  ontend...Values.
-00010a50: 9394 2981 947d 9428 6a3b 0300 004e 8c09  ..)..}.(j;...N..
-00010a60: 6765 6e65 7261 746f 7294 4e8c 0964 6174  generator.N..dat
-00010a70: 6573 7461 6d70 944e 8c0b 736f 7572 6365  estamp.N..source
-00010a80: 5f6c 696e 6b94 4e8c 0a73 6f75 7263 655f  _link.N..source_
-00010a90: 7572 6c94 4e8c 0d74 6f63 5f62 6163 6b6c  url.N..toc_backl
-00010aa0: 696e 6b73 948c 0565 6e74 7279 948c 1266  inks...entry...f
-00010ab0: 6f6f 746e 6f74 655f 6261 636b 6c69 6e6b  ootnote_backlink
-00010ac0: 7394 4b01 8c0d 7365 6374 6e75 6d5f 7866  s.K...sectnum_xf
-00010ad0: 6f72 6d94 4b01 8c0e 7374 7269 705f 636f  orm.K...strip_co
-00010ae0: 6d6d 656e 7473 944e 8c1b 7374 7269 705f  mments.N..strip_
-00010af0: 656c 656d 656e 7473 5f77 6974 685f 636c  elements_with_cl
-00010b00: 6173 7365 7394 4e8c 0d73 7472 6970 5f63  asses.N..strip_c
-00010b10: 6c61 7373 6573 944e 8c0c 7265 706f 7274  lasses.N..report
-00010b20: 5f6c 6576 656c 944b 026a f002 0000 4b05  _level.K.j....K.
-00010b30: 8c11 6578 6974 5f73 7461 7475 735f 6c65  ..exit_status_le
-00010b40: 7665 6c94 4b05 8c05 6465 6275 6794 4e8c  vel.K...debug.N.
-00010b50: 0e77 6172 6e69 6e67 5f73 7472 6561 6d94  .warning_stream.
-00010b60: 4e8c 0974 7261 6365 6261 636b 9488 6aec  N..traceback..j.
-00010b70: 0200 0068 818c 1c69 6e70 7574 5f65 6e63  ...h...input_enc
-00010b80: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-00010b90: 6c65 7294 8c06 7374 7269 6374 948c 0f6f  ler...strict...o
-00010ba0: 7574 7075 745f 656e 636f 6469 6e67 948c  utput_encoding..
-00010bb0: 0575 7466 2d38 948c 1d6f 7574 7075 745f  .utf-8...output_
-00010bc0: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
-00010bd0: 616e 646c 6572 946a c50d 0000 8c0e 6572  andler.j......er
-00010be0: 726f 725f 656e 636f 6469 6e67 948c 0575  ror_encoding...u
-00010bf0: 7466 2d38 948c 1c65 7272 6f72 5f65 6e63  tf-8...error_enc
-00010c00: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-00010c10: 6c65 7294 8c10 6261 636b 736c 6173 6872  ler...backslashr
-00010c20: 6570 6c61 6365 946a f402 0000 686a 8c13  eplace.j....hj..
-00010c30: 7265 636f 7264 5f64 6570 656e 6465 6e63  record_dependenc
-00010c40: 6965 7394 4e68 0a4e 8c09 6964 5f70 7265  ies.Nh.N..id_pre
-00010c50: 6669 7894 685e 6ae0 0200 006a e102 0000  fix.h^j....j....
-00010c60: 8c0d 6475 6d70 5f73 6574 7469 6e67 7394  ..dump_settings.
-00010c70: 4e8c 0e64 756d 705f 696e 7465 726e 616c  N..dump_internal
-00010c80: 7394 4e8c 0f64 756d 705f 7472 616e 7366  s.N..dump_transf
-00010c90: 6f72 6d73 944e 8c0f 6475 6d70 5f70 7365  orms.N..dump_pse
-00010ca0: 7564 6f5f 786d 6c94 4e8c 1065 7870 6f73  udo_xml.N..expos
-00010cb0: 655f 696e 7465 726e 616c 7394 4e8c 0e73  e_internals.N..s
-00010cc0: 7472 6963 745f 7669 7369 746f 7294 4e8c  trict_visitor.N.
-00010cd0: 0f5f 6469 7361 626c 655f 636f 6e66 6967  ._disable_config
-00010ce0: 944e 8c07 5f73 6f75 7263 6594 6a35 0300  .N.._source.j5..
-00010cf0: 008c 0c5f 6465 7374 696e 6174 696f 6e94  ..._destination.
-00010d00: 4e8c 0d5f 636f 6e66 6967 5f66 696c 6573  N.._config_files
-00010d10: 945d 946a f102 0000 888c 0b72 6177 5f65  .].j.......raw_e
-00010d20: 6e61 626c 6564 944b 018c 116c 696e 655f  nabled.K...line_
-00010d30: 6c65 6e67 7468 5f6c 696d 6974 944d 1027  length_limit.M.'
-00010d40: 6ae8 0200 004e 6ae6 0200 006a e702 0000  j....Nj....j....
-00010d50: 8c15 7065 705f 6669 6c65 5f75 726c 5f74  ..pep_file_url_t
-00010d60: 656d 706c 6174 6594 8c08 7065 702d 2530  emplate...pep-%0
-00010d70: 3464 946a eb02 0000 4e6a e902 0000 6aea  4d.j....Nj....j.
-00010d80: 0200 008c 0974 6162 5f77 6964 7468 944b  .....tab_width.K
-00010d90: 0868 9389 8c10 7379 6e74 6178 5f68 6967  .h....syntax_hig
-00010da0: 686c 6967 6874 948c 046c 6f6e 6794 6af5  hlight...long.j.
-00010db0: 0200 0088 6af2 0200 006a f302 0000 8c1d  ....j....j......
-00010dc0: 6368 6172 6163 7465 725f 6c65 7665 6c5f  character_level_
-00010dd0: 696e 6c69 6e65 5f6d 6172 6b75 7094 896a  inline_markup..j
-00010de0: ed02 0000 898c 0d64 6f63 696e 666f 5f78  .......docinfo_x
-00010df0: 666f 726d 944b 016a ee02 0000 896a e202  form.K.j.....j..
-00010e00: 0000 6ae3 0200 006a e402 0000 896a e502  ..j....j.....j..
-00010e10: 0000 886a ef02 0000 8968 5a4e 7562 8c08  ...j.....hZNub..
-00010e20: 7265 706f 7274 6572 944e 8c10 696e 6469  reporter.N..indi
-00010e30: 7265 6374 5f74 6172 6765 7473 945d 948c  rect_targets.]..
-00010e40: 1173 7562 7374 6974 7574 696f 6e5f 6465  .substitution_de
-00010e50: 6673 947d 948c 1273 7562 7374 6974 7574  fs.}...substitut
-00010e60: 696f 6e5f 6e61 6d65 7394 7d94 8c08 7265  ion_names.}...re
-00010e70: 666e 616d 6573 947d 948c 0672 6566 6964  fnames.}...refid
-00010e80: 7394 7d94 8c07 6e61 6d65 6964 7394 7d94  s.}...nameids.}.
-00010e90: 286a a30d 0000 6aa0 0d00 006a e903 0000  (j....j....j....
-00010ea0: 6ae6 0300 006a bb03 0000 6ab8 0300 006a  j....j....j....j
-00010eb0: 9b04 0000 6a98 0400 006a 8c04 0000 6a89  ....j....j....j.
-00010ec0: 0400 006a 8b0c 0000 6a88 0c00 006a 6c05  ...j....j....jl.
-00010ed0: 0000 6a69 0500 006a 5905 0000 6a56 0500  ..ji...jY...jV..
-00010ee0: 006a 2906 0000 6a26 0600 006a 980b 0000  .j)...j&...j....
-00010ef0: 6a95 0b00 006a 3b08 0000 6a38 0800 006a  j....j;...j8...j
-00010f00: 0908 0000 6a06 0800 006a 6f09 0000 6a6c  ....j....jo...jl
-00010f10: 0900 006a e609 0000 6ae3 0900 006a 5d0a  ...j....j....j].
-00010f20: 0000 6a5a 0a00 006a a20a 0000 6a9f 0a00  ..jZ...j....j...
-00010f30: 006a 900b 0000 6a8d 0b00 006a 830c 0000  .j....j....j....
-00010f40: 6a80 0c00 006a 420c 0000 6a3f 0c00 006a  j....jB...j?...j
-00010f50: 7b0c 0000 6a78 0c00 006a 0a0d 0000 6a07  {...jx...j....j.
-00010f60: 0d00 006a 9b0d 0000 6a98 0d00 0075 8c09  ...j....j....u..
-00010f70: 6e61 6d65 7479 7065 7394 7d94 286a a30d  nametypes.}.(j..
-00010f80: 0000 896a e903 0000 896a bb03 0000 886a  ...j.....j.....j
-00010f90: 9b04 0000 896a 8c04 0000 886a 8b0c 0000  .....j.....j....
-00010fa0: 896a 6c05 0000 896a 5905 0000 886a 2906  .jl....jY....j).
-00010fb0: 0000 896a 980b 0000 896a 3b08 0000 896a  ...j.....j;....j
-00010fc0: 0908 0000 886a 6f09 0000 896a e609 0000  .....jo....j....
-00010fd0: 896a 5d0a 0000 896a a20a 0000 896a 900b  .j]....j.....j..
-00010fe0: 0000 896a 830c 0000 896a 420c 0000 896a  ...j.....jB....j
-00010ff0: 7b0c 0000 896a 0a0d 0000 896a 9b0d 0000  {....j.....j....
-00011000: 8975 6a26 0300 007d 9428 6aa0 0d00 006a  .uj&...}.(j....j
-00011010: 3803 0000 6ae6 0300 006a 4b03 0000 6ab8  8...j....jK...j.
-00011020: 0300 006a b203 0000 6a98 0400 006a ec03  ...j....j....j..
-00011030: 0000 6a89 0400 006a 8304 0000 6a88 0c00  ..j....j....j...
-00011040: 006a 9e04 0000 6a69 0500 006a f604 0000  .j....ji...j....
-00011050: 6a56 0500 006a 5005 0000 6a26 0600 006a  jV...jP...j&...j
-00011060: 6f05 0000 6a95 0b00 006a 2c06 0000 6a38  o...j....j,...j8
-00011070: 0800 006a 1307 0000 6a06 0800 006a 0008  ...j....j....j..
-00011080: 0000 6a6c 0900 006a 3e08 0000 6ae3 0900  ..jl...j>...j...
-00011090: 006a 7209 0000 6a5a 0a00 006a e909 0000  .jr...jZ...j....
-000110a0: 6a9f 0a00 006a 600a 0000 6a8d 0b00 006a  j....j`...j....j
-000110b0: a50a 0000 6a80 0c00 006a 9b0b 0000 6a3f  ....j....j....j?
-000110c0: 0c00 006a ec0b 0000 6a78 0c00 006a 450c  ...j....jx...jE.
-000110d0: 0000 6a07 0d00 006a 8e0c 0000 6a98 0d00  ..j....j....j...
-000110e0: 006a 0d0d 0000 758c 0d66 6f6f 746e 6f74  .j....u..footnot
-000110f0: 655f 7265 6673 947d 948c 0d63 6974 6174  e_refs.}...citat
-00011100: 696f 6e5f 7265 6673 947d 948c 0d61 7574  ion_refs.}...aut
-00011110: 6f66 6f6f 746e 6f74 6573 945d 948c 1161  ofootnotes.]...a
-00011120: 7574 6f66 6f6f 746e 6f74 655f 7265 6673  utofootnote_refs
-00011130: 945d 948c 1073 796d 626f 6c5f 666f 6f74  .]...symbol_foot
-00011140: 6e6f 7465 7394 5d94 8c14 7379 6d62 6f6c  notes.]...symbol
-00011150: 5f66 6f6f 746e 6f74 655f 7265 6673 945d  _footnote_refs.]
-00011160: 948c 0966 6f6f 746e 6f74 6573 945d 948c  ...footnotes.]..
-00011170: 0963 6974 6174 696f 6e73 945d 948c 1261  .citations.]...a
-00011180: 7574 6f66 6f6f 746e 6f74 655f 7374 6172  utofootnote_star
-00011190: 7494 4b01 8c15 7379 6d62 6f6c 5f66 6f6f  t.K...symbol_foo
-000111a0: 746e 6f74 655f 7374 6172 7494 4b00 8c0a  tnote_start.K...
-000111b0: 6964 5f63 6f75 6e74 6572 946a f902 0000  id_counter.j....
-000111c0: 8c07 436f 756e 7465 7294 9394 7d94 8594  ..Counter...}...
-000111d0: 5294 8c0e 7061 7273 655f 6d65 7373 6167  R...parse_messag
-000111e0: 6573 945d 948c 1274 7261 6e73 666f 726d  es.]...transform
-000111f0: 5f6d 6573 7361 6765 7394 5d94 8c0b 7472  _messages.]...tr
-00011200: 616e 7366 6f72 6d65 7294 4e8c 0b69 6e63  ansformer.N..inc
-00011210: 6c75 6465 5f6c 6f67 945d 948c 0969 6e64  lude_log.]...ind
-00011220: 6578 2e72 7374 9428 4e4e 4e4e 7494 8694  ex.rst.(NNNNt...
-00011230: 618c 0a64 6563 6f72 6174 696f 6e94 4e6a  a..decoration.Nj
-00011240: 3303 0000 6a11 0300 0075 6273 8c08 6d65  3...j....ubs..me
-00011250: 7461 6461 7461 946a fb02 0000 6afc 0200  tadata.j....j...
-00011260: 008c 0464 6963 7494 9394 8594 5294 8c06  ...dict.....R...
-00011270: 7469 746c 6573 947d 946a cd02 0000 6a3c  titles.}.j....j<
-00011280: 0300 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
-00011290: 6a14 0300 005d 946a 1e03 0000 8c07 5765  j....].j......We
-000112a0: 6c63 6f6d 6594 8594 8194 7d94 6a23 0300  lcome.....}.j#..
-000112b0: 006a 1d0e 0000 7362 616a 2403 0000 7d94  .j....sbaj$...}.
-000112c0: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-000112d0: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-000112e0: 0000 5d94 756a 3203 0000 6a3b 0300 0075  ..].uj2...j;...u
-000112f0: 6273 8c0a 6c6f 6e67 7469 746c 6573 947d  bs..longtitles.}
-00011300: 946a cd02 0000 6a1d 0e00 0073 8c04 746f  .j....j....s..to
-00011310: 6373 947d 946a cd02 0000 6a16 0300 008c  cs.}.j....j.....
-00011320: 0b62 756c 6c65 745f 6c69 7374 9493 9429  .bullet_list...)
-00011330: 8194 7d94 286a 1303 0000 685e 6a14 0300  ..}.(j....h^j...
-00011340: 005d 946a 1603 0000 8c09 6c69 7374 5f69  .].j......list_i
-00011350: 7465 6d94 9394 2981 947d 9428 6a13 0300  tem...)..}.(j...
-00011360: 0068 5e6a 1403 0000 5d94 286a 0e03 0000  .h^j....].(j....
-00011370: 8c11 636f 6d70 6163 745f 7061 7261 6772  ..compact_paragr
-00011380: 6170 6894 9394 2981 947d 9428 6a13 0300  aph...)..}.(j...
-00011390: 0068 5e6a 1403 0000 5d94 6a9e 0300 0029  .h^j....].j....)
-000113a0: 8194 7d94 286a 1303 0000 685e 6a14 0300  ..}.(j....h^j...
-000113b0: 005d 946a 1e03 0000 8c07 5765 6c63 6f6d  .].j......Welcom
-000113c0: 6594 8594 8194 7d94 6a23 0300 006a 3d0e  e.....}.j#...j=.
-000113d0: 0000 7362 616a 2403 0000 7d94 286a 2603  ..sbaj$...}.(j&.
-000113e0: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
-000113f0: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
-00011400: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-00011410: 6675 7269 946a cd02 0000 8c0a 616e 6368  furi.j......anch
-00011420: 6f72 6e61 6d65 9468 5e75 6a32 0300 006a  orname.h^uj2...j
-00011430: 9d03 0000 6a23 0300 006a 3a0e 0000 7562  ....j#...j:...ub
-00011440: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
-00011450: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
-00011460: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
-00011470: 0000 6a38 0e00 006a 2303 0000 6a35 0e00  ..j8...j#...j5..
-00011480: 0075 626a 2f0e 0000 2981 947d 9428 6a13  .ubj/...)..}.(j.
-00011490: 0300 0068 5e6a 1403 0000 5d94 286a 340e  ...h^j....].(j4.
-000114a0: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
-000114b0: 1403 0000 5d94 6a39 0e00 0029 8194 7d94  ....].j9...)..}.
-000114c0: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
-000114d0: 9e03 0000 2981 947d 9428 6a13 0300 0068  ....)..}.(j....h
-000114e0: 5e6a 1403 0000 5d94 6a1e 0300 008c 0c49  ^j....].j......I
-000114f0: 6e74 726f 6475 6374 696f 6e94 8594 8194  ntroduction.....
-00011500: 7d94 6a23 0300 006a 5c0e 0000 7362 616a  }.j#...j\...sbaj
-00011510: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
-00011520: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
-00011530: 005d 946a 2e03 0000 5d94 8c08 696e 7465  .].j....]...inte
-00011540: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00011550: cd02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
-00011560: 948c 0d23 696e 7472 6f64 7563 7469 6f6e  ...#introduction
-00011570: 9475 6a32 0300 006a 9d03 0000 6a23 0300  .uj2...j....j#..
-00011580: 006a 590e 0000 7562 616a 2403 0000 7d94  .jY...ubaj$...}.
-00011590: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-000115a0: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-000115b0: 0000 5d94 756a 3203 0000 6a38 0e00 006a  ..].uj2...j8...j
-000115c0: 2303 0000 6a56 0e00 0075 6261 6a24 0300  #...jV...ubaj$..
-000115d0: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
-000115e0: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
-000115f0: 6a2e 0300 005d 9475 6a32 0300 006a 330e  j....].uj2...j3.
-00011600: 0000 6a23 0300 006a 530e 0000 7562 6a34  ..j#...jS...ubj4
-00011610: 0e00 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
-00011620: 6a14 0300 005d 946a 390e 0000 2981 947d  j....].j9...)..}
-00011630: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
-00011640: 6a9e 0300 0029 8194 7d94 286a 1303 0000  j....)..}.(j....
-00011650: 685e 6a14 0300 005d 946a 1e03 0000 8c0c  h^j....].j......
-00011660: 436f 6e74 7269 6275 7469 6f6e 9485 9481  Contribution....
-00011670: 947d 946a 2303 0000 6a7f 0e00 0073 6261  .}.j#...j....sba
-00011680: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
-00011690: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
-000116a0: 0000 5d94 6a2e 0300 005d 948c 0869 6e74  ..].j....]...int
-000116b0: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
-000116c0: 6acd 0200 008c 0a61 6e63 686f 726e 616d  j......anchornam
-000116d0: 6594 8c0d 2363 6f6e 7472 6962 7574 696f  e...#contributio
-000116e0: 6e94 756a 3203 0000 6a9d 0300 006a 2303  n.uj2...j....j#.
-000116f0: 0000 6a7c 0e00 0075 6261 6a24 0300 007d  ..j|...ubaj$...}
-00011700: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
-00011710: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
-00011720: 0300 005d 9475 6a32 0300 006a 380e 0000  ...].uj2...j8...
-00011730: 6a23 0300 006a 790e 0000 7562 616a 2403  j#...jy...ubaj$.
-00011740: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
-00011750: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
-00011760: 946a 2e03 0000 5d94 756a 3203 0000 6a33  .j....].uj2...j3
-00011770: 0e00 006a 2303 0000 6a53 0e00 0075 626a  ...j#...jS...ubj
-00011780: 340e 0000 2981 947d 9428 6a13 0300 0068  4...)..}.(j....h
-00011790: 5e6a 1403 0000 5d94 286a 390e 0000 2981  ^j....].(j9...).
-000117a0: 947d 9428 6a13 0300 0068 5e6a 1403 0000  .}.(j....h^j....
-000117b0: 5d94 6a9e 0300 0029 8194 7d94 286a 1303  ].j....)..}.(j..
-000117c0: 0000 685e 6a14 0300 005d 946a 1e03 0000  ..h^j....].j....
-000117d0: 8c0b 4765 7420 7374 6172 7465 6494 8594  ..Get started...
-000117e0: 8194 7d94 6a23 0300 006a a20e 0000 7362  ..}.j#...j....sb
-000117f0: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
-00011800: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
-00011810: 0300 005d 946a 2e03 0000 5d94 8c08 696e  ...].j....]...in
-00011820: 7465 726e 616c 9488 8c06 7265 6675 7269  ternal....refuri
-00011830: 946a cd02 0000 8c0a 616e 6368 6f72 6e61  .j......anchorna
-00011840: 6d65 948c 0c23 6765 742d 7374 6172 7465  me...#get-starte
-00011850: 6494 756a 3203 0000 6a9d 0300 006a 2303  d.uj2...j....j#.
-00011860: 0000 6a9f 0e00 0075 6261 6a24 0300 007d  ..j....ubaj$...}
-00011870: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
-00011880: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
-00011890: 0300 005d 9475 6a32 0300 006a 380e 0000  ...].uj2...j8...
-000118a0: 6a23 0300 006a 9c0e 0000 7562 6a2f 0e00  j#...j....ubj/..
-000118b0: 0029 8194 7d94 286a 1303 0000 685e 6a14  .)..}.(j....h^j.
-000118c0: 0300 005d 9428 6a34 0e00 0029 8194 7d94  ...].(j4...)..}.
-000118d0: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
-000118e0: 390e 0000 2981 947d 9428 6a13 0300 0068  9...)..}.(j....h
-000118f0: 5e6a 1403 0000 5d94 6a9e 0300 0029 8194  ^j....].j....)..
-00011900: 7d94 286a 1303 0000 685e 6a14 0300 005d  }.(j....h^j....]
-00011910: 946a 1e03 0000 8c0c 496e 7374 616c 6c61  .j......Installa
-00011920: 7469 6f6e 9485 9481 947d 946a 2303 0000  tion.....}.j#...
-00011930: 6ac2 0e00 0073 6261 6a24 0300 007d 9428  j....sbaj$...}.(
-00011940: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-00011950: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-00011960: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
-00011970: 0672 6566 7572 6994 6acd 0200 008c 0a61  .refuri.j......a
-00011980: 6e63 686f 726e 616d 6594 8c0d 2369 6e73  nchorname...#ins
-00011990: 7461 6c6c 6174 696f 6e94 756a 3203 0000  tallation.uj2...
-000119a0: 6a9d 0300 006a 2303 0000 6abf 0e00 0075  j....j#...j....u
-000119b0: 6261 6a24 0300 007d 9428 6a26 0300 005d  baj$...}.(j&...]
-000119c0: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
-000119d0: 2c03 0000 5d94 6a2e 0300 005d 9475 6a32  ,...].j....].uj2
-000119e0: 0300 006a 380e 0000 6a23 0300 006a bc0e  ...j8...j#...j..
-000119f0: 0000 7562 616a 2403 0000 7d94 286a 2603  ..ubaj$...}.(j&.
-00011a00: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
-00011a10: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
-00011a20: 756a 3203 0000 6a33 0e00 006a 2303 0000  uj2...j3...j#...
-00011a30: 6ab9 0e00 0075 626a 340e 0000 2981 947d  j....ubj4...)..}
-00011a40: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
-00011a50: 6a39 0e00 0029 8194 7d94 286a 1303 0000  j9...)..}.(j....
-00011a60: 685e 6a14 0300 005d 946a 9e03 0000 2981  h^j....].j....).
-00011a70: 947d 9428 6a13 0300 0068 5e6a 1403 0000  .}.(j....h^j....
-00011a80: 5d94 6a1e 0300 008c 0b50 7265 7065 7261  ].j......Prepera
-00011a90: 7469 6f6e 9485 9481 947d 946a 2303 0000  tion.....}.j#...
-00011aa0: 6ae5 0e00 0073 6261 6a24 0300 007d 9428  j....sbaj$...}.(
-00011ab0: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-00011ac0: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-00011ad0: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
-00011ae0: 0672 6566 7572 6994 6acd 0200 008c 0a61  .refuri.j......a
-00011af0: 6e63 686f 726e 616d 6594 8c0c 2370 7265  nchorname...#pre
-00011b00: 7065 7261 7469 6f6e 9475 6a32 0300 006a  peration.uj2...j
-00011b10: 9d03 0000 6a23 0300 006a e20e 0000 7562  ....j#...j....ub
-00011b20: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
-00011b30: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
-00011b40: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
-00011b50: 0000 6a38 0e00 006a 2303 0000 6adf 0e00  ..j8...j#...j...
-00011b60: 0075 6261 6a24 0300 007d 9428 6a26 0300  .ubaj$...}.(j&..
-00011b70: 005d 946a 2803 0000 5d94 6a2a 0300 005d  .].j(...].j*...]
-00011b80: 946a 2c03 0000 5d94 6a2e 0300 005d 9475  .j,...].j....].u
-00011b90: 6a32 0300 006a 330e 0000 6a23 0300 006a  j2...j3...j#...j
-00011ba0: b90e 0000 7562 6a34 0e00 0029 8194 7d94  ....ubj4...)..}.
-00011bb0: 286a 1303 0000 685e 6a14 0300 005d 9428  (j....h^j....].(
-00011bc0: 6a39 0e00 0029 8194 7d94 286a 1303 0000  j9...)..}.(j....
-00011bd0: 685e 6a14 0300 005d 946a 9e03 0000 2981  h^j....].j....).
-00011be0: 947d 9428 6a13 0300 0068 5e6a 1403 0000  .}.(j....h^j....
-00011bf0: 5d94 6a1e 0300 008c 0555 7361 6765 9485  ].j......Usage..
-00011c00: 9481 947d 946a 2303 0000 6a08 0f00 0073  ...}.j#...j....s
-00011c10: 6261 6a24 0300 007d 9428 6a26 0300 005d  baj$...}.(j&...]
-00011c20: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
-00011c30: 2c03 0000 5d94 6a2e 0300 005d 948c 0869  ,...].j....]...i
-00011c40: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
-00011c50: 6994 6acd 0200 008c 0a61 6e63 686f 726e  i.j......anchorn
-00011c60: 616d 6594 8c06 2375 7361 6765 9475 6a32  ame...#usage.uj2
-00011c70: 0300 006a 9d03 0000 6a23 0300 006a 050f  ...j....j#...j..
-00011c80: 0000 7562 616a 2403 0000 7d94 286a 2603  ..ubaj$...}.(j&.
-00011c90: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
-00011ca0: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
-00011cb0: 756a 3203 0000 6a38 0e00 006a 2303 0000  uj2...j8...j#...
-00011cc0: 6a02 0f00 0075 626a 2f0e 0000 2981 947d  j....ubj/...)..}
-00011cd0: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
-00011ce0: 286a 340e 0000 2981 947d 9428 6a13 0300  (j4...)..}.(j...
-00011cf0: 0068 5e6a 1403 0000 5d94 6a39 0e00 0029  .h^j....].j9...)
-00011d00: 8194 7d94 286a 1303 0000 685e 6a14 0300  ..}.(j....h^j...
-00011d10: 005d 946a 9e03 0000 2981 947d 9428 6a13  .].j....)..}.(j.
-00011d20: 0300 0068 5e6a 1403 0000 5d94 6a1e 0300  ...h^j....].j...
-00011d30: 008c 054d 6f64 656c 9485 9481 947d 946a  ...Model.....}.j
-00011d40: 2303 0000 6a28 0f00 0073 6261 6a24 0300  #...j(...sbaj$..
-00011d50: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
-00011d60: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
-00011d70: 6a2e 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
-00011d80: 6c94 888c 0672 6566 7572 6994 6acd 0200  l....refuri.j...
-00011d90: 008c 0a61 6e63 686f 726e 616d 6594 8c06  ...anchorname...
-00011da0: 236d 6f64 656c 9475 6a32 0300 006a 9d03  #model.uj2...j..
-00011db0: 0000 6a23 0300 006a 250f 0000 7562 616a  ..j#...j%...ubaj
-00011dc0: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
-00011dd0: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
-00011de0: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
-00011df0: 6a38 0e00 006a 2303 0000 6a22 0f00 0075  j8...j#...j"...u
-00011e00: 6261 6a24 0300 007d 9428 6a26 0300 005d  baj$...}.(j&...]
-00011e10: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
-00011e20: 2c03 0000 5d94 6a2e 0300 005d 9475 6a32  ,...].j....].uj2
-00011e30: 0300 006a 330e 0000 6a23 0300 006a 1f0f  ...j3...j#...j..
-00011e40: 0000 7562 6a34 0e00 0029 8194 7d94 286a  ..ubj4...)..}.(j
-00011e50: 1303 0000 685e 6a14 0300 005d 946a 390e  ....h^j....].j9.
-00011e60: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
-00011e70: 1403 0000 5d94 6a9e 0300 0029 8194 7d94  ....].j....)..}.
-00011e80: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
-00011e90: 1e03 0000 8c04 4261 7365 9485 9481 947d  ......Base.....}
-00011ea0: 946a 2303 0000 6a4b 0f00 0073 6261 6a24  .j#...jK...sbaj$
-00011eb0: 0300 007d 9428 6a26 0300 005d 946a 2803  ...}.(j&...].j(.
-00011ec0: 0000 5d94 6a2a 0300 005d 946a 2c03 0000  ..].j*...].j,...
-00011ed0: 5d94 6a2e 0300 005d 948c 0869 6e74 6572  ].j....]...inter
-00011ee0: 6e61 6c94 888c 0672 6566 7572 6994 6acd  nal....refuri.j.
-00011ef0: 0200 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
-00011f00: 8c05 2362 6173 6594 756a 3203 0000 6a9d  ..#base.uj2...j.
-00011f10: 0300 006a 2303 0000 6a48 0f00 0075 6261  ...j#...jH...uba
-00011f20: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
-00011f30: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
-00011f40: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
-00011f50: 006a 380e 0000 6a23 0300 006a 450f 0000  .j8...j#...jE...
-00011f60: 7562 616a 2403 0000 7d94 286a 2603 0000  ubaj$...}.(j&...
-00011f70: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
-00011f80: 6a2c 0300 005d 946a 2e03 0000 5d94 756a  j,...].j....].uj
-00011f90: 3203 0000 6a33 0e00 006a 2303 0000 6a1f  2...j3...j#...j.
-00011fa0: 0f00 0075 626a 340e 0000 2981 947d 9428  ...ubj4...)..}.(
-00011fb0: 6a13 0300 0068 5e6a 1403 0000 5d94 6a39  j....h^j....].j9
-00011fc0: 0e00 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
-00011fd0: 6a14 0300 005d 946a 9e03 0000 2981 947d  j....].j....)..}
-00011fe0: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
-00011ff0: 6a1e 0300 008c 0456 6965 7794 8594 8194  j......View.....
-00012000: 7d94 6a23 0300 006a 6e0f 0000 7362 616a  }.j#...jn...sbaj
-00012010: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
-00012020: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
-00012030: 005d 946a 2e03 0000 5d94 8c08 696e 7465  .].j....]...inte
-00012040: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
-00012050: cd02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
-00012060: 948c 0523 7669 6577 9475 6a32 0300 006a  ...#view.uj2...j
-00012070: 9d03 0000 6a23 0300 006a 6b0f 0000 7562  ....j#...jk...ub
-00012080: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
-00012090: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
-000120a0: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
-000120b0: 0000 6a38 0e00 006a 2303 0000 6a68 0f00  ..j8...j#...jh..
-000120c0: 0075 6261 6a24 0300 007d 9428 6a26 0300  .ubaj$...}.(j&..
-000120d0: 005d 946a 2803 0000 5d94 6a2a 0300 005d  .].j(...].j*...]
-000120e0: 946a 2c03 0000 5d94 6a2e 0300 005d 9475  .j,...].j....].u
-000120f0: 6a32 0300 006a 330e 0000 6a23 0300 006a  j2...j3...j#...j
-00012100: 1f0f 0000 7562 6a34 0e00 0029 8194 7d94  ....ubj4...)..}.
-00012110: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
-00012120: 390e 0000 2981 947d 9428 6a13 0300 0068  9...)..}.(j....h
-00012130: 5e6a 1403 0000 5d94 6a9e 0300 0029 8194  ^j....].j....)..
-00012140: 7d94 286a 1303 0000 685e 6a14 0300 005d  }.(j....h^j....]
-00012150: 946a 1e03 0000 8c06 4469 616c 6f67 9485  .j......Dialog..
-00012160: 9481 947d 946a 2303 0000 6a91 0f00 0073  ...}.j#...j....s
-00012170: 6261 6a24 0300 007d 9428 6a26 0300 005d  baj$...}.(j&...]
-00012180: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
-00012190: 2c03 0000 5d94 6a2e 0300 005d 948c 0869  ,...].j....]...i
-000121a0: 6e74 6572 6e61 6c94 888c 0672 6566 7572  nternal....refur
-000121b0: 6994 6acd 0200 008c 0a61 6e63 686f 726e  i.j......anchorn
-000121c0: 616d 6594 8c07 2364 6961 6c6f 6794 756a  ame...#dialog.uj
-000121d0: 3203 0000 6a9d 0300 006a 2303 0000 6a8e  2...j....j#...j.
-000121e0: 0f00 0075 6261 6a24 0300 007d 9428 6a26  ...ubaj$...}.(j&
-000121f0: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
-00012200: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-00012210: 9475 6a32 0300 006a 380e 0000 6a23 0300  .uj2...j8...j#..
-00012220: 006a 8b0f 0000 7562 616a 2403 0000 7d94  .j....ubaj$...}.
-00012230: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-00012240: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-00012250: 0000 5d94 756a 3203 0000 6a33 0e00 006a  ..].uj2...j3...j
-00012260: 2303 0000 6a1f 0f00 0075 626a 340e 0000  #...j....ubj4...
-00012270: 2981 947d 9428 6a13 0300 0068 5e6a 1403  )..}.(j....h^j..
-00012280: 0000 5d94 6a39 0e00 0029 8194 7d94 286a  ..].j9...)..}.(j
-00012290: 1303 0000 685e 6a14 0300 005d 946a 9e03  ....h^j....].j..
-000122a0: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
-000122b0: 1403 0000 5d94 6a1e 0300 008c 0657 6964  ....].j......Wid
-000122c0: 6765 7494 8594 8194 7d94 6a23 0300 006a  get.....}.j#...j
-000122d0: b40f 0000 7362 616a 2403 0000 7d94 286a  ....sbaj$...}.(j
-000122e0: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
-000122f0: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
-00012300: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
-00012310: 7265 6675 7269 946a cd02 0000 8c0a 616e  refuri.j......an
-00012320: 6368 6f72 6e61 6d65 948c 0723 7769 6467  chorname...#widg
-00012330: 6574 9475 6a32 0300 006a 9d03 0000 6a23  et.uj2...j....j#
-00012340: 0300 006a b10f 0000 7562 616a 2403 0000  ...j....ubaj$...
-00012350: 7d94 286a 2603 0000 5d94 6a28 0300 005d  }.(j&...].j(...]
-00012360: 946a 2a03 0000 5d94 6a2c 0300 005d 946a  .j*...].j,...].j
-00012370: 2e03 0000 5d94 756a 3203 0000 6a38 0e00  ....].uj2...j8..
-00012380: 006a 2303 0000 6aae 0f00 0075 6261 6a24  .j#...j....ubaj$
-00012390: 0300 007d 9428 6a26 0300 005d 946a 2803  ...}.(j&...].j(.
-000123a0: 0000 5d94 6a2a 0300 005d 946a 2c03 0000  ..].j*...].j,...
-000123b0: 5d94 6a2e 0300 005d 9475 6a32 0300 006a  ].j....].uj2...j
-000123c0: 330e 0000 6a23 0300 006a 1f0f 0000 7562  3...j#...j....ub
-000123d0: 6a34 0e00 0029 8194 7d94 286a 1303 0000  j4...)..}.(j....
-000123e0: 685e 6a14 0300 005d 946a 390e 0000 2981  h^j....].j9...).
-000123f0: 947d 9428 6a13 0300 0068 5e6a 1403 0000  .}.(j....h^j....
-00012400: 5d94 6a9e 0300 0029 8194 7d94 286a 1303  ].j....)..}.(j..
-00012410: 0000 685e 6a14 0300 005d 946a 1e03 0000  ..h^j....].j....
-00012420: 8c06 4163 7469 6f6e 9485 9481 947d 946a  ..Action.....}.j
-00012430: 2303 0000 6ad7 0f00 0073 6261 6a24 0300  #...j....sbaj$..
-00012440: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
-00012450: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
-00012460: 6a2e 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
-00012470: 6c94 888c 0672 6566 7572 6994 6acd 0200  l....refuri.j...
-00012480: 008c 0a61 6e63 686f 726e 616d 6594 8c07  ...anchorname...
-00012490: 2361 6374 696f 6e94 756a 3203 0000 6a9d  #action.uj2...j.
-000124a0: 0300 006a 2303 0000 6ad4 0f00 0075 6261  ...j#...j....uba
-000124b0: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
-000124c0: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
-000124d0: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
-000124e0: 006a 380e 0000 6a23 0300 006a d10f 0000  .j8...j#...j....
-000124f0: 7562 616a 2403 0000 7d94 286a 2603 0000  ubaj$...}.(j&...
-00012500: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
-00012510: 6a2c 0300 005d 946a 2e03 0000 5d94 756a  j,...].j....].uj
-00012520: 3203 0000 6a33 0e00 006a 2303 0000 6a1f  2...j3...j#...j.
-00012530: 0f00 0075 6265 6a24 0300 007d 9428 6a26  ...ubej$...}.(j&
-00012540: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
-00012550: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-00012560: 9475 6a32 0300 006a 2e0e 0000 6a23 0300  .uj2...j....j#..
-00012570: 006a 020f 0000 7562 656a 2403 0000 7d94  .j....ubej$...}.
-00012580: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-00012590: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-000125a0: 0000 5d94 756a 3203 0000 6a33 0e00 006a  ..].uj2...j3...j
-000125b0: 2303 0000 6ab9 0e00 0075 626a 340e 0000  #...j....ubj4...
-000125c0: 2981 947d 9428 6a13 0300 0068 5e6a 1403  )..}.(j....h^j..
-000125d0: 0000 5d94 286a 390e 0000 2981 947d 9428  ..].(j9...)..}.(
-000125e0: 6a13 0300 0068 5e6a 1403 0000 5d94 6a9e  j....h^j....].j.
-000125f0: 0300 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
-00012600: 6a14 0300 005d 946a 1e03 0000 8c1a 5275  j....].j......Ru
-00012610: 6e2c 2044 6576 656c 6f70 6d65 6e74 2061  n, Development a
-00012620: 6e64 2042 7569 6c64 9485 9481 947d 946a  nd Build.....}.j
-00012630: 2303 0000 6a06 1000 0073 6261 6a24 0300  #...j....sbaj$..
-00012640: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
-00012650: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
-00012660: 6a2e 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
-00012670: 6c94 888c 0672 6566 7572 6994 6acd 0200  l....refuri.j...
-00012680: 008c 0a61 6e63 686f 726e 616d 6594 8c1a  ...anchorname...
-00012690: 2372 756e 2d64 6576 656c 6f70 6d65 6e74  #run-development
-000126a0: 2d61 6e64 2d62 7569 6c64 9475 6a32 0300  -and-build.uj2..
-000126b0: 006a 9d03 0000 6a23 0300 006a 0310 0000  .j....j#...j....
-000126c0: 7562 616a 2403 0000 7d94 286a 2603 0000  ubaj$...}.(j&...
-000126d0: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
-000126e0: 6a2c 0300 005d 946a 2e03 0000 5d94 756a  j,...].j....].uj
-000126f0: 3203 0000 6a38 0e00 006a 2303 0000 6a00  2...j8...j#...j.
-00012700: 1000 0075 626a 2f0e 0000 2981 947d 9428  ...ubj/...)..}.(
-00012710: 6a13 0300 0068 5e6a 1403 0000 5d94 286a  j....h^j....].(j
-00012720: 340e 0000 2981 947d 9428 6a13 0300 0068  4...)..}.(j....h
-00012730: 5e6a 1403 0000 5d94 6a39 0e00 0029 8194  ^j....].j9...)..
-00012740: 7d94 286a 1303 0000 685e 6a14 0300 005d  }.(j....h^j....]
-00012750: 946a 9e03 0000 2981 947d 9428 6a13 0300  .j....)..}.(j...
-00012760: 0068 5e6a 1403 0000 5d94 6a1e 0300 008c  .h^j....].j.....
-00012770: 0b44 6576 656c 6f70 6d65 6e74 9485 9481  .Development....
-00012780: 947d 946a 2303 0000 6a26 1000 0073 6261  .}.j#...j&...sba
-00012790: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
-000127a0: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
-000127b0: 0000 5d94 6a2e 0300 005d 948c 0869 6e74  ..].j....]...int
-000127c0: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
-000127d0: 6acd 0200 008c 0a61 6e63 686f 726e 616d  j......anchornam
-000127e0: 6594 8c0c 2364 6576 656c 6f70 6d65 6e74  e...#development
-000127f0: 9475 6a32 0300 006a 9d03 0000 6a23 0300  .uj2...j....j#..
-00012800: 006a 2310 0000 7562 616a 2403 0000 7d94  .j#...ubaj$...}.
-00012810: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-00012820: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-00012830: 0000 5d94 756a 3203 0000 6a38 0e00 006a  ..].uj2...j8...j
-00012840: 2303 0000 6a20 1000 0075 6261 6a24 0300  #...j ...ubaj$..
-00012850: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
-00012860: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
-00012870: 6a2e 0300 005d 9475 6a32 0300 006a 330e  j....].uj2...j3.
-00012880: 0000 6a23 0300 006a 1d10 0000 7562 6a34  ..j#...j....ubj4
-00012890: 0e00 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
-000128a0: 6a14 0300 005d 946a 390e 0000 2981 947d  j....].j9...)..}
-000128b0: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
-000128c0: 6a9e 0300 0029 8194 7d94 286a 1303 0000  j....)..}.(j....
-000128d0: 685e 6a14 0300 005d 946a 1e03 0000 8c05  h^j....].j......
-000128e0: 4275 696c 6494 8594 8194 7d94 6a23 0300  Build.....}.j#..
-000128f0: 006a 4910 0000 7362 616a 2403 0000 7d94  .jI...sbaj$...}.
-00012900: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-00012910: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-00012920: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
-00012930: 8c06 7265 6675 7269 946a cd02 0000 8c0a  ..refuri.j......
-00012940: 616e 6368 6f72 6e61 6d65 948c 0623 6275  anchorname...#bu
-00012950: 696c 6494 756a 3203 0000 6a9d 0300 006a  ild.uj2...j....j
-00012960: 2303 0000 6a46 1000 0075 6261 6a24 0300  #...jF...ubaj$..
-00012970: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
-00012980: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
-00012990: 6a2e 0300 005d 9475 6a32 0300 006a 380e  j....].uj2...j8.
-000129a0: 0000 6a23 0300 006a 4310 0000 7562 616a  ..j#...jC...ubaj
-000129b0: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
-000129c0: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
-000129d0: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
-000129e0: 6a33 0e00 006a 2303 0000 6a1d 1000 0075  j3...j#...j....u
-000129f0: 6265 6a24 0300 007d 9428 6a26 0300 005d  bej$...}.(j&...]
-00012a00: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
-00012a10: 2c03 0000 5d94 6a2e 0300 005d 9475 6a32  ,...].j....].uj2
-00012a20: 0300 006a 2e0e 0000 6a23 0300 006a 0010  ...j....j#...j..
-00012a30: 0000 7562 656a 2403 0000 7d94 286a 2603  ..ubej$...}.(j&.
-00012a40: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
-00012a50: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
-00012a60: 756a 3203 0000 6a33 0e00 006a 2303 0000  uj2...j3...j#...
-00012a70: 6ab9 0e00 0075 6265 6a24 0300 007d 9428  j....ubej$...}.(
-00012a80: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-00012a90: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-00012aa0: 005d 9475 6a32 0300 006a 2e0e 0000 6a23  .].uj2...j....j#
-00012ab0: 0300 006a 9c0e 0000 7562 656a 2403 0000  ...j....ubej$...
-00012ac0: 7d94 286a 2603 0000 5d94 6a28 0300 005d  }.(j&...].j(...]
-00012ad0: 946a 2a03 0000 5d94 6a2c 0300 005d 946a  .j*...].j,...].j
-00012ae0: 2e03 0000 5d94 756a 3203 0000 6a33 0e00  ....].uj2...j3..
-00012af0: 006a 2303 0000 6a53 0e00 0075 626a 340e  .j#...jS...ubj4.
-00012b00: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
-00012b10: 1403 0000 5d94 6a39 0e00 0029 8194 7d94  ....].j9...)..}.
-00012b20: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
-00012b30: 9e03 0000 2981 947d 9428 6a13 0300 0068  ....)..}.(j....h
-00012b40: 5e6a 1403 0000 5d94 6a1e 0300 008c 1253  ^j....].j......S
-00012b50: 616d 706c 6520 6170 706c 6963 6174 696f  ample applicatio
-00012b60: 6e94 8594 8194 7d94 6a23 0300 006a 8410  n.....}.j#...j..
-00012b70: 0000 7362 616a 2403 0000 7d94 286a 2603  ..sbaj$...}.(j&.
-00012b80: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
-00012b90: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
-00012ba0: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
-00012bb0: 6675 7269 946a cd02 0000 8c0a 616e 6368  furi.j......anch
-00012bc0: 6f72 6e61 6d65 948c 1323 7361 6d70 6c65  orname...#sample
-00012bd0: 2d61 7070 6c69 6361 7469 6f6e 9475 6a32  -application.uj2
-00012be0: 0300 006a 9d03 0000 6a23 0300 006a 8110  ...j....j#...j..
-00012bf0: 0000 7562 616a 2403 0000 7d94 286a 2603  ..ubaj$...}.(j&.
-00012c00: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
-00012c10: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
-00012c20: 756a 3203 0000 6a38 0e00 006a 2303 0000  uj2...j8...j#...
-00012c30: 6a7e 1000 0075 6261 6a24 0300 007d 9428  j~...ubaj$...}.(
-00012c40: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
-00012c50: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
-00012c60: 005d 9475 6a32 0300 006a 330e 0000 6a23  .].uj2...j3...j#
-00012c70: 0300 006a 530e 0000 7562 6a34 0e00 0029  ...jS...ubj4...)
-00012c80: 8194 7d94 286a 1303 0000 685e 6a14 0300  ..}.(j....h^j...
-00012c90: 005d 9428 6a39 0e00 0029 8194 7d94 286a  .].(j9...)..}.(j
-00012ca0: 1303 0000 685e 6a14 0300 005d 946a 9e03  ....h^j....].j..
-00012cb0: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
-00012cc0: 1403 0000 5d94 6a1e 0300 008c 054e 6f74  ....].j......Not
-00012cd0: 6573 9485 9481 947d 946a 2303 0000 6aa7  es.....}.j#...j.
-00012ce0: 1000 0073 6261 6a24 0300 007d 9428 6a26  ...sbaj$...}.(j&
-00012cf0: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
-00012d00: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-00012d10: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
-00012d20: 6566 7572 6994 6acd 0200 008c 0a61 6e63  efuri.j......anc
-00012d30: 686f 726e 616d 6594 8c06 236e 6f74 6573  horname...#notes
-00012d40: 9475 6a32 0300 006a 9d03 0000 6a23 0300  .uj2...j....j#..
-00012d50: 006a a410 0000 7562 616a 2403 0000 7d94  .j....ubaj$...}.
-00012d60: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
-00012d70: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
-00012d80: 0000 5d94 756a 3203 0000 6a38 0e00 006a  ..].uj2...j8...j
-00012d90: 2303 0000 6aa1 1000 0075 626a 2f0e 0000  #...j....ubj/...
-00012da0: 2981 947d 9428 6a13 0300 0068 5e6a 1403  )..}.(j....h^j..
-00012db0: 0000 5d94 6a32 0d00 0029 8194 7d94 286a  ..].j2...)..}.(j
-00012dc0: 1303 0000 685e 6a14 0300 005d 946a 2403  ....h^j....].j$.
-00012dd0: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
-00012de0: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
-00012df0: 946a 2e03 0000 5d94 8c06 7061 7265 6e74  .j....]...parent
-00012e00: 946a cd02 0000 8c07 656e 7472 6965 7394  .j......entries.
-00012e10: 6a3d 0d00 008c 0c69 6e63 6c75 6465 6669  j=.....includefi
-00012e20: 6c65 7394 6a3f 0d00 008c 086d 6178 6465  les.j?.....maxde
-00012e30: 7074 6894 4b02 8c07 6361 7074 696f 6e94  pth.K...caption.
-00012e40: 4e8c 0467 6c6f 6294 898c 0668 6964 6465  N..glob....hidde
-00012e50: 6e94 888c 0d69 6e63 6c75 6465 6869 6464  n....includehidd
-00012e60: 656e 9489 8c08 6e75 6d62 6572 6564 944b  en....numbered.K
-00012e70: 008c 0a74 6974 6c65 736f 6e6c 7994 898c  ...titlesonly...
-00012e80: 0a72 6177 656e 7472 6965 7394 6a48 0d00  .rawentries.jH..
-00012e90: 0075 6a32 0300 006a 310d 0000 6a34 0300  .uj2...j1...j4..
-00012ea0: 006a 3503 0000 6a36 0300 004b 0b6a 2303  .j5...j6...K.j#.
-00012eb0: 0000 6abe 1000 0075 6261 6a24 0300 007d  ..j....ubaj$...}
-00012ec0: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
-00012ed0: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
-00012ee0: 0300 005d 9475 6a32 0300 006a 2e0e 0000  ...].uj2...j....
-00012ef0: 6a23 0300 006a a110 0000 7562 656a 2403  j#...j....ubej$.
-00012f00: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
-00012f10: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
-00012f20: 946a 2e03 0000 5d94 756a 3203 0000 6a33  .j....].uj2...j3
-00012f30: 0e00 006a 2303 0000 6a53 0e00 0075 6265  ...j#...jS...ube
-00012f40: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
-00012f50: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
-00012f60: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
-00012f70: 006a 2e0e 0000 6a23 0300 006a 350e 0000  .j....j#...j5...
-00012f80: 7562 656a 2403 0000 7d94 286a 2603 0000  ubej$...}.(j&...
-00012f90: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
-00012fa0: 6a2c 0300 005d 946a 2e03 0000 5d94 756a  j,...].j....].uj
-00012fb0: 3203 0000 6a33 0e00 006a 2303 0000 6a30  2...j3...j#...j0
-00012fc0: 0e00 0075 6261 6a24 0300 007d 9428 6a26  ...ubaj$...}.(j&
-00012fd0: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
-00012fe0: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
-00012ff0: 9475 6a32 0300 006a 2e0e 0000 7562 738c  .uj2...j....ubs.
-00013000: 0f74 6f63 5f6e 756d 5f65 6e74 7269 6573  .toc_num_entries
-00013010: 947d 946a cd02 0000 4b12 738c 0e74 6f63  .}.j....K.s..toc
-00013020: 5f73 6563 6e75 6d62 6572 7394 7d94 8c0e  _secnumbers.}...
-00013030: 746f 635f 6669 676e 756d 6265 7273 947d  toc_fignumbers.}
-00013040: 948c 1074 6f63 7472 6565 5f69 6e63 6c75  ...toctree_inclu
-00013050: 6465 7394 7d94 6acd 0200 005d 9473 8c10  des.}.j....].s..
-00013060: 6669 6c65 735f 746f 5f72 6562 7569 6c64  files_to_rebuild
-00013070: 947d 948c 0d67 6c6f 625f 746f 6374 7265  .}...glob_toctre
-00013080: 6573 948f 948c 116e 756d 6265 7265 645f  es.....numbered_
-00013090: 746f 6374 7265 6573 948f 948c 0a64 6f6d  toctrees.....dom
-000130a0: 6169 6e64 6174 6194 7d94 288c 0163 947d  aindata.}.(..c.}
-000130b0: 9428 8c0b 726f 6f74 5f73 796d 626f 6c94  .(..root_symbol.
-000130c0: 6acf 0200 008c 0653 796d 626f 6c94 9394  j......Symbol...
-000130d0: 2981 947d 9428 6a23 0300 004e 8c0c 7369  )..}.(j#...N..si
-000130e0: 626c 696e 6741 626f 7665 944e 8c0c 7369  blingAbove.N..si
-000130f0: 626c 696e 6742 656c 6f77 944e 8c05 6964  blingBelow.N..id
-00013100: 656e 7494 4e8c 0b64 6563 6c61 7261 7469  ent.N..declarati
-00013110: 6f6e 944e 8c07 646f 636e 616d 6594 4e6a  on.N..docname.Nj
-00013120: 3603 0000 4e8c 0f69 7352 6564 6563 6c61  6...N..isRedecla
-00013130: 7261 7469 6f6e 9489 8c09 5f63 6869 6c64  ration...._child
-00013140: 7265 6e94 5d94 8c0d 5f61 6e6f 6e43 6869  ren.]..._anonChi
-00013150: 6c64 7265 6e94 5d94 7562 8c07 6f62 6a65  ldren.].ub..obje
-00013160: 6374 7394 7d94 6862 4b00 758c 0963 6861  cts.}.hbK.u..cha
-00013170: 6e67 6573 6574 947d 9428 8c07 6368 616e  ngeset.}.(..chan
-00013180: 6765 7394 7d94 6862 4b00 758c 0863 6974  ges.}.hbK.u..cit
-00013190: 6174 696f 6e94 7d94 2868 624b 006a 010e  ation.}.(hbK.j..
-000131a0: 0000 7d94 6af5 0d00 007d 9475 8c03 6370  ..}.j....}.u..cp
-000131b0: 7094 7d94 286a 0611 0000 6ad2 0200 006a  p.}.(j....j....j
-000131c0: 0711 0000 9394 2981 947d 9428 6a23 0300  ......)..}.(j#..
-000131d0: 004e 6a0b 1100 004e 6a0c 1100 004e 8c09  .Nj....Nj....N..
-000131e0: 6964 656e 744f 724f 7094 4e8c 0e74 656d  identOrOp.N..tem
-000131f0: 706c 6174 6550 6172 616d 7394 4e8c 0c74  plateParams.N..t
-00013200: 656d 706c 6174 6541 7267 7394 4e6a 0e11  emplateArgs.Nj..
-00013210: 0000 4e6a 0f11 0000 4e6a 3603 0000 4e6a  ..Nj....Nj6...Nj
-00013220: 1011 0000 896a 1111 0000 5d94 6a13 1100  .....j....].j...
-00013230: 005d 9475 626a 2a03 0000 7d94 6862 4b00  .].ubj*...}.hbK.
-00013240: 7568 777d 9428 6862 4b00 6a3c 0d00 007d  uhw}.(hbK.j<...}
-00013250: 946a cd02 0000 5d94 7375 8c02 6a73 947d  .j....].su..js.}
-00013260: 9428 6a15 1100 007d 948c 076d 6f64 756c  .(j....}...modul
-00013270: 6573 947d 9468 624b 0075 8c04 6d61 7468  es.}.hbK.u..math
-00013280: 947d 9428 6a15 1100 007d 948c 0d68 6173  .}.(j....}...has
-00013290: 5f65 7175 6174 696f 6e73 947d 946a cd02  _equations.}.j..
-000132a0: 0000 8973 6862 4b00 7568 b17d 9428 6a15  ...shbK.uh.}.(j.
-000132b0: 1100 007d 946a 3011 0000 7d94 6862 4b00  ...}.j0...}.hbK.
-000132c0: 758c 0372 7374 947d 9428 6a15 1100 007d  u..rst.}.(j....}
-000132d0: 9468 624b 0075 8c03 7374 6494 7d94 288c  .hbK.u..std.}.(.
-000132e0: 0b70 726f 676f 7074 696f 6e73 947d 946a  .progoptions.}.j
-000132f0: 1511 0000 7d94 8c06 6c61 6265 6c73 947d  ....}...labels.}
-00013300: 9428 8c08 6765 6e69 6e64 6578 946a 4411  .(..genindex.jD.
-00013310: 0000 685e 8c0d 7370 6869 6e78 2e6c 6f63  ..h^..sphinx.loc
-00013320: 616c 6594 8c11 5f54 7261 6e73 6c61 7469  ale..._Translati
-00013330: 6f6e 5072 6f78 7994 9394 2981 946a d902  onProxy...)..j..
-00013340: 0000 8c07 6765 6e65 7261 6c94 8c05 496e  ....general...In
-00013350: 6465 7894 8794 6287 948c 086d 6f64 696e  dex...b....modin
-00013360: 6465 7894 8c0b 7079 2d6d 6f64 696e 6465  dex...py-modinde
-00013370: 7894 685e 6a47 1100 0029 8194 6ad9 0200  x.h^jG...)..j...
-00013380: 006a 4911 0000 8c0c 4d6f 6475 6c65 2049  .jI.....Module I
-00013390: 6e64 6578 9487 9462 8794 8c06 7365 6172  ndex...b....sear
-000133a0: 6368 946a 5311 0000 685e 6a47 1100 0029  ch.jS...h^jG...)
-000133b0: 8194 6ad9 0200 006a 4911 0000 8c0b 5365  ..j....jI.....Se
-000133c0: 6172 6368 2050 6167 6594 8794 6287 948c  arch Page...b...
-000133d0: 0b70 792d 6d6f 6469 6e64 6578 946a 5811  .py-modindex.jX.
-000133e0: 0000 685e 8c13 5079 7468 6f6e 204d 6f64  ..h^..Python Mod
-000133f0: 756c 6520 496e 6465 7894 8794 758c 0a61  ule Index...u..a
-00013400: 6e6f 6e6c 6162 656c 7394 7d94 286a 4411  nonlabels.}.(jD.
-00013410: 0000 6a44 1100 0068 5e86 946a 4d11 0000  ..jD...h^..jM...
-00013420: 6a4e 1100 0068 5e86 946a 5311 0000 6a53  jN...h^..jS...jS
-00013430: 1100 0068 5e86 946a 5811 0000 6a58 1100  ...h^..jX...jX..
-00013440: 0068 5e86 9475 6862 4b00 8c05 7465 726d  .h^..uhbK...term
-00013450: 7394 7d94 7575 8c06 696d 6167 6573 948c  s.}.uu..images..
-00013460: 0b73 7068 696e 782e 7574 696c 948c 1046  .sphinx.util...F
-00013470: 696c 656e 616d 6555 6e69 7144 6963 7494  ilenameUniqDict.
-00013480: 9394 2981 948f 9462 8c07 646c 6669 6c65  ..)....b..dlfile
-00013490: 7394 6a64 1100 008c 0d44 6f77 6e6c 6f61  s.jd.....Downloa
-000134a0: 6446 696c 6573 9493 9429 8194 8c12 6f72  dFiles...)....or
-000134b0: 6967 696e 616c 5f69 6d61 6765 5f75 7269  iginal_image_uri
-000134c0: 947d 948c 0974 656d 705f 6461 7461 947d  .}...temp_data.}
-000134d0: 948c 0b72 6566 5f63 6f6e 7465 7874 947d  ...ref_context.}
-000134e0: 948c 145f 7365 6172 6368 5f69 6e64 6578  ..._search_index
-000134f0: 5f74 6974 6c65 7394 7d94 8c17 5f73 6561  _titles.}..._sea
-00013500: 7263 685f 696e 6465 785f 6669 6c65 6e61  rch_index_filena
-00013510: 6d65 7394 7d94 8c15 5f73 6561 7263 685f  mes.}..._search_
-00013520: 696e 6465 785f 6d61 7070 696e 6794 7d94  index_mapping.}.
-00013530: 8c1b 5f73 6561 7263 685f 696e 6465 785f  .._search_index_
-00013540: 7469 746c 655f 6d61 7070 696e 6794 7d94  title_mapping.}.
-00013550: 8c18 5f73 6561 7263 685f 696e 6465 785f  .._search_index_
-00013560: 616c 6c5f 7469 746c 6573 947d 948c 1b5f  all_titles.}..._
-00013570: 7365 6172 6368 5f69 6e64 6578 5f69 6e64  search_index_ind
-00013580: 6578 5f65 6e74 7269 6573 947d 948c 165f  ex_entries.}..._
-00013590: 7365 6172 6368 5f69 6e64 6578 5f6f 626a  search_index_obj
-000135a0: 7479 7065 7394 7d94 8c16 5f73 6561 7263  types.}..._searc
-000135b0: 685f 696e 6465 785f 6f62 6a6e 616d 6573  h_index_objnames
-000135c0: 947d 9475 622e                           .}.ub.
+0000d6f0: 6f64 656c 2864 6174 615b 2769 7465 6d27  odel(data['item'
+0000d700: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000d710: 2020 6974 656d 2e74 6974 6c65 203d 2069    item.title = i
+0000d720: 7465 6d2e 6669 7273 746e 616d 6520 2b20  tem.firstname + 
+0000d730: 2720 2720 2b20 6974 656d 2e6c 6173 746e  ' ' + item.lastn
+0000d740: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+0000d750: 2020 2069 6620 6974 656d 2e73 6176 6528     if item.save(
+0000d760: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000d770: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0000d780: 2c20 6974 656d 2e74 6974 6c65 202b 2027  , item.title + '
+0000d790: 2073 6176 6564 2073 7563 6365 7373 6675   saved successfu
+0000d7a0: 6c6c 7927 0a20 2020 2020 2020 2020 2020  lly'.           
+0000d7b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000d7c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000d7d0: 726e 2046 616c 7365 2c20 2745 7272 6f72  rn False, 'Error
+0000d7e0: 2077 6869 6c65 2073 6176 696e 6720 2720   while saving ' 
+0000d7f0: 2b20 6974 656d 2e74 6974 6c65 946a 1403  + item.title.j..
+0000d800: 0000 5d94 6a1e 0300 0058 1304 0000 6672  ..].j....X....fr
+0000d810: 6f6d 2064 6563 6f72 655f 6261 7365 2069  om decore_base i
+0000d820: 6d70 6f72 7420 6465 636f 7265 0a66 726f  mport decore.fro
+0000d830: 6d20 6d6f 6465 6c73 2e66 6972 7374 5f6d  m models.first_m
+0000d840: 6f64 656c 2069 6d70 6f72 7420 4669 7273  odel import Firs
+0000d850: 745f 6d6f 6465 6c0a 0a40 6465 636f 7265  t_model..@decore
+0000d860: 2e62 6173 6528 7469 746c 653d 274d 7920  .base(title='My 
+0000d870: 4669 7273 7420 4261 7365 272c 2069 636f  First Base', ico
+0000d880: 6e3d 276d 6469 2d68 6f6d 6527 2c20 6d6f  n='mdi-home', mo
+0000d890: 6465 6c3d 4669 7273 745f 6d6f 6465 6c29  del=First_model)
+0000d8a0: 0a63 6c61 7373 2046 6972 7374 5f62 6173  .class First_bas
+0000d8b0: 653a 0a20 2020 4064 6563 6f72 652e 7669  e:.   @decore.vi
+0000d8c0: 6577 2874 6974 6c65 3d27 5065 7273 6f6e  ew(title='Person
+0000d8d0: 272c 2069 636f 6e3d 276d 6469 2d61 6363  ', icon='mdi-acc
+0000d8e0: 6f75 6e74 272c 2074 7970 653d 2774 6162  ount', type='tab
+0000d8f0: 6c65 272c 2066 6965 6c64 733d 5b46 6972  le', fields=[Fir
+0000d900: 7374 5f6d 6f64 656c 2e66 6972 7374 6e61  st_model.firstna
+0000d910: 6d65 2c20 4669 7273 745f 6d6f 6465 6c2e  me, First_model.
+0000d920: 6c61 7374 6e61 6d65 5d29 0a20 2020 6465  lastname]).   de
+0000d930: 6620 6669 7273 745f 7669 6577 2829 3a0a  f first_view():.
+0000d940: 2020 2020 2020 4064 6563 6f72 652e 6469        @decore.di
+0000d950: 616c 6f67 2874 6974 6c65 3d27 4164 6420  alog(title='Add 
+0000d960: 5065 7273 6f6e 272c 2069 636f 6e3d 276d  Person', icon='m
+0000d970: 6469 2d70 6c75 7327 2c20 7479 7065 3d27  di-plus', type='
+0000d980: 7374 616e 6461 7264 272c 2064 6973 706c  standard', displ
+0000d990: 6179 3d27 6472 6177 6572 272c 2061 6374  ay='drawer', act
+0000d9a0: 6976 6174 6f72 3d27 6465 6661 756c 742d  ivator='default-
+0000d9b0: 6d65 6e75 2729 0a20 2020 2020 2064 6566  menu').      def
+0000d9c0: 2066 6972 7374 5f64 6961 6c6f 6728 293a   first_dialog():
+0000d9d0: 0a20 2020 2020 2020 2020 4064 6563 6f72  .         @decor
+0000d9e0: 652e 7769 6467 6574 2874 6974 6c65 3d27  e.widget(title='
+0000d9f0: 4164 6420 5065 7273 6f6e 2046 6f72 6d27  Add Person Form'
+0000da00: 2c20 6963 6f6e 3d27 6d64 692d 6163 636f  , icon='mdi-acco
+0000da10: 756e 7427 2c20 7479 7065 3d27 666f 726d  unt', type='form
+0000da20: 272c 2066 6965 6c64 733d 5b46 6972 7374  ', fields=[First
+0000da30: 5f6d 6f64 656c 2e66 6972 7374 6e61 6d65  _model.firstname
+0000da40: 2c20 4669 7273 745f 6d6f 6465 6c2e 6c61  , First_model.la
+0000da50: 7374 6e61 6d65 5d29 0a20 2020 2020 2020  stname]).       
+0000da60: 2020 6465 6620 6669 7273 745f 7769 6467    def first_widg
+0000da70: 6574 2829 3a0a 2020 2020 2020 2020 2020  et():.          
+0000da80: 2020 4064 6563 6f72 652e 6163 7469 6f6e    @decore.action
+0000da90: 2874 6974 6c65 3d27 5361 7665 2050 6572  (title='Save Per
+0000daa0: 736f 6e27 2c20 6963 6f6e 3d27 6d64 692d  son', icon='mdi-
+0000dab0: 636f 6e74 656e 742d 7361 7665 272c 2074  content-save', t
+0000dac0: 7970 653d 2773 7562 6d69 7427 290a 2020  ype='submit').  
+0000dad0: 2020 2020 2020 2020 2020 6465 6620 6669            def fi
+0000dae0: 7273 745f 6163 7469 6f6e 2873 656c 662c  rst_action(self,
+0000daf0: 2064 6174 6129 3a0a 2020 2020 2020 2020   data):.        
+0000db00: 2020 2020 2020 2069 7465 6d20 3d20 4669         item = Fi
+0000db10: 7273 745f 6d6f 6465 6c28 6461 7461 5b27  rst_model(data['
+0000db20: 6974 656d 275d 290a 2020 2020 2020 2020  item']).        
+0000db30: 2020 2020 2020 2069 7465 6d2e 7469 746c         item.titl
+0000db40: 6520 3d20 6974 656d 2e66 6972 7374 6e61  e = item.firstna
+0000db50: 6d65 202b 2027 2027 202b 2069 7465 6d2e  me + ' ' + item.
+0000db60: 6c61 7374 6e61 6d65 0a20 2020 2020 2020  lastname.       
+0000db70: 2020 2020 2020 2020 6966 2069 7465 6d2e          if item.
+0000db80: 7361 7665 2829 3a0a 2020 2020 2020 2020  save():.        
+0000db90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000dba0: 2054 7275 652c 2069 7465 6d2e 7469 746c   True, item.titl
+0000dbb0: 6520 2b20 2720 7361 7665 6420 7375 6363  e + ' saved succ
+0000dbc0: 6573 7366 756c 6c79 270a 2020 2020 2020  essfully'.      
+0000dbd0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbf0: 2072 6574 7572 6e20 4661 6c73 652c 2027   return False, '
+0000dc00: 4572 726f 7220 7768 696c 6520 7361 7669  Error while savi
+0000dc10: 6e67 2027 202b 2069 7465 6d2e 7469 746c  ng ' + item.titl
+0000dc20: 6594 8594 8194 7d94 6a23 0300 006a 080b  e.....}.j#...j..
+0000dc30: 0000 7362 616a 2403 0000 7d94 286a 2603  ..sbaj$...}.(j&.
+0000dc40: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
+0000dc50: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
+0000dc60: 6a30 0300 006a 3103 0000 6a33 0500 0089  j0...j1...j3....
+0000dc70: 6869 8c06 7079 7468 6f6e 946a 3505 0000  hi..python.j5...
+0000dc80: 7d94 756a 3203 0000 6a23 0500 006a 3403  }.uj2...j#...j4.
+0000dc90: 0000 6a5c 0300 006a 3603 0000 4bcc 6a23  ..j\...j6...K.j#
+0000dca0: 0300 006a a50a 0000 6a33 0300 006a 1103  ...j....j3...j..
+0000dcb0: 0000 7562 6a53 0700 0029 8194 7d94 286a  ..ubjS...)..}.(j
+0000dcc0: 1303 0000 5817 0100 0054 6f20 6372 6561  ....X....To crea
+0000dcd0: 7465 2061 2072 6563 6f72 6420 7769 7468  te a record with
+0000dce0: 2064 6563 6f72 6520 4261 7365 2c20 7765   decore Base, we
+0000dcf0: 206e 6565 6420 746f 2063 7265 6174 6520   need to create 
+0000dd00: 616e 2069 6e73 7461 6e63 6520 6f66 2074  an instance of t
+0000dd10: 6865 206d 6f64 656c 2e20 496e 206f 7572  he model. In our
+0000dd20: 2063 6173 6520 2a2a 4669 7273 745f 6d6f   case **First_mo
+0000dd30: 6465 6c2a 2a2e 2054 6865 2069 6e73 7461  del**. The insta
+0000dd40: 6e63 6520 6973 2066 696c 6c65 6420 7769  nce is filled wi
+0000dd50: 7468 2074 6865 2064 6174 6120 6672 6f6d  th the data from
+0000dd60: 2074 6865 2066 6f72 6d20 616e 6420 7468   the form and th
+0000dd70: 656e 2073 6176 6564 2e0a 0a54 6865 2049  en saved...The I
+0000dd80: 4420 696e 2074 6865 2066 6f72 6d20 6f66  D in the form of
+0000dd90: 2061 2055 5549 4420 6973 2067 656e 6572   a UUID is gener
+0000dda0: 6174 6564 2061 7574 6f6d 6174 6963 616c  ated automatical
+0000ddb0: 6c79 2061 6e64 2064 6f65 7320 6e6f 7420  ly and does not 
+0000ddc0: 6861 7665 2074 6f20 6265 2073 7065 6369  have to be speci
+0000ddd0: 6669 6564 2073 6570 6172 6174 656c 792e  fied separately.
+0000dde0: 946a 1403 0000 5d94 286a 5e03 0000 2981  .j....].(j^...).
+0000ddf0: 947d 9428 6a13 0300 008c b054 6f20 6372  .}.(j......To cr
+0000de00: 6561 7465 2061 2072 6563 6f72 6420 7769  eate a record wi
+0000de10: 7468 2064 6563 6f72 6520 4261 7365 2c20  th decore Base, 
+0000de20: 7765 206e 6565 6420 746f 2063 7265 6174  we need to creat
+0000de30: 6520 616e 2069 6e73 7461 6e63 6520 6f66  e an instance of
+0000de40: 2074 6865 206d 6f64 656c 2e20 496e 206f   the model. In o
+0000de50: 7572 2063 6173 6520 2a2a 4669 7273 745f  ur case **First_
+0000de60: 6d6f 6465 6c2a 2a2e 2054 6865 2069 6e73  model**. The ins
+0000de70: 7461 6e63 6520 6973 2066 696c 6c65 6420  tance is filled 
+0000de80: 7769 7468 2074 6865 2064 6174 6120 6672  with the data fr
+0000de90: 6f6d 2074 6865 2066 6f72 6d20 616e 6420  om the form and 
+0000dea0: 7468 656e 2073 6176 6564 2e94 6a14 0300  then saved..j...
+0000deb0: 005d 9428 6a1e 0300 008c 5d54 6f20 6372  .].(j.....]To cr
+0000dec0: 6561 7465 2061 2072 6563 6f72 6420 7769  eate a record wi
+0000ded0: 7468 2064 6563 6f72 6520 4261 7365 2c20  th decore Base, 
+0000dee0: 7765 206e 6565 6420 746f 2063 7265 6174  we need to creat
+0000def0: 6520 616e 2069 6e73 7461 6e63 6520 6f66  e an instance of
+0000df00: 2074 6865 206d 6f64 656c 2e20 496e 206f   the model. In o
+0000df10: 7572 2063 6173 6520 9485 9481 947d 9428  ur case .....}.(
+0000df20: 6a23 0300 006a 1c0b 0000 6a33 0300 006a  j#...j....j3...j
+0000df30: 1103 0000 6a34 0300 004e 6a36 0300 004e  ....j4...Nj6...N
+0000df40: 7562 6a72 0300 0029 8194 7d94 286a 1303  ubjr...)..}.(j..
+0000df50: 0000 8c0f 2a2a 4669 7273 745f 6d6f 6465  ....**First_mode
+0000df60: 6c2a 2a94 6a14 0300 005d 946a 1e03 0000  l**.j....].j....
+0000df70: 8c0b 4669 7273 745f 6d6f 6465 6c94 8594  ..First_model...
+0000df80: 8194 7d94 286a 2303 0000 6a24 0b00 006a  ..}.(j#...j$...j
+0000df90: 3303 0000 6a11 0300 006a 3403 0000 4e6a  3...j....j4...Nj
+0000dfa0: 3603 0000 4e75 6261 6a24 0300 007d 9428  6...Nubaj$...}.(
+0000dfb0: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
+0000dfc0: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
+0000dfd0: 005d 9475 6a32 0300 006a 7103 0000 6a23  .].uj2...jq...j#
+0000dfe0: 0300 006a 1c0b 0000 7562 6a1e 0300 008c  ...j....ubj.....
+0000dff0: 442e 2054 6865 2069 6e73 7461 6e63 6520  D. The instance 
+0000e000: 6973 2066 696c 6c65 6420 7769 7468 2074  is filled with t
+0000e010: 6865 2064 6174 6120 6672 6f6d 2074 6865  he data from the
+0000e020: 2066 6f72 6d20 616e 6420 7468 656e 2073   form and then s
+0000e030: 6176 6564 2e94 8594 8194 7d94 286a 2303  aved......}.(j#.
+0000e040: 0000 6a1c 0b00 006a 3303 0000 6a11 0300  ..j....j3...j...
+0000e050: 006a 3403 0000 4e6a 3603 0000 4e75 6265  .j4...Nj6...Nube
+0000e060: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+0000e070: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+0000e080: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+0000e090: 006a 5d03 0000 6a34 0300 006a 5c03 0000  .j]...j4...j\...
+0000e0a0: 6a36 0300 004b e36a 2303 0000 6a18 0b00  j6...K.j#...j...
+0000e0b0: 0075 626a 5e03 0000 2981 947d 9428 6a13  .ubj^...)..}.(j.
+0000e0c0: 0300 008c 6554 6865 2049 4420 696e 2074  ....eThe ID in t
+0000e0d0: 6865 2066 6f72 6d20 6f66 2061 2055 5549  he form of a UUI
+0000e0e0: 4420 6973 2067 656e 6572 6174 6564 2061  D is generated a
+0000e0f0: 7574 6f6d 6174 6963 616c 6c79 2061 6e64  utomatically and
+0000e100: 2064 6f65 7320 6e6f 7420 6861 7665 2074   does not have t
+0000e110: 6f20 6265 2073 7065 6369 6669 6564 2073  o be specified s
+0000e120: 6570 6172 6174 656c 792e 946a 1403 0000  eparately..j....
+0000e130: 5d94 6a1e 0300 008c 6554 6865 2049 4420  ].j.....eThe ID 
+0000e140: 696e 2074 6865 2066 6f72 6d20 6f66 2061  in the form of a
+0000e150: 2055 5549 4420 6973 2067 656e 6572 6174   UUID is generat
+0000e160: 6564 2061 7574 6f6d 6174 6963 616c 6c79  ed automatically
+0000e170: 2061 6e64 2064 6f65 7320 6e6f 7420 6861   and does not ha
+0000e180: 7665 2074 6f20 6265 2073 7065 6369 6669  ve to be specifi
+0000e190: 6564 2073 6570 6172 6174 656c 792e 9485  ed separately...
+0000e1a0: 9481 947d 9428 6a23 0300 006a 3c0b 0000  ...}.(j#...j<...
+0000e1b0: 6a33 0300 006a 1103 0000 6a34 0300 004e  j3...j....j4...N
+0000e1c0: 6a36 0300 004e 7562 616a 2403 0000 7d94  j6...Nubaj$...}.
+0000e1d0: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
+0000e1e0: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
+0000e1f0: 0000 5d94 756a 3203 0000 6a5d 0300 006a  ..].uj2...j]...j
+0000e200: 3403 0000 6a5c 0300 006a 3603 0000 4be5  4...j\...j6...K.
+0000e210: 6a23 0300 006a 180b 0000 7562 656a 2403  j#...j....ubej$.
+0000e220: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
+0000e230: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
+0000e240: 946a 2e03 0000 5d94 756a 3203 0000 6a52  .j....].uj2...jR
+0000e250: 0700 006a 2303 0000 6aa5 0a00 006a 3303  ...j#...j....j3.
+0000e260: 0000 6a11 0300 006a 3403 0000 6a5c 0300  ..j....j4...j\..
+0000e270: 006a 3603 0000 4e75 626a 1e08 0000 2981  .j6...Nubj....).
+0000e280: 947d 9428 6a13 0300 008c 9954 6865 2066  .}.(j......The f
+0000e290: 6965 6c64 202a 2a74 6974 6c65 2a2a 2077  ield **title** w
+0000e2a0: 6173 2069 6e68 6572 6974 6564 2066 726f  as inherited fro
+0000e2b0: 6d20 7468 6520 636c 6173 7320 2a2a 4465  m the class **De
+0000e2c0: 666f 726d 5f6d 6f64 656c 2a2a 2061 6e64  form_model** and
+0000e2d0: 206d 7573 7420 6265 2075 7365 6420 666f   must be used fo
+0000e2e0: 7220 6561 6368 2072 6563 6f72 6420 6372  r each record cr
+0000e2f0: 6561 7469 6f6e 2e20 4f74 6865 7277 6973  eation. Otherwis
+0000e300: 6520 7468 6520 6974 656d 2077 696c 6c20  e the item will 
+0000e310: 6661 696c 2074 6865 2076 616c 6964 6174  fail the validat
+0000e320: 696f 6e2e 946a 1403 0000 5d94 6a5e 0300  ion..j....].j^..
+0000e330: 0029 8194 7d94 286a 1303 0000 6a52 0b00  .)..}.(j....jR..
+0000e340: 006a 1403 0000 5d94 286a 1e03 0000 8c0a  .j....].(j......
+0000e350: 5468 6520 6669 656c 6420 9485 9481 947d  The field .....}
+0000e360: 9428 6a23 0300 006a 540b 0000 6a33 0300  .(j#...jT...j3..
+0000e370: 006a 1103 0000 6a34 0300 004e 6a36 0300  .j....j4...Nj6..
+0000e380: 004e 7562 6a72 0300 0029 8194 7d94 286a  .Nubjr...)..}.(j
+0000e390: 1303 0000 8c09 2a2a 7469 746c 652a 2a94  ......**title**.
+0000e3a0: 6a14 0300 005d 946a 1e03 0000 8c05 7469  j....].j......ti
+0000e3b0: 746c 6594 8594 8194 7d94 286a 2303 0000  tle.....}.(j#...
+0000e3c0: 6a5b 0b00 006a 3303 0000 6a11 0300 006a  j[...j3...j....j
+0000e3d0: 3403 0000 4e6a 3603 0000 4e75 6261 6a24  4...Nj6...Nubaj$
+0000e3e0: 0300 007d 9428 6a26 0300 005d 946a 2803  ...}.(j&...].j(.
+0000e3f0: 0000 5d94 6a2a 0300 005d 946a 2c03 0000  ..].j*...].j,...
+0000e400: 5d94 6a2e 0300 005d 9475 6a32 0300 006a  ].j....].uj2...j
+0000e410: 7103 0000 6a23 0300 006a 540b 0000 7562  q...j#...jT...ub
+0000e420: 6a1e 0300 008c 1e20 7761 7320 696e 6865  j...... was inhe
+0000e430: 7269 7465 6420 6672 6f6d 2074 6865 2063  rited from the c
+0000e440: 6c61 7373 2094 8594 8194 7d94 286a 2303  lass .....}.(j#.
+0000e450: 0000 6a54 0b00 006a 3303 0000 6a11 0300  ..jT...j3...j...
+0000e460: 006a 3403 0000 4e6a 3603 0000 4e75 626a  .j4...Nj6...Nubj
+0000e470: 7203 0000 2981 947d 9428 6a13 0300 008c  r...)..}.(j.....
+0000e480: 102a 2a44 6566 6f72 6d5f 6d6f 6465 6c2a  .**Deform_model*
+0000e490: 2a94 6a14 0300 005d 946a 1e03 0000 8c0c  *.j....].j......
+0000e4a0: 4465 666f 726d 5f6d 6f64 656c 9485 9481  Deform_model....
+0000e4b0: 947d 9428 6a23 0300 006a 6d0b 0000 6a33  .}.(j#...jm...j3
+0000e4c0: 0300 006a 1103 0000 6a34 0300 004e 6a36  ...j....j4...Nj6
+0000e4d0: 0300 004e 7562 616a 2403 0000 7d94 286a  ...Nubaj$...}.(j
+0000e4e0: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
+0000e4f0: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
+0000e500: 5d94 756a 3203 0000 6a71 0300 006a 2303  ].uj2...jq...j#.
+0000e510: 0000 6a54 0b00 0075 626a 1e03 0000 8c58  ..jT...ubj.....X
+0000e520: 2061 6e64 206d 7573 7420 6265 2075 7365   and must be use
+0000e530: 6420 666f 7220 6561 6368 2072 6563 6f72  d for each recor
+0000e540: 6420 6372 6561 7469 6f6e 2e20 4f74 6865  d creation. Othe
+0000e550: 7277 6973 6520 7468 6520 6974 656d 2077  rwise the item w
+0000e560: 696c 6c20 6661 696c 2074 6865 2076 616c  ill fail the val
+0000e570: 6964 6174 696f 6e2e 9485 9481 947d 9428  idation......}.(
+0000e580: 6a23 0300 006a 540b 0000 6a33 0300 006a  j#...jT...j3...j
+0000e590: 1103 0000 6a34 0300 004e 6a36 0300 004e  ....j4...Nj6...N
+0000e5a0: 7562 656a 2403 0000 7d94 286a 2603 0000  ubej$...}.(j&...
+0000e5b0: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
+0000e5c0: 6a2c 0300 005d 946a 2e03 0000 5d94 756a  j,...].j....].uj
+0000e5d0: 3203 0000 6a5d 0300 006a 3403 0000 6a5c  2...j]...j4...j\
+0000e5e0: 0300 006a 3603 0000 4be8 6a23 0300 006a  ...j6...K.j#...j
+0000e5f0: 500b 0000 7562 616a 2403 0000 7d94 286a  P...ubaj$...}.(j
+0000e600: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
+0000e610: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
+0000e620: 5d94 756a 3203 0000 6a1d 0800 006a 2303  ].uj2...j....j#.
+0000e630: 0000 6aa5 0a00 006a 3303 0000 6a11 0300  ..j....j3...j...
+0000e640: 006a 3403 0000 6a5c 0300 006a 3603 0000  .j4...j\...j6...
+0000e650: 4e75 6265 6a24 0300 007d 9428 6a26 0300  Nubej$...}.(j&..
+0000e660: 005d 948c 0661 6374 696f 6e94 616a 2803  .]...action.aj(.
+0000e670: 0000 5d94 6a2a 0300 005d 948c 0661 6374  ..].j*...]...act
+0000e680: 696f 6e94 616a 2c03 0000 5d94 6a2e 0300  ion.aj,...].j...
+0000e690: 005d 9475 6a32 0300 0068 4e6a 2303 0000  .].uj2...hNj#...
+0000e6a0: 6a2c 0600 006a 3303 0000 6a11 0300 006a  j,...j3...j....j
+0000e6b0: 3403 0000 6a5c 0300 006a 3603 0000 4bc7  4...j\...j6...K.
+0000e6c0: 7562 656a 2403 0000 7d94 286a 2603 0000  ubej$...}.(j&...
+0000e6d0: 5d94 8c05 7573 6167 6594 616a 2803 0000  ]...usage.aj(...
+0000e6e0: 5d94 6a2a 0300 005d 948c 0575 7361 6765  ].j*...]...usage
+0000e6f0: 9461 6a2c 0300 005d 946a 2e03 0000 5d94  .aj,...].j....].
+0000e700: 756a 3203 0000 684e 6a23 0300 006a 9e04  uj2...hNj#...j..
+0000e710: 0000 6a33 0300 006a 1103 0000 6a34 0300  ..j3...j....j4..
+0000e720: 006a 5c03 0000 6a36 0300 004b 3c75 626a  .j\...j6...K<ubj
+0000e730: 3703 0000 2981 947d 9428 6a13 0300 0068  7...)..}.(j....h
+0000e740: 5e6a 1403 0000 5d94 286a 3c03 0000 2981  ^j....].(j<...).
+0000e750: 947d 9428 6a13 0300 008c 1a52 756e 2c20  .}.(j......Run, 
+0000e760: 4465 7665 6c6f 706d 656e 7420 616e 6420  Development and 
+0000e770: 4275 696c 6494 6a14 0300 005d 946a 1e03  Build.j....].j..
+0000e780: 0000 8c1a 5275 6e2c 2044 6576 656c 6f70  ....Run, Develop
+0000e790: 6d65 6e74 2061 6e64 2042 7569 6c64 9485  ment and Build..
+0000e7a0: 9481 947d 9428 6a23 0300 006a 9e0b 0000  ...}.(j#...j....
+0000e7b0: 6a33 0300 006a 1103 0000 6a34 0300 004e  j3...j....j4...N
+0000e7c0: 6a36 0300 004e 7562 616a 2403 0000 7d94  j6...Nubaj$...}.
+0000e7d0: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
+0000e7e0: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
+0000e7f0: 0000 5d94 756a 3203 0000 6a3b 0300 006a  ..].uj2...j;...j
+0000e800: 2303 0000 6a9b 0b00 006a 3303 0000 6a11  #...j....j3...j.
+0000e810: 0300 006a 3403 0000 6a5c 0300 006a 3603  ...j4...j\...j6.
+0000e820: 0000 4beb 7562 6a5e 0300 0029 8194 7d94  ..K.ubj^...)..}.
+0000e830: 286a 1303 0000 8c71 546f 2073 7461 7274  (j.....qTo start
+0000e840: 206f 6e6c 7920 796f 7572 2061 7070 6c69   only your appli
+0000e850: 6361 7469 6f6e 2c20 7275 6e20 6060 7079  cation, run ``py
+0000e860: 7468 6f6e 2061 7070 2e70 7960 6020 696e  thon app.py`` in
+0000e870: 2079 6f75 7220 7072 6f6a 6563 7420 726f   your project ro
+0000e880: 6f74 2064 6972 6563 746f 7279 2e20 5573  ot directory. Us
+0000e890: 6520 7468 6520 7465 726d 696e 616c 2069  e the terminal i
+0000e8a0: 6e20 7673 636f 6465 2e94 6a14 0300 005d  n vscode..j....]
+0000e8b0: 9428 6a1e 0300 008c 2454 6f20 7374 6172  .(j.....$To star
+0000e8c0: 7420 6f6e 6c79 2079 6f75 7220 6170 706c  t only your appl
+0000e8d0: 6963 6174 696f 6e2c 2072 756e 2094 8594  ication, run ...
+0000e8e0: 8194 7d94 286a 2303 0000 6aac 0b00 006a  ..}.(j#...j....j
+0000e8f0: 3303 0000 6a11 0300 006a 3403 0000 4e6a  3...j....j4...Nj
+0000e900: 3603 0000 4e75 626a f905 0000 2981 947d  6...Nubj....)..}
+0000e910: 9428 6a13 0300 008c 1160 6070 7974 686f  .(j......``pytho
+0000e920: 6e20 6170 702e 7079 6060 946a 1403 0000  n app.py``.j....
+0000e930: 5d94 6a1e 0300 008c 0d70 7974 686f 6e20  ].j......python 
+0000e940: 6170 702e 7079 9485 9481 947d 9428 6a23  app.py.....}.(j#
+0000e950: 0300 006a b40b 0000 6a33 0300 006a 1103  ...j....j3...j..
+0000e960: 0000 6a34 0300 004e 6a36 0300 004e 7562  ..j4...Nj6...Nub
+0000e970: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
+0000e980: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
+0000e990: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
+0000e9a0: 0000 6af8 0500 006a 2303 0000 6aac 0b00  ..j....j#...j...
+0000e9b0: 0075 626a 1e03 0000 8c3c 2069 6e20 796f  .ubj.....< in yo
+0000e9c0: 7572 2070 726f 6a65 6374 2072 6f6f 7420  ur project root 
+0000e9d0: 6469 7265 6374 6f72 792e 2055 7365 2074  directory. Use t
+0000e9e0: 6865 2074 6572 6d69 6e61 6c20 696e 2076  he terminal in v
+0000e9f0: 7363 6f64 652e 9485 9481 947d 9428 6a23  scode......}.(j#
+0000ea00: 0300 006a ac0b 0000 6a33 0300 006a 1103  ...j....j3...j..
+0000ea10: 0000 6a34 0300 004e 6a36 0300 004e 7562  ..j4...Nj6...Nub
+0000ea20: 656a 2403 0000 7d94 286a 2603 0000 5d94  ej$...}.(j&...].
+0000ea30: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
+0000ea40: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
+0000ea50: 0000 6a5d 0300 006a 3403 0000 6a5c 0300  ..j]...j4...j\..
+0000ea60: 006a 3603 0000 4bec 6a23 0300 006a 9b0b  .j6...K.j#...j..
+0000ea70: 0000 6a33 0300 006a 1103 0000 7562 6a5e  ..j3...j....ubj^
+0000ea80: 0300 0029 8194 7d94 286a 1303 0000 8c34  ...)..}.(j.....4
+0000ea90: 4f70 656e 2074 6865 2062 726f 7773 6572  Open the browser
+0000eaa0: 2061 6e64 2074 7970 6520 6060 6874 7470   and type ``http
+0000eab0: 3a2f 2f6c 6f63 616c 686f 7374 3a35 3535  ://localhost:555
+0000eac0: 3560 602e 946a 1403 0000 5d94 286a 1e03  5``..j....].(j..
+0000ead0: 0000 8c1a 4f70 656e 2074 6865 2062 726f  ....Open the bro
+0000eae0: 7773 6572 2061 6e64 2074 7970 6520 9485  wser and type ..
+0000eaf0: 9481 947d 9428 6a23 0300 006a cc0b 0000  ...}.(j#...j....
+0000eb00: 6a33 0300 006a 1103 0000 6a34 0300 004e  j3...j....j4...N
+0000eb10: 6a36 0300 004e 7562 6af9 0500 0029 8194  j6...Nubj....)..
+0000eb20: 7d94 286a 1303 0000 8c19 6060 6874 7470  }.(j......``http
+0000eb30: 3a2f 2f6c 6f63 616c 686f 7374 3a35 3535  ://localhost:555
+0000eb40: 3560 6094 6a14 0300 005d 946a 1e03 0000  5``.j....].j....
+0000eb50: 8c15 6874 7470 3a2f 2f6c 6f63 616c 686f  ..http://localho
+0000eb60: 7374 3a35 3535 3594 8594 8194 7d94 286a  st:5555.....}.(j
+0000eb70: 2303 0000 6ad4 0b00 006a 3303 0000 6a11  #...j....j3...j.
+0000eb80: 0300 006a 3403 0000 4e6a 3603 0000 4e75  ...j4...Nj6...Nu
+0000eb90: 6261 6a24 0300 007d 9428 6a26 0300 005d  baj$...}.(j&...]
+0000eba0: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
+0000ebb0: 2c03 0000 5d94 6a2e 0300 005d 9475 6a32  ,...].j....].uj2
+0000ebc0: 0300 006a f805 0000 6a23 0300 006a cc0b  ...j....j#...j..
+0000ebd0: 0000 7562 6a1e 0300 008c 012e 9485 9481  ..ubj...........
+0000ebe0: 947d 9428 6a23 0300 006a cc0b 0000 6a33  .}.(j#...j....j3
+0000ebf0: 0300 006a 1103 0000 6a34 0300 004e 6a36  ...j....j4...Nj6
+0000ec00: 0300 004e 7562 656a 2403 0000 7d94 286a  ...Nubej$...}.(j
+0000ec10: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
+0000ec20: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
+0000ec30: 5d94 756a 3203 0000 6a5d 0300 006a 3403  ].uj2...j]...j4.
+0000ec40: 0000 6a5c 0300 006a 3603 0000 4bee 6a23  ..j\...j6...K.j#
+0000ec50: 0300 006a 9b0b 0000 6a33 0300 006a 1103  ...j....j3...j..
+0000ec60: 0000 7562 6a37 0300 0029 8194 7d94 286a  ..ubj7...)..}.(j
+0000ec70: 1303 0000 685e 6a14 0300 005d 9428 6a3c  ....h^j....].(j<
+0000ec80: 0300 0029 8194 7d94 286a 1303 0000 8c0b  ...)..}.(j......
+0000ec90: 4465 7665 6c6f 706d 656e 7494 6a14 0300  Development.j...
+0000eca0: 005d 946a 1e03 0000 8c0b 4465 7665 6c6f  .].j......Develo
+0000ecb0: 706d 656e 7494 8594 8194 7d94 286a 2303  pment.....}.(j#.
+0000ecc0: 0000 6aef 0b00 006a 3303 0000 6a11 0300  ..j....j3...j...
+0000ecd0: 006a 3403 0000 4e6a 3603 0000 4e75 6261  .j4...Nj6...Nuba
+0000ece0: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+0000ecf0: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+0000ed00: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+0000ed10: 006a 3b03 0000 6a23 0300 006a ec0b 0000  .j;...j#...j....
+0000ed20: 6a33 0300 006a 1103 0000 6a34 0300 006a  j3...j....j4...j
+0000ed30: 5c03 0000 6a36 0300 004b f175 626a 5e03  \...j6...K.ubj^.
+0000ed40: 0000 2981 947d 9428 6a13 0300 008c 6c54  ..)..}.(j.....lT
+0000ed50: 6f20 6465 7665 6c6f 7020 796f 7572 2061  o develop your a
+0000ed60: 7070 6c69 6361 7469 6f6e 2c20 7573 6520  pplication, use 
+0000ed70: 796f 7572 2064 6562 7567 6765 7220 7769  your debugger wi
+0000ed80: 7468 2074 6865 2060 605b 6465 765d 2064  th the ``[dev] d
+0000ed90: 6563 6f72 6520 6261 7365 2064 6576 656c  ecore base devel
+0000eda0: 6f70 6d65 6e74 6060 2070 726f 6669 6c65  opment`` profile
+0000edb0: 2069 6e20 7673 636f 6465 2e94 6a14 0300   in vscode..j...
+0000edc0: 005d 9428 6a1e 0300 008c 3854 6f20 6465  .].(j.....8To de
+0000edd0: 7665 6c6f 7020 796f 7572 2061 7070 6c69  velop your appli
+0000ede0: 6361 7469 6f6e 2c20 7573 6520 796f 7572  cation, use your
+0000edf0: 2064 6562 7567 6765 7220 7769 7468 2074   debugger with t
+0000ee00: 6865 2094 8594 8194 7d94 286a 2303 0000  he .....}.(j#...
+0000ee10: 6afd 0b00 006a 3303 0000 6a11 0300 006a  j....j3...j....j
+0000ee20: 3403 0000 4e6a 3603 0000 4e75 626a f905  4...Nj6...Nubj..
+0000ee30: 0000 2981 947d 9428 6a13 0300 008c 2160  ..)..}.(j.....!`
+0000ee40: 605b 6465 765d 2064 6563 6f72 6520 6261  `[dev] decore ba
+0000ee50: 7365 2064 6576 656c 6f70 6d65 6e74 6060  se development``
+0000ee60: 946a 1403 0000 5d94 6a1e 0300 008c 1d5b  .j....].j......[
+0000ee70: 6465 765d 2064 6563 6f72 6520 6261 7365  dev] decore base
+0000ee80: 2064 6576 656c 6f70 6d65 6e74 9485 9481   development....
+0000ee90: 947d 9428 6a23 0300 006a 050c 0000 6a33  .}.(j#...j....j3
+0000eea0: 0300 006a 1103 0000 6a34 0300 004e 6a36  ...j....j4...Nj6
+0000eeb0: 0300 004e 7562 616a 2403 0000 7d94 286a  ...Nubaj$...}.(j
+0000eec0: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
+0000eed0: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
+0000eee0: 5d94 756a 3203 0000 6af8 0500 006a 2303  ].uj2...j....j#.
+0000eef0: 0000 6afd 0b00 0075 626a 1e03 0000 8c13  ..j....ubj......
+0000ef00: 2070 726f 6669 6c65 2069 6e20 7673 636f   profile in vsco
+0000ef10: 6465 2e94 8594 8194 7d94 286a 2303 0000  de......}.(j#...
+0000ef20: 6afd 0b00 006a 3303 0000 6a11 0300 006a  j....j3...j....j
+0000ef30: 3403 0000 4e6a 3603 0000 4e75 6265 6a24  4...Nj6...Nubej$
+0000ef40: 0300 007d 9428 6a26 0300 005d 946a 2803  ...}.(j&...].j(.
+0000ef50: 0000 5d94 6a2a 0300 005d 946a 2c03 0000  ..].j*...].j,...
+0000ef60: 5d94 6a2e 0300 005d 9475 6a32 0300 006a  ].j....].uj2...j
+0000ef70: 5d03 0000 6a34 0300 006a 5c03 0000 6a36  ]...j4...j\...j6
+0000ef80: 0300 004b f26a 2303 0000 6aec 0b00 006a  ...K.j#...j....j
+0000ef90: 3303 0000 6a11 0300 0075 626a 5e03 0000  3...j....ubj^...
+0000efa0: 2981 947d 9428 6a13 0300 008c 344f 7065  )..}.(j.....4Ope
+0000efb0: 6e20 7468 6520 6272 6f77 7365 7220 616e  n the browser an
+0000efc0: 6420 7479 7065 2060 6068 7474 703a 2f2f  d type ``http://
+0000efd0: 6c6f 6361 6c68 6f73 743a 3535 3535 6060  localhost:5555``
+0000efe0: 2e94 6a14 0300 005d 9428 6a1e 0300 008c  ..j....].(j.....
+0000eff0: 1a4f 7065 6e20 7468 6520 6272 6f77 7365  .Open the browse
+0000f000: 7220 616e 6420 7479 7065 2094 8594 8194  r and type .....
+0000f010: 7d94 286a 2303 0000 6a1d 0c00 006a 3303  }.(j#...j....j3.
+0000f020: 0000 6a11 0300 006a 3403 0000 4e6a 3603  ..j....j4...Nj6.
+0000f030: 0000 4e75 626a f905 0000 2981 947d 9428  ..Nubj....)..}.(
+0000f040: 6a13 0300 008c 1960 6068 7474 703a 2f2f  j......``http://
+0000f050: 6c6f 6361 6c68 6f73 743a 3535 3535 6060  localhost:5555``
+0000f060: 946a 1403 0000 5d94 6a1e 0300 008c 1568  .j....].j......h
+0000f070: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+0000f080: 3535 3535 9485 9481 947d 9428 6a23 0300  5555.....}.(j#..
+0000f090: 006a 250c 0000 6a33 0300 006a 1103 0000  .j%...j3...j....
+0000f0a0: 6a34 0300 004e 6a36 0300 004e 7562 616a  j4...Nj6...Nubaj
+0000f0b0: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
+0000f0c0: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
+0000f0d0: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
+0000f0e0: 6af8 0500 006a 2303 0000 6a1d 0c00 0075  j....j#...j....u
+0000f0f0: 626a 1e03 0000 8c01 2e94 8594 8194 7d94  bj............}.
+0000f100: 286a 2303 0000 6a1d 0c00 006a 3303 0000  (j#...j....j3...
+0000f110: 6a11 0300 006a 3403 0000 4e6a 3603 0000  j....j4...Nj6...
+0000f120: 4e75 6265 6a24 0300 007d 9428 6a26 0300  Nubej$...}.(j&..
+0000f130: 005d 946a 2803 0000 5d94 6a2a 0300 005d  .].j(...].j*...]
+0000f140: 946a 2c03 0000 5d94 6a2e 0300 005d 9475  .j,...].j....].u
+0000f150: 6a32 0300 006a 5d03 0000 6a34 0300 006a  j2...j]...j4...j
+0000f160: 5c03 0000 6a36 0300 004b f46a 2303 0000  \...j6...K.j#...
+0000f170: 6aec 0b00 006a 3303 0000 6a11 0300 0075  j....j3...j....u
+0000f180: 6265 6a24 0300 007d 9428 6a26 0300 005d  bej$...}.(j&...]
+0000f190: 948c 0b64 6576 656c 6f70 6d65 6e74 9461  ...development.a
+0000f1a0: 6a28 0300 005d 946a 2a03 0000 5d94 8c0b  j(...].j*...]...
+0000f1b0: 6465 7665 6c6f 706d 656e 7494 616a 2c03  development.aj,.
+0000f1c0: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+0000f1d0: 0068 4e6a 2303 0000 6a9b 0b00 006a 3303  .hNj#...j....j3.
+0000f1e0: 0000 6a11 0300 006a 3403 0000 6a5c 0300  ..j....j4...j\..
+0000f1f0: 006a 3603 0000 4bf1 7562 6a37 0300 0029  .j6...K.ubj7...)
+0000f200: 8194 7d94 286a 1303 0000 685e 6a14 0300  ..}.(j....h^j...
+0000f210: 005d 9428 6a3c 0300 0029 8194 7d94 286a  .].(j<...)..}.(j
+0000f220: 1303 0000 8c05 4275 696c 6494 6a14 0300  ......Build.j...
+0000f230: 005d 946a 1e03 0000 8c05 4275 696c 6494  .].j......Build.
+0000f240: 8594 8194 7d94 286a 2303 0000 6a48 0c00  ....}.(j#...jH..
+0000f250: 006a 3303 0000 6a11 0300 006a 3403 0000  .j3...j....j4...
+0000f260: 4e6a 3603 0000 4e75 6261 6a24 0300 007d  Nj6...Nubaj$...}
+0000f270: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
+0000f280: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
+0000f290: 0300 005d 9475 6a32 0300 006a 3b03 0000  ...].uj2...j;...
+0000f2a0: 6a23 0300 006a 450c 0000 6a33 0300 006a  j#...jE...j3...j
+0000f2b0: 1103 0000 6a34 0300 006a 5c03 0000 6a36  ....j4...j\...j6
+0000f2c0: 0300 004b f775 626a 5e03 0000 2981 947d  ...K.ubj^...)..}
+0000f2d0: 9428 6a13 0300 008c 7454 6f20 6275 696c  .(j.....tTo buil
+0000f2e0: 6420 796f 7572 2061 7070 6c69 6361 7469  d your applicati
+0000f2f0: 6f6e 2c20 7275 6e20 6060 7079 7468 6f6e  on, run ``python
+0000f300: 2061 7070 2e70 7920 2d2d 6275 696c 6460   app.py --build`
+0000f310: 6020 696e 2079 6f75 7220 7072 6f6a 6563  ` in your projec
+0000f320: 7420 726f 6f74 2064 6972 6563 746f 7279  t root directory
+0000f330: 2e20 5573 6520 7468 6520 7465 726d 696e  . Use the termin
+0000f340: 616c 2069 6e20 7673 636f 6465 2e94 6a14  al in vscode..j.
+0000f350: 0300 005d 9428 6a1e 0300 008c 1f54 6f20  ...].(j......To 
+0000f360: 6275 696c 6420 796f 7572 2061 7070 6c69  build your appli
+0000f370: 6361 7469 6f6e 2c20 7275 6e20 9485 9481  cation, run ....
+0000f380: 947d 9428 6a23 0300 006a 560c 0000 6a33  .}.(j#...jV...j3
+0000f390: 0300 006a 1103 0000 6a34 0300 004e 6a36  ...j....j4...Nj6
+0000f3a0: 0300 004e 7562 6af9 0500 0029 8194 7d94  ...Nubj....)..}.
+0000f3b0: 286a 1303 0000 8c19 6060 7079 7468 6f6e  (j......``python
+0000f3c0: 2061 7070 2e70 7920 2d2d 6275 696c 6460   app.py --build`
+0000f3d0: 6094 6a14 0300 005d 946a 1e03 0000 8c15  `.j....].j......
+0000f3e0: 7079 7468 6f6e 2061 7070 2e70 7920 2d2d  python app.py --
+0000f3f0: 6275 696c 6494 8594 8194 7d94 286a 2303  build.....}.(j#.
+0000f400: 0000 6a5e 0c00 006a 3303 0000 6a11 0300  ..j^...j3...j...
+0000f410: 006a 3403 0000 4e6a 3603 0000 4e75 6261  .j4...Nj6...Nuba
+0000f420: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+0000f430: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+0000f440: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+0000f450: 006a f805 0000 6a23 0300 006a 560c 0000  .j....j#...jV...
+0000f460: 7562 6a1e 0300 008c 3c20 696e 2079 6f75  ubj.....< in you
+0000f470: 7220 7072 6f6a 6563 7420 726f 6f74 2064  r project root d
+0000f480: 6972 6563 746f 7279 2e20 5573 6520 7468  irectory. Use th
+0000f490: 6520 7465 726d 696e 616c 2069 6e20 7673  e terminal in vs
+0000f4a0: 636f 6465 2e94 8594 8194 7d94 286a 2303  code......}.(j#.
+0000f4b0: 0000 6a56 0c00 006a 3303 0000 6a11 0300  ..jV...j3...j...
+0000f4c0: 006a 3403 0000 4e6a 3603 0000 4e75 6265  .j4...Nj6...Nube
+0000f4d0: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+0000f4e0: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+0000f4f0: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+0000f500: 006a 5d03 0000 6a34 0300 006a 5c03 0000  .j]...j4...j\...
+0000f510: 6a36 0300 004b f86a 2303 0000 6a45 0c00  j6...K.j#...jE..
+0000f520: 006a 3303 0000 6a11 0300 0075 6265 6a24  .j3...j....ubej$
+0000f530: 0300 007d 9428 6a26 0300 005d 948c 0562  ...}.(j&...]...b
+0000f540: 7569 6c64 9461 6a28 0300 005d 946a 2a03  uild.aj(...].j*.
+0000f550: 0000 5d94 8c05 6275 696c 6494 616a 2c03  ..]...build.aj,.
+0000f560: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+0000f570: 0068 4e6a 2303 0000 6a9b 0b00 006a 3303  .hNj#...j....j3.
+0000f580: 0000 6a11 0300 006a 3403 0000 6a5c 0300  ..j....j4...j\..
+0000f590: 006a 3603 0000 4bf7 7562 656a 2403 0000  .j6...K.ubej$...
+0000f5a0: 7d94 286a 2603 0000 5d94 8c19 7275 6e2d  }.(j&...]...run-
+0000f5b0: 6465 7665 6c6f 706d 656e 742d 616e 642d  development-and-
+0000f5c0: 6275 696c 6494 616a 2803 0000 5d94 6a2a  build.aj(...].j*
+0000f5d0: 0300 005d 948c 1a72 756e 2c20 6465 7665  ...]...run, deve
+0000f5e0: 6c6f 706d 656e 7420 616e 6420 6275 696c  lopment and buil
+0000f5f0: 6494 616a 2c03 0000 5d94 6a2e 0300 005d  d.aj,...].j....]
+0000f600: 9475 6a32 0300 0068 4e6a 2303 0000 6a9e  .uj2...hNj#...j.
+0000f610: 0400 006a 3303 0000 6a11 0300 006a 3403  ...j3...j....j4.
+0000f620: 0000 6a5c 0300 006a 3603 0000 4beb 7562  ..j\...j6...K.ub
+0000f630: 656a 2403 0000 7d94 286a 2603 0000 5d94  ej$...}.(j&...].
+0000f640: 8c0b 6765 742d 7374 6172 7465 6494 616a  ..get-started.aj
+0000f650: 2803 0000 5d94 6a2a 0300 005d 948c 0b67  (...].j*...]...g
+0000f660: 6574 2073 7461 7274 6564 9461 6a2c 0300  et started.aj,..
+0000f670: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
+0000f680: 684e 6a23 0300 006a 3803 0000 6a33 0300  hNj#...j8...j3..
+0000f690: 006a 1103 0000 6a34 0300 006a 5c03 0000  .j....j4...j\...
+0000f6a0: 6a36 0300 004b 1a75 626a 3703 0000 2981  j6...K.ubj7...).
+0000f6b0: 947d 9428 6a13 0300 0068 5e6a 1403 0000  .}.(j....h^j....
+0000f6c0: 5d94 286a 3c03 0000 2981 947d 9428 6a13  ].(j<...)..}.(j.
+0000f6d0: 0300 008c 1253 616d 706c 6520 6170 706c  .....Sample appl
+0000f6e0: 6963 6174 696f 6e94 6a14 0300 005d 946a  ication.j....].j
+0000f6f0: 1e03 0000 8c12 5361 6d70 6c65 2061 7070  ......Sample app
+0000f700: 6c69 6361 7469 6f6e 9485 9481 947d 9428  lication.....}.(
+0000f710: 6a23 0300 006a 910c 0000 6a33 0300 006a  j#...j....j3...j
+0000f720: 1103 0000 6a34 0300 004e 6a36 0300 004e  ....j4...Nj6...N
+0000f730: 7562 616a 2403 0000 7d94 286a 2603 0000  ubaj$...}.(j&...
+0000f740: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
+0000f750: 6a2c 0300 005d 946a 2e03 0000 5d94 756a  j,...].j....].uj
+0000f760: 3203 0000 6a3b 0300 006a 2303 0000 6a8e  2...j;...j#...j.
+0000f770: 0c00 006a 3303 0000 6a11 0300 006a 3403  ...j3...j....j4.
+0000f780: 0000 6a5c 0300 006a 3603 0000 4bfb 7562  ..j\...j6...K.ub
+0000f790: 6a5e 0300 0029 8194 7d94 286a 1303 0000  j^...)..}.(j....
+0000f7a0: 8c9e 546f 2062 6574 7465 7220 756e 6465  ..To better unde
+0000f7b0: 7273 7461 6e64 2068 6f77 2064 6563 6f72  rstand how decor
+0000f7c0: 6520 6261 7365 2077 6f72 6b73 2c20 6974  e base works, it
+0000f7d0: 2069 7320 6265 7374 2074 6f20 6c6f 6f6b   is best to look
+0000f7e0: 2061 7420 7468 6520 7361 6d70 6c65 2061   at the sample a
+0000f7f0: 7070 6c69 6361 7469 6f6e 2e20 5468 6520  pplication. The 
+0000f800: 6170 706c 6963 6174 696f 6e20 7265 7072  application repr
+0000f810: 6573 656e 7473 206d 7920 636f 6e74 696e  esents my contin
+0000f820: 756f 7573 2064 6576 656c 6f70 6d65 6e74  uous development
+0000f830: 206f 6620 6465 636f 7265 2062 6173 652e   of decore base.
+0000f840: 946a 1403 0000 5d94 6a1e 0300 008c 9e54  .j....].j......T
+0000f850: 6f20 6265 7474 6572 2075 6e64 6572 7374  o better underst
+0000f860: 616e 6420 686f 7720 6465 636f 7265 2062  and how decore b
+0000f870: 6173 6520 776f 726b 732c 2069 7420 6973  ase works, it is
+0000f880: 2062 6573 7420 746f 206c 6f6f 6b20 6174   best to look at
+0000f890: 2074 6865 2073 616d 706c 6520 6170 706c   the sample appl
+0000f8a0: 6963 6174 696f 6e2e 2054 6865 2061 7070  ication. The app
+0000f8b0: 6c69 6361 7469 6f6e 2072 6570 7265 7365  lication represe
+0000f8c0: 6e74 7320 6d79 2063 6f6e 7469 6e75 6f75  nts my continuou
+0000f8d0: 7320 6465 7665 6c6f 706d 656e 7420 6f66  s development of
+0000f8e0: 2064 6563 6f72 6520 6261 7365 2e94 8594   decore base....
+0000f8f0: 8194 7d94 286a 2303 0000 6a9f 0c00 006a  ..}.(j#...j....j
+0000f900: 3303 0000 6a11 0300 006a 3403 0000 4e6a  3...j....j4...Nj
+0000f910: 3603 0000 4e75 6261 6a24 0300 007d 9428  6...Nubaj$...}.(
+0000f920: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
+0000f930: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
+0000f940: 005d 9475 6a32 0300 006a 5d03 0000 6a34  .].uj2...j]...j4
+0000f950: 0300 006a 5c03 0000 6a36 0300 004b fc6a  ...j\...j6...K.j
+0000f960: 2303 0000 6a8e 0c00 006a 3303 0000 6a11  #...j....j3...j.
+0000f970: 0300 0075 626a 5e03 0000 2981 947d 9428  ...ubj^...)..}.(
+0000f980: 6a13 0300 008c 4868 7474 7073 3a2f 2f67  j.....Hhttps://g
+0000f990: 6974 6875 622e 636f 6d2f 4b65 6d6f 5061  ithub.com/KemoPa
+0000f9a0: 6e7a 6168 2f64 6563 6f72 655f 4261 7365  nzah/decore_Base
+0000f9b0: 2f74 7265 652f 6d61 7374 6572 2f64 6563  /tree/master/dec
+0000f9c0: 6f72 655f 6261 7365 2f73 616d 706c 6594  ore_base/sample.
+0000f9d0: 6a14 0300 005d 946a 9e03 0000 2981 947d  j....].j....)..}
+0000f9e0: 9428 6a13 0300 006a af0c 0000 6a14 0300  .(j....j....j...
+0000f9f0: 005d 946a 1e03 0000 8c48 6874 7470 733a  .].j.....Hhttps:
+0000fa00: 2f2f 6769 7468 7562 2e63 6f6d 2f4b 656d  //github.com/Kem
+0000fa10: 6f50 616e 7a61 682f 6465 636f 7265 5f42  oPanzah/decore_B
+0000fa20: 6173 652f 7472 6565 2f6d 6173 7465 722f  ase/tree/master/
+0000fa30: 6465 636f 7265 5f62 6173 652f 7361 6d70  decore_base/samp
+0000fa40: 6c65 9485 9481 947d 9428 6a23 0300 006a  le.....}.(j#...j
+0000fa50: b10c 0000 6a33 0300 006a 1103 0000 6a34  ....j3...j....j4
+0000fa60: 0300 004e 6a36 0300 004e 7562 616a 2403  ...Nj6...Nubaj$.
+0000fa70: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
+0000fa80: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
+0000fa90: 946a 2e03 0000 5d94 8c06 7265 6675 7269  .j....]...refuri
+0000faa0: 946a af0c 0000 756a 3203 0000 6a9d 0300  .j....uj2...j...
+0000fab0: 006a 2303 0000 6aad 0c00 0075 6261 6a24  .j#...j....ubaj$
+0000fac0: 0300 007d 9428 6a26 0300 005d 946a 2803  ...}.(j&...].j(.
+0000fad0: 0000 5d94 6a2a 0300 005d 946a 2c03 0000  ..].j*...].j,...
+0000fae0: 5d94 6a2e 0300 005d 9475 6a32 0300 006a  ].j....].uj2...j
+0000faf0: 5d03 0000 6a34 0300 006a 5c03 0000 6a36  ]...j4...j\...j6
+0000fb00: 0300 004b fe6a 2303 0000 6a8e 0c00 006a  ...K.j#...j....j
+0000fb10: 3303 0000 6a11 0300 0075 626a 5e03 0000  3...j....ubj^...
+0000fb20: 2981 947d 9428 6a13 0300 008c b054 6f20  )..}.(j......To 
+0000fb30: 7379 6e63 6872 6f6e 697a 6520 7468 6520  synchronize the 
+0000fb40: 7361 6d70 6c65 2061 7070 6c69 6361 7469  sample applicati
+0000fb50: 6f6e 2077 6974 6820 6120 7375 6266 6f6c  on with a subfol
+0000fb60: 6465 7220 6f66 2074 6865 2070 726f 6a65  der of the proje
+0000fb70: 6374 2072 6f6f 7420 6469 7265 6374 6f72  ct root director
+0000fb80: 792c 2072 756e 2060 6070 7974 686f 6e20  y, run ``python 
+0000fb90: 6170 702e 7079 202d 2d73 616d 706c 6560  app.py --sample`
+0000fba0: 6020 696e 2079 6f75 7220 7072 6f6a 6563  ` in your projec
+0000fbb0: 7420 726f 6f74 2064 6972 6563 746f 7279  t root directory
+0000fbc0: 2e20 5573 6520 7468 6520 7465 726d 696e  . Use the termin
+0000fbd0: 616c 2069 6e20 7673 636f 6465 2e94 6a14  al in vscode..j.
+0000fbe0: 0300 005d 9428 6a1e 0300 008c 5a54 6f20  ...].(j.....ZTo 
+0000fbf0: 7379 6e63 6872 6f6e 697a 6520 7468 6520  synchronize the 
+0000fc00: 7361 6d70 6c65 2061 7070 6c69 6361 7469  sample applicati
+0000fc10: 6f6e 2077 6974 6820 6120 7375 6266 6f6c  on with a subfol
+0000fc20: 6465 7220 6f66 2074 6865 2070 726f 6a65  der of the proje
+0000fc30: 6374 2072 6f6f 7420 6469 7265 6374 6f72  ct root director
+0000fc40: 792c 2072 756e 2094 8594 8194 7d94 286a  y, run .....}.(j
+0000fc50: 2303 0000 6ac5 0c00 006a 3303 0000 6a11  #...j....j3...j.
+0000fc60: 0300 006a 3403 0000 4e6a 3603 0000 4e75  ...j4...Nj6...Nu
+0000fc70: 626a f905 0000 2981 947d 9428 6a13 0300  bj....)..}.(j...
+0000fc80: 008c 1a60 6070 7974 686f 6e20 6170 702e  ...``python app.
+0000fc90: 7079 202d 2d73 616d 706c 6560 6094 6a14  py --sample``.j.
+0000fca0: 0300 005d 946a 1e03 0000 8c16 7079 7468  ...].j......pyth
+0000fcb0: 6f6e 2061 7070 2e70 7920 2d2d 7361 6d70  on app.py --samp
+0000fcc0: 6c65 9485 9481 947d 9428 6a23 0300 006a  le.....}.(j#...j
+0000fcd0: cd0c 0000 6a33 0300 006a 1103 0000 6a34  ....j3...j....j4
+0000fce0: 0300 004e 6a36 0300 004e 7562 616a 2403  ...Nj6...Nubaj$.
+0000fcf0: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
+0000fd00: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
+0000fd10: 946a 2e03 0000 5d94 756a 3203 0000 6af8  .j....].uj2...j.
+0000fd20: 0500 006a 2303 0000 6ac5 0c00 0075 626a  ...j#...j....ubj
+0000fd30: 1e03 0000 8c3c 2069 6e20 796f 7572 2070  .....< in your p
+0000fd40: 726f 6a65 6374 2072 6f6f 7420 6469 7265  roject root dire
+0000fd50: 6374 6f72 792e 2055 7365 2074 6865 2074  ctory. Use the t
+0000fd60: 6572 6d69 6e61 6c20 696e 2076 7363 6f64  erminal in vscod
+0000fd70: 652e 9485 9481 947d 9428 6a23 0300 006a  e......}.(j#...j
+0000fd80: c50c 0000 6a33 0300 006a 1103 0000 6a34  ....j3...j....j4
+0000fd90: 0300 004e 6a36 0300 004e 7562 656a 2403  ...Nj6...Nubej$.
+0000fda0: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
+0000fdb0: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
+0000fdc0: 946a 2e03 0000 5d94 756a 3203 0000 6a5d  .j....].uj2...j]
+0000fdd0: 0300 006a 3403 0000 6a5c 0300 006a 3603  ...j4...j\...j6.
+0000fde0: 0000 4d00 016a 2303 0000 6a8e 0c00 006a  ..M..j#...j....j
+0000fdf0: 3303 0000 6a11 0300 0075 626a 5e03 0000  3...j....ubj^...
+0000fe00: 2981 947d 9428 6a13 0300 008c 7f54 6f20  )..}.(j......To 
+0000fe10: 7275 6e20 7468 6520 7361 6d70 6c65 2061  run the sample a
+0000fe20: 7070 6c69 6361 7469 6f6e 2061 6674 6572  pplication after
+0000fe30: 2073 796e 6368 726f 6e69 7a61 7469 6f6e   synchronization
+0000fe40: 2c20 7573 6520 796f 7572 2064 6562 7567  , use your debug
+0000fe50: 6765 7220 7769 7468 2074 6865 2060 605b  ger with the ``[
+0000fe60: 736d 705d 2064 6563 6f72 6520 6261 7365  smp] decore base
+0000fe70: 2073 616d 706c 6560 6020 7072 6f66 696c   sample`` profil
+0000fe80: 6520 696e 2076 7363 6f64 652e 946a 1403  e in vscode..j..
+0000fe90: 0000 5d94 286a 1e03 0000 8c50 546f 2072  ..].(j.....PTo r
+0000fea0: 756e 2074 6865 2073 616d 706c 6520 6170  un the sample ap
+0000feb0: 706c 6963 6174 696f 6e20 6166 7465 7220  plication after 
+0000fec0: 7379 6e63 6872 6f6e 697a 6174 696f 6e2c  synchronization,
+0000fed0: 2075 7365 2079 6f75 7220 6465 6275 6767   use your debugg
+0000fee0: 6572 2077 6974 6820 7468 6520 9485 9481  er with the ....
+0000fef0: 947d 9428 6a23 0300 006a e50c 0000 6a33  .}.(j#...j....j3
+0000ff00: 0300 006a 1103 0000 6a34 0300 004e 6a36  ...j....j4...Nj6
+0000ff10: 0300 004e 7562 6af9 0500 0029 8194 7d94  ...Nubj....)..}.
+0000ff20: 286a 1303 0000 8c1c 6060 5b73 6d70 5d20  (j......``[smp] 
+0000ff30: 6465 636f 7265 2062 6173 6520 7361 6d70  decore base samp
+0000ff40: 6c65 6060 946a 1403 0000 5d94 6a1e 0300  le``.j....].j...
+0000ff50: 008c 185b 736d 705d 2064 6563 6f72 6520  ...[smp] decore 
+0000ff60: 6261 7365 2073 616d 706c 6594 8594 8194  base sample.....
+0000ff70: 7d94 286a 2303 0000 6aed 0c00 006a 3303  }.(j#...j....j3.
+0000ff80: 0000 6a11 0300 006a 3403 0000 4e6a 3603  ..j....j4...Nj6.
+0000ff90: 0000 4e75 6261 6a24 0300 007d 9428 6a26  ..Nubaj$...}.(j&
+0000ffa0: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
+0000ffb0: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
+0000ffc0: 9475 6a32 0300 006a f805 0000 6a23 0300  .uj2...j....j#..
+0000ffd0: 006a e50c 0000 7562 6a1e 0300 008c 1320  .j....ubj...... 
+0000ffe0: 7072 6f66 696c 6520 696e 2076 7363 6f64  profile in vscod
+0000fff0: 652e 9485 9481 947d 9428 6a23 0300 006a  e......}.(j#...j
+00010000: e50c 0000 6a33 0300 006a 1103 0000 9526  ....j3...j.....&
+00010010: 3500 0000 0000 006a 3403 0000 4e6a 3603  5......j4...Nj6.
+00010020: 0000 4e75 6265 6a24 0300 007d 9428 6a26  ..Nubej$...}.(j&
+00010030: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
+00010040: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
+00010050: 9475 6a32 0300 006a 5d03 0000 6a34 0300  .uj2...j]...j4..
+00010060: 006a 5c03 0000 6a36 0300 004d 0201 6a23  .j\...j6...M..j#
+00010070: 0300 006a 8e0c 0000 6a33 0300 006a 1103  ...j....j3...j..
+00010080: 0000 7562 656a 2403 0000 7d94 286a 2603  ..ubej$...}.(j&.
+00010090: 0000 5d94 8c12 7361 6d70 6c65 2d61 7070  ..]...sample-app
+000100a0: 6c69 6361 7469 6f6e 9461 6a28 0300 005d  lication.aj(...]
+000100b0: 946a 2a03 0000 5d94 8c12 7361 6d70 6c65  .j*...]...sample
+000100c0: 2061 7070 6c69 6361 7469 6f6e 9461 6a2c   application.aj,
+000100d0: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
+000100e0: 0000 684e 6a23 0300 006a 3803 0000 6a33  ..hNj#...j8...j3
+000100f0: 0300 006a 1103 0000 6a34 0300 006a 5c03  ...j....j4...j\.
+00010100: 0000 6a36 0300 004b fb75 626a 3703 0000  ..j6...K.ubj7...
+00010110: 2981 947d 9428 6a13 0300 0068 5e6a 1403  )..}.(j....h^j..
+00010120: 0000 5d94 286a 3c03 0000 2981 947d 9428  ..].(j<...)..}.(
+00010130: 6a13 0300 008c 054e 6f74 6573 946a 1403  j......Notes.j..
+00010140: 0000 5d94 6a1e 0300 008c 054e 6f74 6573  ..].j......Notes
+00010150: 9485 9481 947d 9428 6a23 0300 006a 100d  .....}.(j#...j..
+00010160: 0000 6a33 0300 006a 1103 0000 6a34 0300  ..j3...j....j4..
+00010170: 004e 6a36 0300 004e 7562 616a 2403 0000  .Nj6...Nubaj$...
+00010180: 7d94 286a 2603 0000 5d94 6a28 0300 005d  }.(j&...].j(...]
+00010190: 946a 2a03 0000 5d94 6a2c 0300 005d 946a  .j*...].j,...].j
+000101a0: 2e03 0000 5d94 756a 3203 0000 6a3b 0300  ....].uj2...j;..
+000101b0: 006a 2303 0000 6a0d 0d00 006a 3303 0000  .j#...j....j3...
+000101c0: 6a11 0300 006a 3403 0000 6a5c 0300 006a  j....j4...j\...j
+000101d0: 3603 0000 4d05 0175 626a 5e03 0000 2981  6...M..ubj^...).
+000101e0: 947d 9428 6a13 0300 008c 4654 6869 7320  .}.(j.....FThis 
+000101f0: 646f 6375 6d65 6e74 6174 696f 6e20 7761  documentation wa
+00010200: 7320 7472 616e 736c 6174 6564 2066 726f  s translated fro
+00010210: 6d20 4765 726d 616e 2069 6e74 6f20 456e  m German into En
+00010220: 676c 6973 6820 7769 7468 2044 6565 706c  glish with Deepl
+00010230: 2e94 6a14 0300 005d 946a 1e03 0000 8c46  ..j....].j.....F
+00010240: 5468 6973 2064 6f63 756d 656e 7461 7469  This documentati
+00010250: 6f6e 2077 6173 2074 7261 6e73 6c61 7465  on was translate
+00010260: 6420 6672 6f6d 2047 6572 6d61 6e20 696e  d from German in
+00010270: 746f 2045 6e67 6c69 7368 2077 6974 6820  to English with 
+00010280: 4465 6570 6c2e 9485 9481 947d 9428 6a23  Deepl......}.(j#
+00010290: 0300 006a 1e0d 0000 6a33 0300 006a 1103  ...j....j3...j..
+000102a0: 0000 6a34 0300 004e 6a36 0300 004e 7562  ..j4...Nj6...Nub
+000102b0: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
+000102c0: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
+000102d0: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
+000102e0: 0000 6a5d 0300 006a 3403 0000 6a5c 0300  ..j]...j4...j\..
+000102f0: 006a 3603 0000 4d06 016a 2303 0000 6a0d  .j6...M..j#...j.
+00010300: 0d00 006a 3303 0000 6a11 0300 0075 626a  ...j3...j....ubj
+00010310: 1603 0000 8c08 636f 6d70 6f75 6e64 9493  ......compound..
+00010320: 9429 8194 7d94 286a 1303 0000 685e 6a14  .)..}.(j....h^j.
+00010330: 0300 005d 946a 0e03 0000 8c07 746f 6374  ...].j......toct
+00010340: 7265 6594 9394 2981 947d 9428 6a13 0300  ree...)..}.(j...
+00010350: 0068 5e6a 1403 0000 5d94 6a24 0300 007d  .h^j....].j$...}
+00010360: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
+00010370: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
+00010380: 0300 005d 946a 2303 0000 6acd 0200 008c  ...].j#...j.....
+00010390: 0765 6e74 7269 6573 945d 948c 0c69 6e63  .entries.]...inc
+000103a0: 6c75 6465 6669 6c65 7394 5d94 8c08 6d61  ludefiles.]...ma
+000103b0: 7864 6570 7468 944b 028c 0763 6170 7469  xdepth.K...capti
+000103c0: 6f6e 944e 8c04 676c 6f62 9489 8c06 6869  on.N..glob....hi
+000103d0: 6464 656e 9488 8c0d 696e 636c 7564 6568  dden....includeh
+000103e0: 6964 6465 6e94 898c 086e 756d 6265 7265  idden....numbere
+000103f0: 6494 4b00 8c0a 7469 746c 6573 6f6e 6c79  d.K...titlesonly
+00010400: 9489 8c0a 7261 7765 6e74 7269 6573 945d  ....rawentries.]
+00010410: 9475 6a32 0300 006a 310d 0000 6a34 0300  .uj2...j1...j4..
+00010420: 006a 3503 0000 6a36 0300 004b 0b6a 2303  .j5...j6...K.j#.
+00010430: 0000 6a2e 0d00 0075 6261 6a24 0300 007d  ..j....ubaj$...}
+00010440: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
+00010450: 8c0f 746f 6374 7265 652d 7772 6170 7065  ..toctree-wrappe
+00010460: 7294 616a 2a03 0000 5d94 6a2c 0300 005d  r.aj*...].j,...]
+00010470: 946a 2e03 0000 5d94 756a 3203 0000 6a2c  .j....].uj2...j,
+00010480: 0d00 006a 2303 0000 6a0d 0d00 006a 3303  ...j#...j....j3.
+00010490: 0000 6a11 0300 006a 3403 0000 6a35 0300  ..j....j4...j5..
+000104a0: 006a 3603 0000 4e75 626a 1803 0000 2981  .j6...Nubj....).
+000104b0: 947d 9428 6a13 0300 008c 1249 6e64 6963  .}.(j......Indic
+000104c0: 6573 2061 6e64 2074 6162 6c65 7394 6a14  es and tables.j.
+000104d0: 0300 005d 946a 1e03 0000 8c12 496e 6469  ...].j......Indi
+000104e0: 6365 7320 616e 6420 7461 626c 6573 9485  ces and tables..
+000104f0: 9481 947d 946a 2303 0000 6a50 0d00 0073  ...}.j#...jP...s
+00010500: 6261 6a24 0300 007d 9428 6a26 0300 005d  baj$...}.(j&...]
+00010510: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
+00010520: 2c03 0000 5d94 6a2e 0300 005d 946a 3003  ,...].j....].j0.
+00010530: 0000 6a31 0300 0075 6a32 0300 006a 1703  ..j1...uj2...j..
+00010540: 0000 6a23 0300 006a 0d0d 0000 6a33 0300  ..j#...j....j3..
+00010550: 006a 1103 0000 6a34 0300 006a 3503 0000  .j....j4...j5...
+00010560: 6a36 0300 004b 0f75 626a 1803 0000 2981  j6...K.ubj....).
+00010570: 947d 9428 6a13 0300 008c 123d 3d3d 3d3d  .}.(j......=====
+00010580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d94 6a14  =============.j.
+00010590: 0300 005d 946a 1e03 0000 8c12 3d3d 3d3d  ...].j......====
+000105a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 9485  ==============..
+000105b0: 9481 947d 946a 2303 0000 6a5e 0d00 0073  ...}.j#...j^...s
+000105c0: 6261 6a24 0300 007d 9428 6a26 0300 005d  baj$...}.(j&...]
+000105d0: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
+000105e0: 2c03 0000 5d94 6a2e 0300 005d 946a 3003  ,...].j....].j0.
+000105f0: 0000 6a31 0300 0075 6a32 0300 006a 1703  ..j1...uj2...j..
+00010600: 0000 6a23 0300 006a 0d0d 0000 6a33 0300  ..j#...j....j3..
+00010610: 006a 1103 0000 6a34 0300 006a 3503 0000  .j....j4...j5...
+00010620: 6a36 0300 004b 1175 626a 1803 0000 2981  j6...K.ubj....).
+00010630: 947d 9428 6a13 0300 008c 112a 203a 7265  .}.(j......* :re
+00010640: 663a 6067 656e 696e 6465 7860 946a 1403  f:`genindex`.j..
+00010650: 0000 5d94 6a1e 0300 008c 112a 203a 7265  ..].j......* :re
+00010660: 663a 6067 656e 696e 6465 7860 9485 9481  f:`genindex`....
+00010670: 947d 946a 2303 0000 6a6c 0d00 0073 6261  .}.j#...jl...sba
+00010680: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+00010690: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+000106a0: 0000 5d94 6a2e 0300 005d 946a 3003 0000  ..].j....].j0...
+000106b0: 6a31 0300 0075 6a32 0300 006a 1703 0000  j1...uj2...j....
+000106c0: 6a23 0300 006a 0d0d 0000 6a33 0300 006a  j#...j....j3...j
+000106d0: 1103 0000 6a34 0300 006a 3503 0000 6a36  ....j4...j5...j6
+000106e0: 0300 004b 1275 626a 1803 0000 2981 947d  ...K.ubj....)..}
+000106f0: 9428 6a13 0300 008c 112a 203a 7265 663a  .(j......* :ref:
+00010700: 606d 6f64 696e 6465 7860 946a 1403 0000  `modindex`.j....
+00010710: 5d94 6a1e 0300 008c 112a 203a 7265 663a  ].j......* :ref:
+00010720: 606d 6f64 696e 6465 7860 9485 9481 947d  `modindex`.....}
+00010730: 946a 2303 0000 6a7a 0d00 0073 6261 6a24  .j#...jz...sbaj$
+00010740: 0300 007d 9428 6a26 0300 005d 946a 2803  ...}.(j&...].j(.
+00010750: 0000 5d94 6a2a 0300 005d 946a 2c03 0000  ..].j*...].j,...
+00010760: 5d94 6a2e 0300 005d 946a 3003 0000 6a31  ].j....].j0...j1
+00010770: 0300 0075 6a32 0300 006a 1703 0000 6a23  ...uj2...j....j#
+00010780: 0300 006a 0d0d 0000 6a33 0300 006a 1103  ...j....j3...j..
+00010790: 0000 6a34 0300 006a 3503 0000 6a36 0300  ..j4...j5...j6..
+000107a0: 004b 1375 626a 1803 0000 2981 947d 9428  .K.ubj....)..}.(
+000107b0: 6a13 0300 008c 0f2a 203a 7265 663a 6073  j......* :ref:`s
+000107c0: 6561 7263 6860 946a 1403 0000 5d94 6a1e  earch`.j....].j.
+000107d0: 0300 008c 0f2a 203a 7265 663a 6073 6561  .....* :ref:`sea
+000107e0: 7263 6860 9485 9481 947d 946a 2303 0000  rch`.....}.j#...
+000107f0: 6a88 0d00 0073 6261 6a24 0300 007d 9428  j....sbaj$...}.(
+00010800: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
+00010810: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
+00010820: 005d 946a 3003 0000 6a31 0300 0075 6a32  .].j0...j1...uj2
+00010830: 0300 006a 1703 0000 6a23 0300 006a 0d0d  ...j....j#...j..
+00010840: 0000 6a33 0300 006a 1103 0000 6a34 0300  ..j3...j....j4..
+00010850: 006a 3503 0000 6a36 0300 004b 1475 6265  .j5...j6...K.ube
+00010860: 6a24 0300 007d 9428 6a26 0300 005d 948c  j$...}.(j&...]..
+00010870: 056e 6f74 6573 9461 6a28 0300 005d 946a  .notes.aj(...].j
+00010880: 2a03 0000 5d94 8c05 6e6f 7465 7394 616a  *...]...notes.aj
+00010890: 2c03 0000 5d94 6a2e 0300 005d 9475 6a32  ,...].j....].uj2
+000108a0: 0300 0068 4e6a 2303 0000 6a38 0300 006a  ...hNj#...j8...j
+000108b0: 3303 0000 6a11 0300 006a 3403 0000 6a5c  3...j....j4...j\
+000108c0: 0300 006a 3603 0000 4d05 0175 6265 6a24  ...j6...M..ubej$
+000108d0: 0300 007d 9428 6a26 0300 005d 948c 0777  ...}.(j&...]...w
+000108e0: 656c 636f 6d65 9461 6a28 0300 005d 946a  elcome.aj(...].j
+000108f0: 2a03 0000 5d94 8c07 7765 6c63 6f6d 6594  *...]...welcome.
+00010900: 616a 2c03 0000 5d94 6a2e 0300 005d 9475  aj,...].j....].u
+00010910: 6a32 0300 0068 4e6a 2303 0000 6a11 0300  j2...hNj#...j...
+00010920: 006a 3303 0000 6a11 0300 006a 3403 0000  .j3...j....j4...
+00010930: 6a35 0300 006a 3603 0000 4b07 7562 656a  j5...j6...K.ubej
+00010940: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
+00010950: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
+00010960: 005d 946a 2e03 0000 5d94 8c06 736f 7572  .].j....]...sour
+00010970: 6365 946a 3503 0000 756a 3203 0000 6a0f  ce.j5...uj2...j.
+00010980: 0300 008c 0e63 7572 7265 6e74 5f73 6f75  .....current_sou
+00010990: 7263 6594 4e8c 0c63 7572 7265 6e74 5f6c  rce.N..current_l
+000109a0: 696e 6594 4e6a de02 0000 8c11 646f 6375  ine.Nj......docu
+000109b0: 7469 6c73 2e66 726f 6e74 656e 6494 8c06  tils.frontend...
+000109c0: 5661 6c75 6573 9493 9429 8194 7d94 286a  Values...)..}.(j
+000109d0: 3b03 0000 4e8c 0967 656e 6572 6174 6f72  ;...N..generator
+000109e0: 944e 8c09 6461 7465 7374 616d 7094 4e8c  .N..datestamp.N.
+000109f0: 0b73 6f75 7263 655f 6c69 6e6b 944e 8c0a  .source_link.N..
+00010a00: 736f 7572 6365 5f75 726c 944e 8c0d 746f  source_url.N..to
+00010a10: 635f 6261 636b 6c69 6e6b 7394 8c05 656e  c_backlinks...en
+00010a20: 7472 7994 8c12 666f 6f74 6e6f 7465 5f62  try...footnote_b
+00010a30: 6163 6b6c 696e 6b73 944b 018c 0d73 6563  acklinks.K...sec
+00010a40: 746e 756d 5f78 666f 726d 944b 018c 0e73  tnum_xform.K...s
+00010a50: 7472 6970 5f63 6f6d 6d65 6e74 7394 4e8c  trip_comments.N.
+00010a60: 1b73 7472 6970 5f65 6c65 6d65 6e74 735f  .strip_elements_
+00010a70: 7769 7468 5f63 6c61 7373 6573 944e 8c0d  with_classes.N..
+00010a80: 7374 7269 705f 636c 6173 7365 7394 4e8c  strip_classes.N.
+00010a90: 0c72 6570 6f72 745f 6c65 7665 6c94 4b02  .report_level.K.
+00010aa0: 6af0 0200 004b 058c 1165 7869 745f 7374  j....K...exit_st
+00010ab0: 6174 7573 5f6c 6576 656c 944b 058c 0564  atus_level.K...d
+00010ac0: 6562 7567 944e 8c0e 7761 726e 696e 675f  ebug.N..warning_
+00010ad0: 7374 7265 616d 944e 8c09 7472 6163 6562  stream.N..traceb
+00010ae0: 6163 6b94 886a ec02 0000 6881 8c1c 696e  ack..j....h...in
+00010af0: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
+00010b00: 6f72 5f68 616e 646c 6572 948c 0673 7472  or_handler...str
+00010b10: 6963 7494 8c0f 6f75 7470 7574 5f65 6e63  ict...output_enc
+00010b20: 6f64 696e 6794 8c05 7574 662d 3894 8c1d  oding...utf-8...
+00010b30: 6f75 7470 7574 5f65 6e63 6f64 696e 675f  output_encoding_
+00010b40: 6572 726f 725f 6861 6e64 6c65 7294 6ac5  error_handler.j.
+00010b50: 0d00 008c 0e65 7272 6f72 5f65 6e63 6f64  .....error_encod
+00010b60: 696e 6794 8c05 7574 662d 3894 8c1c 6572  ing...utf-8...er
+00010b70: 726f 725f 656e 636f 6469 6e67 5f65 7272  ror_encoding_err
+00010b80: 6f72 5f68 616e 646c 6572 948c 1062 6163  or_handler...bac
+00010b90: 6b73 6c61 7368 7265 706c 6163 6594 6af4  kslashreplace.j.
+00010ba0: 0200 0068 6a8c 1372 6563 6f72 645f 6465  ...hj..record_de
+00010bb0: 7065 6e64 656e 6369 6573 944e 680a 4e8c  pendencies.Nh.N.
+00010bc0: 0969 645f 7072 6566 6978 9468 5e6a e002  .id_prefix.h^j..
+00010bd0: 0000 6ae1 0200 008c 0d64 756d 705f 7365  ..j......dump_se
+00010be0: 7474 696e 6773 944e 8c0e 6475 6d70 5f69  ttings.N..dump_i
+00010bf0: 6e74 6572 6e61 6c73 944e 8c0f 6475 6d70  nternals.N..dump
+00010c00: 5f74 7261 6e73 666f 726d 7394 4e8c 0f64  _transforms.N..d
+00010c10: 756d 705f 7073 6575 646f 5f78 6d6c 944e  ump_pseudo_xml.N
+00010c20: 8c10 6578 706f 7365 5f69 6e74 6572 6e61  ..expose_interna
+00010c30: 6c73 944e 8c0e 7374 7269 6374 5f76 6973  ls.N..strict_vis
+00010c40: 6974 6f72 944e 8c0f 5f64 6973 6162 6c65  itor.N.._disable
+00010c50: 5f63 6f6e 6669 6794 4e8c 075f 736f 7572  _config.N.._sour
+00010c60: 6365 946a 3503 0000 8c0c 5f64 6573 7469  ce.j5....._desti
+00010c70: 6e61 7469 6f6e 944e 8c0d 5f63 6f6e 6669  nation.N.._confi
+00010c80: 675f 6669 6c65 7394 5d94 6af1 0200 0088  g_files.].j.....
+00010c90: 8c0b 7261 775f 656e 6162 6c65 6494 4b01  ..raw_enabled.K.
+00010ca0: 8c11 6c69 6e65 5f6c 656e 6774 685f 6c69  ..line_length_li
+00010cb0: 6d69 7494 4d10 276a e802 0000 4e6a e602  mit.M.'j....Nj..
+00010cc0: 0000 6ae7 0200 008c 1570 6570 5f66 696c  ..j......pep_fil
+00010cd0: 655f 7572 6c5f 7465 6d70 6c61 7465 948c  e_url_template..
+00010ce0: 0870 6570 2d25 3034 6494 6aeb 0200 004e  .pep-%04d.j....N
+00010cf0: 6ae9 0200 006a ea02 0000 8c09 7461 625f  j....j......tab_
+00010d00: 7769 6474 6894 4b08 6893 898c 1073 796e  width.K.h....syn
+00010d10: 7461 785f 6869 6768 6c69 6768 7494 8c04  tax_highlight...
+00010d20: 6c6f 6e67 946a f502 0000 886a f202 0000  long.j.....j....
+00010d30: 6af3 0200 008c 1d63 6861 7261 6374 6572  j......character
+00010d40: 5f6c 6576 656c 5f69 6e6c 696e 655f 6d61  _level_inline_ma
+00010d50: 726b 7570 9489 6aed 0200 0089 8c0d 646f  rkup..j.......do
+00010d60: 6369 6e66 6f5f 7866 6f72 6d94 4b01 6aee  cinfo_xform.K.j.
+00010d70: 0200 0089 6ae2 0200 006a e302 0000 6ae4  ....j....j....j.
+00010d80: 0200 0089 6ae5 0200 0088 6aef 0200 0089  ....j.....j.....
+00010d90: 685a 4e75 628c 0872 6570 6f72 7465 7294  hZNub..reporter.
+00010da0: 4e8c 1069 6e64 6972 6563 745f 7461 7267  N..indirect_targ
+00010db0: 6574 7394 5d94 8c11 7375 6273 7469 7475  ets.]...substitu
+00010dc0: 7469 6f6e 5f64 6566 7394 7d94 8c12 7375  tion_defs.}...su
+00010dd0: 6273 7469 7475 7469 6f6e 5f6e 616d 6573  bstitution_names
+00010de0: 947d 948c 0872 6566 6e61 6d65 7394 7d94  .}...refnames.}.
+00010df0: 8c06 7265 6669 6473 947d 948c 076e 616d  ..refids.}...nam
+00010e00: 6569 6473 947d 9428 6aa3 0d00 006a a00d  eids.}.(j....j..
+00010e10: 0000 6ae9 0300 006a e603 0000 6abb 0300  ..j....j....j...
+00010e20: 006a b803 0000 6a9b 0400 006a 9804 0000  .j....j....j....
+00010e30: 6a8c 0400 006a 8904 0000 6a8b 0c00 006a  j....j....j....j
+00010e40: 880c 0000 6a6c 0500 006a 6905 0000 6a59  ....jl...ji...jY
+00010e50: 0500 006a 5605 0000 6a29 0600 006a 2606  ...jV...j)...j&.
+00010e60: 0000 6a98 0b00 006a 950b 0000 6a3b 0800  ..j....j....j;..
+00010e70: 006a 3808 0000 6a09 0800 006a 0608 0000  .j8...j....j....
+00010e80: 6a6f 0900 006a 6c09 0000 6ae6 0900 006a  jo...jl...j....j
+00010e90: e309 0000 6a5d 0a00 006a 5a0a 0000 6aa2  ....j]...jZ...j.
+00010ea0: 0a00 006a 9f0a 0000 6a90 0b00 006a 8d0b  ...j....j....j..
+00010eb0: 0000 6a83 0c00 006a 800c 0000 6a42 0c00  ..j....j....jB..
+00010ec0: 006a 3f0c 0000 6a7b 0c00 006a 780c 0000  .j?...j{...jx...
+00010ed0: 6a0a 0d00 006a 070d 0000 6a9b 0d00 006a  j....j....j....j
+00010ee0: 980d 0000 758c 096e 616d 6574 7970 6573  ....u..nametypes
+00010ef0: 947d 9428 6aa3 0d00 0089 6ae9 0300 0089  .}.(j.....j.....
+00010f00: 6abb 0300 0088 6a9b 0400 0089 6a8c 0400  j.....j.....j...
+00010f10: 0088 6a8b 0c00 0089 6a6c 0500 0089 6a59  ..j.....jl....jY
+00010f20: 0500 0088 6a29 0600 0089 6a98 0b00 0089  ....j)....j.....
+00010f30: 6a3b 0800 0089 6a09 0800 0088 6a6f 0900  j;....j.....jo..
+00010f40: 0089 6ae6 0900 0089 6a5d 0a00 0089 6aa2  ..j.....j]....j.
+00010f50: 0a00 0089 6a90 0b00 0089 6a83 0c00 0089  ....j.....j.....
+00010f60: 6a42 0c00 0089 6a7b 0c00 0089 6a0a 0d00  jB....j{....j...
+00010f70: 0089 6a9b 0d00 0089 756a 2603 0000 7d94  ..j.....uj&...}.
+00010f80: 286a a00d 0000 6a38 0300 006a e603 0000  (j....j8...j....
+00010f90: 6a4b 0300 006a b803 0000 6ab2 0300 006a  jK...j....j....j
+00010fa0: 9804 0000 6aec 0300 006a 8904 0000 6a83  ....j....j....j.
+00010fb0: 0400 006a 880c 0000 6a9e 0400 006a 6905  ...j....j....ji.
+00010fc0: 0000 6af6 0400 006a 5605 0000 6a50 0500  ..j....jV...jP..
+00010fd0: 006a 2606 0000 6a6f 0500 006a 950b 0000  .j&...jo...j....
+00010fe0: 6a2c 0600 006a 3808 0000 6a13 0700 006a  j,...j8...j....j
+00010ff0: 0608 0000 6a00 0800 006a 6c09 0000 6a3e  ....j....jl...j>
+00011000: 0800 006a e309 0000 6a72 0900 006a 5a0a  ...j....jr...jZ.
+00011010: 0000 6ae9 0900 006a 9f0a 0000 6a60 0a00  ..j....j....j`..
+00011020: 006a 8d0b 0000 6aa5 0a00 006a 800c 0000  .j....j....j....
+00011030: 6a9b 0b00 006a 3f0c 0000 6aec 0b00 006a  j....j?...j....j
+00011040: 780c 0000 6a45 0c00 006a 070d 0000 6a8e  x...jE...j....j.
+00011050: 0c00 006a 980d 0000 6a0d 0d00 0075 8c0d  ...j....j....u..
+00011060: 666f 6f74 6e6f 7465 5f72 6566 7394 7d94  footnote_refs.}.
+00011070: 8c0d 6369 7461 7469 6f6e 5f72 6566 7394  ..citation_refs.
+00011080: 7d94 8c0d 6175 746f 666f 6f74 6e6f 7465  }...autofootnote
+00011090: 7394 5d94 8c11 6175 746f 666f 6f74 6e6f  s.]...autofootno
+000110a0: 7465 5f72 6566 7394 5d94 8c10 7379 6d62  te_refs.]...symb
+000110b0: 6f6c 5f66 6f6f 746e 6f74 6573 945d 948c  ol_footnotes.]..
+000110c0: 1473 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
+000110d0: 5f72 6566 7394 5d94 8c09 666f 6f74 6e6f  _refs.]...footno
+000110e0: 7465 7394 5d94 8c09 6369 7461 7469 6f6e  tes.]...citation
+000110f0: 7394 5d94 8c12 6175 746f 666f 6f74 6e6f  s.]...autofootno
+00011100: 7465 5f73 7461 7274 944b 018c 1573 796d  te_start.K...sym
+00011110: 626f 6c5f 666f 6f74 6e6f 7465 5f73 7461  bol_footnote_sta
+00011120: 7274 944b 008c 0a69 645f 636f 756e 7465  rt.K...id_counte
+00011130: 7294 6af9 0200 008c 0743 6f75 6e74 6572  r.j......Counter
+00011140: 9493 947d 9485 9452 948c 0e70 6172 7365  ...}...R...parse
+00011150: 5f6d 6573 7361 6765 7394 5d94 8c12 7472  _messages.]...tr
+00011160: 616e 7366 6f72 6d5f 6d65 7373 6167 6573  ansform_messages
+00011170: 945d 948c 0b74 7261 6e73 666f 726d 6572  .]...transformer
+00011180: 944e 8c0b 696e 636c 7564 655f 6c6f 6794  .N..include_log.
+00011190: 5d94 8c09 696e 6465 782e 7273 7494 284e  ]...index.rst.(N
+000111a0: 4e4e 4e74 9486 9461 8c0a 6465 636f 7261  NNNt...a..decora
+000111b0: 7469 6f6e 944e 6a33 0300 006a 1103 0000  tion.Nj3...j....
+000111c0: 7562 738c 086d 6574 6164 6174 6194 6afb  ubs..metadata.j.
+000111d0: 0200 006a fc02 0000 8c04 6469 6374 9493  ...j......dict..
+000111e0: 9485 9452 948c 0674 6974 6c65 7394 7d94  ...R...titles.}.
+000111f0: 6acd 0200 006a 3c03 0000 2981 947d 9428  j....j<...)..}.(
+00011200: 6a13 0300 0068 5e6a 1403 0000 5d94 6a1e  j....h^j....].j.
+00011210: 0300 008c 0757 656c 636f 6d65 9485 9481  .....Welcome....
+00011220: 947d 946a 2303 0000 6a1d 0e00 0073 6261  .}.j#...j....sba
+00011230: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+00011240: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+00011250: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+00011260: 006a 3b03 0000 7562 738c 0a6c 6f6e 6774  .j;...ubs..longt
+00011270: 6974 6c65 7394 7d94 6acd 0200 006a 1d0e  itles.}.j....j..
+00011280: 0000 738c 0474 6f63 7394 7d94 6acd 0200  ..s..tocs.}.j...
+00011290: 006a 1603 0000 8c0b 6275 6c6c 6574 5f6c  .j......bullet_l
+000112a0: 6973 7494 9394 2981 947d 9428 6a13 0300  ist...)..}.(j...
+000112b0: 0068 5e6a 1403 0000 5d94 6a16 0300 008c  .h^j....].j.....
+000112c0: 096c 6973 745f 6974 656d 9493 9429 8194  .list_item...)..
+000112d0: 7d94 286a 1303 0000 685e 6a14 0300 005d  }.(j....h^j....]
+000112e0: 9428 6a0e 0300 008c 1163 6f6d 7061 6374  .(j......compact
+000112f0: 5f70 6172 6167 7261 7068 9493 9429 8194  _paragraph...)..
+00011300: 7d94 286a 1303 0000 685e 6a14 0300 005d  }.(j....h^j....]
+00011310: 946a 9e03 0000 2981 947d 9428 6a13 0300  .j....)..}.(j...
+00011320: 0068 5e6a 1403 0000 5d94 6a1e 0300 008c  .h^j....].j.....
+00011330: 0757 656c 636f 6d65 9485 9481 947d 946a  .Welcome.....}.j
+00011340: 2303 0000 6a3d 0e00 0073 6261 6a24 0300  #...j=...sbaj$..
+00011350: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
+00011360: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
+00011370: 6a2e 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
+00011380: 6c94 888c 0672 6566 7572 6994 6acd 0200  l....refuri.j...
+00011390: 008c 0a61 6e63 686f 726e 616d 6594 685e  ...anchorname.h^
+000113a0: 756a 3203 0000 6a9d 0300 006a 2303 0000  uj2...j....j#...
+000113b0: 6a3a 0e00 0075 6261 6a24 0300 007d 9428  j:...ubaj$...}.(
+000113c0: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
+000113d0: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
+000113e0: 005d 9475 6a32 0300 006a 380e 0000 6a23  .].uj2...j8...j#
+000113f0: 0300 006a 350e 0000 7562 6a2f 0e00 0029  ...j5...ubj/...)
+00011400: 8194 7d94 286a 1303 0000 685e 6a14 0300  ..}.(j....h^j...
+00011410: 005d 9428 6a34 0e00 0029 8194 7d94 286a  .].(j4...)..}.(j
+00011420: 1303 0000 685e 6a14 0300 005d 946a 390e  ....h^j....].j9.
+00011430: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
+00011440: 1403 0000 5d94 6a9e 0300 0029 8194 7d94  ....].j....)..}.
+00011450: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
+00011460: 1e03 0000 8c0c 496e 7472 6f64 7563 7469  ......Introducti
+00011470: 6f6e 9485 9481 947d 946a 2303 0000 6a5c  on.....}.j#...j\
+00011480: 0e00 0073 6261 6a24 0300 007d 9428 6a26  ...sbaj$...}.(j&
+00011490: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
+000114a0: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
+000114b0: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
+000114c0: 6566 7572 6994 6acd 0200 008c 0a61 6e63  efuri.j......anc
+000114d0: 686f 726e 616d 6594 8c0d 2369 6e74 726f  horname...#intro
+000114e0: 6475 6374 696f 6e94 756a 3203 0000 6a9d  duction.uj2...j.
+000114f0: 0300 006a 2303 0000 6a59 0e00 0075 6261  ...j#...jY...uba
+00011500: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+00011510: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+00011520: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+00011530: 006a 380e 0000 6a23 0300 006a 560e 0000  .j8...j#...jV...
+00011540: 7562 616a 2403 0000 7d94 286a 2603 0000  ubaj$...}.(j&...
+00011550: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
+00011560: 6a2c 0300 005d 946a 2e03 0000 5d94 756a  j,...].j....].uj
+00011570: 3203 0000 6a33 0e00 006a 2303 0000 6a53  2...j3...j#...jS
+00011580: 0e00 0075 626a 340e 0000 2981 947d 9428  ...ubj4...)..}.(
+00011590: 6a13 0300 0068 5e6a 1403 0000 5d94 6a39  j....h^j....].j9
+000115a0: 0e00 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
+000115b0: 6a14 0300 005d 946a 9e03 0000 2981 947d  j....].j....)..}
+000115c0: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
+000115d0: 6a1e 0300 008c 0c43 6f6e 7472 6962 7574  j......Contribut
+000115e0: 696f 6e94 8594 8194 7d94 6a23 0300 006a  ion.....}.j#...j
+000115f0: 7f0e 0000 7362 616a 2403 0000 7d94 286a  ....sbaj$...}.(j
+00011600: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
+00011610: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
+00011620: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
+00011630: 7265 6675 7269 946a cd02 0000 8c0a 616e  refuri.j......an
+00011640: 6368 6f72 6e61 6d65 948c 0d23 636f 6e74  chorname...#cont
+00011650: 7269 6275 7469 6f6e 9475 6a32 0300 006a  ribution.uj2...j
+00011660: 9d03 0000 6a23 0300 006a 7c0e 0000 7562  ....j#...j|...ub
+00011670: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
+00011680: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
+00011690: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
+000116a0: 0000 6a38 0e00 006a 2303 0000 6a79 0e00  ..j8...j#...jy..
+000116b0: 0075 6261 6a24 0300 007d 9428 6a26 0300  .ubaj$...}.(j&..
+000116c0: 005d 946a 2803 0000 5d94 6a2a 0300 005d  .].j(...].j*...]
+000116d0: 946a 2c03 0000 5d94 6a2e 0300 005d 9475  .j,...].j....].u
+000116e0: 6a32 0300 006a 330e 0000 6a23 0300 006a  j2...j3...j#...j
+000116f0: 530e 0000 7562 6a34 0e00 0029 8194 7d94  S...ubj4...)..}.
+00011700: 286a 1303 0000 685e 6a14 0300 005d 9428  (j....h^j....].(
+00011710: 6a39 0e00 0029 8194 7d94 286a 1303 0000  j9...)..}.(j....
+00011720: 685e 6a14 0300 005d 946a 9e03 0000 2981  h^j....].j....).
+00011730: 947d 9428 6a13 0300 0068 5e6a 1403 0000  .}.(j....h^j....
+00011740: 5d94 6a1e 0300 008c 0b47 6574 2073 7461  ].j......Get sta
+00011750: 7274 6564 9485 9481 947d 946a 2303 0000  rted.....}.j#...
+00011760: 6aa2 0e00 0073 6261 6a24 0300 007d 9428  j....sbaj$...}.(
+00011770: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
+00011780: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
+00011790: 005d 948c 0869 6e74 6572 6e61 6c94 888c  .]...internal...
+000117a0: 0672 6566 7572 6994 6acd 0200 008c 0a61  .refuri.j......a
+000117b0: 6e63 686f 726e 616d 6594 8c0c 2367 6574  nchorname...#get
+000117c0: 2d73 7461 7274 6564 9475 6a32 0300 006a  -started.uj2...j
+000117d0: 9d03 0000 6a23 0300 006a 9f0e 0000 7562  ....j#...j....ub
+000117e0: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
+000117f0: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
+00011800: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
+00011810: 0000 6a38 0e00 006a 2303 0000 6a9c 0e00  ..j8...j#...j...
+00011820: 0075 626a 2f0e 0000 2981 947d 9428 6a13  .ubj/...)..}.(j.
+00011830: 0300 0068 5e6a 1403 0000 5d94 286a 340e  ...h^j....].(j4.
+00011840: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
+00011850: 1403 0000 5d94 6a39 0e00 0029 8194 7d94  ....].j9...)..}.
+00011860: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
+00011870: 9e03 0000 2981 947d 9428 6a13 0300 0068  ....)..}.(j....h
+00011880: 5e6a 1403 0000 5d94 6a1e 0300 008c 0c49  ^j....].j......I
+00011890: 6e73 7461 6c6c 6174 696f 6e94 8594 8194  nstallation.....
+000118a0: 7d94 6a23 0300 006a c20e 0000 7362 616a  }.j#...j....sbaj
+000118b0: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
+000118c0: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
+000118d0: 005d 946a 2e03 0000 5d94 8c08 696e 7465  .].j....]...inte
+000118e0: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
+000118f0: cd02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00011900: 948c 0d23 696e 7374 616c 6c61 7469 6f6e  ...#installation
+00011910: 9475 6a32 0300 006a 9d03 0000 6a23 0300  .uj2...j....j#..
+00011920: 006a bf0e 0000 7562 616a 2403 0000 7d94  .j....ubaj$...}.
+00011930: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
+00011940: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
+00011950: 0000 5d94 756a 3203 0000 6a38 0e00 006a  ..].uj2...j8...j
+00011960: 2303 0000 6abc 0e00 0075 6261 6a24 0300  #...j....ubaj$..
+00011970: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
+00011980: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
+00011990: 6a2e 0300 005d 9475 6a32 0300 006a 330e  j....].uj2...j3.
+000119a0: 0000 6a23 0300 006a b90e 0000 7562 6a34  ..j#...j....ubj4
+000119b0: 0e00 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
+000119c0: 6a14 0300 005d 946a 390e 0000 2981 947d  j....].j9...)..}
+000119d0: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
+000119e0: 6a9e 0300 0029 8194 7d94 286a 1303 0000  j....)..}.(j....
+000119f0: 685e 6a14 0300 005d 946a 1e03 0000 8c0b  h^j....].j......
+00011a00: 5072 6570 6572 6174 696f 6e94 8594 8194  Preperation.....
+00011a10: 7d94 6a23 0300 006a e50e 0000 7362 616a  }.j#...j....sbaj
+00011a20: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
+00011a30: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
+00011a40: 005d 946a 2e03 0000 5d94 8c08 696e 7465  .].j....]...inte
+00011a50: 726e 616c 9488 8c06 7265 6675 7269 946a  rnal....refuri.j
+00011a60: cd02 0000 8c0a 616e 6368 6f72 6e61 6d65  ......anchorname
+00011a70: 948c 0c23 7072 6570 6572 6174 696f 6e94  ...#preperation.
+00011a80: 756a 3203 0000 6a9d 0300 006a 2303 0000  uj2...j....j#...
+00011a90: 6ae2 0e00 0075 6261 6a24 0300 007d 9428  j....ubaj$...}.(
+00011aa0: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
+00011ab0: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
+00011ac0: 005d 9475 6a32 0300 006a 380e 0000 6a23  .].uj2...j8...j#
+00011ad0: 0300 006a df0e 0000 7562 616a 2403 0000  ...j....ubaj$...
+00011ae0: 7d94 286a 2603 0000 5d94 6a28 0300 005d  }.(j&...].j(...]
+00011af0: 946a 2a03 0000 5d94 6a2c 0300 005d 946a  .j*...].j,...].j
+00011b00: 2e03 0000 5d94 756a 3203 0000 6a33 0e00  ....].uj2...j3..
+00011b10: 006a 2303 0000 6ab9 0e00 0075 626a 340e  .j#...j....ubj4.
+00011b20: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
+00011b30: 1403 0000 5d94 286a 390e 0000 2981 947d  ....].(j9...)..}
+00011b40: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
+00011b50: 6a9e 0300 0029 8194 7d94 286a 1303 0000  j....)..}.(j....
+00011b60: 685e 6a14 0300 005d 946a 1e03 0000 8c05  h^j....].j......
+00011b70: 5573 6167 6594 8594 8194 7d94 6a23 0300  Usage.....}.j#..
+00011b80: 006a 080f 0000 7362 616a 2403 0000 7d94  .j....sbaj$...}.
+00011b90: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
+00011ba0: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
+00011bb0: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
+00011bc0: 8c06 7265 6675 7269 946a cd02 0000 8c0a  ..refuri.j......
+00011bd0: 616e 6368 6f72 6e61 6d65 948c 0623 7573  anchorname...#us
+00011be0: 6167 6594 756a 3203 0000 6a9d 0300 006a  age.uj2...j....j
+00011bf0: 2303 0000 6a05 0f00 0075 6261 6a24 0300  #...j....ubaj$..
+00011c00: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
+00011c10: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
+00011c20: 6a2e 0300 005d 9475 6a32 0300 006a 380e  j....].uj2...j8.
+00011c30: 0000 6a23 0300 006a 020f 0000 7562 6a2f  ..j#...j....ubj/
+00011c40: 0e00 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
+00011c50: 6a14 0300 005d 9428 6a34 0e00 0029 8194  j....].(j4...)..
+00011c60: 7d94 286a 1303 0000 685e 6a14 0300 005d  }.(j....h^j....]
+00011c70: 946a 390e 0000 2981 947d 9428 6a13 0300  .j9...)..}.(j...
+00011c80: 0068 5e6a 1403 0000 5d94 6a9e 0300 0029  .h^j....].j....)
+00011c90: 8194 7d94 286a 1303 0000 685e 6a14 0300  ..}.(j....h^j...
+00011ca0: 005d 946a 1e03 0000 8c05 4d6f 6465 6c94  .].j......Model.
+00011cb0: 8594 8194 7d94 6a23 0300 006a 280f 0000  ....}.j#...j(...
+00011cc0: 7362 616a 2403 0000 7d94 286a 2603 0000  sbaj$...}.(j&...
+00011cd0: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
+00011ce0: 6a2c 0300 005d 946a 2e03 0000 5d94 8c08  j,...].j....]...
+00011cf0: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
+00011d00: 7269 946a cd02 0000 8c0a 616e 6368 6f72  ri.j......anchor
+00011d10: 6e61 6d65 948c 0623 6d6f 6465 6c94 756a  name...#model.uj
+00011d20: 3203 0000 6a9d 0300 006a 2303 0000 6a25  2...j....j#...j%
+00011d30: 0f00 0075 6261 6a24 0300 007d 9428 6a26  ...ubaj$...}.(j&
+00011d40: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
+00011d50: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
+00011d60: 9475 6a32 0300 006a 380e 0000 6a23 0300  .uj2...j8...j#..
+00011d70: 006a 220f 0000 7562 616a 2403 0000 7d94  .j"...ubaj$...}.
+00011d80: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
+00011d90: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
+00011da0: 0000 5d94 756a 3203 0000 6a33 0e00 006a  ..].uj2...j3...j
+00011db0: 2303 0000 6a1f 0f00 0075 626a 340e 0000  #...j....ubj4...
+00011dc0: 2981 947d 9428 6a13 0300 0068 5e6a 1403  )..}.(j....h^j..
+00011dd0: 0000 5d94 6a39 0e00 0029 8194 7d94 286a  ..].j9...)..}.(j
+00011de0: 1303 0000 685e 6a14 0300 005d 946a 9e03  ....h^j....].j..
+00011df0: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
+00011e00: 1403 0000 5d94 6a1e 0300 008c 0442 6173  ....].j......Bas
+00011e10: 6594 8594 8194 7d94 6a23 0300 006a 4b0f  e.....}.j#...jK.
+00011e20: 0000 7362 616a 2403 0000 7d94 286a 2603  ..sbaj$...}.(j&.
+00011e30: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
+00011e40: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
+00011e50: 8c08 696e 7465 726e 616c 9488 8c06 7265  ..internal....re
+00011e60: 6675 7269 946a cd02 0000 8c0a 616e 6368  furi.j......anch
+00011e70: 6f72 6e61 6d65 948c 0523 6261 7365 9475  orname...#base.u
+00011e80: 6a32 0300 006a 9d03 0000 6a23 0300 006a  j2...j....j#...j
+00011e90: 480f 0000 7562 616a 2403 0000 7d94 286a  H...ubaj$...}.(j
+00011ea0: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
+00011eb0: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
+00011ec0: 5d94 756a 3203 0000 6a38 0e00 006a 2303  ].uj2...j8...j#.
+00011ed0: 0000 6a45 0f00 0075 6261 6a24 0300 007d  ..jE...ubaj$...}
+00011ee0: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
+00011ef0: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
+00011f00: 0300 005d 9475 6a32 0300 006a 330e 0000  ...].uj2...j3...
+00011f10: 6a23 0300 006a 1f0f 0000 7562 6a34 0e00  j#...j....ubj4..
+00011f20: 0029 8194 7d94 286a 1303 0000 685e 6a14  .)..}.(j....h^j.
+00011f30: 0300 005d 946a 390e 0000 2981 947d 9428  ...].j9...)..}.(
+00011f40: 6a13 0300 0068 5e6a 1403 0000 5d94 6a9e  j....h^j....].j.
+00011f50: 0300 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
+00011f60: 6a14 0300 005d 946a 1e03 0000 8c04 5669  j....].j......Vi
+00011f70: 6577 9485 9481 947d 946a 2303 0000 6a6e  ew.....}.j#...jn
+00011f80: 0f00 0073 6261 6a24 0300 007d 9428 6a26  ...sbaj$...}.(j&
+00011f90: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
+00011fa0: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
+00011fb0: 948c 0869 6e74 6572 6e61 6c94 888c 0672  ...internal....r
+00011fc0: 6566 7572 6994 6acd 0200 008c 0a61 6e63  efuri.j......anc
+00011fd0: 686f 726e 616d 6594 8c05 2376 6965 7794  horname...#view.
+00011fe0: 756a 3203 0000 6a9d 0300 006a 2303 0000  uj2...j....j#...
+00011ff0: 6a6b 0f00 0075 6261 6a24 0300 007d 9428  jk...ubaj$...}.(
+00012000: 6a26 0300 005d 946a 2803 0000 5d94 6a2a  j&...].j(...].j*
+00012010: 0300 005d 946a 2c03 0000 5d94 6a2e 0300  ...].j,...].j...
+00012020: 005d 9475 6a32 0300 006a 380e 0000 6a23  .].uj2...j8...j#
+00012030: 0300 006a 680f 0000 7562 616a 2403 0000  ...jh...ubaj$...
+00012040: 7d94 286a 2603 0000 5d94 6a28 0300 005d  }.(j&...].j(...]
+00012050: 946a 2a03 0000 5d94 6a2c 0300 005d 946a  .j*...].j,...].j
+00012060: 2e03 0000 5d94 756a 3203 0000 6a33 0e00  ....].uj2...j3..
+00012070: 006a 2303 0000 6a1f 0f00 0075 626a 340e  .j#...j....ubj4.
+00012080: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
+00012090: 1403 0000 5d94 6a39 0e00 0029 8194 7d94  ....].j9...)..}.
+000120a0: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
+000120b0: 9e03 0000 2981 947d 9428 6a13 0300 0068  ....)..}.(j....h
+000120c0: 5e6a 1403 0000 5d94 6a1e 0300 008c 0644  ^j....].j......D
+000120d0: 6961 6c6f 6794 8594 8194 7d94 6a23 0300  ialog.....}.j#..
+000120e0: 006a 910f 0000 7362 616a 2403 0000 7d94  .j....sbaj$...}.
+000120f0: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
+00012100: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
+00012110: 0000 5d94 8c08 696e 7465 726e 616c 9488  ..]...internal..
+00012120: 8c06 7265 6675 7269 946a cd02 0000 8c0a  ..refuri.j......
+00012130: 616e 6368 6f72 6e61 6d65 948c 0723 6469  anchorname...#di
+00012140: 616c 6f67 9475 6a32 0300 006a 9d03 0000  alog.uj2...j....
+00012150: 6a23 0300 006a 8e0f 0000 7562 616a 2403  j#...j....ubaj$.
+00012160: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
+00012170: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
+00012180: 946a 2e03 0000 5d94 756a 3203 0000 6a38  .j....].uj2...j8
+00012190: 0e00 006a 2303 0000 6a8b 0f00 0075 6261  ...j#...j....uba
+000121a0: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+000121b0: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+000121c0: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+000121d0: 006a 330e 0000 6a23 0300 006a 1f0f 0000  .j3...j#...j....
+000121e0: 7562 6a34 0e00 0029 8194 7d94 286a 1303  ubj4...)..}.(j..
+000121f0: 0000 685e 6a14 0300 005d 946a 390e 0000  ..h^j....].j9...
+00012200: 2981 947d 9428 6a13 0300 0068 5e6a 1403  )..}.(j....h^j..
+00012210: 0000 5d94 6a9e 0300 0029 8194 7d94 286a  ..].j....)..}.(j
+00012220: 1303 0000 685e 6a14 0300 005d 946a 1e03  ....h^j....].j..
+00012230: 0000 8c06 5769 6467 6574 9485 9481 947d  ....Widget.....}
+00012240: 946a 2303 0000 6ab4 0f00 0073 6261 6a24  .j#...j....sbaj$
+00012250: 0300 007d 9428 6a26 0300 005d 946a 2803  ...}.(j&...].j(.
+00012260: 0000 5d94 6a2a 0300 005d 946a 2c03 0000  ..].j*...].j,...
+00012270: 5d94 6a2e 0300 005d 948c 0869 6e74 6572  ].j....]...inter
+00012280: 6e61 6c94 888c 0672 6566 7572 6994 6acd  nal....refuri.j.
+00012290: 0200 008c 0a61 6e63 686f 726e 616d 6594  .....anchorname.
+000122a0: 8c07 2377 6964 6765 7494 756a 3203 0000  ..#widget.uj2...
+000122b0: 6a9d 0300 006a 2303 0000 6ab1 0f00 0075  j....j#...j....u
+000122c0: 6261 6a24 0300 007d 9428 6a26 0300 005d  baj$...}.(j&...]
+000122d0: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
+000122e0: 2c03 0000 5d94 6a2e 0300 005d 9475 6a32  ,...].j....].uj2
+000122f0: 0300 006a 380e 0000 6a23 0300 006a ae0f  ...j8...j#...j..
+00012300: 0000 7562 616a 2403 0000 7d94 286a 2603  ..ubaj$...}.(j&.
+00012310: 0000 5d94 6a28 0300 005d 946a 2a03 0000  ..].j(...].j*...
+00012320: 5d94 6a2c 0300 005d 946a 2e03 0000 5d94  ].j,...].j....].
+00012330: 756a 3203 0000 6a33 0e00 006a 2303 0000  uj2...j3...j#...
+00012340: 6a1f 0f00 0075 626a 340e 0000 2981 947d  j....ubj4...)..}
+00012350: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
+00012360: 6a39 0e00 0029 8194 7d94 286a 1303 0000  j9...)..}.(j....
+00012370: 685e 6a14 0300 005d 946a 9e03 0000 2981  h^j....].j....).
+00012380: 947d 9428 6a13 0300 0068 5e6a 1403 0000  .}.(j....h^j....
+00012390: 5d94 6a1e 0300 008c 0641 6374 696f 6e94  ].j......Action.
+000123a0: 8594 8194 7d94 6a23 0300 006a d70f 0000  ....}.j#...j....
+000123b0: 7362 616a 2403 0000 7d94 286a 2603 0000  sbaj$...}.(j&...
+000123c0: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
+000123d0: 6a2c 0300 005d 946a 2e03 0000 5d94 8c08  j,...].j....]...
+000123e0: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
+000123f0: 7269 946a cd02 0000 8c0a 616e 6368 6f72  ri.j......anchor
+00012400: 6e61 6d65 948c 0723 6163 7469 6f6e 9475  name...#action.u
+00012410: 6a32 0300 006a 9d03 0000 6a23 0300 006a  j2...j....j#...j
+00012420: d40f 0000 7562 616a 2403 0000 7d94 286a  ....ubaj$...}.(j
+00012430: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
+00012440: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
+00012450: 5d94 756a 3203 0000 6a38 0e00 006a 2303  ].uj2...j8...j#.
+00012460: 0000 6ad1 0f00 0075 6261 6a24 0300 007d  ..j....ubaj$...}
+00012470: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
+00012480: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
+00012490: 0300 005d 9475 6a32 0300 006a 330e 0000  ...].uj2...j3...
+000124a0: 6a23 0300 006a 1f0f 0000 7562 656a 2403  j#...j....ubej$.
+000124b0: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
+000124c0: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
+000124d0: 946a 2e03 0000 5d94 756a 3203 0000 6a2e  .j....].uj2...j.
+000124e0: 0e00 006a 2303 0000 6a02 0f00 0075 6265  ...j#...j....ube
+000124f0: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+00012500: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+00012510: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+00012520: 006a 330e 0000 6a23 0300 006a b90e 0000  .j3...j#...j....
+00012530: 7562 6a34 0e00 0029 8194 7d94 286a 1303  ubj4...)..}.(j..
+00012540: 0000 685e 6a14 0300 005d 9428 6a39 0e00  ..h^j....].(j9..
+00012550: 0029 8194 7d94 286a 1303 0000 685e 6a14  .)..}.(j....h^j.
+00012560: 0300 005d 946a 9e03 0000 2981 947d 9428  ...].j....)..}.(
+00012570: 6a13 0300 0068 5e6a 1403 0000 5d94 6a1e  j....h^j....].j.
+00012580: 0300 008c 1a52 756e 2c20 4465 7665 6c6f  .....Run, Develo
+00012590: 706d 656e 7420 616e 6420 4275 696c 6494  pment and Build.
+000125a0: 8594 8194 7d94 6a23 0300 006a 0610 0000  ....}.j#...j....
+000125b0: 7362 616a 2403 0000 7d94 286a 2603 0000  sbaj$...}.(j&...
+000125c0: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
+000125d0: 6a2c 0300 005d 946a 2e03 0000 5d94 8c08  j,...].j....]...
+000125e0: 696e 7465 726e 616c 9488 8c06 7265 6675  internal....refu
+000125f0: 7269 946a cd02 0000 8c0a 616e 6368 6f72  ri.j......anchor
+00012600: 6e61 6d65 948c 1a23 7275 6e2d 6465 7665  name...#run-deve
+00012610: 6c6f 706d 656e 742d 616e 642d 6275 696c  lopment-and-buil
+00012620: 6494 756a 3203 0000 6a9d 0300 006a 2303  d.uj2...j....j#.
+00012630: 0000 6a03 1000 0075 6261 6a24 0300 007d  ..j....ubaj$...}
+00012640: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
+00012650: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
+00012660: 0300 005d 9475 6a32 0300 006a 380e 0000  ...].uj2...j8...
+00012670: 6a23 0300 006a 0010 0000 7562 6a2f 0e00  j#...j....ubj/..
+00012680: 0029 8194 7d94 286a 1303 0000 685e 6a14  .)..}.(j....h^j.
+00012690: 0300 005d 9428 6a34 0e00 0029 8194 7d94  ...].(j4...)..}.
+000126a0: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
+000126b0: 390e 0000 2981 947d 9428 6a13 0300 0068  9...)..}.(j....h
+000126c0: 5e6a 1403 0000 5d94 6a9e 0300 0029 8194  ^j....].j....)..
+000126d0: 7d94 286a 1303 0000 685e 6a14 0300 005d  }.(j....h^j....]
+000126e0: 946a 1e03 0000 8c0b 4465 7665 6c6f 706d  .j......Developm
+000126f0: 656e 7494 8594 8194 7d94 6a23 0300 006a  ent.....}.j#...j
+00012700: 2610 0000 7362 616a 2403 0000 7d94 286a  &...sbaj$...}.(j
+00012710: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
+00012720: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
+00012730: 5d94 8c08 696e 7465 726e 616c 9488 8c06  ]...internal....
+00012740: 7265 6675 7269 946a cd02 0000 8c0a 616e  refuri.j......an
+00012750: 6368 6f72 6e61 6d65 948c 0c23 6465 7665  chorname...#deve
+00012760: 6c6f 706d 656e 7494 756a 3203 0000 6a9d  lopment.uj2...j.
+00012770: 0300 006a 2303 0000 6a23 1000 0075 6261  ...j#...j#...uba
+00012780: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+00012790: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+000127a0: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+000127b0: 006a 380e 0000 6a23 0300 006a 2010 0000  .j8...j#...j ...
+000127c0: 7562 616a 2403 0000 7d94 286a 2603 0000  ubaj$...}.(j&...
+000127d0: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
+000127e0: 6a2c 0300 005d 946a 2e03 0000 5d94 756a  j,...].j....].uj
+000127f0: 3203 0000 6a33 0e00 006a 2303 0000 6a1d  2...j3...j#...j.
+00012800: 1000 0075 626a 340e 0000 2981 947d 9428  ...ubj4...)..}.(
+00012810: 6a13 0300 0068 5e6a 1403 0000 5d94 6a39  j....h^j....].j9
+00012820: 0e00 0029 8194 7d94 286a 1303 0000 685e  ...)..}.(j....h^
+00012830: 6a14 0300 005d 946a 9e03 0000 2981 947d  j....].j....)..}
+00012840: 9428 6a13 0300 0068 5e6a 1403 0000 5d94  .(j....h^j....].
+00012850: 6a1e 0300 008c 0542 7569 6c64 9485 9481  j......Build....
+00012860: 947d 946a 2303 0000 6a49 1000 0073 6261  .}.j#...jI...sba
+00012870: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+00012880: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+00012890: 0000 5d94 6a2e 0300 005d 948c 0869 6e74  ..].j....]...int
+000128a0: 6572 6e61 6c94 888c 0672 6566 7572 6994  ernal....refuri.
+000128b0: 6acd 0200 008c 0a61 6e63 686f 726e 616d  j......anchornam
+000128c0: 6594 8c06 2362 7569 6c64 9475 6a32 0300  e...#build.uj2..
+000128d0: 006a 9d03 0000 6a23 0300 006a 4610 0000  .j....j#...jF...
+000128e0: 7562 616a 2403 0000 7d94 286a 2603 0000  ubaj$...}.(j&...
+000128f0: 5d94 6a28 0300 005d 946a 2a03 0000 5d94  ].j(...].j*...].
+00012900: 6a2c 0300 005d 946a 2e03 0000 5d94 756a  j,...].j....].uj
+00012910: 3203 0000 6a38 0e00 006a 2303 0000 6a43  2...j8...j#...jC
+00012920: 1000 0075 6261 6a24 0300 007d 9428 6a26  ...ubaj$...}.(j&
+00012930: 0300 005d 946a 2803 0000 5d94 6a2a 0300  ...].j(...].j*..
+00012940: 005d 946a 2c03 0000 5d94 6a2e 0300 005d  .].j,...].j....]
+00012950: 9475 6a32 0300 006a 330e 0000 6a23 0300  .uj2...j3...j#..
+00012960: 006a 1d10 0000 7562 656a 2403 0000 7d94  .j....ubej$...}.
+00012970: 286a 2603 0000 5d94 6a28 0300 005d 946a  (j&...].j(...].j
+00012980: 2a03 0000 5d94 6a2c 0300 005d 946a 2e03  *...].j,...].j..
+00012990: 0000 5d94 756a 3203 0000 6a2e 0e00 006a  ..].uj2...j....j
+000129a0: 2303 0000 6a00 1000 0075 6265 6a24 0300  #...j....ubej$..
+000129b0: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
+000129c0: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
+000129d0: 6a2e 0300 005d 9475 6a32 0300 006a 330e  j....].uj2...j3.
+000129e0: 0000 6a23 0300 006a b90e 0000 7562 656a  ..j#...j....ubej
+000129f0: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
+00012a00: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
+00012a10: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
+00012a20: 6a2e 0e00 006a 2303 0000 6a9c 0e00 0075  j....j#...j....u
+00012a30: 6265 6a24 0300 007d 9428 6a26 0300 005d  bej$...}.(j&...]
+00012a40: 946a 2803 0000 5d94 6a2a 0300 005d 946a  .j(...].j*...].j
+00012a50: 2c03 0000 5d94 6a2e 0300 005d 9475 6a32  ,...].j....].uj2
+00012a60: 0300 006a 330e 0000 6a23 0300 006a 530e  ...j3...j#...jS.
+00012a70: 0000 7562 6a34 0e00 0029 8194 7d94 286a  ..ubj4...)..}.(j
+00012a80: 1303 0000 685e 6a14 0300 005d 946a 390e  ....h^j....].j9.
+00012a90: 0000 2981 947d 9428 6a13 0300 0068 5e6a  ..)..}.(j....h^j
+00012aa0: 1403 0000 5d94 6a9e 0300 0029 8194 7d94  ....].j....)..}.
+00012ab0: 286a 1303 0000 685e 6a14 0300 005d 946a  (j....h^j....].j
+00012ac0: 1e03 0000 8c12 5361 6d70 6c65 2061 7070  ......Sample app
+00012ad0: 6c69 6361 7469 6f6e 9485 9481 947d 946a  lication.....}.j
+00012ae0: 2303 0000 6a84 1000 0073 6261 6a24 0300  #...j....sbaj$..
+00012af0: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
+00012b00: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
+00012b10: 6a2e 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
+00012b20: 6c94 888c 0672 6566 7572 6994 6acd 0200  l....refuri.j...
+00012b30: 008c 0a61 6e63 686f 726e 616d 6594 8c13  ...anchorname...
+00012b40: 2373 616d 706c 652d 6170 706c 6963 6174  #sample-applicat
+00012b50: 696f 6e94 756a 3203 0000 6a9d 0300 006a  ion.uj2...j....j
+00012b60: 2303 0000 6a81 1000 0075 6261 6a24 0300  #...j....ubaj$..
+00012b70: 007d 9428 6a26 0300 005d 946a 2803 0000  .}.(j&...].j(...
+00012b80: 5d94 6a2a 0300 005d 946a 2c03 0000 5d94  ].j*...].j,...].
+00012b90: 6a2e 0300 005d 9475 6a32 0300 006a 380e  j....].uj2...j8.
+00012ba0: 0000 6a23 0300 006a 7e10 0000 7562 616a  ..j#...j~...ubaj
+00012bb0: 2403 0000 7d94 286a 2603 0000 5d94 6a28  $...}.(j&...].j(
+00012bc0: 0300 005d 946a 2a03 0000 5d94 6a2c 0300  ...].j*...].j,..
+00012bd0: 005d 946a 2e03 0000 5d94 756a 3203 0000  .].j....].uj2...
+00012be0: 6a33 0e00 006a 2303 0000 6a53 0e00 0075  j3...j#...jS...u
+00012bf0: 626a 340e 0000 2981 947d 9428 6a13 0300  bj4...)..}.(j...
+00012c00: 0068 5e6a 1403 0000 5d94 286a 390e 0000  .h^j....].(j9...
+00012c10: 2981 947d 9428 6a13 0300 0068 5e6a 1403  )..}.(j....h^j..
+00012c20: 0000 5d94 6a9e 0300 0029 8194 7d94 286a  ..].j....)..}.(j
+00012c30: 1303 0000 685e 6a14 0300 005d 946a 1e03  ....h^j....].j..
+00012c40: 0000 8c05 4e6f 7465 7394 8594 8194 7d94  ....Notes.....}.
+00012c50: 6a23 0300 006a a710 0000 7362 616a 2403  j#...j....sbaj$.
+00012c60: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
+00012c70: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
+00012c80: 946a 2e03 0000 5d94 8c08 696e 7465 726e  .j....]...intern
+00012c90: 616c 9488 8c06 7265 6675 7269 946a cd02  al....refuri.j..
+00012ca0: 0000 8c0a 616e 6368 6f72 6e61 6d65 948c  ....anchorname..
+00012cb0: 0623 6e6f 7465 7394 756a 3203 0000 6a9d  .#notes.uj2...j.
+00012cc0: 0300 006a 2303 0000 6aa4 1000 0075 6261  ...j#...j....uba
+00012cd0: 6a24 0300 007d 9428 6a26 0300 005d 946a  j$...}.(j&...].j
+00012ce0: 2803 0000 5d94 6a2a 0300 005d 946a 2c03  (...].j*...].j,.
+00012cf0: 0000 5d94 6a2e 0300 005d 9475 6a32 0300  ..].j....].uj2..
+00012d00: 006a 380e 0000 6a23 0300 006a a110 0000  .j8...j#...j....
+00012d10: 7562 6a2f 0e00 0029 8194 7d94 286a 1303  ubj/...)..}.(j..
+00012d20: 0000 685e 6a14 0300 005d 946a 320d 0000  ..h^j....].j2...
+00012d30: 2981 947d 9428 6a13 0300 0068 5e6a 1403  )..}.(j....h^j..
+00012d40: 0000 5d94 6a24 0300 007d 9428 6a26 0300  ..].j$...}.(j&..
+00012d50: 005d 946a 2803 0000 5d94 6a2a 0300 005d  .].j(...].j*...]
+00012d60: 946a 2c03 0000 5d94 6a2e 0300 005d 948c  .j,...].j....]..
+00012d70: 0670 6172 656e 7494 6acd 0200 008c 0765  .parent.j......e
+00012d80: 6e74 7269 6573 946a 3d0d 0000 8c0c 696e  ntries.j=.....in
+00012d90: 636c 7564 6566 696c 6573 946a 3f0d 0000  cludefiles.j?...
+00012da0: 8c08 6d61 7864 6570 7468 944b 028c 0763  ..maxdepth.K...c
+00012db0: 6170 7469 6f6e 944e 8c04 676c 6f62 9489  aption.N..glob..
+00012dc0: 8c06 6869 6464 656e 9488 8c0d 696e 636c  ..hidden....incl
+00012dd0: 7564 6568 6964 6465 6e94 898c 086e 756d  udehidden....num
+00012de0: 6265 7265 6494 4b00 8c0a 7469 746c 6573  bered.K...titles
+00012df0: 6f6e 6c79 9489 8c0a 7261 7765 6e74 7269  only....rawentri
+00012e00: 6573 946a 480d 0000 756a 3203 0000 6a31  es.jH...uj2...j1
+00012e10: 0d00 006a 3403 0000 6a35 0300 006a 3603  ...j4...j5...j6.
+00012e20: 0000 4b0b 6a23 0300 006a be10 0000 7562  ..K.j#...j....ub
+00012e30: 616a 2403 0000 7d94 286a 2603 0000 5d94  aj$...}.(j&...].
+00012e40: 6a28 0300 005d 946a 2a03 0000 5d94 6a2c  j(...].j*...].j,
+00012e50: 0300 005d 946a 2e03 0000 5d94 756a 3203  ...].j....].uj2.
+00012e60: 0000 6a2e 0e00 006a 2303 0000 6aa1 1000  ..j....j#...j...
+00012e70: 0075 6265 6a24 0300 007d 9428 6a26 0300  .ubej$...}.(j&..
+00012e80: 005d 946a 2803 0000 5d94 6a2a 0300 005d  .].j(...].j*...]
+00012e90: 946a 2c03 0000 5d94 6a2e 0300 005d 9475  .j,...].j....].u
+00012ea0: 6a32 0300 006a 330e 0000 6a23 0300 006a  j2...j3...j#...j
+00012eb0: 530e 0000 7562 656a 2403 0000 7d94 286a  S...ubej$...}.(j
+00012ec0: 2603 0000 5d94 6a28 0300 005d 946a 2a03  &...].j(...].j*.
+00012ed0: 0000 5d94 6a2c 0300 005d 946a 2e03 0000  ..].j,...].j....
+00012ee0: 5d94 756a 3203 0000 6a2e 0e00 006a 2303  ].uj2...j....j#.
+00012ef0: 0000 6a35 0e00 0075 6265 6a24 0300 007d  ..j5...ubej$...}
+00012f00: 9428 6a26 0300 005d 946a 2803 0000 5d94  .(j&...].j(...].
+00012f10: 6a2a 0300 005d 946a 2c03 0000 5d94 6a2e  j*...].j,...].j.
+00012f20: 0300 005d 9475 6a32 0300 006a 330e 0000  ...].uj2...j3...
+00012f30: 6a23 0300 006a 300e 0000 7562 616a 2403  j#...j0...ubaj$.
+00012f40: 0000 7d94 286a 2603 0000 5d94 6a28 0300  ..}.(j&...].j(..
+00012f50: 005d 946a 2a03 0000 5d94 6a2c 0300 005d  .].j*...].j,...]
+00012f60: 946a 2e03 0000 5d94 756a 3203 0000 6a2e  .j....].uj2...j.
+00012f70: 0e00 0075 6273 8c0f 746f 635f 6e75 6d5f  ...ubs..toc_num_
+00012f80: 656e 7472 6965 7394 7d94 6acd 0200 004b  entries.}.j....K
+00012f90: 1273 8c0e 746f 635f 7365 636e 756d 6265  .s..toc_secnumbe
+00012fa0: 7273 947d 948c 0e74 6f63 5f66 6967 6e75  rs.}...toc_fignu
+00012fb0: 6d62 6572 7394 7d94 8c10 746f 6374 7265  mbers.}...toctre
+00012fc0: 655f 696e 636c 7564 6573 947d 946a cd02  e_includes.}.j..
+00012fd0: 0000 5d94 738c 1066 696c 6573 5f74 6f5f  ..].s..files_to_
+00012fe0: 7265 6275 696c 6494 7d94 8c0d 676c 6f62  rebuild.}...glob
+00012ff0: 5f74 6f63 7472 6565 7394 8f94 8c11 6e75  _toctrees.....nu
+00013000: 6d62 6572 6564 5f74 6f63 7472 6565 7394  mbered_toctrees.
+00013010: 8f94 8c0a 646f 6d61 696e 6461 7461 947d  ....domaindata.}
+00013020: 9428 8c01 6394 7d94 288c 0b72 6f6f 745f  .(..c.}.(..root_
+00013030: 7379 6d62 6f6c 946a cf02 0000 8c06 5379  symbol.j......Sy
+00013040: 6d62 6f6c 9493 9429 8194 7d94 286a 2303  mbol...)..}.(j#.
+00013050: 0000 4e8c 0c73 6962 6c69 6e67 4162 6f76  ..N..siblingAbov
+00013060: 6594 4e8c 0c73 6962 6c69 6e67 4265 6c6f  e.N..siblingBelo
+00013070: 7794 4e8c 0569 6465 6e74 944e 8c0b 6465  w.N..ident.N..de
+00013080: 636c 6172 6174 696f 6e94 4e8c 0764 6f63  claration.N..doc
+00013090: 6e61 6d65 944e 6a36 0300 004e 8c0f 6973  name.Nj6...N..is
+000130a0: 5265 6465 636c 6172 6174 696f 6e94 898c  Redeclaration...
+000130b0: 095f 6368 696c 6472 656e 945d 948c 0d5f  ._children.]..._
+000130c0: 616e 6f6e 4368 696c 6472 656e 945d 9475  anonChildren.].u
+000130d0: 628c 076f 626a 6563 7473 947d 9468 624b  b..objects.}.hbK
+000130e0: 0075 8c09 6368 616e 6765 7365 7494 7d94  .u..changeset.}.
+000130f0: 288c 0763 6861 6e67 6573 947d 9468 624b  (..changes.}.hbK
+00013100: 0075 8c08 6369 7461 7469 6f6e 947d 9428  .u..citation.}.(
+00013110: 6862 4b00 6a01 0e00 007d 946a f50d 0000  hbK.j....}.j....
+00013120: 7d94 758c 0363 7070 947d 9428 6a06 1100  }.u..cpp.}.(j...
+00013130: 006a d202 0000 6a07 1100 0093 9429 8194  .j....j......)..
+00013140: 7d94 286a 2303 0000 4e6a 0b11 0000 4e6a  }.(j#...Nj....Nj
+00013150: 0c11 0000 4e8c 0969 6465 6e74 4f72 4f70  ....N..identOrOp
+00013160: 944e 8c0e 7465 6d70 6c61 7465 5061 7261  .N..templatePara
+00013170: 6d73 944e 8c0c 7465 6d70 6c61 7465 4172  ms.N..templateAr
+00013180: 6773 944e 6a0e 1100 004e 6a0f 1100 004e  gs.Nj....Nj....N
+00013190: 6a36 0300 004e 6a10 1100 0089 6a11 1100  j6...Nj.....j...
+000131a0: 005d 946a 1311 0000 5d94 7562 6a2a 0300  .].j....].ubj*..
+000131b0: 007d 9468 624b 0075 6877 7d94 2868 624b  .}.hbK.uhw}.(hbK
+000131c0: 006a 3c0d 0000 7d94 6acd 0200 005d 9473  .j<...}.j....].s
+000131d0: 758c 026a 7394 7d94 286a 1511 0000 7d94  u..js.}.(j....}.
+000131e0: 8c07 6d6f 6475 6c65 7394 7d94 6862 4b00  ..modules.}.hbK.
+000131f0: 758c 046d 6174 6894 7d94 286a 1511 0000  u..math.}.(j....
+00013200: 7d94 8c0d 6861 735f 6571 7561 7469 6f6e  }...has_equation
+00013210: 7394 7d94 6acd 0200 0089 7368 624b 0075  s.}.j.....shbK.u
+00013220: 68b1 7d94 286a 1511 0000 7d94 6a30 1100  h.}.(j....}.j0..
+00013230: 007d 9468 624b 0075 8c03 7273 7494 7d94  .}.hbK.u..rst.}.
+00013240: 286a 1511 0000 7d94 6862 4b00 758c 0373  (j....}.hbK.u..s
+00013250: 7464 947d 9428 8c0b 7072 6f67 6f70 7469  td.}.(..progopti
+00013260: 6f6e 7394 7d94 6a15 1100 007d 948c 066c  ons.}.j....}...l
+00013270: 6162 656c 7394 7d94 288c 0867 656e 696e  abels.}.(..genin
+00013280: 6465 7894 6a44 1100 0068 5e8c 0d73 7068  dex.jD...h^..sph
+00013290: 696e 782e 6c6f 6361 6c65 948c 115f 5472  inx.locale..._Tr
+000132a0: 616e 736c 6174 696f 6e50 726f 7879 9493  anslationProxy..
+000132b0: 9429 8194 6ad9 0200 008c 0767 656e 6572  .)..j......gener
+000132c0: 616c 948c 0549 6e64 6578 9487 9462 8794  al...Index...b..
+000132d0: 8c08 6d6f 6469 6e64 6578 948c 0b70 792d  ..modindex...py-
+000132e0: 6d6f 6469 6e64 6578 9468 5e6a 4711 0000  modindex.h^jG...
+000132f0: 2981 946a d902 0000 6a49 1100 008c 0c4d  )..j....jI.....M
+00013300: 6f64 756c 6520 496e 6465 7894 8794 6287  odule Index...b.
+00013310: 948c 0673 6561 7263 6894 6a53 1100 0068  ...search.jS...h
+00013320: 5e6a 4711 0000 2981 946a d902 0000 6a49  ^jG...)..j....jI
+00013330: 1100 008c 0b53 6561 7263 6820 5061 6765  .....Search Page
+00013340: 9487 9462 8794 8c0b 7079 2d6d 6f64 696e  ...b....py-modin
+00013350: 6465 7894 6a58 1100 0068 5e8c 1350 7974  dex.jX...h^..Pyt
+00013360: 686f 6e20 4d6f 6475 6c65 2049 6e64 6578  hon Module Index
+00013370: 9487 9475 8c0a 616e 6f6e 6c61 6265 6c73  ...u..anonlabels
+00013380: 947d 9428 6a44 1100 006a 4411 0000 685e  .}.(jD...jD...h^
+00013390: 8694 6a4d 1100 006a 4e11 0000 685e 8694  ..jM...jN...h^..
+000133a0: 6a53 1100 006a 5311 0000 685e 8694 6a58  jS...jS...h^..jX
+000133b0: 1100 006a 5811 0000 685e 8694 7568 624b  ...jX...h^..uhbK
+000133c0: 008c 0574 6572 6d73 947d 9475 758c 0669  ...terms.}.uu..i
+000133d0: 6d61 6765 7394 8c0b 7370 6869 6e78 2e75  mages...sphinx.u
+000133e0: 7469 6c94 8c10 4669 6c65 6e61 6d65 556e  til...FilenameUn
+000133f0: 6971 4469 6374 9493 9429 8194 8f94 628c  iqDict...)....b.
+00013400: 0764 6c66 696c 6573 946a 6411 0000 8c0d  .dlfiles.jd.....
+00013410: 446f 776e 6c6f 6164 4669 6c65 7394 9394  DownloadFiles...
+00013420: 2981 948c 126f 7269 6769 6e61 6c5f 696d  )....original_im
+00013430: 6167 655f 7572 6994 7d94 8c09 7465 6d70  age_uri.}...temp
+00013440: 5f64 6174 6194 7d94 8c0b 7265 665f 636f  _data.}...ref_co
+00013450: 6e74 6578 7494 7d94 8c14 5f73 6561 7263  ntext.}..._searc
+00013460: 685f 696e 6465 785f 7469 746c 6573 947d  h_index_titles.}
+00013470: 948c 175f 7365 6172 6368 5f69 6e64 6578  ..._search_index
+00013480: 5f66 696c 656e 616d 6573 947d 948c 155f  _filenames.}..._
+00013490: 7365 6172 6368 5f69 6e64 6578 5f6d 6170  search_index_map
+000134a0: 7069 6e67 947d 948c 1b5f 7365 6172 6368  ping.}..._search
+000134b0: 5f69 6e64 6578 5f74 6974 6c65 5f6d 6170  _index_title_map
+000134c0: 7069 6e67 947d 948c 185f 7365 6172 6368  ping.}..._search
+000134d0: 5f69 6e64 6578 5f61 6c6c 5f74 6974 6c65  _index_all_title
+000134e0: 7394 7d94 8c1b 5f73 6561 7263 685f 696e  s.}..._search_in
+000134f0: 6465 785f 696e 6465 785f 656e 7472 6965  dex_index_entrie
+00013500: 7394 7d94 8c16 5f73 6561 7263 685f 696e  s.}..._search_in
+00013510: 6465 785f 6f62 6a74 7970 6573 947d 948c  dex_objtypes.}..
+00013520: 165f 7365 6172 6368 5f69 6e64 6578 5f6f  ._search_index_o
+00013530: 626a 6e61 6d65 7394 7d94 7562 2e         bjnames.}.ub.
```

### Comparing `decore_Base-0.0.22/docs/page/doctrees/index.doctree` & `decore_Base-0.0.23/docs/page/doctrees/index.doctree`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9578 b400 0000 0000 008c 0f73 7068  ...x.........sph
+00000000: 8005 95ef b300 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
 00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
 00000060: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
 00000070: 6805 8cd0 6465 636f 7265 2042 6173 6520  h...decore Base 
@@ -2048,15 +2048,15 @@
 00007ff0: 6add 0700 0075 6268 118c 0c20 6173 2066  j....ubh... as f
 00008000: 6f6c 6c6f 7773 3a94 8594 8194 7d94 2868  ollows:.....}.(h
 00008010: 166a dd07 0000 6826 6803 6827 4e68 294e  .j....h&h.h'Nh)N
 00008020: 7562 6568 177d 9428 6819 5d94 681b 5d94  ubeh.}.(h.].h.].
 00008030: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
 00008040: 5168 2768 5068 294b ca68 166a 9a07 0000  Qh'hPh)K.h.j....
 00008050: 6826 6803 7562 6a18 0200 0029 8194 7d94  h&h.ubj....)..}.
-00008060: 2868 0558 5704 0000 6672 6f6d 2064 6563  (h.XW...from dec
+00008060: 2868 0558 1304 0000 6672 6f6d 2064 6563  (h.X....from dec
 00008070: 6f72 655f 6261 7365 2069 6d70 6f72 7420  ore_base import 
 00008080: 6465 636f 7265 0a66 726f 6d20 6d6f 6465  decore.from mode
 00008090: 6c73 2e66 6972 7374 5f6d 6f64 656c 2069  ls.first_model i
 000080a0: 6d70 6f72 7420 4669 7273 745f 6d6f 6465  mport First_mode
 000080b0: 6c0a 0a40 6465 636f 7265 2e62 6173 6528  l..@decore.base(
 000080c0: 7469 746c 653d 274d 7920 4669 7273 7420  title='My First 
 000080d0: 4261 7365 272c 2069 636f 6e3d 276d 6469  Base', icon='mdi
@@ -2097,793 +2097,784 @@
 00008300: 6963 6f6e 3d27 6d64 692d 636f 6e74 656e  icon='mdi-conten
 00008310: 742d 7361 7665 272c 2074 7970 653d 2773  t-save', type='s
 00008320: 7562 6d69 7427 290a 2020 2020 2020 2020  ubmit').        
 00008330: 2020 2020 6465 6620 6669 7273 745f 6163      def first_ac
 00008340: 7469 6f6e 2873 656c 662c 2064 6174 6129  tion(self, data)
 00008350: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 00008360: 2069 7465 6d20 3d20 4669 7273 745f 6d6f   item = First_mo
-00008370: 6465 6c28 290a 2020 2020 2020 2020 2020  del().          
-00008380: 2020 2020 2069 7465 6d2e 7469 746c 6520       item.title 
-00008390: 3d20 6461 7461 5b27 6669 7273 746e 616d  = data['firstnam
-000083a0: 6527 5d20 2b20 2720 2720 2b20 6461 7461  e'] + ' ' + data
-000083b0: 5b27 6c61 7374 6e61 6d65 275d 0a20 2020  ['lastname'].   
-000083c0: 2020 2020 2020 2020 2020 2020 6974 656d              item
-000083d0: 2e66 6972 7374 6e61 6d65 203d 2064 6174  .firstname = dat
-000083e0: 615b 2766 6972 7374 6e61 6d65 275d 0a20  a['firstname']. 
-000083f0: 2020 2020 2020 2020 2020 2020 2020 6974                it
-00008400: 656d 2e6c 6173 746e 616d 6520 3d20 6461  em.lastname = da
-00008410: 7461 5b27 6c61 7374 6e61 6d65 275d 0a20  ta['lastname']. 
-00008420: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00008430: 2069 7465 6d2e 7361 7665 2829 3a0a 2020   item.save():.  
-00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008450: 7265 7475 726e 2054 7275 652c 2069 7465  return True, ite
-00008460: 6d2e 7469 746c 6520 2b20 2720 7361 7665  m.title + ' save
-00008470: 6420 7375 6363 6573 7366 756c 6c79 270a  d successfully'.
-00008480: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00008490: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000084a0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000084b0: 6c73 652c 2069 7465 6d2e 6572 726f 7294  lse, item.error.
-000084c0: 6807 5d94 6811 5857 0400 0066 726f 6d20  h.].h.XW...from 
-000084d0: 6465 636f 7265 5f62 6173 6520 696d 706f  decore_base impo
-000084e0: 7274 2064 6563 6f72 650a 6672 6f6d 206d  rt decore.from m
-000084f0: 6f64 656c 732e 6669 7273 745f 6d6f 6465  odels.first_mode
-00008500: 6c20 696d 706f 7274 2046 6972 7374 5f6d  l import First_m
-00008510: 6f64 656c 0a0a 4064 6563 6f72 652e 6261  odel..@decore.ba
-00008520: 7365 2874 6974 6c65 3d27 4d79 2046 6972  se(title='My Fir
-00008530: 7374 2042 6173 6527 2c20 6963 6f6e 3d27  st Base', icon='
-00008540: 6d64 692d 686f 6d65 272c 206d 6f64 656c  mdi-home', model
-00008550: 3d46 6972 7374 5f6d 6f64 656c 290a 636c  =First_model).cl
-00008560: 6173 7320 4669 7273 745f 6261 7365 3a0a  ass First_base:.
-00008570: 2020 2040 6465 636f 7265 2e76 6965 7728     @decore.view(
-00008580: 7469 746c 653d 2750 6572 736f 6e27 2c20  title='Person', 
-00008590: 6963 6f6e 3d27 6d64 692d 6163 636f 756e  icon='mdi-accoun
-000085a0: 7427 2c20 7479 7065 3d27 7461 626c 6527  t', type='table'
-000085b0: 2c20 6669 656c 6473 3d5b 4669 7273 745f  , fields=[First_
-000085c0: 6d6f 6465 6c2e 6669 7273 746e 616d 652c  model.firstname,
-000085d0: 2046 6972 7374 5f6d 6f64 656c 2e6c 6173   First_model.las
-000085e0: 746e 616d 655d 290a 2020 2064 6566 2066  tname]).   def f
-000085f0: 6972 7374 5f76 6965 7728 293a 0a20 2020  irst_view():.   
-00008600: 2020 2040 6465 636f 7265 2e64 6961 6c6f     @decore.dialo
-00008610: 6728 7469 746c 653d 2741 6464 2050 6572  g(title='Add Per
-00008620: 736f 6e27 2c20 6963 6f6e 3d27 6d64 692d  son', icon='mdi-
-00008630: 706c 7573 272c 2074 7970 653d 2773 7461  plus', type='sta
-00008640: 6e64 6172 6427 2c20 6469 7370 6c61 793d  ndard', display=
-00008650: 2764 7261 7765 7227 2c20 6163 7469 7661  'drawer', activa
-00008660: 746f 723d 2764 6566 6175 6c74 2d6d 656e  tor='default-men
-00008670: 7527 290a 2020 2020 2020 6465 6620 6669  u').      def fi
-00008680: 7273 745f 6469 616c 6f67 2829 3a0a 2020  rst_dialog():.  
-00008690: 2020 2020 2020 2040 6465 636f 7265 2e77         @decore.w
-000086a0: 6964 6765 7428 7469 746c 653d 2741 6464  idget(title='Add
-000086b0: 2050 6572 736f 6e20 466f 726d 272c 2069   Person Form', i
-000086c0: 636f 6e3d 276d 6469 2d61 6363 6f75 6e74  con='mdi-account
-000086d0: 272c 2074 7970 653d 2766 6f72 6d27 2c20  ', type='form', 
-000086e0: 6669 656c 6473 3d5b 4669 7273 745f 6d6f  fields=[First_mo
-000086f0: 6465 6c2e 6669 7273 746e 616d 652c 2046  del.firstname, F
-00008700: 6972 7374 5f6d 6f64 656c 2e6c 6173 746e  irst_model.lastn
-00008710: 616d 655d 290a 2020 2020 2020 2020 2064  ame]).         d
-00008720: 6566 2066 6972 7374 5f77 6964 6765 7428  ef first_widget(
-00008730: 293a 0a20 2020 2020 2020 2020 2020 2040  ):.            @
-00008740: 6465 636f 7265 2e61 6374 696f 6e28 7469  decore.action(ti
-00008750: 746c 653d 2753 6176 6520 5065 7273 6f6e  tle='Save Person
-00008760: 272c 2069 636f 6e3d 276d 6469 2d63 6f6e  ', icon='mdi-con
-00008770: 7465 6e74 2d73 6176 6527 2c20 7479 7065  tent-save', type
-00008780: 3d27 7375 626d 6974 2729 0a20 2020 2020  ='submit').     
-00008790: 2020 2020 2020 2064 6566 2066 6972 7374         def first
-000087a0: 5f61 6374 696f 6e28 7365 6c66 2c20 6461  _action(self, da
-000087b0: 7461 293a 0a20 2020 2020 2020 2020 2020  ta):.           
-000087c0: 2020 2020 6974 656d 203d 2046 6972 7374      item = First
-000087d0: 5f6d 6f64 656c 2829 0a20 2020 2020 2020  _model().       
-000087e0: 2020 2020 2020 2020 6974 656d 2e74 6974          item.tit
-000087f0: 6c65 203d 2064 6174 615b 2766 6972 7374  le = data['first
-00008800: 6e61 6d65 275d 202b 2027 2027 202b 2064  name'] + ' ' + d
-00008810: 6174 615b 276c 6173 746e 616d 6527 5d0a  ata['lastname'].
-00008820: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00008830: 7465 6d2e 6669 7273 746e 616d 6520 3d20  tem.firstname = 
-00008840: 6461 7461 5b27 6669 7273 746e 616d 6527  data['firstname'
-00008850: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00008860: 2069 7465 6d2e 6c61 7374 6e61 6d65 203d   item.lastname =
-00008870: 2064 6174 615b 276c 6173 746e 616d 6527   data['lastname'
-00008880: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00008890: 2069 6620 6974 656d 2e73 6176 6528 293a   if item.save():
-000088a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088b0: 2020 2072 6574 7572 6e20 5472 7565 2c20     return True, 
-000088c0: 6974 656d 2e74 6974 6c65 202b 2027 2073  item.title + ' s
-000088d0: 6176 6564 2073 7563 6365 7373 6675 6c6c  aved successfull
-000088e0: 7927 0a20 2020 2020 2020 2020 2020 2020  y'.             
-000088f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008900: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008910: 2046 616c 7365 2c20 6974 656d 2e65 7272   False, item.err
-00008920: 6f72 9485 9481 947d 9468 166a fd07 0000  or.....}.h.j....
-00008930: 7362 6168 177d 9428 6819 5d94 681b 5d94  sbah.}.(h.].h.].
-00008940: 681d 5d94 681f 5d94 6821 5d94 6823 6824  h.].h.].h!].h#h$
-00008950: 6a27 0200 0089 6a28 0200 008c 0670 7974  j'....j(.....pyt
-00008960: 686f 6e94 6a2a 0200 007d 9475 6825 6a17  hon.j*...}.uh%j.
-00008970: 0200 0068 2768 5068 294b cc68 166a 9a07  ...h'hPh)K.h.j..
-00008980: 0000 6826 6803 7562 6a48 0400 0029 8194  ..h&h.ubjH...)..
-00008990: 7d94 2868 0558 1701 0000 546f 2063 7265  }.(h.X....To cre
-000089a0: 6174 6520 6120 7265 636f 7264 2077 6974  ate a record wit
-000089b0: 6820 6465 636f 7265 2042 6173 652c 2077  h decore Base, w
-000089c0: 6520 6e65 6564 2074 6f20 6372 6561 7465  e need to create
-000089d0: 2061 6e20 696e 7374 616e 6365 206f 6620   an instance of 
-000089e0: 7468 6520 6d6f 6465 6c2e 2049 6e20 6f75  the model. In ou
-000089f0: 7220 6361 7365 202a 2a46 6972 7374 5f6d  r case **First_m
-00008a00: 6f64 656c 2a2a 2e20 5468 6520 696e 7374  odel**. The inst
-00008a10: 616e 6365 2069 7320 6669 6c6c 6564 2077  ance is filled w
-00008a20: 6974 6820 7468 6520 6461 7461 2066 726f  ith the data fro
-00008a30: 6d20 7468 6520 666f 726d 2061 6e64 2074  m the form and t
-00008a40: 6865 6e20 7361 7665 642e 0a0a 5468 6520  hen saved...The 
-00008a50: 4944 2069 6e20 7468 6520 666f 726d 206f  ID in the form o
-00008a60: 6620 6120 5555 4944 2069 7320 6765 6e65  f a UUID is gene
-00008a70: 7261 7465 6420 6175 746f 6d61 7469 6361  rated automatica
-00008a80: 6c6c 7920 616e 6420 646f 6573 206e 6f74  lly and does not
-00008a90: 2068 6176 6520 746f 2062 6520 7370 6563   have to be spec
-00008aa0: 6966 6965 6420 7365 7061 7261 7465 6c79  ified separately
-00008ab0: 2e94 6807 5d94 2868 5229 8194 7d94 2868  ..h.].(hR)..}.(h
-00008ac0: 058c b054 6f20 6372 6561 7465 2061 2072  ...To create a r
-00008ad0: 6563 6f72 6420 7769 7468 2064 6563 6f72  ecord with decor
-00008ae0: 6520 4261 7365 2c20 7765 206e 6565 6420  e Base, we need 
-00008af0: 746f 2063 7265 6174 6520 616e 2069 6e73  to create an ins
-00008b00: 7461 6e63 6520 6f66 2074 6865 206d 6f64  tance of the mod
-00008b10: 656c 2e20 496e 206f 7572 2063 6173 6520  el. In our case 
-00008b20: 2a2a 4669 7273 745f 6d6f 6465 6c2a 2a2e  **First_model**.
-00008b30: 2054 6865 2069 6e73 7461 6e63 6520 6973   The instance is
-00008b40: 2066 696c 6c65 6420 7769 7468 2074 6865   filled with the
-00008b50: 2064 6174 6120 6672 6f6d 2074 6865 2066   data from the f
-00008b60: 6f72 6d20 616e 6420 7468 656e 2073 6176  orm and then sav
-00008b70: 6564 2e94 6807 5d94 2868 118c 5d54 6f20  ed..h.].(h..]To 
-00008b80: 6372 6561 7465 2061 2072 6563 6f72 6420  create a record 
-00008b90: 7769 7468 2064 6563 6f72 6520 4261 7365  with decore Base
-00008ba0: 2c20 7765 206e 6565 6420 746f 2063 7265  , we need to cre
-00008bb0: 6174 6520 616e 2069 6e73 7461 6e63 6520  ate an instance 
-00008bc0: 6f66 2074 6865 206d 6f64 656c 2e20 496e  of the model. In
-00008bd0: 206f 7572 2063 6173 6520 9485 9481 947d   our case .....}
-00008be0: 9428 6816 6a11 0800 0068 2668 0368 274e  .(h.j....h&h.h'N
-00008bf0: 6829 4e75 6268 6629 8194 7d94 2868 058c  h)Nubhf)..}.(h..
-00008c00: 0f2a 2a46 6972 7374 5f6d 6f64 656c 2a2a  .**First_model**
-00008c10: 9468 075d 9468 118c 0b46 6972 7374 5f6d  .h.].h...First_m
-00008c20: 6f64 656c 9485 9481 947d 9428 6816 6a19  odel.....}.(h.j.
-00008c30: 0800 0068 2668 0368 274e 6829 4e75 6261  ...h&h.h'Nh)Nuba
-00008c40: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-00008c50: 9468 1f5d 9468 215d 9475 6825 6865 6816  .h.].h!].uh%heh.
-00008c60: 6a11 0800 0075 6268 118c 442e 2054 6865  j....ubh..D. The
-00008c70: 2069 6e73 7461 6e63 6520 6973 2066 696c   instance is fil
-00008c80: 6c65 6420 7769 7468 2074 6865 2064 6174  led with the dat
-00008c90: 6120 6672 6f6d 2074 6865 2066 6f72 6d20  a from the form 
-00008ca0: 616e 6420 7468 656e 2073 6176 6564 2e94  and then saved..
-00008cb0: 8594 8194 7d94 2868 166a 1108 0000 6826  ....}.(h.j....h&
-00008cc0: 6803 6827 4e68 294e 7562 6568 177d 9428  h.h'Nh)Nubeh.}.(
-00008cd0: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-00008ce0: 6821 5d94 7568 2568 5168 2768 5068 294b  h!].uh%hQh'hPh)K
-00008cf0: e568 166a 0d08 0000 7562 6852 2981 947d  .h.j....ubhR)..}
-00008d00: 9428 6805 8c65 5468 6520 4944 2069 6e20  .(h..eThe ID in 
-00008d10: 7468 6520 666f 726d 206f 6620 6120 5555  the form of a UU
-00008d20: 4944 2069 7320 6765 6e65 7261 7465 6420  ID is generated 
-00008d30: 6175 746f 6d61 7469 6361 6c6c 7920 616e  automatically an
-00008d40: 6420 646f 6573 206e 6f74 2068 6176 6520  d does not have 
-00008d50: 746f 2062 6520 7370 6563 6966 6965 6420  to be specified 
-00008d60: 7365 7061 7261 7465 6c79 2e94 6807 5d94  separately..h.].
-00008d70: 6811 8c65 5468 6520 4944 2069 6e20 7468  h..eThe ID in th
-00008d80: 6520 666f 726d 206f 6620 6120 5555 4944  e form of a UUID
-00008d90: 2069 7320 6765 6e65 7261 7465 6420 6175   is generated au
-00008da0: 746f 6d61 7469 6361 6c6c 7920 616e 6420  tomatically and 
-00008db0: 646f 6573 206e 6f74 2068 6176 6520 746f  does not have to
-00008dc0: 2062 6520 7370 6563 6966 6965 6420 7365   be specified se
-00008dd0: 7061 7261 7465 6c79 2e94 8594 8194 7d94  parately......}.
-00008de0: 2868 166a 3108 0000 6826 6803 6827 4e68  (h.j1...h&h.h'Nh
-00008df0: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
-00008e00: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-00008e10: 2568 5168 2768 5068 294b e768 166a 0d08  %hQh'hPh)K.h.j..
-00008e20: 0000 7562 6568 177d 9428 6819 5d94 681b  ..ubeh.}.(h.].h.
-00008e30: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-00008e40: 256a 4704 0000 6816 6a9a 0700 0068 2668  %jG...h.j....h&h
-00008e50: 0368 2768 5068 294e 7562 6a13 0500 0029  .h'hPh)Nubj....)
-00008e60: 8194 7d94 2868 058c 9954 6865 2066 6965  ..}.(h...The fie
-00008e70: 6c64 202a 2a74 6974 6c65 2a2a 2077 6173  ld **title** was
-00008e80: 2069 6e68 6572 6974 6564 2066 726f 6d20   inherited from 
-00008e90: 7468 6520 636c 6173 7320 2a2a 4465 666f  the class **Defo
-00008ea0: 726d 5f6d 6f64 656c 2a2a 2061 6e64 206d  rm_model** and m
-00008eb0: 7573 7420 6265 2075 7365 6420 666f 7220  ust be used for 
-00008ec0: 6561 6368 2072 6563 6f72 6420 6372 6561  each record crea
-00008ed0: 7469 6f6e 2e20 4f74 6865 7277 6973 6520  tion. Otherwise 
-00008ee0: 7468 6520 6974 656d 2077 696c 6c20 6661  the item will fa
-00008ef0: 696c 2074 6865 2076 616c 6964 6174 696f  il the validatio
-00008f00: 6e2e 9468 075d 9468 5229 8194 7d94 2868  n..h.].hR)..}.(h
-00008f10: 056a 4708 0000 6807 5d94 2868 118c 0a54  .jG...h.].(h...T
-00008f20: 6865 2066 6965 6c64 2094 8594 8194 7d94  he field .....}.
-00008f30: 2868 166a 4908 0000 6826 6803 6827 4e68  (h.jI...h&h.h'Nh
-00008f40: 294e 7562 6866 2981 947d 9428 6805 8c09  )Nubhf)..}.(h...
-00008f50: 2a2a 7469 746c 652a 2a94 6807 5d94 6811  **title**.h.].h.
-00008f60: 8c05 7469 746c 6594 8594 8194 7d94 2868  ..title.....}.(h
-00008f70: 166a 5008 0000 6826 6803 6827 4e68 294e  .jP...h&h.h'Nh)N
-00008f80: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00008f90: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-00008fa0: 6568 166a 4908 0000 7562 6811 8c1e 2077  eh.jI...ubh... w
-00008fb0: 6173 2069 6e68 6572 6974 6564 2066 726f  as inherited fro
-00008fc0: 6d20 7468 6520 636c 6173 7320 9485 9481  m the class ....
-00008fd0: 947d 9428 6816 6a49 0800 0068 2668 0368  .}.(h.jI...h&h.h
-00008fe0: 274e 6829 4e75 6268 6629 8194 7d94 2868  'Nh)Nubhf)..}.(h
-00008ff0: 058c 102a 2a44 6566 6f72 6d5f 6d6f 6465  ...**Deform_mode
-00009000: 6c2a 2a94 6807 5d94 6811 8c0c 4465 666f  l**.h.].h...Defo
-00009010: 726d 5f6d 6f64 656c 9485 9481 947d 9428  rm_model.....}.(
-00009020: 6816 6a62 0800 0068 2668 0368 274e 6829  h.jb...h&h.h'Nh)
-00009030: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
-00009040: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
-00009050: 6865 6816 6a49 0800 0075 6268 118c 5820  heh.jI...ubh..X 
-00009060: 616e 6420 6d75 7374 2062 6520 7573 6564  and must be used
-00009070: 2066 6f72 2065 6163 6820 7265 636f 7264   for each record
-00009080: 2063 7265 6174 696f 6e2e 204f 7468 6572   creation. Other
-00009090: 7769 7365 2074 6865 2069 7465 6d20 7769  wise the item wi
-000090a0: 6c6c 2066 6169 6c20 7468 6520 7661 6c69  ll fail the vali
-000090b0: 6461 7469 6f6e 2e94 8594 8194 7d94 2868  dation......}.(h
-000090c0: 166a 4908 0000 6826 6803 6827 4e68 294e  .jI...h&h.h'Nh)N
-000090d0: 7562 6568 177d 9428 6819 5d94 681b 5d94  ubeh.}.(h.].h.].
-000090e0: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
-000090f0: 5168 2768 5068 294b ea68 166a 4508 0000  Qh'hPh)K.h.jE...
-00009100: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-00009110: 681d 5d94 681f 5d94 6821 5d94 7568 256a  h.].h.].h!].uh%j
-00009120: 1205 0000 6816 6a9a 0700 0068 2668 0368  ....h.j....h&h.h
-00009130: 2768 5068 294e 7562 6568 177d 9428 6819  'hPh)Nubeh.}.(h.
-00009140: 5d94 8c06 6163 7469 6f6e 9461 681b 5d94  ]...action.ah.].
-00009150: 681d 5d94 8c06 6163 7469 6f6e 9461 681f  h.]...action.ah.
-00009160: 5d94 6821 5d94 7568 2568 2a68 166a 2103  ].h!].uh%h*h.j!.
-00009170: 0000 6826 6803 6827 6850 6829 4bc7 7562  ..h&h.h'hPh)K.ub
-00009180: 6568 177d 9428 6819 5d94 8c05 7573 6167  eh.}.(h.]...usag
-00009190: 6594 6168 1b5d 9468 1d5d 948c 0575 7361  e.ah.].h.]...usa
-000091a0: 6765 9461 681f 5d94 6821 5d94 7568 2568  ge.ah.].h!].uh%h
-000091b0: 2a68 166a 9201 0000 6826 6803 6827 6850  *h.j....h&h.h'hP
-000091c0: 6829 4b3c 7562 682b 2981 947d 9428 6805  h)K<ubh+)..}.(h.
-000091d0: 6806 6807 5d94 2868 3029 8194 7d94 2868  h.h.].(h0)..}.(h
-000091e0: 058c 1a52 756e 2c20 4465 7665 6c6f 706d  ...Run, Developm
-000091f0: 656e 7420 616e 6420 4275 696c 6494 6807  ent and Build.h.
-00009200: 5d94 6811 8c1a 5275 6e2c 2044 6576 656c  ].h...Run, Devel
-00009210: 6f70 6d65 6e74 2061 6e64 2042 7569 6c64  opment and Build
-00009220: 9485 9481 947d 9428 6816 6a93 0800 0068  .....}.(h.j....h
-00009230: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-00009240: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00009250: 9468 215d 9475 6825 682f 6816 6a90 0800  .h!].uh%h/h.j...
-00009260: 0068 2668 0368 2768 5068 294b ed75 6268  .h&h.h'hPh)K.ubh
-00009270: 5229 8194 7d94 2868 058c 7154 6f20 7374  R)..}.(h..qTo st
-00009280: 6172 7420 6f6e 6c79 2079 6f75 7220 6170  art only your ap
-00009290: 706c 6963 6174 696f 6e2c 2072 756e 2060  plication, run `
-000092a0: 6070 7974 686f 6e20 6170 702e 7079 6060  `python app.py``
-000092b0: 2069 6e20 796f 7572 2070 726f 6a65 6374   in your project
-000092c0: 2072 6f6f 7420 6469 7265 6374 6f72 792e   root directory.
-000092d0: 2055 7365 2074 6865 2074 6572 6d69 6e61   Use the termina
-000092e0: 6c20 696e 2076 7363 6f64 652e 9468 075d  l in vscode..h.]
-000092f0: 9428 6811 8c24 546f 2073 7461 7274 206f  .(h..$To start o
-00009300: 6e6c 7920 796f 7572 2061 7070 6c69 6361  nly your applica
-00009310: 7469 6f6e 2c20 7275 6e20 9485 9481 947d  tion, run .....}
-00009320: 9428 6816 6aa1 0800 0068 2668 0368 274e  .(h.j....h&h.h'N
-00009330: 6829 4e75 626a ee02 0000 2981 947d 9428  h)Nubj....)..}.(
-00009340: 6805 8c11 6060 7079 7468 6f6e 2061 7070  h...``python app
-00009350: 2e70 7960 6094 6807 5d94 6811 8c0d 7079  .py``.h.].h...py
-00009360: 7468 6f6e 2061 7070 2e70 7994 8594 8194  thon app.py.....
-00009370: 7d94 2868 166a a908 0000 6826 6803 6827  }.(h.j....h&h.h'
-00009380: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00009390: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-000093a0: 7568 256a ed02 0000 6816 6aa1 0800 0075  uh%j....h.j....u
-000093b0: 6268 118c 3c20 696e 2079 6f75 7220 7072  bh..< in your pr
-000093c0: 6f6a 6563 7420 726f 6f74 2064 6972 6563  oject root direc
-000093d0: 746f 7279 2e20 5573 6520 7468 6520 7465  tory. Use the te
-000093e0: 726d 696e 616c 2069 6e20 7673 636f 6465  rminal in vscode
-000093f0: 2e94 8594 8194 7d94 2868 166a a108 0000  ......}.(h.j....
-00009400: 6826 6803 6827 4e68 294e 7562 6568 177d  h&h.h'Nh)Nubeh.}
-00009410: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00009420: 5d94 6821 5d94 7568 2568 5168 2768 5068  ].h!].uh%hQh'hPh
-00009430: 294b ee68 166a 9008 0000 6826 6803 7562  )K.h.j....h&h.ub
-00009440: 6852 2981 947d 9428 6805 8c34 4f70 656e  hR)..}.(h..4Open
-00009450: 2074 6865 2062 726f 7773 6572 2061 6e64   the browser and
-00009460: 2074 7970 6520 6060 6874 7470 3a2f 2f6c   type ``http://l
-00009470: 6f63 616c 686f 7374 3a35 3535 3560 602e  ocalhost:5555``.
-00009480: 9468 075d 9428 6811 8c1a 4f70 656e 2074  .h.].(h...Open t
-00009490: 6865 2062 726f 7773 6572 2061 6e64 2074  he browser and t
-000094a0: 7970 6520 9485 9481 947d 9428 6816 6ac1  ype .....}.(h.j.
-000094b0: 0800 0068 2668 0368 274e 6829 4e75 626a  ...h&h.h'Nh)Nubj
-000094c0: ee02 0000 2981 947d 9428 6805 8c19 6060  ....)..}.(h...``
-000094d0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
-000094e0: 3a35 3535 3560 6094 6807 5d94 6811 8c15  :5555``.h.].h...
-000094f0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
-00009500: 3a35 3535 3594 8594 8194 7d94 2868 166a  :5555.....}.(h.j
-00009510: c908 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
-00009520: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-00009530: 5d94 681f 5d94 6821 5d94 7568 256a ed02  ].h.].h!].uh%j..
-00009540: 0000 6816 6ac1 0800 0075 6268 118c 012e  ..h.j....ubh....
-00009550: 9485 9481 947d 9428 6816 6ac1 0800 0068  .....}.(h.j....h
-00009560: 2668 0368 274e 6829 4e75 6265 6817 7d94  &h.h'Nh)Nubeh.}.
-00009570: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00009580: 9468 215d 9475 6825 6851 6827 6850 6829  .h!].uh%hQh'hPh)
-00009590: 4bf0 6816 6a90 0800 0068 2668 0375 6268  K.h.j....h&h.ubh
-000095a0: 2b29 8194 7d94 2868 0568 0668 075d 9428  +)..}.(h.h.h.].(
-000095b0: 6830 2981 947d 9428 6805 8c0b 4465 7665  h0)..}.(h...Deve
-000095c0: 6c6f 706d 656e 7494 6807 5d94 6811 8c0b  lopment.h.].h...
-000095d0: 4465 7665 6c6f 706d 656e 7494 8594 8194  Development.....
-000095e0: 7d94 2868 166a e408 0000 6826 6803 6827  }.(h.j....h&h.h'
-000095f0: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00009600: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00009610: 7568 2568 2f68 166a e108 0000 6826 6803  uh%h/h.j....h&h.
-00009620: 6827 6850 6829 4bf3 7562 6852 2981 947d  h'hPh)K.ubhR)..}
-00009630: 9428 6805 8c6c 546f 2064 6576 656c 6f70  .(h..lTo develop
-00009640: 2079 6f75 7220 6170 706c 6963 6174 696f   your applicatio
-00009650: 6e2c 2075 7365 2079 6f75 7220 6465 6275  n, use your debu
-00009660: 6767 6572 2077 6974 6820 7468 6520 6060  gger with the ``
-00009670: 5b64 6576 5d20 6465 636f 7265 2062 6173  [dev] decore bas
-00009680: 6520 6465 7665 6c6f 706d 656e 7460 6020  e development`` 
-00009690: 7072 6f66 696c 6520 696e 2076 7363 6f64  profile in vscod
-000096a0: 652e 9468 075d 9428 6811 8c38 546f 2064  e..h.].(h..8To d
-000096b0: 6576 656c 6f70 2079 6f75 7220 6170 706c  evelop your appl
-000096c0: 6963 6174 696f 6e2c 2075 7365 2079 6f75  ication, use you
-000096d0: 7220 6465 6275 6767 6572 2077 6974 6820  r debugger with 
-000096e0: 7468 6520 9485 9481 947d 9428 6816 6af2  the .....}.(h.j.
-000096f0: 0800 0068 2668 0368 274e 6829 4e75 626a  ...h&h.h'Nh)Nubj
-00009700: ee02 0000 2981 947d 9428 6805 8c21 6060  ....)..}.(h..!``
-00009710: 5b64 6576 5d20 6465 636f 7265 2062 6173  [dev] decore bas
-00009720: 6520 6465 7665 6c6f 706d 656e 7460 6094  e development``.
-00009730: 6807 5d94 6811 8c1d 5b64 6576 5d20 6465  h.].h...[dev] de
-00009740: 636f 7265 2062 6173 6520 6465 7665 6c6f  core base develo
-00009750: 706d 656e 7494 8594 8194 7d94 2868 166a  pment.....}.(h.j
-00009760: fa08 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
-00009770: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-00009780: 5d94 681f 5d94 6821 5d94 7568 256a ed02  ].h.].h!].uh%j..
-00009790: 0000 6816 6af2 0800 0075 6268 118c 1320  ..h.j....ubh... 
-000097a0: 7072 6f66 696c 6520 696e 2076 7363 6f64  profile in vscod
-000097b0: 652e 9485 9481 947d 9428 6816 6af2 0800  e......}.(h.j...
-000097c0: 0068 2668 0368 274e 6829 4e75 6265 6817  .h&h.h'Nh)Nubeh.
-000097d0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-000097e0: 1f5d 9468 215d 9475 6825 6851 6827 6850  .].h!].uh%hQh'hP
-000097f0: 6829 4bf4 6816 6ae1 0800 0068 2668 0375  h)K.h.j....h&h.u
-00009800: 6268 5229 8194 7d94 2868 058c 344f 7065  bhR)..}.(h..4Ope
-00009810: 6e20 7468 6520 6272 6f77 7365 7220 616e  n the browser an
-00009820: 6420 7479 7065 2060 6068 7474 703a 2f2f  d type ``http://
-00009830: 6c6f 6361 6c68 6f73 743a 3535 3535 6060  localhost:5555``
-00009840: 2e94 6807 5d94 2868 118c 1a4f 7065 6e20  ..h.].(h...Open 
-00009850: 7468 6520 6272 6f77 7365 7220 616e 6420  the browser and 
-00009860: 7479 7065 2094 8594 8194 7d94 2868 166a  type .....}.(h.j
-00009870: 1209 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
-00009880: 6aee 0200 0029 8194 7d94 2868 058c 1960  j....)..}.(h...`
-00009890: 6068 7474 703a 2f2f 6c6f 6361 6c68 6f73  `http://localhos
-000098a0: 743a 3535 3535 6060 9468 075d 9468 118c  t:5555``.h.].h..
-000098b0: 1568 7474 703a 2f2f 6c6f 6361 6c68 6f73  .http://localhos
-000098c0: 743a 3535 3535 9485 9481 947d 9428 6816  t:5555.....}.(h.
-000098d0: 6a1a 0900 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
-000098e0: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
-000098f0: 1d5d 9468 1f5d 9468 215d 9475 6825 6aed  .].h.].h!].uh%j.
-00009900: 0200 0068 166a 1209 0000 7562 6811 8c01  ...h.j....ubh...
-00009910: 2e94 8594 8194 7d94 2868 166a 1209 0000  ......}.(h.j....
-00009920: 6826 6803 6827 4e68 294e 7562 6568 177d  h&h.h'Nh)Nubeh.}
-00009930: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00009940: 5d94 6821 5d94 7568 2568 5168 2768 5068  ].h!].uh%hQh'hPh
-00009950: 294b f668 166a e108 0000 6826 6803 7562  )K.h.j....h&h.ub
-00009960: 6568 177d 9428 6819 5d94 8c0b 6465 7665  eh.}.(h.]...deve
-00009970: 6c6f 706d 656e 7494 6168 1b5d 9468 1d5d  lopment.ah.].h.]
-00009980: 948c 0b64 6576 656c 6f70 6d65 6e74 9461  ...development.a
-00009990: 681f 5d94 6821 5d94 7568 2568 2a68 166a  h.].h!].uh%h*h.j
-000099a0: 9008 0000 6826 6803 6827 6850 6829 4bf3  ....h&h.h'hPh)K.
-000099b0: 7562 682b 2981 947d 9428 6805 6806 6807  ubh+)..}.(h.h.h.
-000099c0: 5d94 2868 3029 8194 7d94 2868 058c 0542  ].(h0)..}.(h...B
-000099d0: 7569 6c64 9468 075d 9468 118c 0542 7569  uild.h.].h...Bui
-000099e0: 6c64 9485 9481 947d 9428 6816 6a3d 0900  ld.....}.(h.j=..
-000099f0: 0068 2668 0368 274e 6829 4e75 6261 6817  .h&h.h'Nh)Nubah.
-00009a00: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00009a10: 1f5d 9468 215d 9475 6825 682f 6816 6a3a  .].h!].uh%h/h.j:
-00009a20: 0900 0068 2668 0368 2768 5068 294b f975  ...h&h.h'hPh)K.u
-00009a30: 6268 5229 8194 7d94 2868 058c 7454 6f20  bhR)..}.(h..tTo 
-00009a40: 6275 696c 6420 796f 7572 2061 7070 6c69  build your appli
-00009a50: 6361 7469 6f6e 2c20 7275 6e20 6060 7079  cation, run ``py
-00009a60: 7468 6f6e 2061 7070 2e70 7920 2d2d 6275  thon app.py --bu
-00009a70: 696c 6460 6020 696e 2079 6f75 7220 7072  ild`` in your pr
-00009a80: 6f6a 6563 7420 726f 6f74 2064 6972 6563  oject root direc
-00009a90: 746f 7279 2e20 5573 6520 7468 6520 7465  tory. Use the te
-00009aa0: 726d 696e 616c 2069 6e20 7673 636f 6465  rminal in vscode
-00009ab0: 2e94 6807 5d94 2868 118c 1f54 6f20 6275  ..h.].(h...To bu
-00009ac0: 696c 6420 796f 7572 2061 7070 6c69 6361  ild your applica
-00009ad0: 7469 6f6e 2c20 7275 6e20 9485 9481 947d  tion, run .....}
-00009ae0: 9428 6816 6a4b 0900 0068 2668 0368 274e  .(h.jK...h&h.h'N
-00009af0: 6829 4e75 626a ee02 0000 2981 947d 9428  h)Nubj....)..}.(
-00009b00: 6805 8c19 6060 7079 7468 6f6e 2061 7070  h...``python app
-00009b10: 2e70 7920 2d2d 6275 696c 6460 6094 6807  .py --build``.h.
-00009b20: 5d94 6811 8c15 7079 7468 6f6e 2061 7070  ].h...python app
-00009b30: 2e70 7920 2d2d 6275 696c 6494 8594 8194  .py --build.....
-00009b40: 7d94 2868 166a 5309 0000 6826 6803 6827  }.(h.jS...h&h.h'
-00009b50: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-00009b60: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-00009b70: 7568 256a ed02 0000 6816 6a4b 0900 0075  uh%j....h.jK...u
-00009b80: 6268 118c 3c20 696e 2079 6f75 7220 7072  bh..< in your pr
-00009b90: 6f6a 6563 7420 726f 6f74 2064 6972 6563  oject root direc
-00009ba0: 746f 7279 2e20 5573 6520 7468 6520 7465  tory. Use the te
-00009bb0: 726d 696e 616c 2069 6e20 7673 636f 6465  rminal in vscode
-00009bc0: 2e94 8594 8194 7d94 2868 166a 4b09 0000  ......}.(h.jK...
-00009bd0: 6826 6803 6827 4e68 294e 7562 6568 177d  h&h.h'Nh)Nubeh.}
-00009be0: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00009bf0: 5d94 6821 5d94 7568 2568 5168 2768 5068  ].h!].uh%hQh'hPh
-00009c00: 294b fa68 166a 3a09 0000 6826 6803 7562  )K.h.j:...h&h.ub
-00009c10: 6568 177d 9428 6819 5d94 8c05 6275 696c  eh.}.(h.]...buil
-00009c20: 6494 6168 1b5d 9468 1d5d 948c 0562 7569  d.ah.].h.]...bui
-00009c30: 6c64 9461 681f 5d94 6821 5d94 7568 2568  ld.ah.].h!].uh%h
-00009c40: 2a68 166a 9008 0000 6826 6803 6827 6850  *h.j....h&h.h'hP
-00009c50: 6829 4bf9 7562 6568 177d 9428 6819 5d94  h)K.ubeh.}.(h.].
-00009c60: 8c19 7275 6e2d 6465 7665 6c6f 706d 656e  ..run-developmen
-00009c70: 742d 616e 642d 6275 696c 6494 6168 1b5d  t-and-build.ah.]
-00009c80: 9468 1d5d 948c 1a72 756e 2c20 6465 7665  .h.]...run, deve
-00009c90: 6c6f 706d 656e 7420 616e 6420 6275 696c  lopment and buil
-00009ca0: 6494 6168 1f5d 9468 215d 9475 6825 682a  d.ah.].h!].uh%h*
-00009cb0: 6816 6a92 0100 0068 2668 0368 2768 5068  h.j....h&h.h'hPh
-00009cc0: 294b ed75 6265 6817 7d94 2868 195d 948c  )K.ubeh.}.(h.]..
-00009cd0: 0b67 6574 2d73 7461 7274 6564 9461 681b  .get-started.ah.
-00009ce0: 5d94 681d 5d94 8c0b 6765 7420 7374 6172  ].h.]...get star
-00009cf0: 7465 6494 6168 1f5d 9468 215d 9475 6825  ted.ah.].h!].uh%
-00009d00: 682a 6816 682c 6826 6803 6827 6850 6829  h*h.h,h&h.h'hPh)
-00009d10: 4b1a 7562 682b 2981 947d 9428 6805 6806  K.ubh+)..}.(h.h.
-00009d20: 6807 5d94 2868 3029 8194 7d94 2868 058c  h.].(h0)..}.(h..
-00009d30: 1253 616d 706c 6520 6170 706c 6963 6174  .Sample applicat
-00009d40: 696f 6e94 6807 5d94 6811 8c12 5361 6d70  ion.h.].h...Samp
-00009d50: 6c65 2061 7070 6c69 6361 7469 6f6e 9485  le application..
-00009d60: 9481 947d 9428 6816 6a86 0900 0068 2668  ...}.(h.j....h&h
-00009d70: 0368 274e 6829 4e75 6261 6817 7d94 2868  .h'Nh)Nubah.}.(h
-00009d80: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
-00009d90: 215d 9475 6825 682f 6816 6a83 0900 0068  !].uh%h/h.j....h
-00009da0: 2668 0368 2768 5068 294b fd75 6268 5229  &h.h'hPh)K.ubhR)
-00009db0: 8194 7d94 2868 058c 9e54 6f20 6265 7474  ..}.(h...To bett
-00009dc0: 6572 2075 6e64 6572 7374 616e 6420 686f  er understand ho
-00009dd0: 7720 6465 636f 7265 2062 6173 6520 776f  w decore base wo
-00009de0: 726b 732c 2069 7420 6973 2062 6573 7420  rks, it is best 
-00009df0: 746f 206c 6f6f 6b20 6174 2074 6865 2073  to look at the s
-00009e00: 616d 706c 6520 6170 706c 6963 6174 696f  ample applicatio
-00009e10: 6e2e 2054 6865 2061 7070 6c69 6361 7469  n. The applicati
-00009e20: 6f6e 2072 6570 7265 7365 6e74 7320 6d79  on represents my
-00009e30: 2063 6f6e 7469 6e75 6f75 7320 6465 7665   continuous deve
-00009e40: 6c6f 706d 656e 7420 6f66 2064 6563 6f72  lopment of decor
-00009e50: 6520 6261 7365 2e94 6807 5d94 6811 8c9e  e base..h.].h...
-00009e60: 546f 2062 6574 7465 7220 756e 6465 7273  To better unders
-00009e70: 7461 6e64 2068 6f77 2064 6563 6f72 6520  tand how decore 
-00009e80: 6261 7365 2077 6f72 6b73 2c20 6974 2069  base works, it i
-00009e90: 7320 6265 7374 2074 6f20 6c6f 6f6b 2061  s best to look a
-00009ea0: 7420 7468 6520 7361 6d70 6c65 2061 7070  t the sample app
-00009eb0: 6c69 6361 7469 6f6e 2e20 5468 6520 6170  lication. The ap
-00009ec0: 706c 6963 6174 696f 6e20 7265 7072 6573  plication repres
-00009ed0: 656e 7473 206d 7920 636f 6e74 696e 756f  ents my continuo
-00009ee0: 7573 2064 6576 656c 6f70 6d65 6e74 206f  us development o
-00009ef0: 6620 6465 636f 7265 2062 6173 652e 9485  f decore base...
-00009f00: 9481 947d 9428 6816 6a94 0900 0068 2668  ...}.(h.j....h&h
-00009f10: 0368 274e 6829 4e75 6261 6817 7d94 2868  .h'Nh)Nubah.}.(h
-00009f20: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
-00009f30: 215d 9475 6825 6851 6827 6850 6829 4bfe  !].uh%hQh'hPh)K.
-00009f40: 6816 6a83 0900 0068 2668 0375 6268 5229  h.j....h&h.ubhR)
-00009f50: 8194 7d94 2868 058c 4868 7474 7073 3a2f  ..}.(h..Hhttps:/
-00009f60: 2f67 6974 6875 622e 636f 6d2f 4b65 6d6f  /github.com/Kemo
-00009f70: 5061 6e7a 6168 2f64 6563 6f72 655f 4261  Panzah/decore_Ba
-00009f80: 7365 2f74 7265 652f 6d61 7374 6572 2f64  se/tree/master/d
-00009f90: 6563 6f72 655f 6261 7365 2f73 616d 706c  ecore_base/sampl
-00009fa0: 6594 6807 5d94 6892 2981 947d 9428 6805  e.h.].h.)..}.(h.
-00009fb0: 6aa4 0900 0068 075d 9468 118c 4868 7474  j....h.].h..Hhtt
-00009fc0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00009fd0: 4b65 6d6f 5061 6e7a 6168 2f64 6563 6f72  KemoPanzah/decor
-00009fe0: 655f 4261 7365 2f74 7265 652f 6d61 7374  e_Base/tree/mast
-00009ff0: 6572 2f64 6563 6f72 655f 6261 7365 2f73  er/decore_base/s
-0000a000: 616d 706c 6594 8594 8194 7d94 2868 166a  ample.....}.(h.j
-0000a010: a609 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
-0000a020: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-0000a030: 5d94 681f 5d94 6821 5d94 8c06 7265 6675  ].h.].h!]...refu
-0000a040: 7269 946a a409 0000 7568 2568 9168 166a  ri.j....uh%h.h.j
-0000a050: a209 0000 7562 6168 177d 9428 6819 5d94  ....ubah.}.(h.].
-0000a060: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-0000a070: 7568 2568 5168 2768 5068 294d 0001 6816  uh%hQh'hPh)M..h.
-0000a080: 6a83 0900 0068 2668 0375 6268 5229 8194  j....h&h.ubhR)..
-0000a090: 7d94 2868 058c b054 6f20 7379 6e63 6872  }.(h...To synchr
-0000a0a0: 6f6e 697a 6520 7468 6520 7361 6d70 6c65  onize the sample
-0000a0b0: 2061 7070 6c69 6361 7469 6f6e 2077 6974   application wit
-0000a0c0: 6820 6120 7375 6266 6f6c 6465 7220 6f66  h a subfolder of
-0000a0d0: 2074 6865 2070 726f 6a65 6374 2072 6f6f   the project roo
-0000a0e0: 7420 6469 7265 6374 6f72 792c 2072 756e  t directory, run
-0000a0f0: 2060 6070 7974 686f 6e20 6170 702e 7079   ``python app.py
-0000a100: 202d 2d73 616d 706c 6560 6020 696e 2079   --sample`` in y
-0000a110: 6f75 7220 7072 6f6a 6563 7420 726f 6f74  our project root
-0000a120: 2064 6972 6563 746f 7279 2e20 5573 6520   directory. Use 
-0000a130: 7468 6520 7465 726d 696e 616c 2069 6e20  the terminal in 
-0000a140: 7673 636f 6465 2e94 6807 5d94 2868 118c  vscode..h.].(h..
-0000a150: 5a54 6f20 7379 6e63 6872 6f6e 697a 6520  ZTo synchronize 
-0000a160: 7468 6520 7361 6d70 6c65 2061 7070 6c69  the sample appli
-0000a170: 6361 7469 6f6e 2077 6974 6820 6120 7375  cation with a su
-0000a180: 6266 6f6c 6465 7220 6f66 2074 6865 2070  bfolder of the p
-0000a190: 726f 6a65 6374 2072 6f6f 7420 6469 7265  roject root dire
-0000a1a0: 6374 6f72 792c 2072 756e 2094 8594 8194  ctory, run .....
-0000a1b0: 7d94 2868 166a ba09 0000 6826 6803 6827  }.(h.j....h&h.h'
-0000a1c0: 4e68 294e 7562 6aee 0200 0029 8194 7d94  Nh)Nubj....)..}.
-0000a1d0: 2868 058c 1a60 6070 7974 686f 6e20 6170  (h...``python ap
-0000a1e0: 702e 7079 202d 2d73 616d 706c 6560 6094  p.py --sample``.
-0000a1f0: 6807 5d94 6811 8c16 7079 7468 6f6e 2061  h.].h...python a
-0000a200: 7070 2e70 7920 2d2d 7361 6d70 6c65 9485  pp.py --sample..
-0000a210: 9481 947d 9428 6816 6ac2 0900 0068 2668  ...}.(h.j....h&h
-0000a220: 0368 274e 6829 4e75 6261 6817 7d94 2868  .h'Nh)Nubah.}.(h
-0000a230: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
-0000a240: 215d 9475 6825 6aed 0200 0068 166a ba09  !].uh%j....h.j..
-0000a250: 0000 7562 6811 8c3c 2069 6e20 796f 7572  ..ubh..< in your
-0000a260: 2070 726f 6a65 6374 2072 6f6f 7420 6469   project root di
-0000a270: 7265 6374 6f72 792e 2055 7365 2074 6865  rectory. Use the
-0000a280: 2074 6572 6d69 6e61 6c20 696e 2076 7363   terminal in vsc
-0000a290: 6f64 652e 9485 9481 947d 9428 6816 6aba  ode......}.(h.j.
-0000a2a0: 0900 0068 2668 0368 274e 6829 4e75 6265  ...h&h.h'Nh)Nube
-0000a2b0: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
-0000a2c0: 9468 1f5d 9468 215d 9475 6825 6851 6827  .h.].h!].uh%hQh'
-0000a2d0: 6850 6829 4d02 0168 166a 8309 0000 6826  hPh)M..h.j....h&
-0000a2e0: 6803 7562 6852 2981 947d 9428 6805 8c7f  h.ubhR)..}.(h...
+00008370: 6465 6c28 6461 7461 5b27 6974 656d 275d  del(data['item']
+00008380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008390: 2069 7465 6d2e 7469 746c 6520 3d20 6974   item.title = it
+000083a0: 656d 2e66 6972 7374 6e61 6d65 202b 2027  em.firstname + '
+000083b0: 2027 202b 2069 7465 6d2e 6c61 7374 6e61   ' + item.lastna
+000083c0: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
+000083d0: 2020 6966 2069 7465 6d2e 7361 7665 2829    if item.save()
+000083e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000083f0: 2020 2020 7265 7475 726e 2054 7275 652c      return True,
+00008400: 2069 7465 6d2e 7469 746c 6520 2b20 2720   item.title + ' 
+00008410: 7361 7665 6420 7375 6363 6573 7366 756c  saved successful
+00008420: 6c79 270a 2020 2020 2020 2020 2020 2020  ly'.            
+00008430: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00008440: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00008450: 6e20 4661 6c73 652c 2027 4572 726f 7220  n False, 'Error 
+00008460: 7768 696c 6520 7361 7669 6e67 2027 202b  while saving ' +
+00008470: 2069 7465 6d2e 7469 746c 6594 6807 5d94   item.title.h.].
+00008480: 6811 5813 0400 0066 726f 6d20 6465 636f  h.X....from deco
+00008490: 7265 5f62 6173 6520 696d 706f 7274 2064  re_base import d
+000084a0: 6563 6f72 650a 6672 6f6d 206d 6f64 656c  ecore.from model
+000084b0: 732e 6669 7273 745f 6d6f 6465 6c20 696d  s.first_model im
+000084c0: 706f 7274 2046 6972 7374 5f6d 6f64 656c  port First_model
+000084d0: 0a0a 4064 6563 6f72 652e 6261 7365 2874  ..@decore.base(t
+000084e0: 6974 6c65 3d27 4d79 2046 6972 7374 2042  itle='My First B
+000084f0: 6173 6527 2c20 6963 6f6e 3d27 6d64 692d  ase', icon='mdi-
+00008500: 686f 6d65 272c 206d 6f64 656c 3d46 6972  home', model=Fir
+00008510: 7374 5f6d 6f64 656c 290a 636c 6173 7320  st_model).class 
+00008520: 4669 7273 745f 6261 7365 3a0a 2020 2040  First_base:.   @
+00008530: 6465 636f 7265 2e76 6965 7728 7469 746c  decore.view(titl
+00008540: 653d 2750 6572 736f 6e27 2c20 6963 6f6e  e='Person', icon
+00008550: 3d27 6d64 692d 6163 636f 756e 7427 2c20  ='mdi-account', 
+00008560: 7479 7065 3d27 7461 626c 6527 2c20 6669  type='table', fi
+00008570: 656c 6473 3d5b 4669 7273 745f 6d6f 6465  elds=[First_mode
+00008580: 6c2e 6669 7273 746e 616d 652c 2046 6972  l.firstname, Fir
+00008590: 7374 5f6d 6f64 656c 2e6c 6173 746e 616d  st_model.lastnam
+000085a0: 655d 290a 2020 2064 6566 2066 6972 7374  e]).   def first
+000085b0: 5f76 6965 7728 293a 0a20 2020 2020 2040  _view():.      @
+000085c0: 6465 636f 7265 2e64 6961 6c6f 6728 7469  decore.dialog(ti
+000085d0: 746c 653d 2741 6464 2050 6572 736f 6e27  tle='Add Person'
+000085e0: 2c20 6963 6f6e 3d27 6d64 692d 706c 7573  , icon='mdi-plus
+000085f0: 272c 2074 7970 653d 2773 7461 6e64 6172  ', type='standar
+00008600: 6427 2c20 6469 7370 6c61 793d 2764 7261  d', display='dra
+00008610: 7765 7227 2c20 6163 7469 7661 746f 723d  wer', activator=
+00008620: 2764 6566 6175 6c74 2d6d 656e 7527 290a  'default-menu').
+00008630: 2020 2020 2020 6465 6620 6669 7273 745f        def first_
+00008640: 6469 616c 6f67 2829 3a0a 2020 2020 2020  dialog():.      
+00008650: 2020 2040 6465 636f 7265 2e77 6964 6765     @decore.widge
+00008660: 7428 7469 746c 653d 2741 6464 2050 6572  t(title='Add Per
+00008670: 736f 6e20 466f 726d 272c 2069 636f 6e3d  son Form', icon=
+00008680: 276d 6469 2d61 6363 6f75 6e74 272c 2074  'mdi-account', t
+00008690: 7970 653d 2766 6f72 6d27 2c20 6669 656c  ype='form', fiel
+000086a0: 6473 3d5b 4669 7273 745f 6d6f 6465 6c2e  ds=[First_model.
+000086b0: 6669 7273 746e 616d 652c 2046 6972 7374  firstname, First
+000086c0: 5f6d 6f64 656c 2e6c 6173 746e 616d 655d  _model.lastname]
+000086d0: 290a 2020 2020 2020 2020 2064 6566 2066  ).         def f
+000086e0: 6972 7374 5f77 6964 6765 7428 293a 0a20  irst_widget():. 
+000086f0: 2020 2020 2020 2020 2020 2040 6465 636f             @deco
+00008700: 7265 2e61 6374 696f 6e28 7469 746c 653d  re.action(title=
+00008710: 2753 6176 6520 5065 7273 6f6e 272c 2069  'Save Person', i
+00008720: 636f 6e3d 276d 6469 2d63 6f6e 7465 6e74  con='mdi-content
+00008730: 2d73 6176 6527 2c20 7479 7065 3d27 7375  -save', type='su
+00008740: 626d 6974 2729 0a20 2020 2020 2020 2020  bmit').         
+00008750: 2020 2064 6566 2066 6972 7374 5f61 6374     def first_act
+00008760: 696f 6e28 7365 6c66 2c20 6461 7461 293a  ion(self, data):
+00008770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008780: 6974 656d 203d 2046 6972 7374 5f6d 6f64  item = First_mod
+00008790: 656c 2864 6174 615b 2769 7465 6d27 5d29  el(data['item'])
+000087a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000087b0: 6974 656d 2e74 6974 6c65 203d 2069 7465  item.title = ite
+000087c0: 6d2e 6669 7273 746e 616d 6520 2b20 2720  m.firstname + ' 
+000087d0: 2720 2b20 6974 656d 2e6c 6173 746e 616d  ' + item.lastnam
+000087e0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000087f0: 2069 6620 6974 656d 2e73 6176 6528 293a   if item.save():
+00008800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008810: 2020 2072 6574 7572 6e20 5472 7565 2c20     return True, 
+00008820: 6974 656d 2e74 6974 6c65 202b 2027 2073  item.title + ' s
+00008830: 6176 6564 2073 7563 6365 7373 6675 6c6c  aved successfull
+00008840: 7927 0a20 2020 2020 2020 2020 2020 2020  y'.             
+00008850: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008860: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00008870: 2046 616c 7365 2c20 2745 7272 6f72 2077   False, 'Error w
+00008880: 6869 6c65 2073 6176 696e 6720 2720 2b20  hile saving ' + 
+00008890: 6974 656d 2e74 6974 6c65 9485 9481 947d  item.title.....}
+000088a0: 9468 166a fd07 0000 7362 6168 177d 9428  .h.j....sbah.}.(
+000088b0: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+000088c0: 6821 5d94 6823 6824 6a27 0200 0089 6a28  h!].h#h$j'....j(
+000088d0: 0200 008c 0670 7974 686f 6e94 6a2a 0200  .....python.j*..
+000088e0: 007d 9475 6825 6a17 0200 0068 2768 5068  .}.uh%j....h'hPh
+000088f0: 294b cc68 166a 9a07 0000 6826 6803 7562  )K.h.j....h&h.ub
+00008900: 6a48 0400 0029 8194 7d94 2868 0558 1701  jH...)..}.(h.X..
+00008910: 0000 546f 2063 7265 6174 6520 6120 7265  ..To create a re
+00008920: 636f 7264 2077 6974 6820 6465 636f 7265  cord with decore
+00008930: 2042 6173 652c 2077 6520 6e65 6564 2074   Base, we need t
+00008940: 6f20 6372 6561 7465 2061 6e20 696e 7374  o create an inst
+00008950: 616e 6365 206f 6620 7468 6520 6d6f 6465  ance of the mode
+00008960: 6c2e 2049 6e20 6f75 7220 6361 7365 202a  l. In our case *
+00008970: 2a46 6972 7374 5f6d 6f64 656c 2a2a 2e20  *First_model**. 
+00008980: 5468 6520 696e 7374 616e 6365 2069 7320  The instance is 
+00008990: 6669 6c6c 6564 2077 6974 6820 7468 6520  filled with the 
+000089a0: 6461 7461 2066 726f 6d20 7468 6520 666f  data from the fo
+000089b0: 726d 2061 6e64 2074 6865 6e20 7361 7665  rm and then save
+000089c0: 642e 0a0a 5468 6520 4944 2069 6e20 7468  d...The ID in th
+000089d0: 6520 666f 726d 206f 6620 6120 5555 4944  e form of a UUID
+000089e0: 2069 7320 6765 6e65 7261 7465 6420 6175   is generated au
+000089f0: 746f 6d61 7469 6361 6c6c 7920 616e 6420  tomatically and 
+00008a00: 646f 6573 206e 6f74 2068 6176 6520 746f  does not have to
+00008a10: 2062 6520 7370 6563 6966 6965 6420 7365   be specified se
+00008a20: 7061 7261 7465 6c79 2e94 6807 5d94 2868  parately..h.].(h
+00008a30: 5229 8194 7d94 2868 058c b054 6f20 6372  R)..}.(h...To cr
+00008a40: 6561 7465 2061 2072 6563 6f72 6420 7769  eate a record wi
+00008a50: 7468 2064 6563 6f72 6520 4261 7365 2c20  th decore Base, 
+00008a60: 7765 206e 6565 6420 746f 2063 7265 6174  we need to creat
+00008a70: 6520 616e 2069 6e73 7461 6e63 6520 6f66  e an instance of
+00008a80: 2074 6865 206d 6f64 656c 2e20 496e 206f   the model. In o
+00008a90: 7572 2063 6173 6520 2a2a 4669 7273 745f  ur case **First_
+00008aa0: 6d6f 6465 6c2a 2a2e 2054 6865 2069 6e73  model**. The ins
+00008ab0: 7461 6e63 6520 6973 2066 696c 6c65 6420  tance is filled 
+00008ac0: 7769 7468 2074 6865 2064 6174 6120 6672  with the data fr
+00008ad0: 6f6d 2074 6865 2066 6f72 6d20 616e 6420  om the form and 
+00008ae0: 7468 656e 2073 6176 6564 2e94 6807 5d94  then saved..h.].
+00008af0: 2868 118c 5d54 6f20 6372 6561 7465 2061  (h..]To create a
+00008b00: 2072 6563 6f72 6420 7769 7468 2064 6563   record with dec
+00008b10: 6f72 6520 4261 7365 2c20 7765 206e 6565  ore Base, we nee
+00008b20: 6420 746f 2063 7265 6174 6520 616e 2069  d to create an i
+00008b30: 6e73 7461 6e63 6520 6f66 2074 6865 206d  nstance of the m
+00008b40: 6f64 656c 2e20 496e 206f 7572 2063 6173  odel. In our cas
+00008b50: 6520 9485 9481 947d 9428 6816 6a11 0800  e .....}.(h.j...
+00008b60: 0068 2668 0368 274e 6829 4e75 6268 6629  .h&h.h'Nh)Nubhf)
+00008b70: 8194 7d94 2868 058c 0f2a 2a46 6972 7374  ..}.(h...**First
+00008b80: 5f6d 6f64 656c 2a2a 9468 075d 9468 118c  _model**.h.].h..
+00008b90: 0b46 6972 7374 5f6d 6f64 656c 9485 9481  .First_model....
+00008ba0: 947d 9428 6816 6a19 0800 0068 2668 0368  .}.(h.j....h&h.h
+00008bb0: 274e 6829 4e75 6261 6817 7d94 2868 195d  'Nh)Nubah.}.(h.]
+00008bc0: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
+00008bd0: 9475 6825 6865 6816 6a11 0800 0075 6268  .uh%heh.j....ubh
+00008be0: 118c 442e 2054 6865 2069 6e73 7461 6e63  ..D. The instanc
+00008bf0: 6520 6973 2066 696c 6c65 6420 7769 7468  e is filled with
+00008c00: 2074 6865 2064 6174 6120 6672 6f6d 2074   the data from t
+00008c10: 6865 2066 6f72 6d20 616e 6420 7468 656e  he form and then
+00008c20: 2073 6176 6564 2e94 8594 8194 7d94 2868   saved......}.(h
+00008c30: 166a 1108 0000 6826 6803 6827 4e68 294e  .j....h&h.h'Nh)N
+00008c40: 7562 6568 177d 9428 6819 5d94 681b 5d94  ubeh.}.(h.].h.].
+00008c50: 681d 5d94 681f 5d94 6821 5d94 7568 2568  h.].h.].h!].uh%h
+00008c60: 5168 2768 5068 294b e368 166a 0d08 0000  Qh'hPh)K.h.j....
+00008c70: 7562 6852 2981 947d 9428 6805 8c65 5468  ubhR)..}.(h..eTh
+00008c80: 6520 4944 2069 6e20 7468 6520 666f 726d  e ID in the form
+00008c90: 206f 6620 6120 5555 4944 2069 7320 6765   of a UUID is ge
+00008ca0: 6e65 7261 7465 6420 6175 746f 6d61 7469  nerated automati
+00008cb0: 6361 6c6c 7920 616e 6420 646f 6573 206e  cally and does n
+00008cc0: 6f74 2068 6176 6520 746f 2062 6520 7370  ot have to be sp
+00008cd0: 6563 6966 6965 6420 7365 7061 7261 7465  ecified separate
+00008ce0: 6c79 2e94 6807 5d94 6811 8c65 5468 6520  ly..h.].h..eThe 
+00008cf0: 4944 2069 6e20 7468 6520 666f 726d 206f  ID in the form o
+00008d00: 6620 6120 5555 4944 2069 7320 6765 6e65  f a UUID is gene
+00008d10: 7261 7465 6420 6175 746f 6d61 7469 6361  rated automatica
+00008d20: 6c6c 7920 616e 6420 646f 6573 206e 6f74  lly and does not
+00008d30: 2068 6176 6520 746f 2062 6520 7370 6563   have to be spec
+00008d40: 6966 6965 6420 7365 7061 7261 7465 6c79  ified separately
+00008d50: 2e94 8594 8194 7d94 2868 166a 3108 0000  ......}.(h.j1...
+00008d60: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
+00008d70: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+00008d80: 5d94 6821 5d94 7568 2568 5168 2768 5068  ].h!].uh%hQh'hPh
+00008d90: 294b e568 166a 0d08 0000 7562 6568 177d  )K.h.j....ubeh.}
+00008da0: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+00008db0: 5d94 6821 5d94 7568 256a 4704 0000 6816  ].h!].uh%jG...h.
+00008dc0: 6a9a 0700 0068 2668 0368 2768 5068 294e  j....h&h.h'hPh)N
+00008dd0: 7562 6a13 0500 0029 8194 7d94 2868 058c  ubj....)..}.(h..
+00008de0: 9954 6865 2066 6965 6c64 202a 2a74 6974  .The field **tit
+00008df0: 6c65 2a2a 2077 6173 2069 6e68 6572 6974  le** was inherit
+00008e00: 6564 2066 726f 6d20 7468 6520 636c 6173  ed from the clas
+00008e10: 7320 2a2a 4465 666f 726d 5f6d 6f64 656c  s **Deform_model
+00008e20: 2a2a 2061 6e64 206d 7573 7420 6265 2075  ** and must be u
+00008e30: 7365 6420 666f 7220 6561 6368 2072 6563  sed for each rec
+00008e40: 6f72 6420 6372 6561 7469 6f6e 2e20 4f74  ord creation. Ot
+00008e50: 6865 7277 6973 6520 7468 6520 6974 656d  herwise the item
+00008e60: 2077 696c 6c20 6661 696c 2074 6865 2076   will fail the v
+00008e70: 616c 6964 6174 696f 6e2e 9468 075d 9468  alidation..h.].h
+00008e80: 5229 8194 7d94 2868 056a 4708 0000 6807  R)..}.(h.jG...h.
+00008e90: 5d94 2868 118c 0a54 6865 2066 6965 6c64  ].(h...The field
+00008ea0: 2094 8594 8194 7d94 2868 166a 4908 0000   .....}.(h.jI...
+00008eb0: 6826 6803 6827 4e68 294e 7562 6866 2981  h&h.h'Nh)Nubhf).
+00008ec0: 947d 9428 6805 8c09 2a2a 7469 746c 652a  .}.(h...**title*
+00008ed0: 2a94 6807 5d94 6811 8c05 7469 746c 6594  *.h.].h...title.
+00008ee0: 8594 8194 7d94 2868 166a 5008 0000 6826  ....}.(h.jP...h&
+00008ef0: 6803 6827 4e68 294e 7562 6168 177d 9428  h.h'Nh)Nubah.}.(
+00008f00: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00008f10: 6821 5d94 7568 2568 6568 166a 4908 0000  h!].uh%heh.jI...
+00008f20: 7562 6811 8c1e 2077 6173 2069 6e68 6572  ubh... was inher
+00008f30: 6974 6564 2066 726f 6d20 7468 6520 636c  ited from the cl
+00008f40: 6173 7320 9485 9481 947d 9428 6816 6a49  ass .....}.(h.jI
+00008f50: 0800 0068 2668 0368 274e 6829 4e75 6268  ...h&h.h'Nh)Nubh
+00008f60: 6629 8194 7d94 2868 058c 102a 2a44 6566  f)..}.(h...**Def
+00008f70: 6f72 6d5f 6d6f 6465 6c2a 2a94 6807 5d94  orm_model**.h.].
+00008f80: 6811 8c0c 4465 666f 726d 5f6d 6f64 656c  h...Deform_model
+00008f90: 9485 9481 947d 9428 6816 6a62 0800 0068  .....}.(h.jb...h
+00008fa0: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
+00008fb0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00008fc0: 9468 215d 9475 6825 6865 6816 6a49 0800  .h!].uh%heh.jI..
+00008fd0: 0075 6268 118c 5820 616e 6420 6d75 7374  .ubh..X and must
+00008fe0: 2062 6520 7573 6564 2066 6f72 2065 6163   be used for eac
+00008ff0: 6820 7265 636f 7264 2063 7265 6174 696f  h record creatio
+00009000: 6e2e 204f 7468 6572 7769 7365 2074 6865  n. Otherwise the
+00009010: 2069 7465 6d20 7769 6c6c 2066 6169 6c20   item will fail 
+00009020: 7468 6520 7661 6c69 6461 7469 6f6e 2e94  the validation..
+00009030: 8594 8194 7d94 2868 166a 4908 0000 6826  ....}.(h.jI...h&
+00009040: 6803 6827 4e68 294e 7562 6568 177d 9428  h.h'Nh)Nubeh.}.(
+00009050: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00009060: 6821 5d94 7568 2568 5168 2768 5068 294b  h!].uh%hQh'hPh)K
+00009070: e868 166a 4508 0000 7562 6168 177d 9428  .h.jE...ubah.}.(
+00009080: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+00009090: 6821 5d94 7568 256a 1205 0000 6816 6a9a  h!].uh%j....h.j.
+000090a0: 0700 0068 2668 0368 2768 5068 294e 7562  ...h&h.h'hPh)Nub
+000090b0: 6568 177d 9428 6819 5d94 8c06 6163 7469  eh.}.(h.]...acti
+000090c0: 6f6e 9461 681b 5d94 681d 5d94 8c06 6163  on.ah.].h.]...ac
+000090d0: 7469 6f6e 9461 681f 5d94 6821 5d94 7568  tion.ah.].h!].uh
+000090e0: 2568 2a68 166a 2103 0000 6826 6803 6827  %h*h.j!...h&h.h'
+000090f0: 6850 6829 4bc7 7562 6568 177d 9428 6819  hPh)K.ubeh.}.(h.
+00009100: 5d94 8c05 7573 6167 6594 6168 1b5d 9468  ]...usage.ah.].h
+00009110: 1d5d 948c 0575 7361 6765 9461 681f 5d94  .]...usage.ah.].
+00009120: 6821 5d94 7568 2568 2a68 166a 9201 0000  h!].uh%h*h.j....
+00009130: 6826 6803 6827 6850 6829 4b3c 7562 682b  h&h.h'hPh)K<ubh+
+00009140: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+00009150: 3029 8194 7d94 2868 058c 1a52 756e 2c20  0)..}.(h...Run, 
+00009160: 4465 7665 6c6f 706d 656e 7420 616e 6420  Development and 
+00009170: 4275 696c 6494 6807 5d94 6811 8c1a 5275  Build.h.].h...Ru
+00009180: 6e2c 2044 6576 656c 6f70 6d65 6e74 2061  n, Development a
+00009190: 6e64 2042 7569 6c64 9485 9481 947d 9428  nd Build.....}.(
+000091a0: 6816 6a93 0800 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
+000091b0: 4e75 6261 6817 7d94 2868 195d 9468 1b5d  Nubah.}.(h.].h.]
+000091c0: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
+000091d0: 682f 6816 6a90 0800 0068 2668 0368 2768  h/h.j....h&h.h'h
+000091e0: 5068 294b eb75 6268 5229 8194 7d94 2868  Ph)K.ubhR)..}.(h
+000091f0: 058c 7154 6f20 7374 6172 7420 6f6e 6c79  ..qTo start only
+00009200: 2079 6f75 7220 6170 706c 6963 6174 696f   your applicatio
+00009210: 6e2c 2072 756e 2060 6070 7974 686f 6e20  n, run ``python 
+00009220: 6170 702e 7079 6060 2069 6e20 796f 7572  app.py`` in your
+00009230: 2070 726f 6a65 6374 2072 6f6f 7420 6469   project root di
+00009240: 7265 6374 6f72 792e 2055 7365 2074 6865  rectory. Use the
+00009250: 2074 6572 6d69 6e61 6c20 696e 2076 7363   terminal in vsc
+00009260: 6f64 652e 9468 075d 9428 6811 8c24 546f  ode..h.].(h..$To
+00009270: 2073 7461 7274 206f 6e6c 7920 796f 7572   start only your
+00009280: 2061 7070 6c69 6361 7469 6f6e 2c20 7275   application, ru
+00009290: 6e20 9485 9481 947d 9428 6816 6aa1 0800  n .....}.(h.j...
+000092a0: 0068 2668 0368 274e 6829 4e75 626a ee02  .h&h.h'Nh)Nubj..
+000092b0: 0000 2981 947d 9428 6805 8c11 6060 7079  ..)..}.(h...``py
+000092c0: 7468 6f6e 2061 7070 2e70 7960 6094 6807  thon app.py``.h.
+000092d0: 5d94 6811 8c0d 7079 7468 6f6e 2061 7070  ].h...python app
+000092e0: 2e70 7994 8594 8194 7d94 2868 166a a908  .py.....}.(h.j..
+000092f0: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+00009300: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00009310: 681f 5d94 6821 5d94 7568 256a ed02 0000  h.].h!].uh%j....
+00009320: 6816 6aa1 0800 0075 6268 118c 3c20 696e  h.j....ubh..< in
+00009330: 2079 6f75 7220 7072 6f6a 6563 7420 726f   your project ro
+00009340: 6f74 2064 6972 6563 746f 7279 2e20 5573  ot directory. Us
+00009350: 6520 7468 6520 7465 726d 696e 616c 2069  e the terminal i
+00009360: 6e20 7673 636f 6465 2e94 8594 8194 7d94  n vscode......}.
+00009370: 2868 166a a108 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
+00009380: 294e 7562 6568 177d 9428 6819 5d94 681b  )Nubeh.}.(h.].h.
+00009390: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+000093a0: 2568 5168 2768 5068 294b ec68 166a 9008  %hQh'hPh)K.h.j..
+000093b0: 0000 6826 6803 7562 6852 2981 947d 9428  ..h&h.ubhR)..}.(
+000093c0: 6805 8c34 4f70 656e 2074 6865 2062 726f  h..4Open the bro
+000093d0: 7773 6572 2061 6e64 2074 7970 6520 6060  wser and type ``
+000093e0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+000093f0: 3a35 3535 3560 602e 9468 075d 9428 6811  :5555``..h.].(h.
+00009400: 8c1a 4f70 656e 2074 6865 2062 726f 7773  ..Open the brows
+00009410: 6572 2061 6e64 2074 7970 6520 9485 9481  er and type ....
+00009420: 947d 9428 6816 6ac1 0800 0068 2668 0368  .}.(h.j....h&h.h
+00009430: 274e 6829 4e75 626a ee02 0000 2981 947d  'Nh)Nubj....)..}
+00009440: 9428 6805 8c19 6060 6874 7470 3a2f 2f6c  .(h...``http://l
+00009450: 6f63 616c 686f 7374 3a35 3535 3560 6094  ocalhost:5555``.
+00009460: 6807 5d94 6811 8c15 6874 7470 3a2f 2f6c  h.].h...http://l
+00009470: 6f63 616c 686f 7374 3a35 3535 3594 8594  ocalhost:5555...
+00009480: 8194 7d94 2868 166a c908 0000 6826 6803  ..}.(h.j....h&h.
+00009490: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
+000094a0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+000094b0: 5d94 7568 256a ed02 0000 6816 6ac1 0800  ].uh%j....h.j...
+000094c0: 0075 6268 118c 012e 9485 9481 947d 9428  .ubh.........}.(
+000094d0: 6816 6ac1 0800 0068 2668 0368 274e 6829  h.j....h&h.h'Nh)
+000094e0: 4e75 6265 6817 7d94 2868 195d 9468 1b5d  Nubeh.}.(h.].h.]
+000094f0: 9468 1d5d 9468 1f5d 9468 215d 9475 6825  .h.].h.].h!].uh%
+00009500: 6851 6827 6850 6829 4bee 6816 6a90 0800  hQh'hPh)K.h.j...
+00009510: 0068 2668 0375 6268 2b29 8194 7d94 2868  .h&h.ubh+)..}.(h
+00009520: 0568 0668 075d 9428 6830 2981 947d 9428  .h.h.].(h0)..}.(
+00009530: 6805 8c0b 4465 7665 6c6f 706d 656e 7494  h...Development.
+00009540: 6807 5d94 6811 8c0b 4465 7665 6c6f 706d  h.].h...Developm
+00009550: 656e 7494 8594 8194 7d94 2868 166a e408  ent.....}.(h.j..
+00009560: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+00009570: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00009580: 681f 5d94 6821 5d94 7568 2568 2f68 166a  h.].h!].uh%h/h.j
+00009590: e108 0000 6826 6803 6827 6850 6829 4bf1  ....h&h.h'hPh)K.
+000095a0: 7562 6852 2981 947d 9428 6805 8c6c 546f  ubhR)..}.(h..lTo
+000095b0: 2064 6576 656c 6f70 2079 6f75 7220 6170   develop your ap
+000095c0: 706c 6963 6174 696f 6e2c 2075 7365 2079  plication, use y
+000095d0: 6f75 7220 6465 6275 6767 6572 2077 6974  our debugger wit
+000095e0: 6820 7468 6520 6060 5b64 6576 5d20 6465  h the ``[dev] de
+000095f0: 636f 7265 2062 6173 6520 6465 7665 6c6f  core base develo
+00009600: 706d 656e 7460 6020 7072 6f66 696c 6520  pment`` profile 
+00009610: 696e 2076 7363 6f64 652e 9468 075d 9428  in vscode..h.].(
+00009620: 6811 8c38 546f 2064 6576 656c 6f70 2079  h..8To develop y
+00009630: 6f75 7220 6170 706c 6963 6174 696f 6e2c  our application,
+00009640: 2075 7365 2079 6f75 7220 6465 6275 6767   use your debugg
+00009650: 6572 2077 6974 6820 7468 6520 9485 9481  er with the ....
+00009660: 947d 9428 6816 6af2 0800 0068 2668 0368  .}.(h.j....h&h.h
+00009670: 274e 6829 4e75 626a ee02 0000 2981 947d  'Nh)Nubj....)..}
+00009680: 9428 6805 8c21 6060 5b64 6576 5d20 6465  .(h..!``[dev] de
+00009690: 636f 7265 2062 6173 6520 6465 7665 6c6f  core base develo
+000096a0: 706d 656e 7460 6094 6807 5d94 6811 8c1d  pment``.h.].h...
+000096b0: 5b64 6576 5d20 6465 636f 7265 2062 6173  [dev] decore bas
+000096c0: 6520 6465 7665 6c6f 706d 656e 7494 8594  e development...
+000096d0: 8194 7d94 2868 166a fa08 0000 6826 6803  ..}.(h.j....h&h.
+000096e0: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
+000096f0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+00009700: 5d94 7568 256a ed02 0000 6816 6af2 0800  ].uh%j....h.j...
+00009710: 0075 6268 118c 1320 7072 6f66 696c 6520  .ubh... profile 
+00009720: 696e 2076 7363 6f64 652e 9485 9481 947d  in vscode......}
+00009730: 9428 6816 6af2 0800 0068 2668 0368 274e  .(h.j....h&h.h'N
+00009740: 6829 4e75 6265 6817 7d94 2868 195d 9468  h)Nubeh.}.(h.].h
+00009750: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
+00009760: 6825 6851 6827 6850 6829 4bf2 6816 6ae1  h%hQh'hPh)K.h.j.
+00009770: 0800 0068 2668 0375 6268 5229 8194 7d94  ...h&h.ubhR)..}.
+00009780: 2868 058c 344f 7065 6e20 7468 6520 6272  (h..4Open the br
+00009790: 6f77 7365 7220 616e 6420 7479 7065 2060  owser and type `
+000097a0: 6068 7474 703a 2f2f 6c6f 6361 6c68 6f73  `http://localhos
+000097b0: 743a 3535 3535 6060 2e94 6807 5d94 2868  t:5555``..h.].(h
+000097c0: 118c 1a4f 7065 6e20 7468 6520 6272 6f77  ...Open the brow
+000097d0: 7365 7220 616e 6420 7479 7065 2094 8594  ser and type ...
+000097e0: 8194 7d94 2868 166a 1209 0000 6826 6803  ..}.(h.j....h&h.
+000097f0: 6827 4e68 294e 7562 6aee 0200 0029 8194  h'Nh)Nubj....)..
+00009800: 7d94 2868 058c 1960 6068 7474 703a 2f2f  }.(h...``http://
+00009810: 6c6f 6361 6c68 6f73 743a 3535 3535 6060  localhost:5555``
+00009820: 9468 075d 9468 118c 1568 7474 703a 2f2f  .h.].h...http://
+00009830: 6c6f 6361 6c68 6f73 743a 3535 3535 9485  localhost:5555..
+00009840: 9481 947d 9428 6816 6a1a 0900 0068 2668  ...}.(h.j....h&h
+00009850: 0368 274e 6829 4e75 6261 6817 7d94 2868  .h'Nh)Nubah.}.(h
+00009860: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
+00009870: 215d 9475 6825 6aed 0200 0068 166a 1209  !].uh%j....h.j..
+00009880: 0000 7562 6811 8c01 2e94 8594 8194 7d94  ..ubh.........}.
+00009890: 2868 166a 1209 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
+000098a0: 294e 7562 6568 177d 9428 6819 5d94 681b  )Nubeh.}.(h.].h.
+000098b0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+000098c0: 2568 5168 2768 5068 294b f468 166a e108  %hQh'hPh)K.h.j..
+000098d0: 0000 6826 6803 7562 6568 177d 9428 6819  ..h&h.ubeh.}.(h.
+000098e0: 5d94 8c0b 6465 7665 6c6f 706d 656e 7494  ]...development.
+000098f0: 6168 1b5d 9468 1d5d 948c 0b64 6576 656c  ah.].h.]...devel
+00009900: 6f70 6d65 6e74 9461 681f 5d94 6821 5d94  opment.ah.].h!].
+00009910: 7568 2568 2a68 166a 9008 0000 6826 6803  uh%h*h.j....h&h.
+00009920: 6827 6850 6829 4bf1 7562 682b 2981 947d  h'hPh)K.ubh+)..}
+00009930: 9428 6805 6806 6807 5d94 2868 3029 8194  .(h.h.h.].(h0)..
+00009940: 7d94 2868 058c 0542 7569 6c64 9468 075d  }.(h...Build.h.]
+00009950: 9468 118c 0542 7569 6c64 9485 9481 947d  .h...Build.....}
+00009960: 9428 6816 6a3d 0900 0068 2668 0368 274e  .(h.j=...h&h.h'N
+00009970: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
+00009980: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
+00009990: 6825 682f 6816 6a3a 0900 0068 2668 0368  h%h/h.j:...h&h.h
+000099a0: 2768 5068 294b f775 6268 5229 8194 7d94  'hPh)K.ubhR)..}.
+000099b0: 2868 058c 7454 6f20 6275 696c 6420 796f  (h..tTo build yo
+000099c0: 7572 2061 7070 6c69 6361 7469 6f6e 2c20  ur application, 
+000099d0: 7275 6e20 6060 7079 7468 6f6e 2061 7070  run ``python app
+000099e0: 2e70 7920 2d2d 6275 696c 6460 6020 696e  .py --build`` in
+000099f0: 2079 6f75 7220 7072 6f6a 6563 7420 726f   your project ro
+00009a00: 6f74 2064 6972 6563 746f 7279 2e20 5573  ot directory. Us
+00009a10: 6520 7468 6520 7465 726d 696e 616c 2069  e the terminal i
+00009a20: 6e20 7673 636f 6465 2e94 6807 5d94 2868  n vscode..h.].(h
+00009a30: 118c 1f54 6f20 6275 696c 6420 796f 7572  ...To build your
+00009a40: 2061 7070 6c69 6361 7469 6f6e 2c20 7275   application, ru
+00009a50: 6e20 9485 9481 947d 9428 6816 6a4b 0900  n .....}.(h.jK..
+00009a60: 0068 2668 0368 274e 6829 4e75 626a ee02  .h&h.h'Nh)Nubj..
+00009a70: 0000 2981 947d 9428 6805 8c19 6060 7079  ..)..}.(h...``py
+00009a80: 7468 6f6e 2061 7070 2e70 7920 2d2d 6275  thon app.py --bu
+00009a90: 696c 6460 6094 6807 5d94 6811 8c15 7079  ild``.h.].h...py
+00009aa0: 7468 6f6e 2061 7070 2e70 7920 2d2d 6275  thon app.py --bu
+00009ab0: 696c 6494 8594 8194 7d94 2868 166a 5309  ild.....}.(h.jS.
+00009ac0: 0000 6826 6803 6827 4e68 294e 7562 6168  ..h&h.h'Nh)Nubah
+00009ad0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00009ae0: 681f 5d94 6821 5d94 7568 256a ed02 0000  h.].h!].uh%j....
+00009af0: 6816 6a4b 0900 0075 6268 118c 3c20 696e  h.jK...ubh..< in
+00009b00: 2079 6f75 7220 7072 6f6a 6563 7420 726f   your project ro
+00009b10: 6f74 2064 6972 6563 746f 7279 2e20 5573  ot directory. Us
+00009b20: 6520 7468 6520 7465 726d 696e 616c 2069  e the terminal i
+00009b30: 6e20 7673 636f 6465 2e94 8594 8194 7d94  n vscode......}.
+00009b40: 2868 166a 4b09 0000 6826 6803 6827 4e68  (h.jK...h&h.h'Nh
+00009b50: 294e 7562 6568 177d 9428 6819 5d94 681b  )Nubeh.}.(h.].h.
+00009b60: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+00009b70: 2568 5168 2768 5068 294b f868 166a 3a09  %hQh'hPh)K.h.j:.
+00009b80: 0000 6826 6803 7562 6568 177d 9428 6819  ..h&h.ubeh.}.(h.
+00009b90: 5d94 8c05 6275 696c 6494 6168 1b5d 9468  ]...build.ah.].h
+00009ba0: 1d5d 948c 0562 7569 6c64 9461 681f 5d94  .]...build.ah.].
+00009bb0: 6821 5d94 7568 2568 2a68 166a 9008 0000  h!].uh%h*h.j....
+00009bc0: 6826 6803 6827 6850 6829 4bf7 7562 6568  h&h.h'hPh)K.ubeh
+00009bd0: 177d 9428 6819 5d94 8c19 7275 6e2d 6465  .}.(h.]...run-de
+00009be0: 7665 6c6f 706d 656e 742d 616e 642d 6275  velopment-and-bu
+00009bf0: 696c 6494 6168 1b5d 9468 1d5d 948c 1a72  ild.ah.].h.]...r
+00009c00: 756e 2c20 6465 7665 6c6f 706d 656e 7420  un, development 
+00009c10: 616e 6420 6275 696c 6494 6168 1f5d 9468  and build.ah.].h
+00009c20: 215d 9475 6825 682a 6816 6a92 0100 0068  !].uh%h*h.j....h
+00009c30: 2668 0368 2768 5068 294b eb75 6265 6817  &h.h'hPh)K.ubeh.
+00009c40: 7d94 2868 195d 948c 0b67 6574 2d73 7461  }.(h.]...get-sta
+00009c50: 7274 6564 9461 681b 5d94 681d 5d94 8c0b  rted.ah.].h.]...
+00009c60: 6765 7420 7374 6172 7465 6494 6168 1f5d  get started.ah.]
+00009c70: 9468 215d 9475 6825 682a 6816 682c 6826  .h!].uh%h*h.h,h&
+00009c80: 6803 6827 6850 6829 4b1a 7562 682b 2981  h.h'hPh)K.ubh+).
+00009c90: 947d 9428 6805 6806 6807 5d94 2868 3029  .}.(h.h.h.].(h0)
+00009ca0: 8194 7d94 2868 058c 1253 616d 706c 6520  ..}.(h...Sample 
+00009cb0: 6170 706c 6963 6174 696f 6e94 6807 5d94  application.h.].
+00009cc0: 6811 8c12 5361 6d70 6c65 2061 7070 6c69  h...Sample appli
+00009cd0: 6361 7469 6f6e 9485 9481 947d 9428 6816  cation.....}.(h.
+00009ce0: 6a86 0900 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00009cf0: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00009d00: 1d5d 9468 1f5d 9468 215d 9475 6825 682f  .].h.].h!].uh%h/
+00009d10: 6816 6a83 0900 0068 2668 0368 2768 5068  h.j....h&h.h'hPh
+00009d20: 294b fb75 6268 5229 8194 7d94 2868 058c  )K.ubhR)..}.(h..
+00009d30: 9e54 6f20 6265 7474 6572 2075 6e64 6572  .To better under
+00009d40: 7374 616e 6420 686f 7720 6465 636f 7265  stand how decore
+00009d50: 2062 6173 6520 776f 726b 732c 2069 7420   base works, it 
+00009d60: 6973 2062 6573 7420 746f 206c 6f6f 6b20  is best to look 
+00009d70: 6174 2074 6865 2073 616d 706c 6520 6170  at the sample ap
+00009d80: 706c 6963 6174 696f 6e2e 2054 6865 2061  plication. The a
+00009d90: 7070 6c69 6361 7469 6f6e 2072 6570 7265  pplication repre
+00009da0: 7365 6e74 7320 6d79 2063 6f6e 7469 6e75  sents my continu
+00009db0: 6f75 7320 6465 7665 6c6f 706d 656e 7420  ous development 
+00009dc0: 6f66 2064 6563 6f72 6520 6261 7365 2e94  of decore base..
+00009dd0: 6807 5d94 6811 8c9e 546f 2062 6574 7465  h.].h...To bette
+00009de0: 7220 756e 6465 7273 7461 6e64 2068 6f77  r understand how
+00009df0: 2064 6563 6f72 6520 6261 7365 2077 6f72   decore base wor
+00009e00: 6b73 2c20 6974 2069 7320 6265 7374 2074  ks, it is best t
+00009e10: 6f20 6c6f 6f6b 2061 7420 7468 6520 7361  o look at the sa
+00009e20: 6d70 6c65 2061 7070 6c69 6361 7469 6f6e  mple application
+00009e30: 2e20 5468 6520 6170 706c 6963 6174 696f  . The applicatio
+00009e40: 6e20 7265 7072 6573 656e 7473 206d 7920  n represents my 
+00009e50: 636f 6e74 696e 756f 7573 2064 6576 656c  continuous devel
+00009e60: 6f70 6d65 6e74 206f 6620 6465 636f 7265  opment of decore
+00009e70: 2062 6173 652e 9485 9481 947d 9428 6816   base......}.(h.
+00009e80: 6a94 0900 0068 2668 0368 274e 6829 4e75  j....h&h.h'Nh)Nu
+00009e90: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00009ea0: 1d5d 9468 1f5d 9468 215d 9475 6825 6851  .].h.].h!].uh%hQ
+00009eb0: 6827 6850 6829 4bfc 6816 6a83 0900 0068  h'hPh)K.h.j....h
+00009ec0: 2668 0375 6268 5229 8194 7d94 2868 058c  &h.ubhR)..}.(h..
+00009ed0: 4868 7474 7073 3a2f 2f67 6974 6875 622e  Hhttps://github.
+00009ee0: 636f 6d2f 4b65 6d6f 5061 6e7a 6168 2f64  com/KemoPanzah/d
+00009ef0: 6563 6f72 655f 4261 7365 2f74 7265 652f  ecore_Base/tree/
+00009f00: 6d61 7374 6572 2f64 6563 6f72 655f 6261  master/decore_ba
+00009f10: 7365 2f73 616d 706c 6594 6807 5d94 6892  se/sample.h.].h.
+00009f20: 2981 947d 9428 6805 6aa4 0900 0068 075d  )..}.(h.j....h.]
+00009f30: 9468 118c 4868 7474 7073 3a2f 2f67 6974  .h..Hhttps://git
+00009f40: 6875 622e 636f 6d2f 4b65 6d6f 5061 6e7a  hub.com/KemoPanz
+00009f50: 6168 2f64 6563 6f72 655f 4261 7365 2f74  ah/decore_Base/t
+00009f60: 7265 652f 6d61 7374 6572 2f64 6563 6f72  ree/master/decor
+00009f70: 655f 6261 7365 2f73 616d 706c 6594 8594  e_base/sample...
+00009f80: 8194 7d94 2868 166a a609 0000 6826 6803  ..}.(h.j....h&h.
+00009f90: 6827 4e68 294e 7562 6168 177d 9428 6819  h'Nh)Nubah.}.(h.
+00009fa0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+00009fb0: 5d94 8c06 7265 6675 7269 946a a409 0000  ]...refuri.j....
+00009fc0: 7568 2568 9168 166a a209 0000 7562 6168  uh%h.h.j....ubah
+00009fd0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00009fe0: 681f 5d94 6821 5d94 7568 2568 5168 2768  h.].h!].uh%hQh'h
+00009ff0: 5068 294b fe68 166a 8309 0000 6826 6803  Ph)K.h.j....h&h.
+0000a000: 7562 6852 2981 947d 9428 6805 8cb0 546f  ubhR)..}.(h...To
+0000a010: 2073 796e 6368 726f 6e69 7a65 2074 6865   synchronize the
+0000a020: 2073 616d 706c 6520 6170 706c 6963 6174   sample applicat
+0000a030: 696f 6e20 7769 7468 2061 2073 7562 666f  ion with a subfo
+0000a040: 6c64 6572 206f 6620 7468 6520 7072 6f6a  lder of the proj
+0000a050: 6563 7420 726f 6f74 2064 6972 6563 746f  ect root directo
+0000a060: 7279 2c20 7275 6e20 6060 7079 7468 6f6e  ry, run ``python
+0000a070: 2061 7070 2e70 7920 2d2d 7361 6d70 6c65   app.py --sample
+0000a080: 6060 2069 6e20 796f 7572 2070 726f 6a65  `` in your proje
+0000a090: 6374 2072 6f6f 7420 6469 7265 6374 6f72  ct root director
+0000a0a0: 792e 2055 7365 2074 6865 2074 6572 6d69  y. Use the termi
+0000a0b0: 6e61 6c20 696e 2076 7363 6f64 652e 9468  nal in vscode..h
+0000a0c0: 075d 9428 6811 8c5a 546f 2073 796e 6368  .].(h..ZTo synch
+0000a0d0: 726f 6e69 7a65 2074 6865 2073 616d 706c  ronize the sampl
+0000a0e0: 6520 6170 706c 6963 6174 696f 6e20 7769  e application wi
+0000a0f0: 7468 2061 2073 7562 666f 6c64 6572 206f  th a subfolder o
+0000a100: 6620 7468 6520 7072 6f6a 6563 7420 726f  f the project ro
+0000a110: 6f74 2064 6972 6563 746f 7279 2c20 7275  ot directory, ru
+0000a120: 6e20 9485 9481 947d 9428 6816 6aba 0900  n .....}.(h.j...
+0000a130: 0068 2668 0368 274e 6829 4e75 626a ee02  .h&h.h'Nh)Nubj..
+0000a140: 0000 2981 947d 9428 6805 8c1a 6060 7079  ..)..}.(h...``py
+0000a150: 7468 6f6e 2061 7070 2e70 7920 2d2d 7361  thon app.py --sa
+0000a160: 6d70 6c65 6060 9468 075d 9468 118c 1670  mple``.h.].h...p
+0000a170: 7974 686f 6e20 6170 702e 7079 202d 2d73  ython app.py --s
+0000a180: 616d 706c 6594 8594 8194 7d94 2868 166a  ample.....}.(h.j
+0000a190: c209 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
+0000a1a0: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
+0000a1b0: 5d94 681f 5d94 6821 5d94 7568 256a ed02  ].h.].h!].uh%j..
+0000a1c0: 0000 6816 6aba 0900 0075 6268 118c 3c20  ..h.j....ubh..< 
+0000a1d0: 696e 2079 6f75 7220 7072 6f6a 6563 7420  in your project 
+0000a1e0: 726f 6f74 2064 6972 6563 746f 7279 2e20  root directory. 
+0000a1f0: 5573 6520 7468 6520 7465 726d 696e 616c  Use the terminal
+0000a200: 2069 6e20 7673 636f 6465 2e94 8594 8194   in vscode......
+0000a210: 7d94 2868 166a ba09 0000 6826 6803 6827  }.(h.j....h&h.h'
+0000a220: 4e68 294e 7562 6568 177d 9428 6819 5d94  Nh)Nubeh.}.(h.].
+0000a230: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
+0000a240: 7568 2568 5168 2768 5068 294d 0001 6816  uh%hQh'hPh)M..h.
+0000a250: 6a83 0900 0068 2668 0375 6268 5229 8194  j....h&h.ubhR)..
+0000a260: 7d94 2868 058c 7f54 6f20 7275 6e20 7468  }.(h...To run th
+0000a270: 6520 7361 6d70 6c65 2061 7070 6c69 6361  e sample applica
+0000a280: 7469 6f6e 2061 6674 6572 2073 796e 6368  tion after synch
+0000a290: 726f 6e69 7a61 7469 6f6e 2c20 7573 6520  ronization, use 
+0000a2a0: 796f 7572 2064 6562 7567 6765 7220 7769  your debugger wi
+0000a2b0: 7468 2074 6865 2060 605b 736d 705d 2064  th the ``[smp] d
+0000a2c0: 6563 6f72 6520 6261 7365 2073 616d 706c  ecore base sampl
+0000a2d0: 6560 6020 7072 6f66 696c 6520 696e 2076  e`` profile in v
+0000a2e0: 7363 6f64 652e 9468 075d 9428 6811 8c50  scode..h.].(h..P
 0000a2f0: 546f 2072 756e 2074 6865 2073 616d 706c  To run the sampl
 0000a300: 6520 6170 706c 6963 6174 696f 6e20 6166  e application af
 0000a310: 7465 7220 7379 6e63 6872 6f6e 697a 6174  ter synchronizat
 0000a320: 696f 6e2c 2075 7365 2079 6f75 7220 6465  ion, use your de
 0000a330: 6275 6767 6572 2077 6974 6820 7468 6520  bugger with the 
-0000a340: 6060 5b73 6d70 5d20 6465 636f 7265 2062  ``[smp] decore b
-0000a350: 6173 6520 7361 6d70 6c65 6060 2070 726f  ase sample`` pro
-0000a360: 6669 6c65 2069 6e20 7673 636f 6465 2e94  file in vscode..
-0000a370: 6807 5d94 2868 118c 5054 6f20 7275 6e20  h.].(h..PTo run 
-0000a380: 7468 6520 7361 6d70 6c65 2061 7070 6c69  the sample appli
-0000a390: 6361 7469 6f6e 2061 6674 6572 2073 796e  cation after syn
-0000a3a0: 6368 726f 6e69 7a61 7469 6f6e 2c20 7573  chronization, us
-0000a3b0: 6520 796f 7572 2064 6562 7567 6765 7220  e your debugger 
-0000a3c0: 7769 7468 2074 6865 2094 8594 8194 7d94  with the .....}.
-0000a3d0: 2868 166a da09 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
-0000a3e0: 294e 7562 6aee 0200 0029 8194 7d94 2868  )Nubj....)..}.(h
-0000a3f0: 058c 1c60 605b 736d 705d 2064 6563 6f72  ...``[smp] decor
-0000a400: 6520 6261 7365 2073 616d 706c 6560 6094  e base sample``.
-0000a410: 6807 5d94 6811 8c18 5b73 6d70 5d20 6465  h.].h...[smp] de
-0000a420: 636f 7265 2062 6173 6520 7361 6d70 6c65  core base sample
-0000a430: 9485 9481 947d 9428 6816 6ae2 0900 0068  .....}.(h.j....h
-0000a440: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-0000a450: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-0000a460: 9468 215d 9475 6825 6aed 0200 0068 166a  .h!].uh%j....h.j
-0000a470: da09 0000 7562 6811 8c13 2070 726f 6669  ....ubh... profi
-0000a480: 6c65 2069 6e20 7673 636f 6465 2e94 8594  le in vscode....
-0000a490: 8194 7d94 2868 166a da09 0000 6826 6803  ..}.(h.j....h&h.
-0000a4a0: 6827 4e68 294e 7562 6568 177d 9428 6819  h'Nh)Nubeh.}.(h.
-0000a4b0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-0000a4c0: 5d94 7568 2568 5168 2768 5068 294d 0401  ].uh%hQh'hPh)M..
-0000a4d0: 6816 6a83 0900 0068 2668 0375 6265 6817  h.j....h&h.ubeh.
-0000a4e0: 7d94 2868 195d 948c 1273 616d 706c 652d  }.(h.]...sample-
-0000a4f0: 6170 706c 6963 6174 696f 6e94 6168 1b5d  application.ah.]
-0000a500: 9468 1d5d 948c 1273 616d 706c 6520 6170  .h.]...sample ap
-0000a510: 706c 6963 6174 696f 6e94 6168 1f5d 9468  plication.ah.].h
-0000a520: 215d 9475 6825 682a 6816 682c 6826 6803  !].uh%h*h.h,h&h.
-0000a530: 6827 6850 6829 4bfd 7562 682b 2981 947d  h'hPh)K.ubh+)..}
-0000a540: 9428 6805 6806 6807 5d94 2868 3029 8194  .(h.h.h.].(h0)..
-0000a550: 7d94 2868 058c 054e 6f74 6573 9468 075d  }.(h...Notes.h.]
-0000a560: 9468 118c 054e 6f74 6573 9485 9481 947d  .h...Notes.....}
-0000a570: 9428 6816 6a05 0a00 0068 2668 0368 274e  .(h.j....h&h.h'N
-0000a580: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
-0000a590: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9475  .].h.].h.].h!].u
-0000a5a0: 6825 682f 6816 6a02 0a00 0068 2668 0368  h%h/h.j....h&h.h
-0000a5b0: 2768 5068 294d 0701 7562 6852 2981 947d  'hPh)M..ubhR)..}
-0000a5c0: 9428 6805 8c46 5468 6973 2064 6f63 756d  .(h..FThis docum
-0000a5d0: 656e 7461 7469 6f6e 2077 6173 2074 7261  entation was tra
-0000a5e0: 6e73 6c61 7465 6420 6672 6f6d 2047 6572  nslated from Ger
-0000a5f0: 6d61 6e20 696e 746f 2045 6e67 6c69 7368  man into English
-0000a600: 2077 6974 6820 4465 6570 6c2e 9468 075d   with Deepl..h.]
-0000a610: 9468 118c 4654 6869 7320 646f 6375 6d65  .h..FThis docume
-0000a620: 6e74 6174 696f 6e20 7761 7320 7472 616e  ntation was tran
-0000a630: 736c 6174 6564 2066 726f 6d20 4765 726d  slated from Germ
-0000a640: 616e 2069 6e74 6f20 456e 676c 6973 6820  an into English 
-0000a650: 7769 7468 2044 6565 706c 2e94 8594 8194  with Deepl......
-0000a660: 7d94 2868 166a 130a 0000 6826 6803 6827  }.(h.j....h&h.h'
-0000a670: 4e68 294e 7562 6168 177d 9428 6819 5d94  Nh)Nubah.}.(h.].
-0000a680: 681b 5d94 681d 5d94 681f 5d94 6821 5d94  h.].h.].h.].h!].
-0000a690: 7568 2568 5168 2768 5068 294d 0801 6816  uh%hQh'hPh)M..h.
-0000a6a0: 6a02 0a00 0068 2668 0375 6268 098c 0863  j....h&h.ubh...c
-0000a6b0: 6f6d 706f 756e 6494 9394 2981 947d 9428  ompound...)..}.(
-0000a6c0: 6805 6806 6807 5d94 6800 8c07 746f 6374  h.h.h.].h...toct
-0000a6d0: 7265 6594 9394 2981 947d 9428 6805 6806  ree...)..}.(h.h.
-0000a6e0: 6807 5d94 6817 7d94 2868 195d 9468 1b5d  h.].h.}.(h.].h.]
-0000a6f0: 9468 1d5d 9468 1f5d 9468 215d 9468 168c  .h.].h.].h!].h..
-0000a700: 0569 6e64 6578 948c 0765 6e74 7269 6573  .index...entries
-0000a710: 945d 948c 0c69 6e63 6c75 6465 6669 6c65  .]...includefile
-0000a720: 7394 5d94 8c08 6d61 7864 6570 7468 944b  s.]...maxdepth.K
-0000a730: 028c 0763 6170 7469 6f6e 944e 8c04 676c  ...caption.N..gl
-0000a740: 6f62 9489 8c06 6869 6464 656e 9488 8c0d  ob....hidden....
-0000a750: 696e 636c 7564 6568 6964 6465 6e94 898c  includehidden...
-0000a760: 086e 756d 6265 7265 6494 4b00 8c0a 7469  .numbered.K...ti
-0000a770: 746c 6573 6f6e 6c79 9489 8c0a 7261 7765  tlesonly....rawe
-0000a780: 6e74 7269 6573 945d 9475 6825 6a26 0a00  ntries.].uh%j&..
-0000a790: 0068 2768 2868 294b 0b68 166a 230a 0000  .h'h(h)K.h.j#...
-0000a7a0: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
-0000a7b0: 8c0f 746f 6374 7265 652d 7772 6170 7065  ..toctree-wrappe
-0000a7c0: 7294 6168 1d5d 9468 1f5d 9468 215d 9475  r.ah.].h.].h!].u
-0000a7d0: 6825 6a21 0a00 0068 166a 020a 0000 6826  h%j!...h.j....h&
-0000a7e0: 6803 6827 6828 6829 4e75 6268 0b29 8194  h.h'h(h)Nubh.)..
-0000a7f0: 7d94 2868 058c 1249 6e64 6963 6573 2061  }.(h...Indices a
-0000a800: 6e64 2074 6162 6c65 7394 6807 5d94 6811  nd tables.h.].h.
-0000a810: 8c12 496e 6469 6365 7320 616e 6420 7461  ..Indices and ta
-0000a820: 626c 6573 9485 9481 947d 9468 166a 460a  bles.....}.h.jF.
-0000a830: 0000 7362 6168 177d 9428 6819 5d94 681b  ..sbah.}.(h.].h.
-0000a840: 5d94 681d 5d94 681f 5d94 6821 5d94 6823  ].h.].h.].h!].h#
-0000a850: 6824 7568 2568 0a68 166a 020a 0000 6826  h$uh%h.h.j....h&
-0000a860: 6803 6827 6828 6829 4b0f 7562 680b 2981  h.h'h(h)K.ubh.).
-0000a870: 947d 9428 6805 8c12 3d3d 3d3d 3d3d 3d3d  .}.(h...========
-0000a880: 3d3d 3d3d 3d3d 3d3d 3d3d 9468 075d 9468  ==========.h.].h
-0000a890: 118c 123d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ...=============
-0000a8a0: 3d3d 3d3d 3d94 8594 8194 7d94 6816 6a54  =====.....}.h.jT
-0000a8b0: 0a00 0073 6261 6817 7d94 2868 195d 9468  ...sbah.}.(h.].h
-0000a8c0: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9468  .].h.].h.].h!].h
-0000a8d0: 2368 2475 6825 680a 6816 6a02 0a00 0068  #h$uh%h.h.j....h
-0000a8e0: 2668 0368 2768 2868 294b 1175 6268 0b29  &h.h'h(h)K.ubh.)
-0000a8f0: 8194 7d94 2868 058c 112a 203a 7265 663a  ..}.(h...* :ref:
-0000a900: 6067 656e 696e 6465 7860 9468 075d 9468  `genindex`.h.].h
-0000a910: 118c 112a 203a 7265 663a 6067 656e 696e  ...* :ref:`genin
-0000a920: 6465 7860 9485 9481 947d 9468 166a 620a  dex`.....}.h.jb.
-0000a930: 0000 7362 6168 177d 9428 6819 5d94 681b  ..sbah.}.(h.].h.
-0000a940: 5d94 681d 5d94 681f 5d94 6821 5d94 6823  ].h.].h.].h!].h#
-0000a950: 6824 7568 2568 0a68 166a 020a 0000 6826  h$uh%h.h.j....h&
-0000a960: 6803 6827 6828 6829 4b12 7562 680b 2981  h.h'h(h)K.ubh.).
-0000a970: 947d 9428 6805 8c11 2a20 3a72 6566 3a60  .}.(h...* :ref:`
-0000a980: 6d6f 6469 6e64 6578 6094 6807 5d94 6811  modindex`.h.].h.
-0000a990: 8c11 2a20 3a72 6566 3a60 6d6f 6469 6e64  ..* :ref:`modind
-0000a9a0: 6578 6094 8594 8194 7d94 6816 6a70 0a00  ex`.....}.h.jp..
-0000a9b0: 0073 6261 6817 7d94 2868 195d 9468 1b5d  .sbah.}.(h.].h.]
-0000a9c0: 9468 1d5d 9468 1f5d 9468 215d 9468 2368  .h.].h.].h!].h#h
-0000a9d0: 2475 6825 680a 6816 6a02 0a00 0068 2668  $uh%h.h.j....h&h
-0000a9e0: 0368 2768 2868 294b 1375 6268 0b29 8194  .h'h(h)K.ubh.)..
-0000a9f0: 7d94 2868 058c 0f2a 203a 7265 663a 6073  }.(h...* :ref:`s
-0000aa00: 6561 7263 6860 9468 075d 9468 118c 0f2a  earch`.h.].h...*
-0000aa10: 203a 7265 663a 6073 6561 7263 6860 9485   :ref:`search`..
-0000aa20: 9481 947d 9468 166a 7e0a 0000 7362 6168  ...}.h.j~...sbah
-0000aa30: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
-0000aa40: 681f 5d94 6821 5d94 6823 6824 7568 2568  h.].h!].h#h$uh%h
-0000aa50: 0a68 166a 020a 0000 6826 6803 6827 6828  .h.j....h&h.h'h(
-0000aa60: 6829 4b14 7562 6568 177d 9428 6819 5d94  h)K.ubeh.}.(h.].
-0000aa70: 8c05 6e6f 7465 7394 6168 1b5d 9468 1d5d  ..notes.ah.].h.]
-0000aa80: 948c 056e 6f74 6573 9461 681f 5d94 6821  ...notes.ah.].h!
-0000aa90: 5d94 7568 2568 2a68 1668 2c68 2668 0368  ].uh%h*h.h,h&h.h
-0000aaa0: 2768 5068 294d 0701 7562 6568 177d 9428  'hPh)M..ubeh.}.(
-0000aab0: 6819 5d94 8c07 7765 6c63 6f6d 6594 6168  h.]...welcome.ah
-0000aac0: 1b5d 9468 1d5d 948c 0777 656c 636f 6d65  .].h.]...welcome
-0000aad0: 9461 681f 5d94 6821 5d94 7568 2568 2a68  .ah.].h!].uh%h*h
-0000aae0: 1668 0368 2668 0368 2768 2868 294b 0775  .h.h&h.h'h(h)K.u
-0000aaf0: 6265 6817 7d94 2868 195d 9468 1b5d 9468  beh.}.(h.].h.].h
-0000ab00: 1d5d 9468 1f5d 9468 215d 948c 0673 6f75  .].h.].h!]...sou
-0000ab10: 7263 6594 6828 7568 2568 018c 0e63 7572  rce.h(uh%h...cur
-0000ab20: 7265 6e74 5f73 6f75 7263 6594 4e8c 0c63  rent_source.N..c
-0000ab30: 7572 7265 6e74 5f6c 696e 6594 4e8c 0873  urrent_line.N..s
-0000ab40: 6574 7469 6e67 7394 8c11 646f 6375 7469  ettings...docuti
-0000ab50: 6c73 2e66 726f 6e74 656e 6494 8c06 5661  ls.frontend...Va
-0000ab60: 6c75 6573 9493 9429 8194 7d94 2868 2f4e  lues...)..}.(h/N
-0000ab70: 8c09 6765 6e65 7261 746f 7294 4e8c 0964  ..generator.N..d
-0000ab80: 6174 6573 7461 6d70 944e 8c0b 736f 7572  atestamp.N..sour
-0000ab90: 6365 5f6c 696e 6b94 4e8c 0a73 6f75 7263  ce_link.N..sourc
-0000aba0: 655f 7572 6c94 4e8c 0d74 6f63 5f62 6163  e_url.N..toc_bac
-0000abb0: 6b6c 696e 6b73 948c 0565 6e74 7279 948c  klinks...entry..
-0000abc0: 1266 6f6f 746e 6f74 655f 6261 636b 6c69  .footnote_backli
-0000abd0: 6e6b 7394 4b01 8c0d 7365 6374 6e75 6d5f  nks.K...sectnum_
-0000abe0: 7866 6f72 6d94 4b01 8c0e 7374 7269 705f  xform.K...strip_
-0000abf0: 636f 6d6d 656e 7473 944e 8c1b 7374 7269  comments.N..stri
-0000ac00: 705f 656c 656d 656e 7473 5f77 6974 685f  p_elements_with_
-0000ac10: 636c 6173 7365 7394 4e8c 0d73 7472 6970  classes.N..strip
-0000ac20: 5f63 6c61 7373 6573 944e 8c0c 7265 706f  _classes.N..repo
-0000ac30: 7274 5f6c 6576 656c 944b 028c 0a68 616c  rt_level.K...hal
-0000ac40: 745f 6c65 7665 6c94 4b05 8c11 6578 6974  t_level.K...exit
-0000ac50: 5f73 7461 7475 735f 6c65 7665 6c94 4b05  _status_level.K.
-0000ac60: 8c05 6465 6275 6794 4e8c 0e77 6172 6e69  ..debug.N..warni
-0000ac70: 6e67 5f73 7472 6561 6d94 4e8c 0974 7261  ng_stream.N..tra
-0000ac80: 6365 6261 636b 9488 8c0e 696e 7075 745f  ceback....input_
-0000ac90: 656e 636f 6469 6e67 948c 0975 7466 2d38  encoding...utf-8
-0000aca0: 2d73 6967 948c 1c69 6e70 7574 5f65 6e63  -sig...input_enc
-0000acb0: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-0000acc0: 6c65 7294 8c06 7374 7269 6374 948c 0f6f  ler...strict...o
-0000acd0: 7574 7075 745f 656e 636f 6469 6e67 948c  utput_encoding..
-0000ace0: 0575 7466 2d38 948c 1d6f 7574 7075 745f  .utf-8...output_
-0000acf0: 656e 636f 6469 6e67 5f65 7272 6f72 5f68  encoding_error_h
-0000ad00: 616e 646c 6572 946a bf0a 0000 8c0e 6572  andler.j......er
-0000ad10: 726f 725f 656e 636f 6469 6e67 948c 0575  ror_encoding...u
-0000ad20: 7466 2d38 948c 1c65 7272 6f72 5f65 6e63  tf-8...error_enc
-0000ad30: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-0000ad40: 6c65 7294 8c10 6261 636b 736c 6173 6872  ler...backslashr
-0000ad50: 6570 6c61 6365 948c 0d6c 616e 6775 6167  eplace...languag
-0000ad60: 655f 636f 6465 948c 0265 6e94 8c13 7265  e_code...en...re
-0000ad70: 636f 7264 5f64 6570 656e 6465 6e63 6965  cord_dependencie
-0000ad80: 7394 4e8c 0663 6f6e 6669 6794 4e8c 0969  s.N..config.N..i
-0000ad90: 645f 7072 6566 6978 9468 068c 0e61 7574  d_prefix.h...aut
-0000ada0: 6f5f 6964 5f70 7265 6669 7894 8c02 6964  o_id_prefix...id
-0000adb0: 948c 0d64 756d 705f 7365 7474 696e 6773  ...dump_settings
-0000adc0: 944e 8c0e 6475 6d70 5f69 6e74 6572 6e61  .N..dump_interna
-0000add0: 6c73 944e 8c0f 6475 6d70 5f74 7261 6e73  ls.N..dump_trans
-0000ade0: 666f 726d 7394 4e8c 0f64 756d 705f 7073  forms.N..dump_ps
-0000adf0: 6575 646f 5f78 6d6c 944e 8c10 6578 706f  eudo_xml.N..expo
-0000ae00: 7365 5f69 6e74 6572 6e61 6c73 944e 8c0e  se_internals.N..
-0000ae10: 7374 7269 6374 5f76 6973 6974 6f72 944e  strict_visitor.N
-0000ae20: 8c0f 5f64 6973 6162 6c65 5f63 6f6e 6669  .._disable_confi
-0000ae30: 6794 4e8c 075f 736f 7572 6365 9468 288c  g.N.._source.h(.
-0000ae40: 0c5f 6465 7374 696e 6174 696f 6e94 4e8c  ._destination.N.
-0000ae50: 0d5f 636f 6e66 6967 5f66 696c 6573 945d  ._config_files.]
-0000ae60: 948c 1666 696c 655f 696e 7365 7274 696f  ...file_insertio
-0000ae70: 6e5f 656e 6162 6c65 6494 888c 0b72 6177  n_enabled....raw
-0000ae80: 5f65 6e61 626c 6564 944b 018c 116c 696e  _enabled.K...lin
-0000ae90: 655f 6c65 6e67 7468 5f6c 696d 6974 944d  e_length_limit.M
-0000aea0: 1027 8c0e 7065 705f 7265 6665 7265 6e63  .'..pep_referenc
-0000aeb0: 6573 944e 8c0c 7065 705f 6261 7365 5f75  es.N..pep_base_u
-0000aec0: 726c 948c 1868 7474 7073 3a2f 2f70 6570  rl...https://pep
-0000aed0: 732e 7079 7468 6f6e 2e6f 7267 2f94 8c15  s.python.org/...
-0000aee0: 7065 705f 6669 6c65 5f75 726c 5f74 656d  pep_file_url_tem
-0000aef0: 706c 6174 6594 8c08 7065 702d 2530 3464  plate...pep-%04d
-0000af00: 948c 0e72 6663 5f72 6566 6572 656e 6365  ...rfc_reference
-0000af10: 7394 4e8c 0c72 6663 5f62 6173 655f 7572  s.N..rfc_base_ur
-0000af20: 6c94 8c26 6874 7470 733a 2f2f 6461 7461  l..&https://data
-0000af30: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
-0000af40: 2f64 6f63 2f68 746d 6c2f 948c 0974 6162  /doc/html/...tab
-0000af50: 5f77 6964 7468 944b 088c 1d74 7269 6d5f  _width.K...trim_
-0000af60: 666f 6f74 6e6f 7465 5f72 6566 6572 656e  footnote_referen
-0000af70: 6365 5f73 7061 6365 9489 8c10 7379 6e74  ce_space....synt
-0000af80: 6178 5f68 6967 686c 6967 6874 948c 046c  ax_highlight...l
-0000af90: 6f6e 6794 8c0c 736d 6172 745f 7175 6f74  ong...smart_quot
-0000afa0: 6573 9488 8c13 736d 6172 7471 756f 7465  es....smartquote
-0000afb0: 735f 6c6f 6361 6c65 7394 5d94 8c1d 6368  s_locales.]...ch
-0000afc0: 6172 6163 7465 725f 6c65 7665 6c5f 696e  aracter_level_in
-0000afd0: 6c69 6e65 5f6d 6172 6b75 7094 898c 0e64  line_markup....d
-0000afe0: 6f63 7469 746c 655f 7866 6f72 6d94 898c  octitle_xform...
-0000aff0: 0d64 6f63 696e 666f 5f78 666f 726d 944b  .docinfo_xform.K
-0000b000: 018c 1273 6563 7473 7562 7469 746c 655f  ...sectsubtitle_
-0000b010: 7866 6f72 6d94 898c 0d69 6d61 6765 5f6c  xform....image_l
-0000b020: 6f61 6469 6e67 948c 046c 696e 6b94 8c10  oading...link...
-0000b030: 656d 6265 645f 7374 796c 6573 6865 6574  embed_stylesheet
-0000b040: 9489 8c15 636c 6f61 6b5f 656d 6169 6c5f  ....cloak_email_
-0000b050: 6164 6472 6573 7365 7394 888c 1173 6563  addresses....sec
-0000b060: 7469 6f6e 5f73 656c 665f 6c69 6e6b 9489  tion_self_link..
-0000b070: 8c03 656e 7694 4e75 628c 0872 6570 6f72  ..env.Nub..repor
-0000b080: 7465 7294 4e8c 1069 6e64 6972 6563 745f  ter.N..indirect_
-0000b090: 7461 7267 6574 7394 5d94 8c11 7375 6273  targets.]...subs
-0000b0a0: 7469 7475 7469 6f6e 5f64 6566 7394 7d94  titution_defs.}.
-0000b0b0: 8c12 7375 6273 7469 7475 7469 6f6e 5f6e  ..substitution_n
-0000b0c0: 616d 6573 947d 948c 0872 6566 6e61 6d65  ames.}...refname
-0000b0d0: 7394 7d94 8c06 7265 6669 6473 947d 948c  s.}...refids.}..
-0000b0e0: 076e 616d 6569 6473 947d 9428 6a99 0a00  .nameids.}.(j...
-0000b0f0: 006a 960a 0000 68dd 68da 68af 68ac 6a8f  .j....h.h.h.h.j.
-0000b100: 0100 006a 8c01 0000 6a80 0100 006a 7d01  ...j....j....j}.
-0000b110: 0000 6a80 0900 006a 7d09 0000 6a61 0200  ..j....j}...ja..
-0000b120: 006a 5e02 0000 6a4e 0200 006a 4b02 0000  .j^...jN...jK...
-0000b130: 6a1e 0300 006a 1b03 0000 6a8d 0800 006a  j....j....j....j
-0000b140: 8a08 0000 6a30 0500 006a 2d05 0000 6afe  ....j0...j-...j.
-0000b150: 0400 006a fb04 0000 6a64 0600 006a 6106  ...j....jd...ja.
-0000b160: 0000 6adb 0600 006a d806 0000 6a52 0700  ..j....j....jR..
-0000b170: 006a 4f07 0000 6a97 0700 006a 9407 0000  .jO...j....j....
-0000b180: 6a85 0800 006a 8208 0000 6a78 0900 006a  j....j....jx...j
-0000b190: 7509 0000 6a37 0900 006a 3409 0000 6a70  u...j7...j4...jp
-0000b1a0: 0900 006a 6d09 0000 6aff 0900 006a fc09  ...jm...j....j..
-0000b1b0: 0000 6a91 0a00 006a 8e0a 0000 758c 096e  ..j....j....u..n
-0000b1c0: 616d 6574 7970 6573 947d 9428 6a99 0a00  ametypes.}.(j...
-0000b1d0: 0089 68dd 8968 af88 6a8f 0100 0089 6a80  ..h..h..j.....j.
-0000b1e0: 0100 0088 6a80 0900 0089 6a61 0200 0089  ....j.....ja....
-0000b1f0: 6a4e 0200 0088 6a1e 0300 0089 6a8d 0800  jN....j.....j...
-0000b200: 0089 6a30 0500 0089 6afe 0400 0088 6a64  ..j0....j.....jd
-0000b210: 0600 0089 6adb 0600 0089 6a52 0700 0089  ....j.....jR....
-0000b220: 6a97 0700 0089 6a85 0800 0089 6a78 0900  j.....j.....jx..
-0000b230: 0089 6a37 0900 0089 6a70 0900 0089 6aff  ..j7....jp....j.
-0000b240: 0900 0089 6a91 0a00 0089 7568 197d 9428  ....j.....uh.}.(
-0000b250: 6a96 0a00 0068 2c68 da68 3f68 ac68 a66a  j....h,h.h?h.h.j
-0000b260: 8c01 0000 68e0 6a7d 0100 006a 7701 0000  ....h.j}...jw...
-0000b270: 6a7d 0900 006a 9201 0000 6a5e 0200 006a  j}...j....j^...j
-0000b280: ea01 0000 6a4b 0200 006a 4502 0000 6a1b  ....jK...jE...j.
-0000b290: 0300 006a 6402 0000 6a8a 0800 006a 2103  ...jd...j....j!.
-0000b2a0: 0000 6a2d 0500 006a 0804 0000 6afb 0400  ..j-...j....j...
-0000b2b0: 006a f504 0000 6a61 0600 006a 3305 0000  .j....ja...j3...
-0000b2c0: 6ad8 0600 006a 6706 0000 6a4f 0700 006a  j....jg...jO...j
-0000b2d0: de06 0000 6a94 0700 006a 5507 0000 6a82  ....j....jU...j.
-0000b2e0: 0800 006a 9a07 0000 6a75 0900 006a 9008  ...j....ju...j..
-0000b2f0: 0000 6a34 0900 006a e108 0000 6a6d 0900  ..j4...j....jm..
-0000b300: 006a 3a09 0000 6afc 0900 006a 8309 0000  .j:...j....j....
-0000b310: 6a8e 0a00 006a 020a 0000 758c 0d66 6f6f  j....j....u..foo
-0000b320: 746e 6f74 655f 7265 6673 947d 948c 0d63  tnote_refs.}...c
-0000b330: 6974 6174 696f 6e5f 7265 6673 947d 948c  itation_refs.}..
-0000b340: 0d61 7574 6f66 6f6f 746e 6f74 6573 945d  .autofootnotes.]
-0000b350: 948c 1161 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
-0000b360: 7265 6673 945d 948c 1073 796d 626f 6c5f  refs.]...symbol_
-0000b370: 666f 6f74 6e6f 7465 7394 5d94 8c14 7379  footnotes.]...sy
-0000b380: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7265  mbol_footnote_re
-0000b390: 6673 945d 948c 0966 6f6f 746e 6f74 6573  fs.]...footnotes
-0000b3a0: 945d 948c 0963 6974 6174 696f 6e73 945d  .]...citations.]
-0000b3b0: 948c 1261 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
-0000b3c0: 7374 6172 7494 4b01 8c15 7379 6d62 6f6c  start.K...symbol
-0000b3d0: 5f66 6f6f 746e 6f74 655f 7374 6172 7494  _footnote_start.
-0000b3e0: 4b00 8c0a 6964 5f63 6f75 6e74 6572 948c  K...id_counter..
-0000b3f0: 0b63 6f6c 6c65 6374 696f 6e73 948c 0743  .collections...C
-0000b400: 6f75 6e74 6572 9493 947d 9485 9452 948c  ounter...}...R..
-0000b410: 0e70 6172 7365 5f6d 6573 7361 6765 7394  .parse_messages.
-0000b420: 5d94 8c12 7472 616e 7366 6f72 6d5f 6d65  ]...transform_me
-0000b430: 7373 6167 6573 945d 948c 0b74 7261 6e73  ssages.]...trans
-0000b440: 666f 726d 6572 944e 8c0b 696e 636c 7564  former.N..includ
-0000b450: 655f 6c6f 6794 5d94 8c09 696e 6465 782e  e_log.]...index.
-0000b460: 7273 7494 284e 4e4e 4e74 9486 9461 8c0a  rst.(NNNNt...a..
-0000b470: 6465 636f 7261 7469 6f6e 944e 6826 6803  decoration.Nh&h.
-0000b480: 7562 2e                                  ub.
+0000a340: 9485 9481 947d 9428 6816 6ada 0900 0068  .....}.(h.j....h
+0000a350: 2668 0368 274e 6829 4e75 626a ee02 0000  &h.h'Nh)Nubj....
+0000a360: 2981 947d 9428 6805 8c1c 6060 5b73 6d70  )..}.(h...``[smp
+0000a370: 5d20 6465 636f 7265 2062 6173 6520 7361  ] decore base sa
+0000a380: 6d70 6c65 6060 9468 075d 9468 118c 185b  mple``.h.].h...[
+0000a390: 736d 705d 2064 6563 6f72 6520 6261 7365  smp] decore base
+0000a3a0: 2073 616d 706c 6594 8594 8194 7d94 2868   sample.....}.(h
+0000a3b0: 166a e209 0000 6826 6803 6827 4e68 294e  .j....h&h.h'Nh)N
+0000a3c0: 7562 6168 177d 9428 6819 5d94 681b 5d94  ubah.}.(h.].h.].
+0000a3d0: 681d 5d94 681f 5d94 6821 5d94 7568 256a  h.].h.].h!].uh%j
+0000a3e0: ed02 0000 6816 6ada 0900 0075 6268 118c  ....h.j....ubh..
+0000a3f0: 1320 7072 6f66 696c 6520 696e 2076 7363  . profile in vsc
+0000a400: 6f64 652e 9485 9481 947d 9428 6816 6ada  ode......}.(h.j.
+0000a410: 0900 0068 2668 0368 274e 6829 4e75 6265  ...h&h.h'Nh)Nube
+0000a420: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+0000a430: 9468 1f5d 9468 215d 9475 6825 6851 6827  .h.].h!].uh%hQh'
+0000a440: 6850 6829 4d02 0168 166a 8309 0000 6826  hPh)M..h.j....h&
+0000a450: 6803 7562 6568 177d 9428 6819 5d94 8c12  h.ubeh.}.(h.]...
+0000a460: 7361 6d70 6c65 2d61 7070 6c69 6361 7469  sample-applicati
+0000a470: 6f6e 9461 681b 5d94 681d 5d94 8c12 7361  on.ah.].h.]...sa
+0000a480: 6d70 6c65 2061 7070 6c69 6361 7469 6f6e  mple application
+0000a490: 9461 681f 5d94 6821 5d94 7568 2568 2a68  .ah.].h!].uh%h*h
+0000a4a0: 1668 2c68 2668 0368 2768 5068 294b fb75  .h,h&h.h'hPh)K.u
+0000a4b0: 6268 2b29 8194 7d94 2868 0568 0668 075d  bh+)..}.(h.h.h.]
+0000a4c0: 9428 6830 2981 947d 9428 6805 8c05 4e6f  .(h0)..}.(h...No
+0000a4d0: 7465 7394 6807 5d94 6811 8c05 4e6f 7465  tes.h.].h...Note
+0000a4e0: 7394 8594 8194 7d94 2868 166a 050a 0000  s.....}.(h.j....
+0000a4f0: 6826 6803 6827 4e68 294e 7562 6168 177d  h&h.h'Nh)Nubah.}
+0000a500: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+0000a510: 5d94 6821 5d94 7568 2568 2f68 166a 020a  ].h!].uh%h/h.j..
+0000a520: 0000 6826 6803 6827 6850 6829 4d05 0175  ..h&h.h'hPh)M..u
+0000a530: 6268 5229 8194 7d94 2868 058c 4654 6869  bhR)..}.(h..FThi
+0000a540: 7320 646f 6375 6d65 6e74 6174 696f 6e20  s documentation 
+0000a550: 7761 7320 7472 616e 736c 6174 6564 2066  was translated f
+0000a560: 726f 6d20 4765 726d 616e 2069 6e74 6f20  rom German into 
+0000a570: 456e 676c 6973 6820 7769 7468 2044 6565  English with Dee
+0000a580: 706c 2e94 6807 5d94 6811 8c46 5468 6973  pl..h.].h..FThis
+0000a590: 2064 6f63 756d 656e 7461 7469 6f6e 2077   documentation w
+0000a5a0: 6173 2074 7261 6e73 6c61 7465 6420 6672  as translated fr
+0000a5b0: 6f6d 2047 6572 6d61 6e20 696e 746f 2045  om German into E
+0000a5c0: 6e67 6c69 7368 2077 6974 6820 4465 6570  nglish with Deep
+0000a5d0: 6c2e 9485 9481 947d 9428 6816 6a13 0a00  l......}.(h.j...
+0000a5e0: 0068 2668 0368 274e 6829 4e75 6261 6817  .h&h.h'Nh)Nubah.
+0000a5f0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+0000a600: 1f5d 9468 215d 9475 6825 6851 6827 6850  .].h!].uh%hQh'hP
+0000a610: 6829 4d06 0168 166a 020a 0000 6826 6803  h)M..h.j....h&h.
+0000a620: 7562 6809 8c08 636f 6d70 6f75 6e64 9493  ubh...compound..
+0000a630: 9429 8194 7d94 2868 0568 0668 075d 9468  .)..}.(h.h.h.].h
+0000a640: 008c 0774 6f63 7472 6565 9493 9429 8194  ...toctree...)..
+0000a650: 7d94 2868 0568 0668 075d 9468 177d 9428  }.(h.h.h.].h.}.(
+0000a660: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+0000a670: 6821 5d94 6816 8c05 696e 6465 7894 8c07  h!].h...index...
+0000a680: 656e 7472 6965 7394 5d94 8c0c 696e 636c  entries.]...incl
+0000a690: 7564 6566 696c 6573 945d 948c 086d 6178  udefiles.]...max
+0000a6a0: 6465 7074 6894 4b02 8c07 6361 7074 696f  depth.K...captio
+0000a6b0: 6e94 4e8c 0467 6c6f 6294 898c 0668 6964  n.N..glob....hid
+0000a6c0: 6465 6e94 888c 0d69 6e63 6c75 6465 6869  den....includehi
+0000a6d0: 6464 656e 9489 8c08 6e75 6d62 6572 6564  dden....numbered
+0000a6e0: 944b 008c 0a74 6974 6c65 736f 6e6c 7994  .K...titlesonly.
+0000a6f0: 898c 0a72 6177 656e 7472 6965 7394 5d94  ...rawentries.].
+0000a700: 7568 256a 260a 0000 6827 6828 6829 4b0b  uh%j&...h'h(h)K.
+0000a710: 6816 6a23 0a00 0075 6261 6817 7d94 2868  h.j#...ubah.}.(h
+0000a720: 195d 9468 1b5d 948c 0f74 6f63 7472 6565  .].h.]...toctree
+0000a730: 2d77 7261 7070 6572 9461 681d 5d94 681f  -wrapper.ah.].h.
+0000a740: 5d94 6821 5d94 7568 256a 210a 0000 6816  ].h!].uh%j!...h.
+0000a750: 6a02 0a00 0068 2668 0368 2768 2868 294e  j....h&h.h'h(h)N
+0000a760: 7562 680b 2981 947d 9428 6805 8c12 496e  ubh.)..}.(h...In
+0000a770: 6469 6365 7320 616e 6420 7461 626c 6573  dices and tables
+0000a780: 9468 075d 9468 118c 1249 6e64 6963 6573  .h.].h...Indices
+0000a790: 2061 6e64 2074 6162 6c65 7394 8594 8194   and tables.....
+0000a7a0: 7d94 6816 6a46 0a00 0073 6261 6817 7d94  }.h.jF...sbah.}.
+0000a7b0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+0000a7c0: 9468 215d 9468 2368 2475 6825 680a 6816  .h!].h#h$uh%h.h.
+0000a7d0: 6a02 0a00 0068 2668 0368 2768 2868 294b  j....h&h.h'h(h)K
+0000a7e0: 0f75 6268 0b29 8194 7d94 2868 058c 123d  .ubh.)..}.(h...=
+0000a7f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000a800: 3d94 6807 5d94 6811 8c12 3d3d 3d3d 3d3d  =.h.].h...======
+0000a810: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 9485 9481  ============....
+0000a820: 947d 9468 166a 540a 0000 7362 6168 177d  .}.h.jT...sbah.}
+0000a830: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+0000a840: 5d94 6821 5d94 6823 6824 7568 2568 0a68  ].h!].h#h$uh%h.h
+0000a850: 166a 020a 0000 6826 6803 6827 6828 6829  .j....h&h.h'h(h)
+0000a860: 4b11 7562 680b 2981 947d 9428 6805 8c11  K.ubh.)..}.(h...
+0000a870: 2a20 3a72 6566 3a60 6765 6e69 6e64 6578  * :ref:`genindex
+0000a880: 6094 6807 5d94 6811 8c11 2a20 3a72 6566  `.h.].h...* :ref
+0000a890: 3a60 6765 6e69 6e64 6578 6094 8594 8194  :`genindex`.....
+0000a8a0: 7d94 6816 6a62 0a00 0073 6261 6817 7d94  }.h.jb...sbah.}.
+0000a8b0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+0000a8c0: 9468 215d 9468 2368 2475 6825 680a 6816  .h!].h#h$uh%h.h.
+0000a8d0: 6a02 0a00 0068 2668 0368 2768 2868 294b  j....h&h.h'h(h)K
+0000a8e0: 1275 6268 0b29 8194 7d94 2868 058c 112a  .ubh.)..}.(h...*
+0000a8f0: 203a 7265 663a 606d 6f64 696e 6465 7860   :ref:`modindex`
+0000a900: 9468 075d 9468 118c 112a 203a 7265 663a  .h.].h...* :ref:
+0000a910: 606d 6f64 696e 6465 7860 9485 9481 947d  `modindex`.....}
+0000a920: 9468 166a 700a 0000 7362 6168 177d 9428  .h.jp...sbah.}.(
+0000a930: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
+0000a940: 6821 5d94 6823 6824 7568 2568 0a68 166a  h!].h#h$uh%h.h.j
+0000a950: 020a 0000 6826 6803 6827 6828 6829 4b13  ....h&h.h'h(h)K.
+0000a960: 7562 680b 2981 947d 9428 6805 8c0f 2a20  ubh.)..}.(h...* 
+0000a970: 3a72 6566 3a60 7365 6172 6368 6094 6807  :ref:`search`.h.
+0000a980: 5d94 6811 8c0f 2a20 3a72 6566 3a60 7365  ].h...* :ref:`se
+0000a990: 6172 6368 6094 8594 8194 7d94 6816 6a7e  arch`.....}.h.j~
+0000a9a0: 0a00 0073 6261 6817 7d94 2868 195d 9468  ...sbah.}.(h.].h
+0000a9b0: 1b5d 9468 1d5d 9468 1f5d 9468 215d 9468  .].h.].h.].h!].h
+0000a9c0: 2368 2475 6825 680a 6816 6a02 0a00 0068  #h$uh%h.h.j....h
+0000a9d0: 2668 0368 2768 2868 294b 1475 6265 6817  &h.h'h(h)K.ubeh.
+0000a9e0: 7d94 2868 195d 948c 056e 6f74 6573 9461  }.(h.]...notes.a
+0000a9f0: 681b 5d94 681d 5d94 8c05 6e6f 7465 7394  h.].h.]...notes.
+0000aa00: 6168 1f5d 9468 215d 9475 6825 682a 6816  ah.].h!].uh%h*h.
+0000aa10: 682c 6826 6803 6827 6850 6829 4d05 0175  h,h&h.h'hPh)M..u
+0000aa20: 6265 6817 7d94 2868 195d 948c 0777 656c  beh.}.(h.]...wel
+0000aa30: 636f 6d65 9461 681b 5d94 681d 5d94 8c07  come.ah.].h.]...
+0000aa40: 7765 6c63 6f6d 6594 6168 1f5d 9468 215d  welcome.ah.].h!]
+0000aa50: 9475 6825 682a 6816 6803 6826 6803 6827  .uh%h*h.h.h&h.h'
+0000aa60: 6828 6829 4b07 7562 6568 177d 9428 6819  h(h)K.ubeh.}.(h.
+0000aa70: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+0000aa80: 5d94 8c06 736f 7572 6365 9468 2875 6825  ]...source.h(uh%
+0000aa90: 6801 8c0e 6375 7272 656e 745f 736f 7572  h...current_sour
+0000aaa0: 6365 944e 8c0c 6375 7272 656e 745f 6c69  ce.N..current_li
+0000aab0: 6e65 944e 8c08 7365 7474 696e 6773 948c  ne.N..settings..
+0000aac0: 1164 6f63 7574 696c 732e 6672 6f6e 7465  .docutils.fronte
+0000aad0: 6e64 948c 0656 616c 7565 7394 9394 2981  nd...Values...).
+0000aae0: 947d 9428 682f 4e8c 0967 656e 6572 6174  .}.(h/N..generat
+0000aaf0: 6f72 944e 8c09 6461 7465 7374 616d 7094  or.N..datestamp.
+0000ab00: 4e8c 0b73 6f75 7263 655f 6c69 6e6b 944e  N..source_link.N
+0000ab10: 8c0a 736f 7572 6365 5f75 726c 944e 8c0d  ..source_url.N..
+0000ab20: 746f 635f 6261 636b 6c69 6e6b 7394 8c05  toc_backlinks...
+0000ab30: 656e 7472 7994 8c12 666f 6f74 6e6f 7465  entry...footnote
+0000ab40: 5f62 6163 6b6c 696e 6b73 944b 018c 0d73  _backlinks.K...s
+0000ab50: 6563 746e 756d 5f78 666f 726d 944b 018c  ectnum_xform.K..
+0000ab60: 0e73 7472 6970 5f63 6f6d 6d65 6e74 7394  .strip_comments.
+0000ab70: 4e8c 1b73 7472 6970 5f65 6c65 6d65 6e74  N..strip_element
+0000ab80: 735f 7769 7468 5f63 6c61 7373 6573 944e  s_with_classes.N
+0000ab90: 8c0d 7374 7269 705f 636c 6173 7365 7394  ..strip_classes.
+0000aba0: 4e8c 0c72 6570 6f72 745f 6c65 7665 6c94  N..report_level.
+0000abb0: 4b02 8c0a 6861 6c74 5f6c 6576 656c 944b  K...halt_level.K
+0000abc0: 058c 1165 7869 745f 7374 6174 7573 5f6c  ...exit_status_l
+0000abd0: 6576 656c 944b 058c 0564 6562 7567 944e  evel.K...debug.N
+0000abe0: 8c0e 7761 726e 696e 675f 7374 7265 616d  ..warning_stream
+0000abf0: 944e 8c09 7472 6163 6562 6163 6b94 888c  .N..traceback...
+0000ac00: 0e69 6e70 7574 5f65 6e63 6f64 696e 6794  .input_encoding.
+0000ac10: 8c09 7574 662d 382d 7369 6794 8c1c 696e  ..utf-8-sig...in
+0000ac20: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
+0000ac30: 6f72 5f68 616e 646c 6572 948c 0673 7472  or_handler...str
+0000ac40: 6963 7494 8c0f 6f75 7470 7574 5f65 6e63  ict...output_enc
+0000ac50: 6f64 696e 6794 8c05 7574 662d 3894 8c1d  oding...utf-8...
+0000ac60: 6f75 7470 7574 5f65 6e63 6f64 696e 675f  output_encoding_
+0000ac70: 6572 726f 725f 6861 6e64 6c65 7294 6abf  error_handler.j.
+0000ac80: 0a00 008c 0e65 7272 6f72 5f65 6e63 6f64  .....error_encod
+0000ac90: 696e 6794 8c05 7574 662d 3894 8c1c 6572  ing...utf-8...er
+0000aca0: 726f 725f 656e 636f 6469 6e67 5f65 7272  ror_encoding_err
+0000acb0: 6f72 5f68 616e 646c 6572 948c 1062 6163  or_handler...bac
+0000acc0: 6b73 6c61 7368 7265 706c 6163 6594 8c0d  kslashreplace...
+0000acd0: 6c61 6e67 7561 6765 5f63 6f64 6594 8c02  language_code...
+0000ace0: 656e 948c 1372 6563 6f72 645f 6465 7065  en...record_depe
+0000acf0: 6e64 656e 6369 6573 944e 8c06 636f 6e66  ndencies.N..conf
+0000ad00: 6967 944e 8c09 6964 5f70 7265 6669 7894  ig.N..id_prefix.
+0000ad10: 6806 8c0e 6175 746f 5f69 645f 7072 6566  h...auto_id_pref
+0000ad20: 6978 948c 0269 6494 8c0d 6475 6d70 5f73  ix...id...dump_s
+0000ad30: 6574 7469 6e67 7394 4e8c 0e64 756d 705f  ettings.N..dump_
+0000ad40: 696e 7465 726e 616c 7394 4e8c 0f64 756d  internals.N..dum
+0000ad50: 705f 7472 616e 7366 6f72 6d73 944e 8c0f  p_transforms.N..
+0000ad60: 6475 6d70 5f70 7365 7564 6f5f 786d 6c94  dump_pseudo_xml.
+0000ad70: 4e8c 1065 7870 6f73 655f 696e 7465 726e  N..expose_intern
+0000ad80: 616c 7394 4e8c 0e73 7472 6963 745f 7669  als.N..strict_vi
+0000ad90: 7369 746f 7294 4e8c 0f5f 6469 7361 626c  sitor.N.._disabl
+0000ada0: 655f 636f 6e66 6967 944e 8c07 5f73 6f75  e_config.N.._sou
+0000adb0: 7263 6594 6828 8c0c 5f64 6573 7469 6e61  rce.h(.._destina
+0000adc0: 7469 6f6e 944e 8c0d 5f63 6f6e 6669 675f  tion.N.._config_
+0000add0: 6669 6c65 7394 5d94 8c16 6669 6c65 5f69  files.]...file_i
+0000ade0: 6e73 6572 7469 6f6e 5f65 6e61 626c 6564  nsertion_enabled
+0000adf0: 9488 8c0b 7261 775f 656e 6162 6c65 6494  ....raw_enabled.
+0000ae00: 4b01 8c11 6c69 6e65 5f6c 656e 6774 685f  K...line_length_
+0000ae10: 6c69 6d69 7494 4d10 278c 0e70 6570 5f72  limit.M.'..pep_r
+0000ae20: 6566 6572 656e 6365 7394 4e8c 0c70 6570  eferences.N..pep
+0000ae30: 5f62 6173 655f 7572 6c94 8c18 6874 7470  _base_url...http
+0000ae40: 733a 2f2f 7065 7073 2e70 7974 686f 6e2e  s://peps.python.
+0000ae50: 6f72 672f 948c 1570 6570 5f66 696c 655f  org/...pep_file_
+0000ae60: 7572 6c5f 7465 6d70 6c61 7465 948c 0870  url_template...p
+0000ae70: 6570 2d25 3034 6494 8c0e 7266 635f 7265  ep-%04d...rfc_re
+0000ae80: 6665 7265 6e63 6573 944e 8c0c 7266 635f  ferences.N..rfc_
+0000ae90: 6261 7365 5f75 726c 948c 2668 7474 7073  base_url..&https
+0000aea0: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
+0000aeb0: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
+0000aec0: 2f94 8c09 7461 625f 7769 6474 6894 4b08  /...tab_width.K.
+0000aed0: 8c1d 7472 696d 5f66 6f6f 746e 6f74 655f  ..trim_footnote_
+0000aee0: 7265 6665 7265 6e63 655f 7370 6163 6594  reference_space.
+0000aef0: 898c 1073 796e 7461 785f 6869 6768 6c69  ...syntax_highli
+0000af00: 6768 7494 8c04 6c6f 6e67 948c 0c73 6d61  ght...long...sma
+0000af10: 7274 5f71 756f 7465 7394 888c 1373 6d61  rt_quotes....sma
+0000af20: 7274 7175 6f74 6573 5f6c 6f63 616c 6573  rtquotes_locales
+0000af30: 945d 948c 1d63 6861 7261 6374 6572 5f6c  .]...character_l
+0000af40: 6576 656c 5f69 6e6c 696e 655f 6d61 726b  evel_inline_mark
+0000af50: 7570 9489 8c0e 646f 6374 6974 6c65 5f78  up....doctitle_x
+0000af60: 666f 726d 9489 8c0d 646f 6369 6e66 6f5f  form....docinfo_
+0000af70: 7866 6f72 6d94 4b01 8c12 7365 6374 7375  xform.K...sectsu
+0000af80: 6274 6974 6c65 5f78 666f 726d 9489 8c0d  btitle_xform....
+0000af90: 696d 6167 655f 6c6f 6164 696e 6794 8c04  image_loading...
+0000afa0: 6c69 6e6b 948c 1065 6d62 6564 5f73 7479  link...embed_sty
+0000afb0: 6c65 7368 6565 7494 898c 1563 6c6f 616b  lesheet....cloak
+0000afc0: 5f65 6d61 696c 5f61 6464 7265 7373 6573  _email_addresses
+0000afd0: 9488 8c11 7365 6374 696f 6e5f 7365 6c66  ....section_self
+0000afe0: 5f6c 696e 6b94 898c 0365 6e76 944e 7562  _link....env.Nub
+0000aff0: 8c08 7265 706f 7274 6572 944e 8c10 696e  ..reporter.N..in
+0000b000: 6469 7265 6374 5f74 6172 6765 7473 945d  direct_targets.]
+0000b010: 948c 1173 7562 7374 6974 7574 696f 6e5f  ...substitution_
+0000b020: 6465 6673 947d 948c 1273 7562 7374 6974  defs.}...substit
+0000b030: 7574 696f 6e5f 6e61 6d65 7394 7d94 8c08  ution_names.}...
+0000b040: 7265 666e 616d 6573 947d 948c 0672 6566  refnames.}...ref
+0000b050: 6964 7394 7d94 8c07 6e61 6d65 6964 7394  ids.}...nameids.
+0000b060: 7d94 286a 990a 0000 6a96 0a00 0068 dd68  }.(j....j....h.h
+0000b070: da68 af68 ac6a 8f01 0000 6a8c 0100 006a  .h.h.j....j....j
+0000b080: 8001 0000 6a7d 0100 006a 8009 0000 6a7d  ....j}...j....j}
+0000b090: 0900 006a 6102 0000 6a5e 0200 006a 4e02  ...ja...j^...jN.
+0000b0a0: 0000 6a4b 0200 006a 1e03 0000 6a1b 0300  ..jK...j....j...
+0000b0b0: 006a 8d08 0000 6a8a 0800 006a 3005 0000  .j....j....j0...
+0000b0c0: 6a2d 0500 006a fe04 0000 6afb 0400 006a  j-...j....j....j
+0000b0d0: 6406 0000 6a61 0600 006a db06 0000 6ad8  d...ja...j....j.
+0000b0e0: 0600 006a 5207 0000 6a4f 0700 006a 9707  ...jR...jO...j..
+0000b0f0: 0000 6a94 0700 006a 8508 0000 6a82 0800  ..j....j....j...
+0000b100: 006a 7809 0000 6a75 0900 006a 3709 0000  .jx...ju...j7...
+0000b110: 6a34 0900 006a 7009 0000 6a6d 0900 006a  j4...jp...jm...j
+0000b120: ff09 0000 6afc 0900 006a 910a 0000 6a8e  ....j....j....j.
+0000b130: 0a00 0075 8c09 6e61 6d65 7479 7065 7394  ...u..nametypes.
+0000b140: 7d94 286a 990a 0000 8968 dd89 68af 886a  }.(j.....h..h..j
+0000b150: 8f01 0000 896a 8001 0000 886a 8009 0000  .....j.....j....
+0000b160: 896a 6102 0000 896a 4e02 0000 886a 1e03  .ja....jN....j..
+0000b170: 0000 896a 8d08 0000 896a 3005 0000 896a  ...j.....j0....j
+0000b180: fe04 0000 886a 6406 0000 896a db06 0000  .....jd....j....
+0000b190: 896a 5207 0000 896a 9707 0000 896a 8508  .jR....j.....j..
+0000b1a0: 0000 896a 7809 0000 896a 3709 0000 896a  ...jx....j7....j
+0000b1b0: 7009 0000 896a ff09 0000 896a 910a 0000  p....j.....j....
+0000b1c0: 8975 6819 7d94 286a 960a 0000 682c 68da  .uh.}.(j....h,h.
+0000b1d0: 683f 68ac 68a6 6a8c 0100 0068 e06a 7d01  h?h.h.j....h.j}.
+0000b1e0: 0000 6a77 0100 006a 7d09 0000 6a92 0100  ..jw...j}...j...
+0000b1f0: 006a 5e02 0000 6aea 0100 006a 4b02 0000  .j^...j....jK...
+0000b200: 6a45 0200 006a 1b03 0000 6a64 0200 006a  jE...j....jd...j
+0000b210: 8a08 0000 6a21 0300 006a 2d05 0000 6a08  ....j!...j-...j.
+0000b220: 0400 006a fb04 0000 6af5 0400 006a 6106  ...j....j....ja.
+0000b230: 0000 6a33 0500 006a d806 0000 6a67 0600  ..j3...j....jg..
+0000b240: 006a 4f07 0000 6ade 0600 006a 9407 0000  .jO...j....j....
+0000b250: 6a55 0700 006a 8208 0000 6a9a 0700 006a  jU...j....j....j
+0000b260: 7509 0000 6a90 0800 006a 3409 0000 6ae1  u...j....j4...j.
+0000b270: 0800 006a 6d09 0000 6a3a 0900 006a fc09  ...jm...j:...j..
+0000b280: 0000 6a83 0900 006a 8e0a 0000 6a02 0a00  ..j....j....j...
+0000b290: 0075 8c0d 666f 6f74 6e6f 7465 5f72 6566  .u..footnote_ref
+0000b2a0: 7394 7d94 8c0d 6369 7461 7469 6f6e 5f72  s.}...citation_r
+0000b2b0: 6566 7394 7d94 8c0d 6175 746f 666f 6f74  efs.}...autofoot
+0000b2c0: 6e6f 7465 7394 5d94 8c11 6175 746f 666f  notes.]...autofo
+0000b2d0: 6f74 6e6f 7465 5f72 6566 7394 5d94 8c10  otnote_refs.]...
+0000b2e0: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 6573  symbol_footnotes
+0000b2f0: 945d 948c 1473 796d 626f 6c5f 666f 6f74  .]...symbol_foot
+0000b300: 6e6f 7465 5f72 6566 7394 5d94 8c09 666f  note_refs.]...fo
+0000b310: 6f74 6e6f 7465 7394 5d94 8c09 6369 7461  otnotes.]...cita
+0000b320: 7469 6f6e 7394 5d94 8c12 6175 746f 666f  tions.]...autofo
+0000b330: 6f74 6e6f 7465 5f73 7461 7274 944b 018c  otnote_start.K..
+0000b340: 1573 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
+0000b350: 5f73 7461 7274 944b 008c 0a69 645f 636f  _start.K...id_co
+0000b360: 756e 7465 7294 8c0b 636f 6c6c 6563 7469  unter...collecti
+0000b370: 6f6e 7394 8c07 436f 756e 7465 7294 9394  ons...Counter...
+0000b380: 7d94 8594 5294 8c0e 7061 7273 655f 6d65  }...R...parse_me
+0000b390: 7373 6167 6573 945d 948c 1274 7261 6e73  ssages.]...trans
+0000b3a0: 666f 726d 5f6d 6573 7361 6765 7394 5d94  form_messages.].
+0000b3b0: 8c0b 7472 616e 7366 6f72 6d65 7294 4e8c  ..transformer.N.
+0000b3c0: 0b69 6e63 6c75 6465 5f6c 6f67 945d 948c  .include_log.]..
+0000b3d0: 0969 6e64 6578 2e72 7374 9428 4e4e 4e4e  .index.rst.(NNNN
+0000b3e0: 7494 8694 618c 0a64 6563 6f72 6174 696f  t...a..decoratio
+0000b3f0: 6e94 4e68 2668 0375 622e                 n.Nh&h.ub.
```

### Comparing `decore_Base-0.0.22/docs/page/html/_static/basic.css` & `decore_Base-0.0.23/docs/page/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/clipboard.min.js` & `decore_Base-0.0.23/docs/page/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/copybutton.css` & `decore_Base-0.0.23/docs/page/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/copybutton.js` & `decore_Base-0.0.23/docs/page/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/copybutton_funcs.js` & `decore_Base-0.0.23/docs/page/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/doctools.js` & `decore_Base-0.0.23/docs/page/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/favicon.ico` & `decore_Base-0.0.23/docs/page/html/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/language_data.js` & `decore_Base-0.0.23/docs/page/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/logo.png` & `decore_Base-0.0.23/docs/page/html/_static/logo.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/pygments.css` & `decore_Base-0.0.23/docs/page/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/scripts/bootstrap.js` & `decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/scripts/bootstrap.js.map` & `decore_Base-0.0.23/docs/page/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/scripts/pydata-sphinx-theme.js` & `decore_Base-0.0.23/docs/page/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map` & `decore_Base-0.0.23/docs/page/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/searchtools.js` & `decore_Base-0.0.23/docs/page/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/sphinx_highlight.js` & `decore_Base-0.0.23/docs/page/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/styles/bootstrap.css` & `decore_Base-0.0.23/docs/page/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/styles/pydata-sphinx-theme.css` & `decore_Base-0.0.23/docs/page/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `decore_Base-0.0.23/docs/page/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/_static/webpack-macros.html` & `decore_Base-0.0.23/docs/page/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/genindex.html` & `decore_Base-0.0.23/docs/page/html/genindex.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/index.html` & `decore_Base-0.0.23/docs/page/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -434,22 +434,20 @@
    <span class="k">def</span> <span class="nf">first_view</span><span class="p">():</span>
       <span class="nd">@decore</span><span class="o">.</span><span class="n">dialog</span><span class="p">(</span><span class="n">title</span><span class="o">=</span><span class="s1">&#39;Add Person&#39;</span><span class="p">,</span> <span class="n">icon</span><span class="o">=</span><span class="s1">&#39;mdi-plus&#39;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="s1">&#39;standard&#39;</span><span class="p">,</span> <span class="n">display</span><span class="o">=</span><span class="s1">&#39;drawer&#39;</span><span class="p">,</span> <span class="n">activator</span><span class="o">=</span><span class="s1">&#39;default-menu&#39;</span><span class="p">)</span>
       <span class="k">def</span> <span class="nf">first_dialog</span><span class="p">():</span>
          <span class="nd">@decore</span><span class="o">.</span><span class="n">widget</span><span class="p">(</span><span class="n">title</span><span class="o">=</span><span class="s1">&#39;Add Person Form&#39;</span><span class="p">,</span> <span class="n">icon</span><span class="o">=</span><span class="s1">&#39;mdi-account&#39;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="s1">&#39;form&#39;</span><span class="p">,</span> <span class="n">fields</span><span class="o">=</span><span class="p">[</span><span class="n">First_model</span><span class="o">.</span><span class="n">firstname</span><span class="p">,</span> <span class="n">First_model</span><span class="o">.</span><span class="n">lastname</span><span class="p">])</span>
          <span class="k">def</span> <span class="nf">first_widget</span><span class="p">():</span>
             <span class="nd">@decore</span><span class="o">.</span><span class="n">action</span><span class="p">(</span><span class="n">title</span><span class="o">=</span><span class="s1">&#39;Save Person&#39;</span><span class="p">,</span> <span class="n">icon</span><span class="o">=</span><span class="s1">&#39;mdi-content-save&#39;</span><span class="p">,</span> <span class="nb">type</span><span class="o">=</span><span class="s1">&#39;submit&#39;</span><span class="p">)</span>
             <span class="k">def</span> <span class="nf">first_action</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">):</span>
-               <span class="n">item</span> <span class="o">=</span> <span class="n">First_model</span><span class="p">()</span>
-               <span class="n">item</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">data</span><span class="p">[</span><span class="s1">&#39;firstname&#39;</span><span class="p">]</span> <span class="o">+</span> <span class="s1">&#39; &#39;</span> <span class="o">+</span> <span class="n">data</span><span class="p">[</span><span class="s1">&#39;lastname&#39;</span><span class="p">]</span>
-               <span class="n">item</span><span class="o">.</span><span class="n">firstname</span> <span class="o">=</span> <span class="n">data</span><span class="p">[</span><span class="s1">&#39;firstname&#39;</span><span class="p">]</span>
-               <span class="n">item</span><span class="o">.</span><span class="n">lastname</span> <span class="o">=</span> <span class="n">data</span><span class="p">[</span><span class="s1">&#39;lastname&#39;</span><span class="p">]</span>
+               <span class="n">item</span> <span class="o">=</span> <span class="n">First_model</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="s1">&#39;item&#39;</span><span class="p">])</span>
+               <span class="n">item</span><span class="o">.</span><span class="n">title</span> <span class="o">=</span> <span class="n">item</span><span class="o">.</span><span class="n">firstname</span> <span class="o">+</span> <span class="s1">&#39; &#39;</span> <span class="o">+</span> <span class="n">item</span><span class="o">.</span><span class="n">lastname</span>
                <span class="k">if</span> <span class="n">item</span><span class="o">.</span><span class="n">save</span><span class="p">():</span>
                   <span class="k">return</span> <span class="kc">True</span><span class="p">,</span> <span class="n">item</span><span class="o">.</span><span class="n">title</span> <span class="o">+</span> <span class="s1">&#39; saved successfully&#39;</span>
                <span class="k">else</span><span class="p">:</span>
-                  <span class="k">return</span> <span class="kc">False</span><span class="p">,</span> <span class="n">item</span><span class="o">.</span><span class="n">error</span>
+                  <span class="k">return</span> <span class="kc">False</span><span class="p">,</span> <span class="s1">&#39;Error while saving &#39;</span> <span class="o">+</span> <span class="n">item</span><span class="o">.</span><span class="n">title</span>
 </pre></div>
 </div>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>To create a record with decore Base, we need to create an instance of the model. In our case <strong>First_model</strong>. The instance is filled with the data from the form and then saved.</p>
 <p>The ID in the form of a UUID is generated automatically and does not have to be specified separately.</p>
 </div>
```

#### html2text {}

```diff
@@ -214,22 +214,20 @@
       def first_dialog():
          @decore.widget(title='Add Person Form', icon='mdi-account',
 type='form', fields=[First_model.firstname, First_model.lastname])
          def first_widget():
             @decore.action(title='Save Person', icon='mdi-content-save',
 type='submit')
             def first_action(self, data):
-               item = First_model()
-               item.title = data['firstname'] + ' ' + data['lastname']
-               item.firstname = data['firstname']
-               item.lastname = data['lastname']
+               item = First_model(data['item'])
+               item.title = item.firstname + ' ' + item.lastname
                if item.save():
                   return True, item.title + ' saved successfully'
                else:
-                  return False, item.error
+                  return False, 'Error while saving ' + item.title
 Note
 To create a record with decore Base, we need to create an instance of the
 model. In our case First_model. The instance is filled with the data from the
 form and then saved.
 The ID in the form of a UUID is generated automatically and does not have to be
 specified separately.
 Warning
```

### Comparing `decore_Base-0.0.22/docs/page/html/search.html` & `decore_Base-0.0.23/docs/page/html/search.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/page/html/searchindex.js` & `decore_Base-0.0.23/docs/page/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -289,14 +289,15 @@
         "item": 0,
         "return": 0,
         "true": 0,
         "successfulli": 0,
         "els": 0,
         "fals": 0,
         "error": 0,
+        "while": 0,
         "fill": 0,
         "uuid": 0,
         "gener": 0,
         "automat": 0,
         "doe": 0,
         "specifi": 0,
         "inherit": 0,
```

### Comparing `decore_Base-0.0.22/docs/state/keybase.kdbx` & `decore_Base-0.0.23/docs/state/keybase.kdbx`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/docs/state/querybase.db` & `decore_Base-0.0.23/docs/state/querybase.db`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/requirements.txt` & `decore_Base-0.0.23/requirements.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.22/setup.cfg` & `decore_Base-0.0.23/setup.cfg`

 * *Files identical despite different names*

