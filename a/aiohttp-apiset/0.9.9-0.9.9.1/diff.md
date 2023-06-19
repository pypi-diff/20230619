# Comparing `tmp/aiohttp-apiset-0.9.9.tar.gz` & `tmp/aiohttp-apiset-0.9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiohttp-apiset-0.9.9.tar", last modified: Thu Jan 30 21:24:22 2020, max compression
+gzip compressed data, was "dist/aiohttp-apiset-0.9.9.1.tar", last modified: Fri Jan 31 00:14:03 2020, max compression
```

## Comparing `aiohttp-apiset-0.9.9.tar` & `aiohttp-apiset-0.9.9.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    11856 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11856 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4252 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset.egg-info/requires.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21838 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/dispatcher.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/jinja2.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/typography.css
--rw-rw-r--   0 travis    (2000) travis    (2000)      773 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/reset.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     3488 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/style.css
--rw-rw-r--   0 travis    (2000) travis    (2000)    41666 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/print.css
--rw-rw-r--   0 travis    (2000) travis    (2000)    43644 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/screen.css
--rw-rw-r--   0 travis    (2000) travis    (2000)   453076 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/swagger-ui.min.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7042 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/swagger-oauth.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    92032 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/jquery-1.8.0.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    43510 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/js-yaml.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)   129835 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/jsoneditor.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      310 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/highlight.9.1.0.pack_extended.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    19371 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/backbone-min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    51894 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/lodash.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    15724 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/marked.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      536 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/jquery.wiggle.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     3518 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/jquery.ba-bbq.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    22724 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/es5-shim.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      349 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/object-assign-pollyfill.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      365 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/jquery.slideto.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    10962 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/highlight.9.1.0.pack.js
--rw-rw-r--   0 travis    (2000) travis    (2000)   130418 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/sanitize-html.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    71504 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/handlebars-4.0.5.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/fonts/
--rw-rw-r--   0 travis    (2000) travis    (2000)    41028 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/fonts/DroidSans.ttf
--rw-rw-r--   0 travis    (2000) travis    (2000)    42480 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/fonts/DroidSans-Bold.ttf
--rw-rw-r--   0 travis    (2000) travis    (2000)     4335 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/favicon-16x16.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     5115 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/explorer_icons.png
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/collapse.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/expand.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)      670 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/wordnik_api.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      631 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/pet_store_api.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     1141 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/favicon-32x32.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     9257 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/throbber.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)     5430 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/favicon.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/logo_small.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      479 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/o2c.html
--rw-rw-r--   0 travis    (2000) travis    (2000)  2704640 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/swagger-ui.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3470 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/el.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2320 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/ko-kr.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2503 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/fr.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     3856 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/geo.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2298 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/pl.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2314 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/pt.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     1421 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/translator.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2721 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/ja.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2286 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/tr.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2203 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/zh-cn.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2464 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/es.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2395 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/ca.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     3100 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/ru.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2342 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/en.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2432 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/it.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      665 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/favicon-16x16.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   141841 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     1424 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)   483073 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui.css.map
--rw-rw-r--   0 travis    (2000) travis    (2000)  4203103 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui-bundle.js.map
--rw-rw-r--   0 travis    (2000) travis    (2000)  1290497 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui.js.map
--rw-rw-r--   0 travis    (2000) travis    (2000)   307021 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui-standalone-preset.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/oauth2-redirect.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      628 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/favicon-32x32.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   974176 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui-bundle.js
--rw-rw-r--   0 travis    (2000) travis    (2000)   361609 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui.js
--rw-rw-r--   0 travis    (2000) travis    (2000)  1367758 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui-standalone-preset.js.map
--rw-rw-r--   0 travis    (2000) travis    (2000)     4056 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/middlewares.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/templates/swagger-ui/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/templates/swagger-ui/2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4678 2020-01-30 21:24:09.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/templates/swagger-ui/2/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/templates/swagger-ui/3/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1463 2020-01-30 21:24:10.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/templates/swagger-ui/3/index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3966 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-01-30 21:24:08.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11610 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/compat.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10508 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/router.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2727 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/operations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7353 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/route.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4558 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/validate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15692 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      656 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/ui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      155 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1544 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/aiohttp_apiset/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2020-01-30 21:24:22.000000 aiohttp-apiset-0.9.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     5539 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2609 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1882 2020-01-30 21:23:13.000000 aiohttp-apiset-0.9.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11858 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11858 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4252 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset.egg-info/requires.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21838 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/dispatcher.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1288 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/jinja2.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/typography.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)      773 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/reset.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3488 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/style.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41666 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/print.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43644 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/screen.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)   453076 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/swagger-ui.min.js
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7042 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/swagger-oauth.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92032 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/jquery-1.8.0.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43510 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/js-yaml.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)   129835 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/jsoneditor.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)      310 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/highlight.9.1.0.pack_extended.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19371 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/backbone-min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51894 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/lodash.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15724 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/marked.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)      536 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/jquery.wiggle.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3518 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/jquery.ba-bbq.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22724 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/es5-shim.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)      349 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/object-assign-pollyfill.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)      365 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/jquery.slideto.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10962 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/highlight.9.1.0.pack.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)   130418 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/sanitize-html.min.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71504 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/handlebars-4.0.5.js
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/fonts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41028 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/fonts/DroidSans.ttf
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42480 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/fonts/DroidSans-Bold.ttf
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4335 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/index.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/favicon-16x16.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5115 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/explorer_icons.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/collapse.gif
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/expand.gif
+-rw-rw-r--   0 travis    (2000) travis    (2000)      670 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/wordnik_api.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      631 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/pet_store_api.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1141 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/favicon-32x32.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9257 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/throbber.gif
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5430 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/favicon.ico
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/logo_small.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      479 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/o2c.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)  2704640 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/swagger-ui.js
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3470 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/el.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2320 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/ko-kr.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2503 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/fr.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3856 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/geo.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2298 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/pl.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2314 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/pt.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1421 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/translator.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2721 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/ja.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2286 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/tr.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2203 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/zh-cn.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2464 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/es.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2395 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/ca.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3100 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/ru.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2342 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/en.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2432 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/it.js
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      665 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/favicon-16x16.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   141841 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1424 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/index.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)   483073 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui.css.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)  4203103 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui-bundle.js.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1290497 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui.js.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)   307021 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui-standalone-preset.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/oauth2-redirect.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      628 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/favicon-32x32.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)   974176 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui-bundle.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)   361609 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1367758 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui-standalone-preset.js.map
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4056 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/middlewares.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/templates/swagger-ui/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/templates/swagger-ui/2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4678 2020-01-31 00:13:49.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/templates/swagger-ui/2/index.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/templates/swagger-ui/3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1463 2020-01-31 00:13:50.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/templates/swagger-ui/3/index.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3966 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1274 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-01-31 00:13:48.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11610 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/compat.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10508 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/router.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2727 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/operations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7353 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/route.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4558 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/validate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15693 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      656 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/ui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      155 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1544 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/aiohttp_apiset/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      176 2020-01-31 00:14:03.000000 aiohttp-apiset-0.9.9.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5539 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2609 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1882 2020-01-31 00:12:52.000000 aiohttp-apiset-0.9.9.1/setup.py
```

### Comparing `aiohttp-apiset-0.9.9/PKG-INFO` & `aiohttp-apiset-0.9.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-apiset
-Version: 0.9.9
+Version: 0.9.9.1
 Summary: Build routes using swagger specification
 Home-page: https://github.com/aamalev/aiohttp_apiset/
 Author: Alexander Malev
 Author-email: malev@somedev.ru
 License: Apache 2
 Description: aiohttp-apiset
         ==============
