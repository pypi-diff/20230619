# Comparing `tmp/archivy-1.7.4.tar.gz` & `tmp/archivy-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/archivy-1.7.4.tar", last modified: Tue Jan 17 15:59:21 2023, max compression
+gzip compressed data, was "archivy-1.7.5.tar", last modified: Mon Jun 19 16:38:09 2023, max compression
```

## Comparing `archivy-1.7.4.tar` & `archivy-1.7.5.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2023-01-17 15:59:15.000000 archivy-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      132 2023-01-17 15:59:15.000000 archivy-1.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2932 2023-01-17 15:59:21.000000 archivy-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2502 2023-01-17 15:59:15.000000 archivy-1.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy/
--rw-r--r--   0 runner    (1001) docker     (116)     3542 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6766 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/api.py
--rw-r--r--   0 runner    (1001) docker     (116)     5771 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy/click_web/
--rw-r--r--   0 runner    (1001) docker     (116)     2552 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/click_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      104 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/click_web/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy/click_web/resources/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/click_web/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14883 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/click_web/resources/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (116)     4345 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/click_web/resources/cmd_form.py
--rw-r--r--   0 runner    (1001) docker     (116)     1931 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/click_web/resources/index.py
--rw-r--r--   0 runner    (1001) docker     (116)     9877 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/click_web/resources/input_fields.py
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/click_web/web_click_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     5738 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    13301 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/data.py
--rw-r--r--   0 runner    (1001) docker     (116)     3194 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/forms.py
--rw-r--r--   0 runner    (1001) docker     (116)     8290 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)    10873 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/models.py
--rw-r--r--   0 runner    (1001) docker     (116)    14678 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/routes.py
--rw-r--r--   0 runner    (1001) docker     (116)     6468 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/search.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy/static/
--rw-r--r--   0 runner    (1001) docker     (116)     1514 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/HIGHLIGHTJS-LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      127 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/accessibility.css
--rw-r--r--   0 runner    (1001) docker     (116)     5914 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/archivy.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1143 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/delete.png
--rw-r--r--   0 runner    (1001) docker     (116)    12507 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/editor.css
--rw-r--r--   0 runner    (1001) docker     (116)   318739 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/editor.js
--rw-r--r--   0 runner    (1001) docker     (116)      907 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/editor_dark.css
--rw-r--r--   0 runner    (1001) docker     (116)   114758 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/highlight.js
--rw-r--r--   0 runner    (1001) docker     (116)     3810 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/logo.png
--rw-r--r--   0 runner    (1001) docker     (116)     9164 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/main.css
--rw-r--r--   0 runner    (1001) docker     (116)     2736 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/main_dark.css
--rw-r--r--   0 runner    (1001) docker     (116)     7580 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/markdown.css
--rw-r--r--   0 runner    (1001) docker     (116)      115 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/markdown_dark.css
--rw-r--r--   0 runner    (1001) docker     (116)    23367 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/math.css
--rw-r--r--   0 runner    (1001) docker     (116)   262137 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/math.js
--rw-r--r--   0 runner    (1001) docker     (116)     1026 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/monokai.css
--rw-r--r--   0 runner    (1001) docker     (116)     7593 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/mvp.css
--rw-r--r--   0 runner    (1001) docker     (116)     1238 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/open_form.js
--rw-r--r--   0 runner    (1001) docker     (116)   113587 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/parser.js
--rw-r--r--   0 runner    (1001) docker     (116)     5520 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/post_and_read.js
--rw-r--r--   0 runner    (1001) docker     (116)      299 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/static/profile.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1077 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy/templates/
--rw-r--r--   0 runner    (1001) docker     (116)     9514 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (116)      951 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/bookmarklet.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy/templates/click_web/
--rw-r--r--   0 runner    (1001) docker     (116)     1631 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/click_web/command_form.html
--rw-r--r--   0 runner    (1001) docker     (116)     2202 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/click_web/form_macros.html
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/click_web/show_tree.html
--rw-r--r--   0 runner    (1001) docker     (116)     1240 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/config.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy/templates/dataobjs/
--rw-r--r--   0 runner    (1001) docker     (116)      909 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/dataobjs/new.html
--rw-r--r--   0 runner    (1001) docker     (116)    21594 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/dataobjs/show.html
--rw-r--r--   0 runner    (1001) docker     (116)     7929 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (116)     1556 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/markdown-parser.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy/templates/tags/
--rw-r--r--   0 runner    (1001) docker     (116)      248 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/tags/all.html
--rw-r--r--   0 runner    (1001) docker     (116)      619 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/tags/show.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy/templates/users/
--rw-r--r--   0 runner    (1001) docker     (116)      681 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/users/edit.html
--rw-r--r--   0 runner    (1001) docker     (116)      754 2023-01-17 15:59:15.000000 archivy-1.7.4/archivy/templates/users/login.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2932 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1914 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       44 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      321 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-01-17 15:59:21.000000 archivy-1.7.4/archivy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1008 2023-01-17 15:59:15.000000 archivy-1.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-17 15:59:21.000000 archivy-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1100 2023-01-17 15:59:15.000000 archivy-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:21.000000 archivy-1.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:15.000000 archivy-1.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7582 2023-01-17 15:59:15.000000 archivy-1.7.4/tests/test_click_web.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-17 15:59:15.000000 archivy-1.7.4/tests/test_request_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.772354 archivy-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 16:38:07.000000 archivy-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-19 16:38:07.000000 archivy-1.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-19 16:38:09.772354 archivy-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-19 16:38:07.000000 archivy-1.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.764355 archivy-1.7.5/archivy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.764355 archivy-1.7.5/archivy/click_web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.764355 archivy-1.7.5/archivy/click_web/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14879 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/cmd_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/resources/input_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/click_web/web_click_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.768355 archivy-1.7.5/archivy/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/HIGHLIGHTJS-LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/accessibility.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/archivy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/editor.css
+-rw-r--r--   0 runner    (1001) docker     (123)   318739 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/editor.js
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/editor_dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)   114758 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/main_dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/markdown.css
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/markdown_dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/math.css
+-rw-r--r--   0 runner    (1001) docker     (123)   262137 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/math.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/monokai.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/mvp.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/open_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)   113587 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/parser.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/post_and_read.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/static/profile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.768355 archivy-1.7.5/archivy/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/bookmarklet.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.768355 archivy-1.7.5/archivy/templates/click_web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/click_web/command_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/click_web/form_macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/click_web/show_tree.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/config.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.768355 archivy-1.7.5/archivy/templates/dataobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/dataobjs/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21594 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/dataobjs/show.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/markdown-parser.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.772354 archivy-1.7.5/archivy/templates/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/tags/all.html
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/tags/show.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.772354 archivy-1.7.5/archivy/templates/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/users/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-19 16:38:07.000000 archivy-1.7.5/archivy/templates/users/login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.764355 archivy-1.7.5/archivy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 16:38:09.000000 archivy-1.7.5/archivy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-19 16:38:07.000000 archivy-1.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:38:09.772354 archivy-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-19 16:38:07.000000 archivy-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:09.772354 archivy-1.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:07.000000 archivy-1.7.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-06-19 16:38:07.000000 archivy-1.7.5/tests/test_click_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:38:07.000000 archivy-1.7.5/tests/test_request_parsing.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `archivy-1.7.4/LICENSE` & `archivy-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/PKG-INFO` & `archivy-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archivy
-Version: 1.7.4
+Version: 1.7.5
 Summary: Minimalist knowledge base focused on digital preservation and building your second brain.
 Home-page: https://github.com/archivy/archivy
 Author: Uzay-G
 Author-email: halcyon@disroot.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `archivy-1.7.4/README.md` & `archivy-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/__init__.py` & `archivy-1.7.5/archivy/__init__.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/api.py` & `archivy-1.7.5/archivy/api.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/cli.py` & `archivy-1.7.5/archivy/cli.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/click_web/__init__.py` & `archivy-1.7.5/archivy/click_web/__init__.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/click_web/resources/cmd_exec.py` & `archivy-1.7.5/archivy/click_web/resources/cmd_exec.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,14 @@
         # only include relevant fields for this command index
         commands_field_infos = [
             fi for fi in self.field_infos if fi.param.command_index == command_index
         ]
         commands_field_infos = sorted(commands_field_infos)
 
         for fi in commands_field_infos:
