# Comparing `tmp/cmdix-2.0.1.tar.gz` & `tmp/cmdix-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdix-2.0.1.tar", last modified: Fri Apr 21 20:48:33 2023, max compression
+gzip compressed data, was "cmdix-2.0.2.tar", last modified: Mon Jun 19 21:50:37 2023, max compression
```

## Comparing `cmdix-2.0.1.tar` & `cmdix-2.0.2.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.640558 cmdix-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 20:48:09.000000 cmdix-2.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-21 20:48:09.000000 cmdix-2.0.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-21 20:48:09.000000 cmdix-2.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.612558 cmdix-2.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-21 20:48:09.000000 cmdix-2.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.612558 cmdix-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-21 20:48:09.000000 cmdix-2.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 20:48:09.000000 cmdix-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-21 20:48:09.000000 cmdix-2.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-21 20:48:09.000000 cmdix-2.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-21 20:48:09.000000 cmdix-2.0.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-21 20:48:09.000000 cmdix-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-21 20:48:33.640558 cmdix-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-21 20:48:09.000000 cmdix-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.616558 cmdix-2.0.1/cmdix/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4795 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.632558 cmdix-2.0.1/cmdix/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/basename.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/bunzip2.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/bzip2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/cal.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/chmod.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/chown.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/chroot.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/crond.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/dirname.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/gunzip.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/httpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/id.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/ln.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/md5sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/mkdir.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/mktemp.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/mv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/nl.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/rmdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sendmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sh.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha1sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha224sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha256sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha384sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sha512sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/shred.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/shuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/touch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/uname.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/uptime.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/uuidgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/wc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/wget.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/whoami.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/yes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/command/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-04-21 20:48:09.000000 cmdix-2.0.1/cmdix/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.616558 cmdix-2.0.1/cmdix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 20:48:33.000000 cmdix-2.0.1/cmdix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-21 20:48:09.000000 cmdix-2.0.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.636558 cmdix-2.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-21 20:48:09.000000 cmdix-2.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-21 20:48:09.000000 cmdix-2.0.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-21 20:48:09.000000 cmdix-2.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 20:48:09.000000 cmdix-2.0.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-21 20:48:09.000000 cmdix-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-21 20:48:09.000000 cmdix-2.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-21 20:48:33.640558 cmdix-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:48:33.640558 cmdix-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_md5sum.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_nl.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_onlyunix.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_pycoreutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_pycoreutils_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_tar.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-21 20:48:09.000000 cmdix-2.0.1/tests/test_uuidgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-21 20:48:09.000000 cmdix-2.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.731521 cmdix-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-19 21:50:18.000000 cmdix-2.0.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-19 21:50:18.000000 cmdix-2.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.719521 cmdix-2.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-19 21:50:18.000000 cmdix-2.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.719521 cmdix-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-19 21:50:18.000000 cmdix-2.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-19 21:50:18.000000 cmdix-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 21:50:18.000000 cmdix-2.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-19 21:50:18.000000 cmdix-2.0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-19 21:50:18.000000 cmdix-2.0.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-19 21:50:18.000000 cmdix-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-19 21:50:37.731521 cmdix-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-19 21:50:18.000000 cmdix-2.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.719521 cmdix-2.0.2/cmdix/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4795 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.731521 cmdix-2.0.2/cmdix/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/bunzip2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/bzip2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/chown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/chroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/crond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/dirname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/gunzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/httpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/ln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/rmdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sendmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha1sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha224sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha256sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha384sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sha512sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/shred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/shuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/touch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/uname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/uptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/uuidgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/wc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/wget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/yes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/command/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-19 21:50:18.000000 cmdix-2.0.2/cmdix/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.719521 cmdix-2.0.2/cmdix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 21:50:37.000000 cmdix-2.0.2/cmdix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 21:50:18.000000 cmdix-2.0.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.731521 cmdix-2.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-19 21:50:18.000000 cmdix-2.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-19 21:50:18.000000 cmdix-2.0.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 21:50:18.000000 cmdix-2.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-19 21:50:18.000000 cmdix-2.0.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-19 21:50:18.000000 cmdix-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-19 21:50:18.000000 cmdix-2.0.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-19 21:50:37.731521 cmdix-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:50:37.731521 cmdix-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_onlyunix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_pycoreutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_pycoreutils_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-19 21:50:18.000000 cmdix-2.0.2/tests/test_uuidgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-19 21:50:18.000000 cmdix-2.0.2/tox.ini
```

### Comparing `cmdix-2.0.1/.github/workflows/main.yml` & `cmdix-2.0.2/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
   # to a non-empty value is sufficient. For tox, it must be one of
   # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