```

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset.egg-info/PKG-INFO` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-apiset
-Version: 0.9.9
+Version: 0.9.9.1
 Summary: Build routes using swagger specification
 Home-page: https://github.com/aamalev/aiohttp_apiset/
 Author: Alexander Malev
 Author-email: malev@somedev.ru
 License: Apache 2
 Description: aiohttp-apiset
         ==============
```

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset.egg-info/SOURCES.txt` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/dispatcher.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/jinja2.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/jinja2.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/reset.css` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/reset.css`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/style.css` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/style.css`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/print.css` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/print.css`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/css/screen.css` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/css/screen.css`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/swagger-ui.min.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/swagger-ui.min.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/swagger-oauth.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/swagger-oauth.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/jquery-1.8.0.min.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/jquery-1.8.0.min.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/js-yaml.min.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/js-yaml.min.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/jsoneditor.min.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/jsoneditor.min.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/backbone-min.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/backbone-min.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/lodash.min.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/lodash.min.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/marked.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/marked.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/jquery.wiggle.min.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/jquery.wiggle.min.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/jquery.ba-bbq.min.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/jquery.ba-bbq.min.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/es5-shim.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/es5-shim.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/highlight.9.1.0.pack.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/highlight.9.1.0.pack.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/sanitize-html.min.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/sanitize-html.min.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lib/handlebars-4.0.5.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lib/handlebars-4.0.5.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/fonts/DroidSans.ttf` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/fonts/DroidSans.ttf`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/fonts/DroidSans-Bold.ttf` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/fonts/DroidSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/index.html` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/index.html`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/explorer_icons.png` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/explorer_icons.png`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/wordnik_api.png` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/wordnik_api.png`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/pet_store_api.png` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/pet_store_api.png`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/favicon-32x32.png` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/throbber.gif` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/throbber.gif`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/images/favicon.ico` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/swagger-ui.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/el.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/el.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/ko-kr.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/ko-kr.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/fr.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/fr.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/geo.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/geo.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/pl.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/pl.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/pt.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/pt.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/translator.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/translator.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/ja.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/ja.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/tr.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/tr.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/zh-cn.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/es.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/es.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/ca.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/ca.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/ru.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/ru.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/en.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/en.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/2/lang/it.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/2/lang/it.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/favicon-16x16.png` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui.css` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/index.html` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/index.html`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui.css.map` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui-bundle.js.map` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui.js.map` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui-standalone-preset.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/oauth2-redirect.html` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/favicon-32x32.png` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui-bundle.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui.js` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/static/swagger-ui/3/swagger-ui-standalone-preset.js.map` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/static/swagger-ui/3/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/middlewares.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/middlewares.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/templates/swagger-ui/2/index.html` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/templates/swagger-ui/2/index.html`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/templates/swagger-ui/3/index.html` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/templates/swagger-ui/3/index.html`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/exceptions.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/utils.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/compat.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/compat.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/router.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/router.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/operations.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/operations.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/route.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/route.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/validate.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/validate.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/loader.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             mapping[key] = value
         return mapping
 
 
 Loader.add_constructor('tag:yaml.org,2002:map', Loader.construct_yaml_map)
 
 
-@lru_cache(100)
+@lru_cache(None)
 def yaml_load(path: Path, encoding) -> dict:
     with path.open(encoding=encoding) as f:
         return yaml.load(f, Loader)
 
 
 class SwaggerLoaderMixin:
     swagger_files = {}
```

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/swagger/ui.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/swagger/ui.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/aiohttp_apiset/views.py` & `aiohttp-apiset-0.9.9.1/aiohttp_apiset/views.py`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/HISTORY.rst` & `aiohttp-apiset-0.9.9.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/README.rst` & `aiohttp-apiset-0.9.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `aiohttp-apiset-0.9.9/setup.py` & `aiohttp-apiset-0.9.9.1/setup.py`

 * *Files identical despite different names*