-
             # must be called mostly for saving and preparing file output.
             fi.before_script_execute()
 
             if fi.cmd_opt.startswith("--"):
                 # it's an option
                 args.extend(self._process_option(fi))
 
@@ -332,15 +331,14 @@
                 dir=self.temp_dir(), prefix=name, suffix=suffix
             )
             self.file_path = filename
             logger.info(f"Saving {self.key} to {filename}")
             file.save(filename)
 
     def __str__(self):
-
         res = [super().__str__()]
         res.append(f"file_path: {self.file_path}")
         return ", ".join(res)
 
 
 class FieldOutFileInfo(FieldFileInfo):
     """
```

### Comparing `archivy-1.7.4/archivy/click_web/resources/cmd_form.py` & `archivy-1.7.5/archivy/click_web/resources/cmd_form.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/click_web/resources/index.py` & `archivy-1.7.5/archivy/click_web/resources/index.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/click_web/resources/input_fields.py` & `archivy-1.7.5/archivy/click_web/resources/input_fields.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/click_web/web_click_types.py` & `archivy-1.7.5/archivy/click_web/web_click_types.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/config.py` & `archivy-1.7.5/archivy/config.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/data.py` & `archivy-1.7.5/archivy/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,22 +43,34 @@
 
 def get_by_id(dataobj_id):
     """Returns filename of dataobj of given id"""
     results = list(get_data_dir().rglob(f"{dataobj_id}-*.md"))
     return results[0] if results else None
 
 
-def build_dir_tree(path, query_dir, load_content=True):
+def load_frontmatter(filepath):
+    count = 0
+    file = open(filepath, "r")
+    data = ""
+    line = "_"
+    while count != 2 and line:
+        line = file.readline()
+        if line in ["---\n", "---"]:
+            count += 1
+        data += line
+    data = frontmatter.loads(data)
+    return data
+
+
+def build_dir_tree(path, query_dir):
     """
     Builds a structured tree of directories and data objects.
 
     - **path**: name of the directory relative to the root directory.
     - **query_dir**: absolute path of the directory we're building the tree of.