@@ -85,16 +88,14 @@
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
@@ -109,14 +110,16 @@
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `cmdix-2.0.1/CHANGES.rst` & `cmdix-2.0.2/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v2.0.2
+======
+
+#13: Fixed destination calculation in ``cp``.
+
 v2.0.1
 ======
 
 Fixed argument reference in ``cp``.
 
 v2.0.0
 ======
```

### Comparing `cmdix-2.0.1/Dockerfile` & `cmdix-2.0.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/LICENSE` & `cmdix-2.0.2/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-Copyright (c) 2009, 2010, 2011 Hans van Leeuwen
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cmdix-2.0.1/PKG-INFO` & `cmdix-2.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdix
-Version: 2.0.1
+Version: 2.0.2
 Summary: Unix commands in Pure Python
 Home-page: https://github.com/jaraco/cmdix
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,20 +23,24 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/cmdix.svg
 
 .. image:: https://github.com/jaraco/cmdix/workflows/tests/badge.svg
    :target: https://github.com/jaraco/cmdix/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 cmdix is a pure Python implementation of various standard UNIX commands,
 like 'ls', 'cp' and 'sleep'. It also contains a shell-like environment which
 will make Unix-users feel right at home on the Windows command-prompt.
```

### Comparing `cmdix-2.0.1/cmdix/__init__.py` & `cmdix-2.0.2/cmdix/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/base64.py` & `cmdix-2.0.2/cmdix/command/base64.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/basename.py` & `cmdix-2.0.2/cmdix/command/basename.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/cal.py` & `cmdix-2.0.2/cmdix/command/cal.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/cat.py` & `cmdix-2.0.2/cmdix/command/cat.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/chmod.py` & `cmdix-2.0.2/cmdix/command/chmod.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/chown.py` & `cmdix-2.0.2/cmdix/command/chown.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/chroot.py` & `cmdix-2.0.2/cmdix/command/chroot.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/cp.py` & `cmdix-2.0.2/cmdix/command/id.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,108 +1,89 @@
 import os
-import os.path
-import shutil
 
+from .. import onlyunix
 from .. import exception
 
+try:
+    import grp
+    import pwd
+except ImportError:
+    pass
 
+
+@onlyunix
 def parseargs(p):
     """
     Add arguments and `func` to `p`.
 
     :param p: ArgumentParser
     :return:  ArgumentParser
     """
+    # TODO: List all groups a user belongs to
     p.set_defaults(func=func)
-    p.description = "Copy SOURCE to DEST, or multiple SOURCE(s) to DIRECTORY."
-    p.add_argument('SOURCE', nargs='+')
-    p.add_argument('DIRECTORY', nargs=1)
+    p.description = (
+        "Print user and group information for the specified "
+        + "USERNAME, or (when USERNAME omitted) for the current "
+        + "user."
+    )
+    p.usage = '%(prog)s [OPTION]... [USERNAME]'
+    p.add_argument('username', nargs='?')
     p.add_argument(
-        "-i",
-        "--interactive",
+        "-a",
         action="store_true",
-        dest="interactive",
-        help="prompt before overwrite",
+        dest="ignoreme",
+        help="ignore, for compatibility with other versions",
     )
     p.add_argument(
-        "-p",
-        "--preserve",
+        "-g",
+        "--group",
         action="store_true",
-        dest="preserve",
-        help="preserve as many attributes as possible",
+        dest="group",
+        help="print only the effective group ID",
     )
     p.add_argument(
-        "-r",
-        "-R",
-        "--recursive",
+        "-n",
+        "--name",
         action="store_true",
-        dest="recursive",
-        help="copy directories recursively",
+        dest="name",
+        help="print a name instead of a number, for -ug",
     )
     p.add_argument(
-        "-v",
-        "--verbose",
+        "-u",
+        "--user",
         action="store_true",
-        dest="verbose",
-        help="print a message for each created directory",
+        dest="user",
+        help="print only the effective group ID",
     )
     return p
 
 
 def func(args):
