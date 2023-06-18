# Comparing `tmp/django-hostutils-0.0.7.tar.gz` & `tmp/django-hostutils-0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hostutils-0.0.7.tar", last modified: Sun Jun 18 22:05:31 2023, max compression
+gzip compressed data, was "django-hostutils-0.0.dev3.tar", last modified: Tue Apr 25 00:40:22 2023, max compression
```

## Comparing `django-hostutils-0.0.7.tar` & `django-hostutils-0.0.dev3.tar`

### file list

```diff
@@ -1,47 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.121721 django-hostutils-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46392 2023-06-18 22:05:31.121721 django-hostutils-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 22:05:31.121721 django-hostutils-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.117721 django-hostutils-0.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 22:05:30.000000 django-hostutils-0.0.7/src/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.117721 django-hostutils-0.0.7/src/django_hostutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46392 2023-06-18 22:05:31.000000 django-hostutils-0.0.7/src/django_hostutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-18 22:05:31.000000 django-hostutils-0.0.7/src/django_hostutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:05:31.000000 django-hostutils-0.0.7/src/django_hostutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-18 22:05:31.000000 django-hostutils-0.0.7/src/django_hostutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 22:05:31.000000 django-hostutils-0.0.7/src/django_hostutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.117721 django-hostutils-0.0.7/src/djangoaddicts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.117721 django-hostutils-0.0.7/src/djangoaddicts/hostutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.117721 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.117721 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.117721 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.117721 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
--rw-r--r--   0 runner    (1001) docker     (123)    11682 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.117721 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_cpu_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_interface_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_partition_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_process_stats.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.121721 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:05:31.121721 django-hostutils-0.0.7/src/djangoaddicts/hostutils/views/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/views/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-18 22:05:10.000000 django-hostutils-0.0.7/src/djangoaddicts/hostutils/views/htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/django_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   133744 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/version_history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_partition_usage.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_process_details.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_htmx.py
```

### Comparing `django-hostutils-0.0.7/LICENSE` & `django-hostutils-0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/forms.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,77 @@
 {% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
+    {% include 'handyhelpers/component/chartjs_components.htm' %}
     <style>
-        .card a { text-decoration: none; }
         .card .card-header {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
+            font-size: 1.25rem;
         }
         .key {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             margin-right: .25rem
         }
         .value {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             margin-left: .25rem
         }
         .titlecard-container {
             display: flex;
-            gap: 1.5rem;
+            gap: 2rem;
             flex-wrap: wrap;
         }
         .titlecard-container > * {
             flex: 1;
         }
         .titlecard {
-            height: 6.75rem;
-            min-width: 5rem;
+            height: 8rem;
         }
         .titlecard .stat {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-size: 2.5rem;
             font-weight: bold;
             text-align: center;
-            margin-top: -1rem;
+            margin-top: -.75rem;
         }
         .titlecard .description {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             font-weight: bold;
             font-size: 1rem;
             text-align: center;
             margin-top: .65rem
         }
 
-        @media (max-width: 975px) {
+        @media (max-width: 800px) {
             .titlecard {
                 height: 6rem;
             }
             .titlecard .stat {
                 font-size: 1.5rem;
             }
             .titlecard .description {
                 font-size: .75rem;
             }
 
-        @media (max-width: 775px) {
-            .titlecard {
-                height: 6rem;
-            }
-            .titlecard .stat {
-                font-size: 1.5rem;
-            }
-            .titlecard .description {
-                font-size: .5rem;
-            }
-
         @media (max-width: 650px) {
             .titlecard {
                 height: 5rem;
             }
             .titlecard .stat {
                 font-size: 1.25rem;
             }
             .titlecard .description {
                 font-size: .5rem;
             }
 
+
     </style>
 {% endblock %}
 
 {% block content %}
 <section class="my-3 animated fadeIn" style="animation-delay: .15s;">
     {% if title or subtitle %}
     <div class="container-fluid">
@@ -164,15 +154,15 @@
     <div class="container-fluid mt-5">
         <div class="card shadow">
             <div class="card-header">CPUs <span class="small">({{ logical_count }})</span></div>
                 <div class="card-body" style="overflow-y: auto; overflow-x: hidden; max-height: 50vh">
                     <ul class="list-group mx-auto justify-content-center" style="max-width: 93%; margin-top: .5%; margin-bottom: .5%">
                         {% for cpu, data in cpu_data.items %}
                         <li class="list-group-item bg-light shadow-sm hvr-grow mb-3">
-                            <a href="#" hx-get="{% url 'hostutils:get_cpu_stats' cpu %}" hx-target="#modal_wrapper">
+                            <a href="#" onClick="showInfo('{% url "hostutils:get_cpu_stats" %}', '{{cpu}}', 'CPU Stats: <small><i>{{cpu}}</i></small>', true);">
                                 <div class="row">
                                     <div class="col-xs-12 col-md-2"><span class="key">CPU:</span><span class="value">{{ cpu }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Percent:</span><span class="value">{{ data.percent }}%</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">System:</span><span class="value">{{ data.time_percent.system }}%</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Idle:</span><span class="value">{{ data.time_percent.idle }}%</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">Frequency:</span><span class="value">{{ data.frequency.current }}</span></div>
                                 </div>
@@ -182,9 +172,9 @@
                     </ul>
                 </div>
             </div>
         </div>
     </div>
 </section>
 
-{% include 'handyhelpers/htmx/bs5/generic_modal.htm' %}
+{% include 'handyhelpers/component/bs5/modals.htm' %}
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %} {%
-load static %} {% load handyhelper_tags %} {% block local_head %}
+load static %} {% load handyhelper_tags %} {% block local_head %} {% include
+'handyhelpers/component/chartjs_components.htm' %}
  {% endblock %} {% block content %}  {% if title or subtitle %}
 {{ title }}
 {{ subtitle|safe }}
 {% endif %}
 {{ physical_count }}
 Physical
 {{ logical_count }}
@@ -21,14 +22,15 @@
 {{ load_avg_5 }}%
 5 minute load average
 {{ load_avg_15 }}%
 15 minute load average
 
 CPUs ({{ logical_count }})
     * {% for cpu, data in cpu_data.items %}
-    * CPU:{{_cpu_}}
-      Percent:{{_data.percent_}}%
-      System:{{_data.time_percent.system_}}%
-      Idle:{{_data.time_percent.idle_}}%
-      Frequency:{{_data.frequency.current_}}
-    * {% endfor %}
- {% include 'handyhelpers/htmx/bs5/generic_modal.htm' %} {% endblock content %}
+    *  %}', '{{cpu}}', 'CPU Stats: {{cpu}}', true);">
+      CPU:{{ cpu }}
+      Percent:{{ data.percent }}%
+      System:{{ data.time_percent.system }}%
+      Idle:{{ data.time_percent.idle }}%
+      Frequency:{{ data.frequency.current }}
+{% endfor %}
+ {% include 'handyhelpers/component/bs5/modals.htm' %} {% endblock content %}
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 {% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     <style>
-        .card a { text-decoration: none; }
         .titlecard-container {
             display: flex;
             gap: 2rem;
             flex-wrap: wrap;
             align-content: center;
             align-items: center;
             justify-content: center;
@@ -16,32 +15,31 @@
         .titlecard-container > * {
             flex: 1;
         }
         .titlecard {
             height: 8rem;
             min-width: 250px;
             max-width: 475;
-            color: var(--bs-light);
-            text-decoration: none;
+            color: var(--light);
         }
         .titlecard .icon {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-size: 2.5rem;
             text-align: left;
             margin-top: -.5rem;
         }
         .titlecard .stat {
-            color: var(--bs-secondary);
+            color: var(--primary);
             font-size: 2rem;
             font-weight: bold;
             text-align: right;
             margin-top: -.5rem;
         }
         .titlecard .description {
-            color: var(--bs-primary);
+            color: var(--secondary);
             font-weight: bold;
             font-size: 1.25rem;
             text-align: left;
         }
         .even-columns {
             display: flex;
             gap: 2rem;
@@ -51,27 +49,27 @@
             flex: 1;
         }
         .datacard {
             margin-bottom: 1rem;
             min-width: 22rem;
         }
         .datacard .card-header {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             font-size: 1.25rem;
         }
         .datacard .card-body {
             min-height: 17rem;
         }
         .datacard .key {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
         }
         .datacard .value {
-            color: var(--bs-secondary);
+            color: var(--secondary);
         }
     </style>
 {% endblock %}
 
 {% block content %}
 
 <section class="my-3 animated fadeIn" style="animation-delay: .15s;">
@@ -109,47 +107,51 @@
                             <div class="col-4 icon"><i class="fa-solid fa-memory fa-lg"></i></div>
                             <div class="col-8 stat">{{ memory.percent }}%</div>
                         </div>
                         <div class="description">Memory Usage</div>
                     </div>
                 </a>
             </div>
+
             <div class="card titlecard shadow hvr-grow">
                 <a href="{% url 'hostutils:host_disk' %}">
                     <div class="card-body">
                         <div class="row mb-3">
                             <div class="col-4 icon"><i class="fa-solid fa-hard-drive fa-lg"></i></div>
                             <div class="col-8 stat">{{ disk_usage.percent }}%</div>
                         </div>
                         <div class="description">Disk Usage</div>
                     </div>
                 </a>
             </div>
+
             <div class="card titlecard shadow hvr-grow">
                 <a href="{% url 'hostutils:host_process' %}">
                     <div class="card-body">
                         <div class="row mb-3">
                             <div class="col-6 icon"><i class="fa-solid fa-gears fa-lg"></i></div>
                             <div class="col-6 stat">{{ pids|length }}</div>
                         </div>
                         <div class="description">Processes</div>
                     </div>
                 </a>
             </div>
+
             <div class="card titlecard shadow hvr-grow">
                 <a href="{% url 'hostutils:host_network' %}">
                     <div class="card-body">
                         <div class="row mb-3">
                             <div class="col-6 icon"><i class="fa-solid fa-network-wired fa-lg"></i></div>
                             <div class="col-6 stat">{{ network|length }}</div>
                         </div>
                         <div class="description">Network Connections</div>
                     </div>
                 </a>
             </div>
+
         </div>
     </div>
 </section>
 
 <section class="mb-5 animated fadeIn" style="animation-delay: .35s;">
     <div class="container-fluid mt-5">
         <div class="m-5">&nbsp;</div>
@@ -183,81 +185,82 @@
                         <div class="col-8 value">{{ platform.machine }}</div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Hostname: </div>
                         <div class="col-8 value">{{ platform.nodename }}</div>
                     </div>
                     <div class="row">
+
                     </div>
                 </div>
             </div>
             <div class="card datacard shadow">
                 <div class="card-header">Memory</div>
                 <div class="card-body">
                     <div class="row mb-2">
                         <div class="col-4 key">Total: </div>
-                        <div class="col-8 value">{{ memory.total|byte_size }}<small class="ms-2">({{ memory.total }})</small></div>
+                        <div class="col-8 value">{{ memory.total|byte_size }}<small class="ml-3">({{ memory.total }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Available: </div>
-                        <div class="col-8 value">{{ memory.available|byte_size }}<small class="ms-2">({{ memory.available }})</small></div>
+                        <div class="col-8 value">{{ memory.available|byte_size }}<small class="ml-3">({{ memory.available }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Used: </div>
-                        <div class="col-8 value">{{ memory.used|byte_size }}<small class="ms-2">({{ memory.used }})</small></div>
+                        <div class="col-8 value">{{ memory.used|byte_size }}<small class="ml-3">({{ memory.used }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Free: </div>
-                        <div class="col-8 value">{{ memory.free|byte_size }}<small class="ms-2">({{ memory.free }})</small></div>
+                        <div class="col-8 value">{{ memory.free|byte_size }}<small class="ml-3">({{ memory.free }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Active: </div>
-                        <div class="col-8 value">{{ memory.active|byte_size }}<small class="ms-2">({{ memory.active }})</small></div>
+                        <div class="col-8 value">{{ memory.active|byte_size }}<small class="ml-3">({{ memory.active }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Inactive: </div>
-                        <div class="col-8 value">{{ memory.inactive|byte_size }}<small class="ms-2">({{ memory.inactive }})</small></div>
+                        <div class="col-8 value">{{ memory.inactive|byte_size }}<small class="ml-3">({{ memory.inactive }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Buffers: </div>
-                        <div class="col-8 value">{{ memory.buffers|byte_size }}<small class="ms-2">({{ memory.buffers }})</small></div>
+                        <div class="col-8 value">{{ memory.buffers|byte_size }}<small class="ml-3">({{ memory.buffers }})</small></div>
                     </div>
                 </div>
             </div>
             <div class="card datacard shadow">
                 <div class="card-header">Disk</div>
                 <div class="card-body">
                     <div class="row mb-2">
                         <div class="col-4 key">Total: </div>
-                        <div class="col-8 value">{{ disk_usage.total|byte_size }}<small class="ms-2">({{ disk_usage.total }})</small></div>
+                        <div class="col-8 value">{{ disk_usage.total|byte_size }}<small class="ml-3">({{ disk_usage.total }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Used: </div>
-                        <div class="col-8 value">{{ disk_usage.used|byte_size }}<small class="ms-2">({{ disk_usage.used }})</small></div>
+                        <div class="col-8 value">{{ disk_usage.used|byte_size }}<small class="ml-3">({{ disk_usage.used }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Free: </div>
-                        <div class="col-8 value">{{ disk_usage.free|byte_size }}<small class="ms-2">({{ disk_usage.free }})</small></div>
+                        <div class="col-8 value">{{ disk_usage.free|byte_size }}<small class="ml-3">({{ disk_usage.free }})</small></div>
                     </div>
                     <div class="row mb-2"></div>
                     <div class="row mb-2">
                         <div class="col-4 key">Read Count: </div>
-                        <div class="col-8 value">{{ disk_io_counters.read_count|byte_size }}<small class="ms-2">({{ disk_io_counters.read_count }})</small></div>
+                        <div class="col-8 value">{{ disk_io_counters.read_count|byte_size }}<small class="ml-3">({{ disk_io_counters.read_count }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Read Bytes: </div>
-                        <div class="col-8 value">{{ disk_io_counters.read_bytes|byte_size }}<small class="ms-2">({{ disk_io_counters.read_bytes }})</small></div>
+                        <div class="col-8 value">{{ disk_io_counters.read_bytes|byte_size }}<small class="ml-3">({{ disk_io_counters.read_bytes }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Write Count: </div>
-                        <div class="col-8 value">{{ disk_io_counters.write_count|byte_size }}<small class="ms-2">({{ disk_io_counters.write_count }})</small></div>
+                        <div class="col-8 value">{{ disk_io_counters.write_count|byte_size }}<small class="ml-3">({{ disk_io_counters.write_count }})</small></div>
                     </div>
                     <div class="row mb-2">
                         <div class="col-4 key">Write Bytes: </div>
-                        <div class="col-8 value">{{ disk_io_counters.write_bytes|byte_size }}<small class="ms-2">({{ disk_io_counters.write_bytes }})</small></div>
+                        <div class="col-8 value">{{ disk_io_counters.write_bytes|byte_size }}<small class="ml-3">({{ disk_io_counters.write_bytes }})</small></div>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 </section>
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 {% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     {% include 'handyhelpers/component/chartjs_components.htm' %}
     <style>
-        .card a { text-decoration: none; }
         .card .card-header {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             font-size: 1.25rem;
         }
         .key {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             margin-right: .25rem
         }
         .value {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             margin-left: .25rem
         }
         .titlecard-container {
             display: flex;
             gap: 2rem;
             flex-wrap: wrap;
             align-content: center;
@@ -29,30 +28,32 @@
             justify-content: center;
         }
         .titlecard-container > * {
             flex: 1;
         }
         .titlecard {
             height: 6rem;
+<!--            min-width: 148px;-->
+<!--            max-width: 475;-->
         }
         .titlecard .icon {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-size: 2.5rem;
             text-align: left;
             margin-top: -.5rem;
         }
         .titlecard .stat {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-size: 2rem;
             font-weight: bold;
             text-align: center;
             margin-top: -.5rem;
         }
         .titlecard .description {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             font-weight: bold;
             font-size: .8rem;
             text-align: center;
         }
     </style>
 {% endblock %}
 
@@ -132,15 +133,15 @@
     <div class="container-fluid mt-5">
         <div class="card shadow">
             <div class="card-header">Partitions <span class="small">({{ partition_lists|length }})</span></div>
                 <div class="card-body" style="overflow-y: auto; overflow-x: hidden; max-height: 50vh">
                     <ul class="list-group mx-auto justify-content-center" style="max-width: 93%; margin-top: .5%; margin-bottom: .5%">
                         {% for item in partition_lists %}
                         <li class="list-group-item bg-light shadow-sm hvr-grow mb-3">
-                            <a href="#" hx-get="{% url 'hostutils:get_partition_stats' %}?part={{ item.mountpoint }}" hx-target="#modal_wrapper">
+                            <a href="#" onClick="showInfo('{% url "hostutils:get_partition_stats" %}', '{{item.mountpoint}}', 'Partition Disk Usage: <small><i>{{item.mountpoint}}</i></small>', true);">
                                 <div class="row mb-1">
                                     <div class="col-xs-12 col-md-3"><span class="key">Device:</span><span class="value">{{ item.device }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Filesystem:</span><span class="value">{{ item.fstype }}</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">Mount Point:</span><span class="value">{{ item.mountpoint }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Max File:</span><span class="value">{{ item.maxfile }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Max Path:</span><span class="value">{{ item.maxpath }}</span></div>
                                 </div>
@@ -156,16 +157,16 @@
         </div>
     </div>
 </section>
 
 <script>
     var style = getComputedStyle(document.body);
     var theme = {};
-    theme.primary = style.getPropertyValue('--bs-primary');
-    theme.secondary = style.getPropertyValue('--bs-secondary');
+    theme.primary = style.getPropertyValue('--primary');
+    theme.secondary = style.getPropertyValue('--secondary');
     new Chart(document.getElementById("disk-usage-chart"), {
     type: 'pie',
     data: {
       labels: ["Used", "Free"],
       datasets: [{
         label: "Disk Usage",
         backgroundColor: [theme.primary, theme.secondary],
@@ -190,16 +191,16 @@
         }
     }
 });
 </script>
 <script>
     var style = getComputedStyle(document.body);
     var theme = {};
-    theme.primary = style.getPropertyValue('--bs-primary');
-    theme.secondary = style.getPropertyValue('--bs-secondary');
+    theme.primary = style.getPropertyValue('--primary');
+    theme.secondary = style.getPropertyValue('--secondary');
     new Chart(document.getElementById("disk-io-chart"), {
     type: 'bar',
     data: {
       labels: ["Read", "Write"],
       datasets: [{
         label: "Disk I/O Counters",
         backgroundColor: [theme.primary, theme.secondary],
@@ -222,9 +223,9 @@
               }
           }
         }
     }
 });
 </script>
 
-{% include 'handyhelpers/htmx/bs5/generic_modal.htm' %}
+{% include 'handyhelpers/component/bs5/modals.htm' %}
 {% endblock content %}
```

#### html2text {}

```diff
@@ -12,15 +12,17 @@
 {{ io_counters.read_bytes|byte_size }}
 Read Bytes
 {{ io_counters.write_bytes|byte_size }}
 Write Bytes
 
 Partitions ({{ partition_lists|length }})
     * {% for item in partition_lists %}
-    * Device:{{_item.device_}}
-      Filesystem:{{_item.fstype_}}
-      Mount_Point:{{_item.mountpoint_}}
-      Max_File:{{_item.maxfile_}}
-      Max_Path:{{_item.maxpath_}}
-      Options:{{_item.opts_}}
-    * {% endfor %}
- {% include 'handyhelpers/htmx/bs5/generic_modal.htm' %} {% endblock content %}
+    *  %}', '{{item.mountpoint}}', 'Partition Disk Usage: {{item.mountpoint}}',
+      true);">
+      Device:{{ item.device }}
+      Filesystem:{{ item.fstype }}
+      Mount Point:{{ item.mountpoint }}
+      Max File:{{ item.maxfile }}
+      Max Path:{{ item.maxpath }}
+      Options:{{ item.opts }}
+{% endfor %}
+ {% include 'handyhelpers/component/bs5/modals.htm' %} {% endblock content %}
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html`

 * *Files 5% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     {% include 'handyhelpers/component/chartjs_components.htm' %}
     <style>
         .card .card-header {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             font-size: 1.25rem;
         }
         .key {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             margin-right: .25rem
         }
         .value {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             margin-left: .25rem
         }
         .titlecard-container {
             display: flex;
             gap: 2rem;
             flex-wrap: wrap;
         }
         .titlecard-container > * {
             flex: 1;
         }
         .titlecard {
             height: 8rem;
         }
         .titlecard .stat {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-size: 2.5rem;
             font-weight: bold;
             text-align: center;
             margin-top: -.75rem;
         }
         .titlecard .description {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             font-weight: bold;
             font-size: 1rem;
             text-align: center;
             margin-top: .65rem
         }
 
     </style>
@@ -177,16 +177,16 @@
         </div>
     </div>
 </section>
 
 <script>
     var style = getComputedStyle(document.body);
     var theme = {};
-    theme.primary = style.getPropertyValue('--bs-primary');
-    theme.secondary = style.getPropertyValue('--bs-secondary');
+    theme.primary = style.getPropertyValue('--primary');
+    theme.secondary = style.getPropertyValue('--secondary');
     new Chart(document.getElementById("virtual-usage-chart"), {
     type: 'pie',
     data: {
       labels: ["Used", "Free"],
       datasets: [{
         label: "Virtual Memory Usage",
         backgroundColor: [theme.primary, theme.secondary],
@@ -211,23 +211,23 @@
         }
     }
 });
 </script>
 <script>
     var style = getComputedStyle(document.body);
     var theme = {};
-    theme.primary = style.getPropertyValue('--bs-primary');
-    theme.secondary = style.getPropertyValue('--bs-secondary');
-    theme.success = style.getPropertyValue('--bs-success');
-    theme.info = style.getPropertyValue('--bs-info');
-    theme.warning = style.getPropertyValue('--bs-warning');
-    theme.danger = style.getPropertyValue('--bs-danger');
-    theme.dark = style.getPropertyValue('--bs-dark');
-    theme.blue = style.getPropertyValue('--bs-blue');
-    theme.indigo = style.getPropertyValue('--bs-indigo');
+    theme.primary = style.getPropertyValue('--primary');
+    theme.secondary = style.getPropertyValue('--secondary');
+    theme.success = style.getPropertyValue('--success');
+    theme.info = style.getPropertyValue('--info');
+    theme.warning = style.getPropertyValue('--warning');
+    theme.danger = style.getPropertyValue('--danger');
+    theme.dark = style.getPropertyValue('--dark');
+    theme.blue = style.getPropertyValue('--blue');
+    theme.indigo = style.getPropertyValue('--indigo');
 
     new Chart(document.getElementById("virtual-stats-chart"), {
     type: 'bar',
     data: {
       labels: ["available", "used", "free", "active", "inactive", "buffers", "cached", "shared", "slab"],
       datasets: [{
         label: "Virtual Memory Stats",
@@ -254,16 +254,16 @@
     }
 });
 </script>
 
 <script>
     var style = getComputedStyle(document.body);
     var theme = {};
-    theme.primary = style.getPropertyValue('--bs-primary');
-    theme.secondary = style.getPropertyValue('--bs-secondary');
+    theme.primary = style.getPropertyValue('--primary');
+    theme.secondary = style.getPropertyValue('--secondary');
     new Chart(document.getElementById("swap-usage-chart"), {
     type: 'pie',
     data: {
       labels: ["Used", "Free"],
       datasets: [{
         label: "Swap Memory Usage",
         backgroundColor: [theme.primary, theme.secondary],
@@ -288,16 +288,16 @@
         }
     }
 });
 </script>
 <script>
     var style = getComputedStyle(document.body);
     var theme = {};
-    theme.primary = style.getPropertyValue('--bs-primary');
-    theme.secondary = style.getPropertyValue('--bs-secondary');
+    theme.primary = style.getPropertyValue('--primary');
+    theme.secondary = style.getPropertyValue('--secondary');
     new Chart(document.getElementById("swap-disk-chart"), {
     type: 'bar',
     data: {
       labels: ["In", "Out"],
       datasets: [{
         label: "Swap Disk Activity",
         backgroundColor: [theme.primary, theme.secondary],
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 {% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     <style>
-        .card a { text-decoration: none; }
         .card .card-header {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             font-size: 1.25rem;
         }
         .connection-card {
             background-color: var(--light);
             padding-left: 1rem;
             padding-right: 1rem;
             margin-bottom: 1rem;
         }
         .key {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             margin-right: .25rem
         }
         .value {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             margin-left: .25rem
         }
         .titlecard-container {
             display: flex;
             gap: 2rem;
             flex-wrap: wrap;
             align-content: center;
@@ -38,28 +37,28 @@
         }
         .titlecard {
             height: 6rem;
             min-width: 148px;
             max-width: 475;
         }
         .titlecard .icon {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-size: 2.5rem;
             text-align: left;
             margin-top: -.5rem;
         }
         .titlecard .stat {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-size: 2rem;
             font-weight: bold;
             text-align: center;
             margin-top: -.5rem;
         }
         .titlecard .description {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             font-weight: bold;
             font-size: .8rem;
             text-align: center;
         }
     </style>
 {% endblock %}
 
@@ -137,15 +136,15 @@
     <div class="container-fluid mt-5">
         <div class="card shadow">
             <div class="card-header">Network Interfaces <span class="small">({{ interface_list|length }})</span></div>
                 <div class="card-body" style="overflow-y: auto; overflow-x: hidden; height: 200px">
                     <ul class="list-group mx-auto justify-content-center" style="max-width: 93%; margin-top: .5%; margin-bottom: .5%">
                         {% for k,v in interface_list.items %}
                         <li class="list-group-item bg-light shadow-sm hvr-grow mb-3">
-                            <a href="#" hx-get="{% url 'hostutils:get_interface_stats' k %}" hx-target="#modal_wrapper">
+                            <a href="#" onClick="showInfo('{% url "hostutils:get_interface_stats" %}', '{{k}}', 'Network Stats: <small><i>{{k}}</i></small>', false);">
                                 <div class="row">
                                     <div class="key h5">{{ k }}:</div>
                                     {% for item in v %}
                                     <div class="col-xs-12 col-md-3"><span class="key">address:</span><span class="value">{{ item.address }}</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">netmask:</span><span class="value">{{ item.netmask }}</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">broadcast:</span><span class="value">{{ item.broadcast }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">family:</span><span class="value">{{ item.family.name }}</span></div>
@@ -186,9 +185,9 @@
                     </ul>
                 </div>
             </div>
         </div>
     </div>
 </section>
 
-{% include 'handyhelpers/htmx/bs5/generic_modal.htm' %}
+{% include 'handyhelpers/component/bs5/modals.htm' %}
 {% endblock content %}
```

#### html2text {}

```diff
@@ -19,30 +19,31 @@
 {{ counters.dropin }}
 Drops In
 {{ counters.dropout }}
 Drops Out
 
 Network Interfaces ({{ interface_list|length }})
     * {% for k,v in interface_list.items %}
-    * {{_k_}}:
-      {%_for_item_in_v_%}
-      address:{{_item.address_}}
-      netmask:{{_item.netmask_}}
-      broadcast:{{_item.broadcast_}}
-      family:{{_item.family.name_}}
-      ptp:{{_item.ptp_}}
-      {%_endfor_%}
-    * {% endfor %}
+    *  %}', '{{k}}', 'Network Stats: {{k}}', false);">
+      {{ k }}:
+      {% for item in v %}
+      address:{{ item.address }}
+      netmask:{{ item.netmask }}
+      broadcast:{{ item.broadcast }}
+      family:{{ item.family.name }}
+      ptp:{{ item.ptp }}
+      {% endfor %}
+{% endfor %}
 
 Network Connections ({{ connection_list|length }})
     * {% for connection in connection_list %}
     * laddr:{{ connection.laddr.ip }}
       lport:{{ connection.laddr.port }}
       family:{{ connection.family.name }}
       fd:{{ connection.fd }}
       status:{{ connection.status }}
       raddr:{{ connection.raddr.ip }}
       rport:{{ connection.raddr.port }}
       type:{{ connection.type }}
       pid:{{ connection.pid }}
       {% endfor %}
- {% include 'handyhelpers/htmx/bs5/generic_modal.htm' %} {% endblock content %}
+ {% include 'handyhelpers/component/bs5/modals.htm' %} {% endblock content %}
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 {% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
     <style>
         .card .card-header {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             font-size: 1.25rem;
         }
         .key {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-weight: bold;
             margin-right: .25rem
         }
         .value {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             margin-left: .25rem
         }
         .titlecard-container {
             display: flex;
             gap: 2rem;
             flex-wrap: wrap;
             align-content: center;
@@ -32,28 +32,28 @@
         .titlecard {
             height: 6rem;
             min-width: 148px;
             max-width: 475;
             cursor: pointer;
         }
         .titlecard .icon {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-size: 2.5rem;
             text-align: left;
             margin-top: -.5rem;
         }
         .titlecard .stat {
-            color: var(--bs-primary);
+            color: var(--primary);
             font-size: 2rem;
             font-weight: bold;
             text-align: center;
             margin-top: -.5rem;
         }
         .titlecard .description {
-            color: var(--bs-secondary);
+            color: var(--secondary);
             font-weight: bold;
             font-size: .8rem;
             text-align: center;
         }
     </style>
 {% endblock %}
 
@@ -131,13 +131,13 @@
 
 <section class="mb-5 animated fadeIn" style="animation-delay: .35s;">
     <div class="container-fluid mt-5" id="id_process_list_container">
         {% include 'hostutils/bs5/snippets/host_process_card.htm' %}
     </div>
 </section>
 
-{% include 'handyhelpers/htmx/bs5/generic_modal.htm' %}
+{% include 'handyhelpers/component/bs5/modals.htm' %}
 {% with filter_form as form_data %}
     {% include 'handyhelpers/generic/bs5/generic_modal_form_htmx.htm' %}
 {% endwith %}
 
 {% endblock content %}
```

#### html2text {}

```diff
@@ -16,10 +16,10 @@
 {{ counts.zombie }}
 Zombie
 {{ counts.dead }}
 Dead
 
 
 {% include 'hostutils/bs5/snippets/host_process_card.htm' %}
- {% include 'handyhelpers/htmx/bs5/generic_modal.htm' %} {% with filter_form as
+ {% include 'handyhelpers/component/bs5/modals.htm' %} {% with filter_form as
 form_data %} {% include 'handyhelpers/generic/bs5/generic_modal_form_htmx.htm'
 %} {% endwith %} {% endblock content %}
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_cpu_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,81 @@
+{% if data %}
 <div class="container-fluid">
     <br/>
     <div class="row">
         <div class="col-7">
             <div class="h3 font-weight-bold text-primary">CPU Times</div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">System: </div>
-                <div class="col-2 text-secondary">{{ time_percent.system }}%</div>
-                <div class="col-6 text-secondary">{{ time.system }}</div>
+                <div class="col-3 text-primary font-weight-bold">System: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.system }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.system }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Idle: </div>
-                <div class="col-2 text-secondary">{{ time_percent.idle }}%</div>
-                <div class="col-6 text-secondary">{{ time.idle }}</div>
+                <div class="col-3 text-primary font-weight-bold">Idle: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.idle }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.idle }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">User: </div>
-                <div class="col-2 text-secondary">{{ time_percent.user }}%</div>
-                <div class="col-6 text-secondary">{{ time.user }}</div>
+                <div class="col-3 text-primary font-weight-bold">User: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.user }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.user }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Nice: </div>
-                <div class="col-2 text-secondary">{{ time_percent.nice }}%</div>
-                <div class="col-6 text-secondary">{{ time.nice }}</div>
+                <div class="col-3 text-primary font-weight-bold">Nice: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.nice }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.nice }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">IO Wait: </div>
-                <div class="col-2 text-secondary">{{ time_percent.iowait }}%</div>
-                <div class="col-6 text-secondary">{{ time.iowait }}</div>
+                <div class="col-3 text-primary font-weight-bold">IO Wait: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.iowait }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.iowait }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">IRQ: </div>
-                <div class="col-2 text-secondary">{{ time_percent.irq }}%</div>
-                <div class="col-6 text-secondary">{{ time.irq }}</div>
+                <div class="col-3 text-primary font-weight-bold">IRQ: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.irq }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.irq }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Soft IRQ: </div>
-                <div class="col-2 text-secondary">{{ time_percent.softirq }}%</div>
-                <div class="col-6 text-secondary">{{ time.system }}</div>
+                <div class="col-3 text-primary font-weight-bold">Soft IRQ: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.softirq }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.system }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Steal: </div>
-                <div class="col-2 text-secondary">{{ time_percent.steal }}%</div>
-                <div class="col-6 text-secondary">{{ time.steal }}</div>
+                <div class="col-3 text-primary font-weight-bold">Steal: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.steal }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.steal }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Guest: </div>
-                <div class="col-2 text-secondary">{{ time_percent.guest }}%</div>
-                <div class="col-6 text-secondary">{{ time.guest }}</div>
+                <div class="col-3 text-primary font-weight-bold">Guest: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.guest }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.guest }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Guest Nice: </div>
-                <div class="col-2 text-secondary">{{ time_percent.guest_nice }}%</div>
-                <div class="col-6 text-secondary">{{ time.guest_nice }}</div>
+                <div class="col-3 text-primary font-weight-bold">Guest Nice: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.guest_nice }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.guest_nice }}</div>
             </div>
 
         </div>
 
         <div class="col-5">
             <div class="h3 font-weight-bold text-primary">CPU Frequencies</div>
             <div class="row m-3">
-                <div class="col-5 text-primary font-weight-bold">Current: </div>
-                <div class="col-7 text-secondary">{{ frequency.current }}</div>
+                <div class="col-6 text-primary font-weight-bold">Current: </div>
+                <div class="col-6 text-secondary">{{ data.frequency.current }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-5 text-primary font-weight-bold">Min: </div>
-                <div class="col-7 text-secondary">{{ frequency.min }}</div>
+                <div class="col-6 text-primary font-weight-bold">Min: </div>
+                <div class="col-6 text-secondary">{{ data.frequency.min }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-5 text-primary font-weight-bold">Max: </div>
-                <div class="col-7 text-secondary">{{ frequency.max }}</div>
+                <div class="col-6 text-primary font-weight-bold">Max: </div>
+                <div class="col-6 text-secondary">{{ data.frequency.max }}</div>
             </div>
         </div>
     </div>
 </div>
+{% else %}
+<div class="container-fluid">
+    data not available for this partition
+</div>
+{% endif %}
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_interface_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_partition_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,28 @@
-{% load handyhelper_tags %}
+{% if data %}
 <div class="container-fluid">
     <div class="row m-3">
-        <div class="col-3 text-primary font-weight-bold">Total: </div>
-        <div class="col-9 text-secondary">{{ data.total|byte_size }}</div>
+        <div class="col-3 text-primary font-weight-bold">Up: </div>
+        <div class="col-9 text-secondary">{{ data.isup }}</div>
     </div>
     <div class="row m-3">
-        <div class="col-3 text-primary font-weight-bold">Used:</div>
-        <div class="col-9 text-secondary">{{ data.used|byte_size }}</div>
+        <div class="col-3 text-primary font-weight-bold">Duplex:</div>
+        <div class="col-9 text-secondary">{{ data.duplex.name }}</div>
     </div>
     <div class="row m-3">
-        <div class="col-3 text-primary font-weight-bold">Free:</div>
-        <div class="col-9 text-secondary">{{ data.free|byte_size }}</div>
+        <div class="col-3 text-primary font-weight-bold">Speed:</div>
+        <div class="col-9 text-secondary">{{ data.speed }}</div>
     </div>
     <div class="row m-3">
-        <div class="col-3 text-primary font-weight-bold">Percent:</div>
-        <div class="col-9 text-secondary">{{ data.percent }}%</div>
+        <div class="col-3 text-primary font-weight-bold">MTU:</div>
+        <div class="col-9 text-secondary">{{ data.mtu }}</div>
     </div>
+    <div class="row m-3">
+        <div class="col-3 text-primary font-weight-bold">Flags:</div>
+        <div class="col-9 text-secondary">{{ data.flags }}</div>
+    </div>
+</div>
+{% else %}
+<div class="container-fluid">
+    data not available for this partition
 </div>
+{% endif %}
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_process_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 {% load handyhelper_tags %}
+{% if data %}
 <div class="container-fluid">
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">PID: </div>
-        <div class="col-9 text-secondary">{{ pid }}</div>
+        <div class="col-9 text-secondary">{{ data.pid }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">PPID: </div>
-        <div class="col-9 text-secondary">{{ ppid }}</div>
+        <div class="col-9 text-secondary">{{ data.ppid }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Name:</div>
-        <div class="col-9 text-secondary">{{ name }}</div>
+        <div class="col-9 text-secondary">{{ data.name }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Status:</div>
-        <div class="col-9 text-secondary">{{ status }}</div>
+        <div class="col-9 text-secondary">{{ data.status }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Stated At:</div>
-        <div class="col-9 text-secondary">{{ create_time|to_datetime }}</div>
+        <div class="col-9 text-secondary">{{ data.create_time|to_datetime }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Username:</div>
-        <div class="col-9 text-secondary">{{ username }}</div>
+        <div class="col-9 text-secondary">{{ data.username }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Command:</div>
-        <div class="col-9 text-secondary">{{ cmdline|join:" " }}</div>
+        <div class="col-9 text-secondary">{{ data.cmdline|join:" " }}</div>
     </div>
-    {% if exe %}
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Executable:</div>
-        <div class="col-9 text-secondary">{{ exe }}</div>
+        <div class="col-9 text-secondary">{{ data.exe }}</div>
     </div>
-    {% endif %}
-    {% if cwd %}
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Working Directory:</div>
-        <div class="col-9 text-secondary">{{ cwd }}</div>
+        <div class="col-9 text-secondary">{{ data.cwd }}</div>
     </div>
-    {% endif %}
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">CPU:</div>
-        <div class="col-9 text-secondary">{{ cpu_num }}</div>
+        <div class="col-9 text-secondary">{{ data.cpu_num }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">CPU Percent:</div>
-        <div class="col-9 text-secondary">{{ cpu_percent }}%</div>
+        <div class="col-9 text-secondary">{{ data.cpu_percent }}%</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Memory Percent:</div>
-        <div class="col-9 text-secondary">{{ memory_percent|percentage }}</div>
+        <div class="col-9 text-secondary">{{ data.memory_percent|percentage }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Thread Count:</div>
-        <div class="col-9 text-secondary">{{ num_threads }}</div>
+        <div class="col-9 text-secondary">{{ data.num_threads }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Threads:</div>
-        <div class="col-9 text-secondary">{% for thread in threads%}{{ thread }}<br>{% endfor %}</div>
+        <div class="col-9 text-secondary">{{ data.threads|join:", " }}</div>
     </div>
 </div>
+{% else %}
+<div class="container-fluid">
+    data not available for this process
+</div>
+{% endif %}
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load handyhelper_tags %}
         <div class="card shadow">
             <div class="card-header">
                 <div class="row">
-                    <div class="col-6 text-start">
+                    <div class="col-6 text-left">
                         Processes <span class="small">({{ process_list|length }})</span>
                     </div>
-                    <div class="col-6 text-end">
+                    <div class="col-6 text-right">
                         <span href="#" data-bs-toggle="modal" data-bs-target="#modal_{{ filter_form.modal_name }}" title="{{ filter_form.tool_tip|default_if_none:'filter' }}" class="mx-1" style="cursor: pointer;">
                             <i class="fas fa-filter"></i>
                         </span>
                         {% if clear_filter %}
                         <span hx-get="{% url 'hostutils:get_host_processes' %}?clear=True" hx-target='#id_process_list_container' title="clear filters" class="mx-1" style="cursor: pointer;" onclick="document.getElementById('form_{{ filter_form.modal_name }}').reset()">
                             <i class="fas fa-undo-alt"></i>
                         </span>
@@ -17,15 +17,15 @@
                     </div>
                 </div>
             </div>
                 <div class="card-body" style="overflow-y: auto; overflow-x: hidden; max-height: 50vh; cursor: pointer;">
                     <ul class="list-group mx-auto justify-content-center" style="max-width: 93%; margin-top: .5%; margin-bottom: .5%">
                         {% for item in process_list %}
                         <li class="list-group-item bg-light shadow-sm hvr-grow mb-3">
-                            <div hx-get="{% url 'hostutils:get_process_stats' item.pid %}" hx-target="#modal_wrapper">
+                            <div onClick="showInfo('{% url "hostutils:get_process_stats" %}', '{{item.pid}}', 'Process Details: <small><i>{{item.name}}</i></small>', true);">
                                 <div class="row">
                                     <div class="col-xs-12 col-md-2"><span class="key">PID:</span><span class="value">{{ item.pid }}</span></div>
                                     <div class="col-xs-12 col-md-4"><span class="key">Name:</span><span class="value">{{ item.name }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Status:</span><span class="value">{{ item.status }}</span></div>
                                     <div class="col-xs-12 col-md-4"><span class="key">Started At:</span><span class="value">{{ item.create_time|to_datetime }}</span></div>
                                 </div>
                             </div>
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/urls.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from django.urls import path
-
-from djangoaddicts.hostutils.views import gui, htmx
+from djangoaddicts.hostutils.views import ajax
+from djangoaddicts.hostutils.views import gui
+from djangoaddicts.hostutils.views import htmx
 
 app_name = "hostutils"
 
 urlpatterns = [
     # host views
     path("host_cpu/", gui.ShowHostCpu.as_view(), name="host_cpu"),
     path("host_details/", gui.ShowHost.as_view(), name="host_details"),
     path("host_disk/", gui.ShowHostDisk.as_view(), name="host_disk"),
     path("host_memory/", gui.ShowHostMemory.as_view(), name="host_memory"),
     path("host_network/", gui.ShowHostNetwork.as_view(), name="host_network"),
     path("host_process/", gui.ShowHostProcesses.as_view(), name="host_process"),
+    # ajax views
+    path("get_cpu_stats/", ajax.GetHostCpuStats.as_view(), name="get_cpu_stats"),
+    path("get_interface_stats/", ajax.GetHostNetworkStats.as_view(), name="get_interface_stats"),
+    path("get_partition_stats/", ajax.GetHostParitionStats.as_view(), name="get_partition_stats"),
+    path("get_process_stats/", ajax.GetHostProcessStats.as_view(), name="get_process_stats"),
     # htmx views
     path("get_host_processes/", htmx.GetHostProcesses.as_view(), name="get_host_processes"),
-    path("get_cpu_stats/<int:cpu>/", htmx.GetHostCpuStats.as_view(), name="get_cpu_stats"),
-    path("get_interface_stats/<str:interface>/", htmx.GetHostNetworkStats.as_view(), name="get_interface_stats"),
-    path("get_partition_stats/", htmx.GetHostParitionStats.as_view(), name="get_partition_stats"),
-    path("get_process_stats/<int:pid>/", htmx.GetHostProcessStats.as_view(), name="get_process_stats"),
 ]
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/views/__init__.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from djangoaddicts.hostutils.views.ajax import (
+    GetHostCpuStats,
+    GetHostNetworkStats,
+    GetHostParitionStats,
+    GetHostProcessStats,
+)
 from djangoaddicts.hostutils.views.gui import (
     ShowHost,
     ShowHostCpu,
     ShowHostDisk,
     ShowHostMemory,
     ShowHostNetwork,
     ShowHostProcesses,
 )
-from djangoaddicts.hostutils.views.htmx import (
-    GetHostCpuStats,
-    GetHostNetworkStats,
-    GetHostParitionStats,
-    GetHostProcesses,
-    GetHostProcessStats,
-)
+from djangoaddicts.hostutils.views.htmx import GetHostProcesses
+
 
 __all__ = [
     "GetHostCpuStats",
     "GetHostNetworkStats",
     "GetHostParitionStats",
     "GetHostProcessStats",
     "GetHostProcesses",
```

### Comparing `django-hostutils-0.0.7/src/djangoaddicts/hostutils/views/gui.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import datetime
-
 import psutil
+
 from dateutil.relativedelta import relativedelta
 from django.shortcuts import render
 from django.views.generic import View
 
 # import forms
 from djangoaddicts.hostutils.forms import HostProcessFilterForm
 
 
 class ShowHost(View):
     """Display dashboard like page showing an overview of host data"""
 
     template_name = "hostutils/bs5/detail/detail_host.html"
-    title = "Host Dashboard"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         now = datetime.datetime.now()
         context = {}
-        context["title"] = self.title
+        context["title"] = "Host Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
         context["cpu_count"] = psutil.cpu_count(logical=False)
         context["memory"] = psutil.virtual_memory()
         context["disk_usage"] = psutil.disk_usage("/")
         context["disk_io_counters"] = psutil.disk_io_counters()
         context["network"] = psutil.net_connections()
         context["pids"] = psutil.pids()
@@ -37,128 +36,123 @@
         )
 
         context["platform"] = psutil.os.uname()
 
         return render(request, self.template_name, context=context)
 
 
-class ShowHostCpu(View):
-    """Display dashboard like page showing host cpu data"""
+class ShowHostProcesses(View):
+    """Display dashboard like page showing host process data"""
 
-    template_name = "hostutils/bs5/detail/cpu.html"
-    title = "CPU Dashboard"
+    template_name = "hostutils/bs5/detail/processes.html"
 
     def get(self, request, *args, **kwargs):
-        """CPU Dashboard"""
+        """allow get method"""
         context = {}
-        context["title"] = self.title
+        context["title"] = "Host Processes"
+        context["now"] = datetime.datetime.now()
         context["subtitle"] = psutil.os.uname()[1]
-        context["stats"] = psutil.cpu_stats()
-        context["physical_count"] = psutil.cpu_count(logical=False)
-        context["logical_count"] = psutil.cpu_count(logical=True)
-        context["percent"] = psutil.cpu_percent(interval=None)
-        context["times_list"] = psutil.cpu_times(percpu=True)
-        context["times_percent_list"] = psutil.cpu_times_percent(percpu=True)
-        context["percent_list"] = psutil.cpu_percent(interval=None, percpu=True)
-        context["frequency_list"] = psutil.cpu_freq(percpu=True)
-        context["cpu_range"] = list(range(psutil.cpu_count(logical=True)))
-        cpu_data = {}
-        for i in range(context["logical_count"]):
-            cpu_data[i] = {
-                "times": context["times_list"][i],
-                "time_percent": context["times_percent_list"][i],
-                "percent": context["percent_list"][i],
-                "frequency": context["frequency_list"][i],
-            }
-        context["cpu_data"] = cpu_data
-        context["load_avg_1"], context["load_avg_5"], context["load_avg_15"] = [
-            round(x / psutil.cpu_count() * 100, 2) for x in psutil.getloadavg()
-        ]
+        process_list = list(psutil.process_iter())
+        context["process_list"] = process_list
+        counts = {
+            "running": len([i for i in process_list if i.status() == "running"]),
+            "sleeping": len([i for i in process_list if i.status() == "sleeping"]),
+            "idle": len([i for i in process_list if i.status() == "idle"]),
+            "stopped": len([i for i in process_list if i.status() == "stopped"]),
+            "zombie": len([i for i in process_list if i.status() == "zombie"]),
+            "dead": len([i for i in process_list if i.status() == "dead"]),
+        }
+        context["counts"] = counts
+        filter_form = {}
+        filter_form["form"] = HostProcessFilterForm(request.GET or None)
+        filter_form["modal_name"] = "filter_processes"
+        filter_form["modal_size"] = "modal-lg"
+        filter_form["modal_title"] = "Filter Host Processes"
+        filter_form["hx_method"] = "hx-get"
+        filter_form["hx_url"] = "/hostutils/get_host_processes"
+        filter_form["hx_target"] = "id_process_list_container"
+        filter_form["method"] = "GET"
+        filter_form["action"] = "Filter"
+        context["filter_form"] = filter_form
+        return render(request, self.template_name, context=context)
+
+
+class ShowHostNetwork(View):
+    """Display dashboard like page showing host network data"""
+
+    template_name = "hostutils/bs5/detail/network.html"
+
+    def get(self, request, *args, **kwargs):
+        """allow get method"""
+        context = {}
+        context["title"] = "Network Dashboard"
+        context["subtitle"] = psutil.os.uname()[1]
+        context["connection_list"] = psutil.net_connections()
+        context["interface_list"] = psutil.net_if_addrs()
+        context["stats_list"] = psutil.net_if_stats()
+        context["counters"] = psutil.net_io_counters()
         return render(request, self.template_name, context=context)
 
 
 class ShowHostDisk(View):
     """Display dashboard like page showing host disk data"""
 
     template_name = "hostutils/bs5/detail/disk.html"
-    title = "Disk Dashboard"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         context = {}
-        context["title"] = self.title
+        context["title"] = "Disk Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
         context["usage"] = psutil.disk_usage("/")
         context["io_counters"] = psutil.disk_io_counters()
         context["partition_lists"] = psutil.disk_partitions()
         return render(request, self.template_name, context=context)
 
 
 class ShowHostMemory(View):
     """Display dashboard like page showing host memory data"""
 
     template_name = "hostutils/bs5/detail/memory.html"
-    title = "Memory Dashboard"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         context = {}
-        context["title"] = self.title
+        context["title"] = "Memory Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
         context["virtual"] = psutil.virtual_memory()
         context["swap"] = psutil.swap_memory()
         return render(request, self.template_name, context=context)
 
 
-class ShowHostNetwork(View):
-    """Display dashboard like page showing host network data"""
-
-    template_name = "hostutils/bs5/detail/network.html"
-    title = "Network Dashboard"
-
-    def get(self, request, *args, **kwargs):
-        """allow get method"""
-        context = {}
-        context["title"] = self.title
-        context["subtitle"] = psutil.os.uname()[1]
-        context["connection_list"] = psutil.net_connections()
-        context["interface_list"] = psutil.net_if_addrs()
-        context["stats_list"] = psutil.net_if_stats()
-        context["counters"] = psutil.net_io_counters()
-        return render(request, self.template_name, context=context)
-
-
-class ShowHostProcesses(View):
-    """Display dashboard like page showing host process data"""
+class ShowHostCpu(View):
+    """Display dashboard like page showing host cpu data"""
 
-    template_name = "hostutils/bs5/detail/processes.html"
-    title = "Process Dashboard"
+    template_name = "hostutils/bs5/detail/cpu.html"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         context = {}
-        context["title"] = self.title
-        context["now"] = datetime.datetime.now()
+        context["title"] = "CPU Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
-        process_list = list(psutil.process_iter())
-        context["process_list"] = process_list
-        counts = {
-            "running": len([i for i in process_list if i.status() == "running"]),
-            "sleeping": len([i for i in process_list if i.status() == "sleeping"]),
-            "idle": len([i for i in process_list if i.status() == "idle"]),
-            "stopped": len([i for i in process_list if i.status() == "stopped"]),
-            "zombie": len([i for i in process_list if i.status() == "zombie"]),
-            "dead": len([i for i in process_list if i.status() == "dead"]),
-        }
-        context["counts"] = counts
-        filter_form = {}
-        filter_form["form"] = HostProcessFilterForm(request.GET or None)
-        filter_form["modal_name"] = "filter_processes"
-        filter_form["modal_size"] = "modal-lg"
-        filter_form["modal_title"] = "Filter Host Processes"
-        filter_form["hx_method"] = "hx-get"
-        filter_form["hx_url"] = "/hostutils/get_host_processes"
-        filter_form["hx_target"] = "id_process_list_container"
-        filter_form["method"] = "GET"
-        filter_form["action"] = "Filter"
-        context["filter_form"] = filter_form
+        context["stats"] = psutil.cpu_stats()
+        context["physical_count"] = psutil.cpu_count(logical=False)
+        context["logical_count"] = psutil.cpu_count(logical=True)
+        context["percent"] = psutil.cpu_percent(interval=None)
+        context["times_list"] = psutil.cpu_times(percpu=True)
+        context["times_percent_list"] = psutil.cpu_times_percent(percpu=True)
+        context["percent_list"] = psutil.cpu_percent(interval=None, percpu=True)
+        context["frequency_list"] = psutil.cpu_freq(percpu=True)
+        context["cpu_range"] = list(range(psutil.cpu_count(logical=True)))
+        cpu_data = {}
+        for i in range(context["logical_count"]):
+            cpu_data[i] = {
+                "times": context["times_list"][i],
+                "time_percent": context["times_percent_list"][i],
+                "percent": context["percent_list"][i],
+                "frequency": context["frequency_list"][i],
+            }
+        context["cpu_data"] = cpu_data
+        context["load_avg_1"], context["load_avg_5"], context["load_avg_15"] = [
+            round(x / psutil.cpu_count() * 100, 2) for x in psutil.getloadavg()
+        ]
         return render(request, self.template_name, context=context)
```