-    - **load_content**: internal option to not save post contents in memory
-        if they're not going to be accessed.
     """
     datacont = Directory(path or "root")
     for filepath in query_dir.rglob("*"):
         current_path = filepath.relative_to(query_dir)
         current_dir = datacont
 
         # iterate through parent directories
@@ -71,24 +83,20 @@
         # handle last part of current_path
         last_seg = current_path.parts[-1]
         if filepath.is_dir():
             if last_seg not in current_dir.child_dirs:
                 current_dir.child_dirs[last_seg] = Directory(last_seg)
             current_dir = current_dir.child_dirs[last_seg]
         elif last_seg.endswith(".md"):
-            data = frontmatter.load(filepath)
-            if not load_content:
-                data.content = ""
+            data = load_frontmatter(filepath)
             current_dir.child_files.append(data)
     return datacont
 
 
-def get_items(
-    collections=[], path="", structured=True, json_format=False, load_content=True
-):
+def get_items(collections=[], path="", structured=True, json_format=False):
     """
     Gets all dataobjs.
 
     Parameters:
 
     - **collections** - filter dataobj by type, eg. bookmark / note
     - **path** - filter by path
@@ -103,17 +111,15 @@
     if not is_relative_to(query_dir, data_dir) or not query_dir.exists():
         raise FileNotFoundError
     if structured:
         return build_dir_tree(path, query_dir)
     else:
         datacont = []
         for filepath in query_dir.rglob("*.md"):
-            data = frontmatter.load(filepath)
-            if not load_content:
-                data.content = ""
+            data = load_frontmatter(filepath)
             data["fullpath"] = str(filepath.parent.relative_to(query_dir))
             if len(collections) == 0 or any(
                 [collection == data["type"] for collection in collections]
             ):
                 if json_format:
                     dict_dataobj = data.__dict__
                     # remove unnecessary yaml handler