-    # Set the _copy function
-    if args.preserve:
-        _copy = shutil.copy2
+    if args.username:
+        u = pwd.getpwnam(args.username)
     else:
-        _copy = shutil.copy
+        u = pwd.getpwuid(os.getuid())
 
-    (dest,) = args.DIRECTORY
-    for src in args.SOURCE:
-        handle(_copy, args, dest, src)
+    uid = u.pw_uid
+    gid = u.pw_gid
+    username = u.pw_name
+    g = grp.getgrgid(gid)
+    groupname = g.gr_name
 
+    if args.group and args.name:
+        return groupname
 
-def handle(_copy, args, dstbase, src):
-    if args.recursive:
-        # Create the base destination directory if it does not exists
-        if not os.path.exists(dstbase):
-            os.mkdir(dstbase)
+    if args.group:
+        return gid
 
-        walk(_copy, args, dstbase, src)
-    else:
-        dstfile = dstbase
-        if os.path.isdir(dstbase):
-            dstfile = os.path.join(dstbase, src)
-        _copy(src, dstfile)
-        if args.verbose:
-            print("'{0}' -> '{1}'".format(src, dstfile))
-
-
-def walk(_copy, args, dstbase, src):
-    # Walk the source directory
-    for root, dirnames, filenames in os.walk(src):
-        if root == dstbase:
-            continue
-        dstmid = root.lstrip(src)
-
-        # Create subdirectories in destination directory
-        for subdir in dirnames:
-            dstdir = os.path.join(dstbase, dstmid, subdir)
-            if not os.path.exists(dstbase):
-                os.mkdir(dstdir)
-            if args.verbose:
-                print("'{0}' -> '{1}'".format(root, dstdir))
-
-        # Copy file
-        for filename in filenames:
-            dstfile = os.path.join(dstbase, dstmid, filename)
-            srcfile = os.path.join(root, filename)
-            if args.interactive and os.path.exists(dstfile):
-                q = input(
-                    "{0}: {1} already ".format(args.prog, dstfile)
-                    + "exists; do you wish to overwrite (y or n)?"
-                )
-                if q.upper() != 'Y':
-                    exception.StdOutException("not overwritten", 2)
-                    continue
-            _copy(srcfile, dstfile)
-            if args.verbose:
-                print("'{0}' -> '{1}'".format(srcfile, dstfile))
+    if args.user and args.name:
+        return username
+
+    if args.user:
+        return uid
+
+    if args.name:
+        exception.StdErrException(
+            "id: cannot print only names " + "or real IDs in default format"
+        )
+
+    print("uid={0}({1}) gid={2}({3})".format(uid, username, gid, username))
```

### Comparing `cmdix-2.0.1/cmdix/command/crond.py` & `cmdix-2.0.2/cmdix/command/crond.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/diff.py` & `cmdix-2.0.2/cmdix/command/diff.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/dirname.py` & `cmdix-2.0.2/cmdix/command/dirname.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/env.py` & `cmdix-2.0.2/cmdix/command/env.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/expand.py` & `cmdix-2.0.2/cmdix/command/expand.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/httpd.py` & `cmdix-2.0.2/cmdix/command/httpd.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/id.py` & `cmdix-2.0.2/cmdix/command/rm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,71 @@
 import os
+import os.path
 
-from .. import onlyunix
-from .. import exception
 
-try:
-    import grp
-    import pwd
-except ImportError:
-    pass
-
-
-@onlyunix
 def parseargs(p):
     """
     Add arguments and `func` to `p`.
 
     :param p: ArgumentParser
     :return:  ArgumentParser
     """
-    # TODO: List all groups a user belongs to
     p.set_defaults(func=func)
