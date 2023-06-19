# Comparing `tmp/powermanim-0.0.6.tar.gz` & `tmp/powermanim-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powermanim-0.0.6.tar", last modified: Fri Apr  7 23:26:19 2023, max compression
+gzip compressed data, was "powermanim-0.0.7.tar", last modified: Mon Jun 19 17:10:10 2023, max compression
```

## Comparing `powermanim-0.0.6.tar` & `powermanim-0.0.7.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-07 23:23:00.000000 powermanim-0.0.6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-07 23:23:00.000000 powermanim-0.0.6/.env.template
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-04-07 23:23:00.000000 powermanim-0.0.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-04-07 23:23:00.000000 powermanim-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4773 2023-04-07 23:23:00.000000 powermanim-0.0.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-04-07 23:23:00.000000 powermanim-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-04-07 23:23:00.000000 powermanim-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-04-07 23:23:00.000000 powermanim-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1939 2023-04-07 23:26:19.965717 powermanim-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-04-07 23:23:00.000000 powermanim-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/data/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-07 23:23:00.000000 powermanim-0.0.6/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/.hugo_build.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/assets/media/
--rw-r--r--   0 runner    (1001) docker     (122)    39583 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/media/banner.png
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/media/book.svg
--rw-r--r--   0 runner    (1001) docker     (122)    15329 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/media/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/assets/media/icons/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/media/icons/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/scss/custom.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/config/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/config/_default/
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/config/_default/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/config/_default/languages.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/config/_default/menus.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/config/_default/params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/content/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/content/authors/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/authors/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/authors/admin/_index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/_index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/docs/chapter1/
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter1/_index.md
--rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter1/reading-list.md
--rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter1/syllabus.md
--rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter1/takeaways.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/docs/chapter2/
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter2/_index.md
--rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter2/reading-list.md
--rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter2/syllabus.md
--rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter2/takeaways.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/home/
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/home/animations.md
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/home/features.md
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/home/index.md
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/go.mod
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/layouts/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/layouts/partials/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/layouts/partials/views/
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/layouts/partials/views/masonry.html
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/netlify.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/docs/static/uploads/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/static/uploads/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-07 23:26:12.000000 powermanim-0.0.6/env.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-04-07 23:23:00.000000 powermanim-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-07 23:26:19.969717 powermanim-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-07 23:23:00.000000 powermanim-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/components/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/chartbars.py
--rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/numberslider.py
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/powermanim.py
--rw-r--r--   0 runner    (1001) docker     (122)     3048 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/vgrouphighlight.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/layouts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4897 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/layouts/arrangedbullets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2152 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/scripts/build_anims
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/showcase/
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/showcase/components/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/components/chartbars.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/components/numberslider.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/components/vgroupghighlight.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/showcase/layouts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/layouts/arrangedbullets.py
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/showcasescene.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/showcase/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/templates/bulletlist.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/templates/sectiontitle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/templates/bulletlist.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/templates/sectiontitle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1939 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 23:24:14.000000 powermanim-0.0.6/src/powermanim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/tests/showcase/
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-04-07 23:23:00.000000 powermanim-0.0.6/tests/showcase/test_showcasing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-19 17:05:56.000000 powermanim-0.0.7/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-19 17:05:56.000000 powermanim-0.0.7/.env.template
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-06-19 17:05:56.000000 powermanim-0.0.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.669212 powermanim-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.673212 powermanim-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-06-19 17:05:56.000000 powermanim-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4773 2023-06-19 17:05:56.000000 powermanim-0.0.7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-06-19 17:05:56.000000 powermanim-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-06-19 17:05:56.000000 powermanim-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-19 17:05:56.000000 powermanim-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1939 2023-06-19 17:10:10.685213 powermanim-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-06-19 17:05:56.000000 powermanim-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.673212 powermanim-0.0.7/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-19 17:05:56.000000 powermanim-0.0.7/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.673212 powermanim-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/.hugo_build.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.669212 powermanim-0.0.7/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/assets/media/
+-rw-r--r--   0 runner    (1001) docker     (122)    39583 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/assets/media/banner.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/assets/media/book.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    15329 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/assets/media/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/assets/media/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/assets/media/icons/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/assets/scss/custom.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.669212 powermanim-0.0.7/docs/config/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/config/_default/
+-rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/config/_default/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/config/_default/languages.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/config/_default/menus.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/config/_default/params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.669212 powermanim-0.0.7/docs/content/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.669212 powermanim-0.0.7/docs/content/authors/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/content/authors/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/authors/admin/_index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/content/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/docs/_index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/content/docs/chapter1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/docs/chapter1/_index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/docs/chapter1/reading-list.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/docs/chapter1/syllabus.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/docs/chapter1/takeaways.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/content/docs/chapter2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/docs/chapter2/_index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/docs/chapter2/reading-list.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/docs/chapter2/syllabus.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/docs/chapter2/takeaways.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/content/home/
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/home/animations.md
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/home/features.md
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/content/home/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/go.mod
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.669212 powermanim-0.0.7/docs/layouts/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.669212 powermanim-0.0.7/docs/layouts/partials/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/layouts/partials/views/
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/layouts/partials/views/masonry.html
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/netlify.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.673212 powermanim-0.0.7/docs/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/docs/static/uploads/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/docs/static/uploads/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-06-19 17:10:00.000000 powermanim-0.0.7/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-19 17:05:56.000000 powermanim-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-19 17:10:10.685213 powermanim-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-19 17:05:56.000000 powermanim-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.673212 powermanim-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.677213 powermanim-0.0.7/src/powermanim/
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-19 17:10:10.000000 powermanim-0.0.7/src/powermanim/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/src/powermanim/components/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/components/chartbars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/components/numberslider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/components/powermanim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3016 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/components/vgrouphighlight.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/src/powermanim/layouts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4897 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/layouts/arrangedbullets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/src/powermanim/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2152 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/scripts/build_anims
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/src/powermanim/showcase/
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/src/powermanim/showcase/components/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/components/chartbars.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/components/numberslider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/components/vgroupghighlight.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/src/powermanim/showcase/layouts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/layouts/arrangedbullets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/showcasescene.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/src/powermanim/showcase/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/templates/bulletlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/showcase/templates/sectiontitle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/src/powermanim/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/templates/bulletlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-19 17:05:56.000000 powermanim-0.0.7/src/powermanim/templates/sectiontitle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/src/powermanim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1939 2023-06-19 17:10:10.000000 powermanim-0.0.7/src/powermanim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-06-19 17:10:10.000000 powermanim-0.0.7/src/powermanim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 17:10:10.000000 powermanim-0.0.7/src/powermanim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 17:07:35.000000 powermanim-0.0.7/src/powermanim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-19 17:10:10.000000 powermanim-0.0.7/src/powermanim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-19 17:10:10.000000 powermanim-0.0.7/src/powermanim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:05:56.000000 powermanim-0.0.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:10:10.681213 powermanim-0.0.7/tests/showcase/
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-19 17:05:56.000000 powermanim-0.0.7/tests/showcase/test_showcasing.py
```

### Comparing `powermanim-0.0.6/.github/workflows/publish.yml` & `powermanim-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/.github/workflows/tests.yml` & `powermanim-0.0.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/.gitignore` & `powermanim-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/.pre-commit-config.yaml` & `powermanim-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/LICENSE` & `powermanim-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/PKG-INFO` & `powermanim-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powermanim
-Version: 0.0.6
+Version: 0.0.7
 Summary: Manim extension with custom components, layouts and slide templates aimed to ease the development of live presentations.
 Home-page: https://github.com/lucmos/powermanim
 Author: Luca Moschella
 Author-email: luca.moschella94@gmail.com
 License: MIT Licence
 Keywords: python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powermanim Version: 0.0.6 Summary: Manim extension