```

### Comparing `archivy-1.7.4/archivy/forms.py` & `archivy-1.7.5/archivy/forms.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/helpers.py` & `archivy-1.7.5/archivy/helpers.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/models.py` & `archivy-1.7.5/archivy/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 # TODO: use this as 'type' field
 # class DataobjType(Enum):
 #     BOOKMARK = 'bookmark'
 #     POCKET_BOOKMARK = 'bookmark imported from pocket'
 #     NOTE = 'note'
 #     PROCESSED_DATAOBJ = 'bookmark that has been processed'
 
+
 # TODO: use this as 'type' field
 # class DataobjType(Enum):
 #     BOOKMARK = 'bookmark'
 #     POCKET_BOOKMARK = 'bookmark imported from pocket'
 #     NOTE = 'note'
 #     PROCESSED_DATAOBJ = 'bookmark that has been processed'
 @attrs(kw_only=True)
```

### Comparing `archivy-1.7.4/archivy/routes.py` & `archivy-1.7.5/archivy/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from archivy.config import Config
 
 import re
 
 
 @app.context_processor
 def pass_defaults():
-    dataobjs = data.get_items(load_content=False)
+    dataobjs = data.get_items()
     version = require("archivy")[0].version
     SEP = sep
     # check windows parsing for js (https://github.com/Uzay-G/archivy/issues/115)
     if SEP == "\\":
         SEP += "\\"
     return dict(dataobjs=dataobjs, SEP=SEP, version=version, config=app.config)
 
@@ -68,15 +68,14 @@
         tag_cloud = set()
         for f in files.child_files:
             for tag in f.get("tags", []):
                 tag_cloud.add(tag)
     except FileNotFoundError:
         flash("Directory does not exist.", "error")
         return redirect("/")
-
     return render_template(
         "home.html",
         title=path or "root",
         search_enabled=app.config["SEARCH_CONF"]["enabled"],
         dir=files,
         current_path=path,
         new_folder_form=forms.NewFolderForm(),
@@ -173,17 +172,15 @@
     )
 
 
 @app.route("/dataobj/<int:dataobj_id>")
 def show_dataobj(dataobj_id):
     dataobj = data.get_item(dataobj_id)
     get_title_id_pairs = lambda x: (x["title"], x["id"])
-    titles = list(
-        map(get_title_id_pairs, data.get_items(structured=False, load_content=False))
-    )
+    titles = list(map(get_title_id_pairs, data.get_items(structured=False)))
     js_ext = ""
     if app.config["DATAOBJ_JS_EXTENSION"]:
         js_ext = (
             (Path(app.config["USER_DIR"]) / app.config["DATAOBJ_JS_EXTENSION"])
             .open("r")
             .read()
         )
```

### Comparing `archivy-1.7.4/archivy/search.py` & `archivy-1.7.5/archivy/search.py`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/HIGHLIGHTJS-LICENSE` & `archivy-1.7.5/archivy/static/HIGHLIGHTJS-LICENSE`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/archivy.svg` & `archivy-1.7.5/archivy/static/archivy.svg`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/delete.png` & `archivy-1.7.5/archivy/static/delete.png`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/editor.css` & `archivy-1.7.5/archivy/static/editor.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/editor.js` & `archivy-1.7.5/archivy/static/editor.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/editor_dark.css` & `archivy-1.7.5/archivy/static/editor_dark.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/highlight.js` & `archivy-1.7.5/archivy/static/highlight.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/logo.png` & `archivy-1.7.5/archivy/static/logo.png`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/main.css` & `archivy-1.7.5/archivy/static/main.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/main_dark.css` & `archivy-1.7.5/archivy/static/main_dark.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/markdown.css` & `archivy-1.7.5/archivy/static/markdown.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/math.css` & `archivy-1.7.5/archivy/static/math.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/math.js` & `archivy-1.7.5/archivy/static/math.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/monokai.css` & `archivy-1.7.5/archivy/static/monokai.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/mvp.css` & `archivy-1.7.5/archivy/static/mvp.css`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/open_form.js` & `archivy-1.7.5/archivy/static/open_form.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/parser.js` & `archivy-1.7.5/archivy/static/parser.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/static/post_and_read.js` & `archivy-1.7.5/archivy/static/post_and_read.js`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/tags.py` & `archivy-1.7.5/archivy/tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 
 from flask import current_app
 from archivy import helpers, data
 from tinydb import Query, operations
 from archivy.search import query_ripgrep_tags
-from archivy.data import get_items
 
 
 def is_tag_format(tag_name):
     return re.match("^[a-zA-Z0-9_-]+$", tag_name)
 
 
 def get_all_tags(force=False):
```