-    p.description = (
-        "Print user and group information for the specified "
-        + "USERNAME, or (when USERNAME omitted) for the current "
-        + "user."
-    )
-    p.usage = '%(prog)s [OPTION]... [USERNAME]'
-    p.add_argument('username', nargs='?')
+    p.description = "print name of current/working directory"
+    p.add_argument('FILE', nargs='+')
     p.add_argument(
-        "-a",
+        "-f",
+        "--force",
         action="store_true",
-        dest="ignoreme",
-        help="ignore, for compatibility with other versions",
+        dest="force",
+        help="ignore nonexistent files, never prompt",
     )
     p.add_argument(
-        "-g",
-        "--group",
+        "-r",
+        "-R",
+        "--recursive",
         action="store_true",
-        dest="group",
-        help="print only the effective group ID",
+        dest="recursive",
+        help="remove directories and their contents recursively",
     )
     p.add_argument(
-        "-n",
-        "--name",
+        "-v",
+        "--verbose",
         action="store_true",
-        dest="name",
-        help="print a name instead of a number, for -ug",
-    )
-    p.add_argument(
-        "-u",
-        "--user",
-        action="store_true",
-        dest="user",
-        help="print only the effective group ID",
+        dest="verbose",
+        help="explain what is being done",
     )
     return p
 
 
 def func(args):
-    if args.username:
-        u = pwd.getpwnam(args.username)
+    def _raise(err):
+        if not args.force:
+            raise err
+
+    for arg in args.FILE:
+        do_it(_raise, arg, args)
+
+
+def do_it(_raise, arg, args):
+    if args.recursive and os.path.isdir(arg):
+        # Remove directory recursively
+        for root, dirs, files in os.walk(arg, topdown=False, onerror=_raise):
+            for name in files:
+                path = os.path.join(root, name)
+                os.remove(path)
+                if args.verbose:
+                    print("Removed file '{0}'\n".format(path))
+            for name in dirs:
+                path = os.path.join(root, name)
+                os.rmdir(path)
+                if args.verbose:
+                    print("Removed directory '{0}'\n".format(path))
+        os.rmdir(arg)
     else:
-        u = pwd.getpwuid(os.getuid())
-
-    uid = u.pw_uid
-    gid = u.pw_gid
-    username = u.pw_name
-    g = grp.getgrgid(gid)
-    groupname = g.gr_name
-
-    if args.group and args.name:
-        return groupname
-
-    if args.group:
-        return gid
-
-    if args.user and args.name:
-        return username
-
-    if args.user:
-        return uid
-
-    if args.name:
-        exception.StdErrException(
-            "id: cannot print only names " + "or real IDs in default format"
-        )
-
-    print("uid={0}({1}) gid={2}({3})".format(uid, username, gid, username))
+        # Remove single file
+        try:
+            os.remove(arg)
+            if args.verbose:
+                print("Removed '{0}'\n".format(arg))
+        except OSError as err:
+            _raise(err)
```

### Comparing `cmdix-2.0.1/cmdix/command/init.py` & `cmdix-2.0.2/cmdix/command/init.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/kill.py` & `cmdix-2.0.2/cmdix/command/kill.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/ln.py` & `cmdix-2.0.2/cmdix/command/ln.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/logger.py` & `cmdix-2.0.2/cmdix/command/logger.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/login.py` & `cmdix-2.0.2/cmdix/command/login.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/ls.py` & `cmdix-2.0.2/cmdix/command/ls.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/mkdir.py` & `cmdix-2.0.2/cmdix/command/mkdir.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/mktemp.py` & `cmdix-2.0.2/cmdix/command/mktemp.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/more.py` & `cmdix-2.0.2/cmdix/command/more.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/mount.py` & `cmdix-2.0.2/cmdix/command/mount.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/mv.py` & `cmdix-2.0.2/cmdix/command/mv.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/nl.py` & `cmdix-2.0.2/cmdix/command/nl.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/pwd.py` & `cmdix-2.0.2/cmdix/command/pwd.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/rmdir.py` & `cmdix-2.0.2/cmdix/command/rmdir.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/sendmail.py` & `cmdix-2.0.2/cmdix/command/sendmail.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/seq.py` & `cmdix-2.0.2/cmdix/command/seq.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/sh.py` & `cmdix-2.0.2/cmdix/command/sh.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/shred.py` & `cmdix-2.0.2/cmdix/command/shred.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/shuf.py` & `cmdix-2.0.2/cmdix/command/shuf.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/sleep.py` & `cmdix-2.0.2/cmdix/command/sleep.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/sort.py` & `cmdix-2.0.2/cmdix/command/sort.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/tail.py` & `cmdix-2.0.2/cmdix/command/tail.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/tar.py` & `cmdix-2.0.2/cmdix/command/tar.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/tee.py` & `cmdix-2.0.2/cmdix/command/tee.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/touch.py` & `cmdix-2.0.2/cmdix/command/touch.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/uname.py` & `cmdix-2.0.2/cmdix/command/uname.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/uptime.py` & `cmdix-2.0.2/cmdix/command/uptime.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/uuidgen.py` & `cmdix-2.0.2/cmdix/command/uuidgen.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/watch.py` & `cmdix-2.0.2/cmdix/command/watch.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/wc.py` & `cmdix-2.0.2/cmdix/command/wc.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/wget.py` & `cmdix-2.0.2/cmdix/command/wget.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/command/zip.py` & `cmdix-2.0.2/cmdix/command/zip.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/compressor.py` & `cmdix-2.0.2/cmdix/compressor.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/exception.py` & `cmdix-2.0.2/cmdix/exception.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/hasher.py` & `cmdix-2.0.2/cmdix/hasher.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix/lib.py` & `cmdix-2.0.2/cmdix/lib.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/cmdix.egg-info/PKG-INFO` & `cmdix-2.0.2/cmdix.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdix
-Version: 2.0.1
+Version: 2.0.2
 Summary: Unix commands in Pure Python
 Home-page: https://github.com/jaraco/cmdix
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,20 +23,24 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/cmdix.svg
 
 .. image:: https://github.com/jaraco/cmdix/workflows/tests/badge.svg
    :target: https://github.com/jaraco/cmdix/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 cmdix is a pure Python implementation of various standard UNIX commands,
 like 'ls', 'cp' and 'sleep'. It also contains a shell-like environment which
 will make Unix-users feel right at home on the Windows command-prompt.