+Metadata-Version: 2.1 Name: powermanim Version: 0.0.7 Summary: Manim extension
 with custom components, layouts and slide templates aimed to ease the
 development of live presentations. Home-page: https://github.com/lucmos/
 powermanim Author: Luca Moschella Author-email: luca.moschella94@gmail.com
 License: MIT Licence Keywords: python Description-Content-Type: text/markdown
 Provides-Extra: docs Provides-Extra: test Provides-Extra: dev License-File:
 LICENSE [![](docs/assets/media/banner.png)](https://lucmos.github.io/
 powermanim)
```

### Comparing `powermanim-0.0.6/README.md` & `powermanim-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/assets/media/banner.png` & `powermanim-0.0.7/docs/assets/media/banner.png`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/assets/media/book.svg` & `powermanim-0.0.7/docs/assets/media/book.svg`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/assets/media/icon.png` & `powermanim-0.0.7/docs/assets/media/icon.png`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/assets/scss/custom.scss` & `powermanim-0.0.7/docs/assets/scss/custom.scss`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/config/_default/config.yaml` & `powermanim-0.0.7/docs/config/_default/config.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/config/_default/languages.yaml` & `powermanim-0.0.7/docs/config/_default/languages.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/config/_default/params.yaml` & `powermanim-0.0.7/docs/config/_default/params.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/content/docs/chapter1/_index.md` & `powermanim-0.0.7/docs/content/docs/chapter1/_index.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/content/docs/chapter1/reading-list.md` & `powermanim-0.0.7/docs/content/docs/chapter1/reading-list.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/content/docs/chapter1/syllabus.md` & `powermanim-0.0.7/docs/content/docs/chapter1/syllabus.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/content/docs/chapter1/takeaways.md` & `powermanim-0.0.7/docs/content/docs/chapter1/takeaways.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/content/docs/chapter2/_index.md` & `powermanim-0.0.7/docs/content/docs/chapter2/_index.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/content/docs/chapter2/reading-list.md` & `powermanim-0.0.7/docs/content/docs/chapter2/reading-list.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/content/docs/chapter2/syllabus.md` & `powermanim-0.0.7/docs/content/docs/chapter2/syllabus.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/content/docs/chapter2/takeaways.md` & `powermanim-0.0.7/docs/content/docs/chapter2/takeaways.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/content/home/animations.md` & `powermanim-0.0.7/docs/content/home/animations.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/docs/layouts/partials/views/masonry.html` & `powermanim-0.0.7/docs/layouts/partials/views/masonry.html`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/pyproject.toml` & `powermanim-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/setup.cfg` & `powermanim-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/components/chartbars.py` & `powermanim-0.0.7/src/powermanim/components/chartbars.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/components/numberslider.py` & `powermanim-0.0.7/src/powermanim/components/numberslider.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/components/powermanim.py` & `powermanim-0.0.7/src/powermanim/components/powermanim.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/components/vgrouphighlight.py` & `powermanim-0.0.7/src/powermanim/components/vgrouphighlight.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,14 @@
             scale_active (float): The scale of the highlighted submobjects.
             scale_about_point (np.ndarray): The point to scale about.
             scale_about_edge (np.ndarray): The edge to scale about.
             **kwargs: Keyword arguments to be passed to the VGroup.
         """
         super().__init__(*args, **kwargs)
 
-        for x in self.submobjects:
-            x.save_state()
-
         self.anim_run_time = anim_run_time
         self.anim_lag_ratio = anim_lag_ratio
         self.active_opacity = active_opacity
         self.scale_active = scale_active
         self.scale_about_point = scale_about_point
         self.scale_about_edge = scale_about_edge
 
@@ -55,22 +52,25 @@
         """
         anims = []
 
         if not isinstance(indices, T.Sequence):
             indices = [indices]
 
         for to_highlight in indices:
-            self.submobjects[to_highlight].target = self.submobjects[to_highlight].saved_state.copy()
-            self.submobjects[to_highlight].target.scale(
+            item = self.submobjects[to_highlight]
+            if not hasattr(item, "saved_state") or item.saved_state is None:
+                item.save_state()
+            item.target = item.saved_state.copy()
+            item.target.scale(
                 self.scale_active,
                 about_point=self.scale_about_point,
                 about_edge=self.scale_about_edge,
             )
-            self.submobjects[to_highlight].target.set_opacity(self.active_opacity)
-            anims.append(MoveToTarget(self.submobjects[to_highlight]))
+            item.target.set_opacity(self.active_opacity)
+            anims.append(MoveToTarget(item))
 
         if self.previously_active_idxs:
             for previously_active_idx in self.previously_active_idxs:
                 if previously_active_idx not in indices:
                     anims.append(
                         self.submobjects[previously_active_idx].animate.restore(),
                     )
```