### Comparing `archivy-1.7.4/archivy/templates/base.html` & `archivy-1.7.5/archivy/templates/base.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/bookmarklet.html` & `archivy-1.7.5/archivy/templates/bookmarklet.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/click_web/command_form.html` & `archivy-1.7.5/archivy/templates/click_web/command_form.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/click_web/form_macros.html` & `archivy-1.7.5/archivy/templates/click_web/form_macros.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/click_web/show_tree.html` & `archivy-1.7.5/archivy/templates/click_web/show_tree.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/config.html` & `archivy-1.7.5/archivy/templates/config.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/dataobjs/new.html` & `archivy-1.7.5/archivy/templates/dataobjs/new.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/dataobjs/show.html` & `archivy-1.7.5/archivy/templates/dataobjs/show.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/home.html` & `archivy-1.7.5/archivy/templates/home.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/markdown-parser.html` & `archivy-1.7.5/archivy/templates/markdown-parser.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/tags/show.html` & `archivy-1.7.5/archivy/templates/tags/show.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/users/edit.html` & `archivy-1.7.5/archivy/templates/users/edit.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy/templates/users/login.html` & `archivy-1.7.5/archivy/templates/users/login.html`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/archivy.egg-info/PKG-INFO` & `archivy-1.7.5/archivy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archivy
-Version: 1.7.4
+Version: 1.7.5
 Summary: Minimalist knowledge base focused on digital preservation and building your second brain.
 Home-page: https://github.com/archivy/archivy
 Author: Uzay-G
 Author-email: halcyon@disroot.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `archivy-1.7.4/archivy.egg-info/SOURCES.txt` & `archivy-1.7.5/archivy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `archivy-1.7.4/requirements.txt` & `archivy-1.7.5/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 # archivy/__init__.py: 7
 # archivy/check_changes.py: 5
 # archivy/data.py: 9
 # archivy/extensions.py: 6
 # archivy/models.py: 13
 # archivy/routes.py: 7
-Flask == 2.0.0
-werkzeug == 2.0.3
-jinja2 == 3.0.0
+Flask == 2.3.2
+werkzeug == 2.3.3
+jinja2 == 3.1.2
 
 # archivy/forms.py: 2
-Flask_WTF == 0.14.3
+Flask_WTF == 1.1.1
 
 # archivy/forms.py: 4
 WTForms == 2.3.1
 
 # archivy/config.py: 2
 appdirs == 1.4.4
 
@@ -49,14 +49,14 @@
 
 # archivy/models.py: 8
 validators == 0.15.0
 
 # archivy/__init__.py: 9
 # archivy/models.py: 13
 # archivy/routes.py: 10
-flask-login == 0.5.0
+flask-login == 0.6.2
 
 click_plugins
 html2text
 flask_compress
 readability-lxml
```

### Comparing `archivy-1.7.4/setup.py` & `archivy-1.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         x.strip()
         for x in all_reqs
         if not x.startswith("#") and not x.startswith("-e git")
     ]
 
 setuptools.setup(
     name="archivy",
-    version="1.7.4",
+    version="1.7.5",
     author="Uzay-G",
     author_email="halcyon@disroot.org",
     description=(
         "Minimalist knowledge base focused on digital preservation"
         " and building your second brain."
     ),
     long_description=long_description,
```

### Comparing `archivy-1.7.4/tests/test_click_web.py` & `archivy-1.7.5/tests/test_click_web.py`

 * *Files identical despite different names*