```

### Comparing `cmdix-2.0.1/cmdix.egg-info/SOURCES.txt` & `cmdix-2.0.2/cmdix.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.rst
 Dockerfile
 LICENSE
 README.rst
 conftest.py
@@ -94,14 +93,15 @@
 docs/history.rst
 docs/index.rst
 tests/__init__.py
 tests/test_base64.py
 tests/test_basename.py
 tests/test_cal.py
 tests/test_cat.py
+tests/test_cp.py
 tests/test_expand.py
 tests/test_login.py
 tests/test_ls.py
 tests/test_md5sum.py
 tests/test_nl.py
 tests/test_onlyunix.py
 tests/test_pycoreutils.py
```

### Comparing `cmdix-2.0.1/cmdix.egg-info/entry_points.txt` & `cmdix-2.0.2/cmdix.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/docs/conf.py` & `cmdix-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/pytest.ini` & `cmdix-2.0.2/pytest.ini`

 * *Files 26% similar despite different names*

```diff
@@ -3,30 +3,25 @@
 addopts=--doctest-modules
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# Suppress deprecation warning in flake8
-	ignore:SelectableGroups dict interface is deprecated::flake8
-
 	# shopkeep/pytest-black#55
 	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
-	# tholo/pytest-flake8#83
-	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
-	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
-
 	# shopkeep/pytest-black#67
 	ignore:'encoding' argument not specified::pytest_black
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
```

### Comparing `cmdix-2.0.1/setup.cfg` & `cmdix-2.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -31,23 +31,21 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
+	pytest-ruff
 	
 	types-backports
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
```

### Comparing `cmdix-2.0.1/tests/__init__.py` & `cmdix-2.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tests/test_base64.py` & `cmdix-2.0.2/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tests/test_cal.py` & `cmdix-2.0.2/tests/test_cal.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tests/test_cat.py` & `cmdix-2.0.2/tests/test_cat.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tests/test_login.py` & `cmdix-2.0.2/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tests/test_ls.py` & `cmdix-2.0.2/tests/test_ls.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tests/test_nl.py` & `cmdix-2.0.2/tests/test_nl.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tests/test_onlyunix.py` & `cmdix-2.0.2/tests/test_onlyunix.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tests/test_tar.py` & `cmdix-2.0.2/tests/test_tar.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tests/test_uuidgen.py` & `cmdix-2.0.2/tests/test_uuidgen.py`

 * *Files identical despite different names*

### Comparing `cmdix-2.0.1/tox.ini` & `cmdix-2.0.2/tox.ini`

 * *Files identical despite different names*