### Comparing `powermanim-0.0.6/src/powermanim/layouts/arrangedbullets.py` & `powermanim-0.0.7/src/powermanim/layouts/arrangedbullets.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/scripts/build_anims` & `powermanim-0.0.7/src/powermanim/scripts/build_anims`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/showcase/__init__.py` & `powermanim-0.0.7/src/powermanim/showcase/__init__.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/showcase/components/chartbars.py` & `powermanim-0.0.7/src/powermanim/showcase/components/chartbars.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/showcase/components/numberslider.py` & `powermanim-0.0.7/src/powermanim/showcase/components/numberslider.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/showcase/components/vgroupghighlight.py` & `powermanim-0.0.7/src/powermanim/showcase/components/vgroupghighlight.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/showcase/layouts/arrangedbullets.py` & `powermanim-0.0.7/src/powermanim/showcase/layouts/arrangedbullets.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/showcase/showcasescene.py` & `powermanim-0.0.7/src/powermanim/showcase/showcasescene.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/showcase/templates/bulletlist.py` & `powermanim-0.0.7/src/powermanim/showcase/templates/bulletlist.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/templates/bulletlist.py` & `powermanim-0.0.7/src/powermanim/templates/bulletlist.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim/templates/sectiontitle.py` & `powermanim-0.0.7/src/powermanim/templates/sectiontitle.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.6/src/powermanim.egg-info/PKG-INFO` & `powermanim-0.0.7/src/powermanim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powermanim
-Version: 0.0.6
+Version: 0.0.7
 Summary: Manim extension with custom components, layouts and slide templates aimed to ease the development of live presentations.
 Home-page: https://github.com/lucmos/powermanim
 Author: Luca Moschella
 Author-email: luca.moschella94@gmail.com
 License: MIT Licence
 Keywords: python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powermanim Version: 0.0.6 Summary: Manim extension
+Metadata-Version: 2.1 Name: powermanim Version: 0.0.7 Summary: Manim extension
 with custom components, layouts and slide templates aimed to ease the
 development of live presentations. Home-page: https://github.com/lucmos/
 powermanim Author: Luca Moschella Author-email: luca.moschella94@gmail.com
 License: MIT Licence Keywords: python Description-Content-Type: text/markdown
 Provides-Extra: docs Provides-Extra: test Provides-Extra: dev License-File:
 LICENSE [![](docs/assets/media/banner.png)](https://lucmos.github.io/
 powermanim)
```

### Comparing `powermanim-0.0.6/src/powermanim.egg-info/SOURCES.txt` & `powermanim-0.0.7/src/powermanim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

