# Comparing `tmp/maptasker-2.0.4.tar.gz` & `tmp/maptasker-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maptasker-2.0.4.tar", max compression
+gzip compressed data, was "maptasker-2.0.5.tar", max compression
```

## Comparing `maptasker-2.0.4.tar` & `maptasker-2.0.5.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    35149 2023-02-10 17:49:08.224000 maptasker-2.0.4/LICENSE.txt
--rw-r--r--   0        0        0      296 2023-03-16 14:54:53.454155 maptasker-2.0.4/README_PyPl.md
--rw-r--r--   0        0        0     8196 2023-02-27 17:44:14.167143 maptasker-2.0.4/maptasker/.DS_Store
--rw-r--r--   0        0        0        0 2023-02-15 21:09:13.241439 maptasker-2.0.4/maptasker/__init__.py
--rw-r--r--   0        0        0     1298 2023-04-21 18:13:43.143443 maptasker-2.0.4/maptasker/main.py
--rw-r--r--   0        0        0     6148 2023-02-27 16:37:40.000000 maptasker-2.0.4/maptasker/src/.DS_Store
--rw-r--r--   0        0        0        0 2023-03-23 17:42:41.454000 maptasker-2.0.4/maptasker/src/__init__.py
--rw-r--r--   0        0        0      212 2023-03-23 17:49:08.090530 maptasker-2.0.4/maptasker/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3789 2023-06-04 16:15:59.616430 maptasker-2.0.4/maptasker/src/__pycache__/actargs.cpython-310.pyc
--rw-r--r--   0        0        0     7468 2023-06-02 17:30:16.499878 maptasker-2.0.4/maptasker/src/__pycache__/action.cpython-310.pyc
--rw-r--r--   0        0        0   111401 2023-06-18 16:43:42.983166 maptasker-2.0.4/maptasker/src/__pycache__/actionc.cpython-310.pyc
--rw-r--r--   0        0        0     2879 2023-05-24 19:01:58.340245 maptasker-2.0.4/maptasker/src/__pycache__/actiond.cpython-310.pyc
--rw-r--r--   0        0        0     4396 2023-06-09 17:38:50.270086 maptasker-2.0.4/maptasker/src/__pycache__/actione.cpython-310.pyc
--rw-r--r--   0        0        0     3268 2023-06-18 16:43:42.958977 maptasker-2.0.4/maptasker/src/__pycache__/actionr.cpython-310.pyc
--rw-r--r--   0        0        0    14567 2023-06-02 17:40:23.794140 maptasker-2.0.4/maptasker/src/__pycache__/actiont.cpython-310.pyc
--rw-r--r--   0        0        0     1005 2023-03-23 17:42:41.454000 maptasker-2.0.4/maptasker/src/__pycache__/argsdict.cpython-310.pyc
--rw-r--r--   0        0        0     1814 2023-06-12 16:12:30.448906 maptasker-2.0.4/maptasker/src/__pycache__/caveats.cpython-310.pyc
--rw-r--r--   0        0        0     4322 2023-05-23 17:42:23.031484 maptasker-2.0.4/maptasker/src/__pycache__/colors.cpython-310.pyc
--rw-r--r--   0        0        0     1690 2023-05-09 16:40:21.938138 maptasker-2.0.4/maptasker/src/__pycache__/colrmode.cpython-310.pyc
--rw-r--r--   0        0        0     3904 2023-05-24 19:12:58.193988 maptasker-2.0.4/maptasker/src/__pycache__/condition.cpython-310.pyc
--rw-r--r--   0        0        0      344 2023-06-18 16:43:42.871678 maptasker-2.0.4/maptasker/src/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     1096 2023-06-12 18:47:26.743258 maptasker-2.0.4/maptasker/src/__pycache__/debug.cpython-310.pyc
--rw-r--r--   0        0        0      378 2023-06-02 16:37:04.467125 maptasker-2.0.4/maptasker/src/__pycache__/depricated.cpython-310.pyc
--rw-r--r--   0        0        0      756 2023-06-01 15:56:50.708765 maptasker-2.0.4/maptasker/src/__pycache__/error.cpython-310.pyc
--rw-r--r--   0        0        0     1315 2023-05-22 19:21:47.087305 maptasker-2.0.4/maptasker/src/__pycache__/frmthtml.cpython-310.pyc
--rw-r--r--   0        0        0     3154 2023-06-06 19:08:23.936538 maptasker-2.0.4/maptasker/src/__pycache__/getbakup.cpython-310.pyc
--rw-r--r--   0        0        0     1349 2023-06-16 17:25:33.895940 maptasker-2.0.4/maptasker/src/__pycache__/getids.cpython-310.pyc
--rw-r--r--   0        0        0     1927 2023-06-09 16:25:01.577587 maptasker-2.0.4/maptasker/src/__pycache__/getputarg.cpython-310.pyc
--rw-r--r--   0        0        0     1099 2023-06-16 18:00:07.569780 maptasker-2.0.4/maptasker/src/__pycache__/initparg.cpython-310.pyc
--rw-r--r--   0        0        0     1259 2023-05-25 18:58:04.869004 maptasker-2.0.4/maptasker/src/__pycache__/kidapp.cpython-310.pyc
--rw-r--r--   0        0        0     5942 2023-06-07 18:35:45.951818 maptasker-2.0.4/maptasker/src/__pycache__/lineout.cpython-310.pyc
--rw-r--r--   0        0        0     6430 2023-06-18 18:59:49.351979 maptasker-2.0.4/maptasker/src/__pycache__/mapit.cpython-310.pyc
--rw-r--r--   0        0        0     2879 2023-05-25 18:58:04.841682 maptasker-2.0.4/maptasker/src/__pycache__/migrate.cpython-310.pyc
--rw-r--r--   0        0        0     5229 2023-06-18 17:34:29.724102 maptasker-2.0.4/maptasker/src/__pycache__/parsearg.cpython-310.pyc
--rw-r--r--   0        0        0     4813 2023-05-26 17:35:25.585117 maptasker-2.0.4/maptasker/src/__pycache__/prefers.cpython-310.pyc
--rw-r--r--   0        0        0     2298 2023-06-14 18:52:04.201292 maptasker-2.0.4/maptasker/src/__pycache__/proclist.cpython-310.pyc
--rw-r--r--   0        0        0     4962 2023-06-18 14:49:54.659332 maptasker-2.0.4/maptasker/src/__pycache__/profiles.cpython-310.pyc
--rw-r--r--   0        0        0      704 2023-06-12 16:38:06.347136 maptasker-2.0.4/maptasker/src/__pycache__/progargs.cpython-310.pyc
--rw-r--r--   0        0        0     7710 2023-06-18 17:38:58.133027 maptasker-2.0.4/maptasker/src/__pycache__/proginit.cpython-310.pyc
--rw-r--r--   0        0        0     8577 2023-06-18 18:50:10.924294 maptasker-2.0.4/maptasker/src/__pycache__/projects.cpython-310.pyc
--rw-r--r--   0        0        0     4964 2023-06-12 18:39:32.522025 maptasker-2.0.4/maptasker/src/__pycache__/runcli.cpython-310.pyc
--rw-r--r--   0        0        0     1861 2023-06-09 18:08:18.952248 maptasker-2.0.4/maptasker/src/__pycache__/rungui.cpython-310.pyc
--rw-r--r--   0        0        0     5101 2023-06-16 18:00:07.648767 maptasker-2.0.4/maptasker/src/__pycache__/scenes.cpython-310.pyc
--rw-r--r--   0        0        0     8098 2023-03-23 17:49:08.215471 maptasker-2.0.4/maptasker/src/__pycache__/servicec.cpython-310.pyc
--rw-r--r--   0        0        0     2565 2023-06-11 15:40:38.257691 maptasker-2.0.4/maptasker/src/__pycache__/share.cpython-310.pyc
--rw-r--r--   0        0        0      998 2023-03-23 17:49:08.120911 maptasker-2.0.4/maptasker/src/__pycache__/shellsort.cpython-310.pyc
--rw-r--r--   0        0        0     2601 2023-06-13 16:29:20.876846 maptasker-2.0.4/maptasker/src/__pycache__/sysconst.cpython-310.pyc
--rw-r--r--   0        0        0     2329 2023-05-23 17:42:23.066794 maptasker-2.0.4/maptasker/src/__pycache__/taskactn.cpython-310.pyc
--rw-r--r--   0        0        0     2091 2023-06-16 17:25:33.824919 maptasker-2.0.4/maptasker/src/__pycache__/taskerd.cpython-310.pyc
--rw-r--r--   0        0        0     1699 2023-05-23 19:26:14.226538 maptasker-2.0.4/maptasker/src/__pycache__/taskflag.cpython-310.pyc
--rw-r--r--   0        0        0     7928 2023-06-16 19:23:46.264837 maptasker-2.0.4/maptasker/src/__pycache__/tasks.cpython-310.pyc
--rw-r--r--   0        0        0     5594 2023-06-16 18:35:42.813632 maptasker-2.0.4/maptasker/src/__pycache__/taskuniq.cpython-310.pyc
--rw-r--r--   0        0        0      579 2023-06-12 15:13:02.654321 maptasker-2.0.4/maptasker/src/__pycache__/twisty.cpython-310.pyc
--rw-r--r--   0        0        0    18308 2023-06-13 19:27:36.255495 maptasker-2.0.4/maptasker/src/__pycache__/userintr.cpython-310.pyc
--rw-r--r--   0        0        0     2674 2023-06-05 17:48:06.086421 maptasker-2.0.4/maptasker/src/__pycache__/xmldata.cpython-310.pyc
--rw-r--r--   0        0        0     7414 2023-06-04 16:15:59.477019 maptasker-2.0.4/maptasker/src/actargs.py
--rw-r--r--   0        0        0    18949 2023-06-02 16:53:30.423052 maptasker-2.0.4/maptasker/src/action.py
--rw-r--r--   0        0        0   154233 2023-06-18 15:37:16.462602 maptasker-2.0.4/maptasker/src/actionc.py
--rw-r--r--   0        0        0     7036 2023-05-24 19:01:58.258828 maptasker-2.0.4/maptasker/src/actiond.py
--rw-r--r--   0        0        0    10560 2023-06-09 17:35:02.599552 maptasker-2.0.4/maptasker/src/actione.py
--rw-r--r--   0        0        0     8224 2023-06-18 15:36:44.590639 maptasker-2.0.4/maptasker/src/actionr.py
--rw-r--r--   0        0        0    17569 2023-06-02 17:39:56.913511 maptasker-2.0.4/maptasker/src/actiont.py
--rw-r--r--   0        0        0     3488 2023-06-12 16:06:29.576743 maptasker-2.0.4/maptasker/src/caveats.py
--rw-r--r--   0        0        0     8244 2023-05-23 17:29:37.974990 maptasker-2.0.4/maptasker/src/colors.py
--rw-r--r--   0        0        0     3242 2023-05-09 16:40:21.806291 maptasker-2.0.4/maptasker/src/colrmode.py
--rw-r--r--   0        0        0     9332 2023-05-24 19:04:05.075671 maptasker-2.0.4/maptasker/src/condition.py
--rw-r--r--   0        0        0     3372 2023-06-18 15:51:17.049620 maptasker-2.0.4/maptasker/src/config.py
--rw-r--r--   0        0        0     2643 2023-06-12 18:45:06.646868 maptasker-2.0.4/maptasker/src/debug.py
--rw-r--r--   0        0        0      417 2023-05-31 19:09:27.920155 maptasker-2.0.4/maptasker/src/depricated.py
--rw-r--r--   0        0        0     1671 2023-06-01 15:32:00.745212 maptasker-2.0.4/maptasker/src/error.py
--rw-r--r--   0        0        0     2221 2023-05-22 19:21:46.589160 maptasker-2.0.4/maptasker/src/frmthtml.py
--rw-r--r--   0        0        0     5145 2023-06-06 19:08:23.863491 maptasker-2.0.4/maptasker/src/getbakup.py
--rw-r--r--   0        0        0     2532 2023-06-16 17:19:30.793740 maptasker-2.0.4/maptasker/src/getids.py
--rw-r--r--   0        0        0     3819 2023-06-09 16:19:09.335881 maptasker-2.0.4/maptasker/src/getputarg.py
--rw-r--r--   0        0        0     3413 2023-06-16 17:58:14.740698 maptasker-2.0.4/maptasker/src/initparg.py
--rw-r--r--   0        0        0     2435 2023-05-25 18:00:06.894522 maptasker-2.0.4/maptasker/src/kidapp.py
--rw-r--r--   0        0        0    11973 2023-06-07 18:33:07.116619 maptasker-2.0.4/maptasker/src/lineout.py
--rw-r--r--   0        0        0    18170 2023-06-18 18:59:49.282569 maptasker-2.0.4/maptasker/src/mapit.py
--rw-r--r--   0        0        0     5145 2023-05-25 18:00:06.900647 maptasker-2.0.4/maptasker/src/migrate.py
--rw-r--r--   0        0        0     9266 2023-06-18 17:06:55.237399 maptasker-2.0.4/maptasker/src/parsearg.py
--rw-r--r--   0        0        0     9205 2023-05-26 17:34:12.026105 maptasker-2.0.4/maptasker/src/prefers.py
--rw-r--r--   0        0        0     5580 2023-06-14 18:52:04.000202 maptasker-2.0.4/maptasker/src/proclist.py
--rw-r--r--   0        0        0    11551 2023-06-16 19:27:33.527686 maptasker-2.0.4/maptasker/src/profiles.py
--rw-r--r--   0        0        0     1985 2023-06-12 16:37:07.347333 maptasker-2.0.4/maptasker/src/progargs.py
--rw-r--r--   0        0        0    14103 2023-06-18 17:38:58.060239 maptasker-2.0.4/maptasker/src/proginit.py
--rw-r--r--   0        0        0    18468 2023-06-18 18:50:10.766540 maptasker-2.0.4/maptasker/src/projects.py
--rw-r--r--   0        0        0    11239 2023-06-12 18:39:32.427057 maptasker-2.0.4/maptasker/src/runcli.py
--rw-r--r--   0        0        0     4530 2023-06-09 18:08:18.889299 maptasker-2.0.4/maptasker/src/rungui.py
--rw-r--r--   0        0        0     9629 2023-06-16 18:00:07.508159 maptasker-2.0.4/maptasker/src/scenes.py
--rw-r--r--   0        0        0    14219 2023-03-23 17:42:41.454000 maptasker-2.0.4/maptasker/src/servicec.py
--rw-r--r--   0        0        0     5496 2023-06-11 15:40:38.119559 maptasker-2.0.4/maptasker/src/share.py
--rw-r--r--   0        0        0     3354 2023-03-23 17:42:41.454000 maptasker-2.0.4/maptasker/src/shellsort.py
--rw-r--r--   0        0        0     4396 2023-06-13 16:28:51.163469 maptasker-2.0.4/maptasker/src/sysconst.py
--rw-r--r--   0        0        0     5837 2023-05-23 17:29:37.959325 maptasker-2.0.4/maptasker/src/taskactn.py
--rw-r--r--   0        0        0     4066 2023-06-16 17:14:13.317736 maptasker-2.0.4/maptasker/src/taskerd.py
--rw-r--r--   0        0        0     2673 2023-05-23 19:05:18.026922 maptasker-2.0.4/maptasker/src/taskflag.py
--rw-r--r--   0        0        0    15856 2023-06-16 19:23:46.121563 maptasker-2.0.4/maptasker/src/tasks.py
--rw-r--r--   0        0        0    12325 2023-06-16 18:35:42.669791 maptasker-2.0.4/maptasker/src/taskuniq.py
--rw-r--r--   0        0        0     1544 2023-06-12 15:13:02.513986 maptasker-2.0.4/maptasker/src/twisty.py
--rw-r--r--   0        0        0    40418 2023-06-13 16:34:54.062732 maptasker-2.0.4/maptasker/src/userintr.py
--rw-r--r--   0        0        0     7081 2023-06-05 17:44:34.728274 maptasker-2.0.4/maptasker/src/xmldata.py
--rw-r--r--   0        0        0     1247 2023-06-13 16:26:19.331401 maptasker-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 maptasker-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-10 17:49:08.224000 maptasker-2.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      296 2023-03-16 14:54:53.454155 maptasker-2.0.5/README_PyPl.md
+-rw-r--r--   0        0        0     8196 2023-02-27 17:44:14.167143 maptasker-2.0.5/maptasker/.DS_Store
+-rw-r--r--   0        0        0        0 2023-02-15 21:09:13.241439 maptasker-2.0.5/maptasker/__init__.py
+-rw-r--r--   0        0        0     1298 2023-04-21 18:13:43.143443 maptasker-2.0.5/maptasker/main.py
+-rw-r--r--   0        0        0     6148 2023-02-27 16:37:40.000000 maptasker-2.0.5/maptasker/src/.DS_Store
+-rw-r--r--   0        0        0        0 2023-03-23 17:42:41.454000 maptasker-2.0.5/maptasker/src/__init__.py
+-rw-r--r--   0        0        0      212 2023-03-23 17:49:08.090530 maptasker-2.0.5/maptasker/src/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3789 2023-06-04 16:15:59.616430 maptasker-2.0.5/maptasker/src/__pycache__/actargs.cpython-310.pyc
+-rw-r--r--   0        0        0     7468 2023-06-02 17:30:16.499878 maptasker-2.0.5/maptasker/src/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0   111401 2023-06-18 16:43:42.983166 maptasker-2.0.5/maptasker/src/__pycache__/actionc.cpython-310.pyc
+-rw-r--r--   0        0        0     2879 2023-05-24 19:01:58.340245 maptasker-2.0.5/maptasker/src/__pycache__/actiond.cpython-310.pyc
+-rw-r--r--   0        0        0     4396 2023-06-09 17:38:50.270086 maptasker-2.0.5/maptasker/src/__pycache__/actione.cpython-310.pyc
+-rw-r--r--   0        0        0     3268 2023-06-18 16:43:42.958977 maptasker-2.0.5/maptasker/src/__pycache__/actionr.cpython-310.pyc
+-rw-r--r--   0        0        0    14567 2023-06-02 17:40:23.794140 maptasker-2.0.5/maptasker/src/__pycache__/actiont.cpython-310.pyc
+-rw-r--r--   0        0        0     1005 2023-03-23 17:42:41.454000 maptasker-2.0.5/maptasker/src/__pycache__/argsdict.cpython-310.pyc
+-rw-r--r--   0        0        0     1814 2023-06-12 16:12:30.448906 maptasker-2.0.5/maptasker/src/__pycache__/caveats.cpython-310.pyc
+-rw-r--r--   0        0        0     4322 2023-05-23 17:42:23.031484 maptasker-2.0.5/maptasker/src/__pycache__/colors.cpython-310.pyc
+-rw-r--r--   0        0        0     1690 2023-05-09 16:40:21.938138 maptasker-2.0.5/maptasker/src/__pycache__/colrmode.cpython-310.pyc
+-rw-r--r--   0        0        0     3904 2023-05-24 19:12:58.193988 maptasker-2.0.5/maptasker/src/__pycache__/condition.cpython-310.pyc
+-rw-r--r--   0        0        0      343 2023-06-19 18:04:51.745808 maptasker-2.0.5/maptasker/src/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     1096 2023-06-12 18:47:26.743258 maptasker-2.0.5/maptasker/src/__pycache__/debug.cpython-310.pyc
+-rw-r--r--   0        0        0      378 2023-06-02 16:37:04.467125 maptasker-2.0.5/maptasker/src/__pycache__/depricated.cpython-310.pyc
+-rw-r--r--   0        0        0      756 2023-06-01 15:56:50.708765 maptasker-2.0.5/maptasker/src/__pycache__/error.cpython-310.pyc
+-rw-r--r--   0        0        0     1315 2023-05-22 19:21:47.087305 maptasker-2.0.5/maptasker/src/__pycache__/frmthtml.cpython-310.pyc
+-rw-r--r--   0        0        0     3154 2023-06-06 19:08:23.936538 maptasker-2.0.5/maptasker/src/__pycache__/getbakup.cpython-310.pyc
+-rw-r--r--   0        0        0     1349 2023-06-16 17:25:33.895940 maptasker-2.0.5/maptasker/src/__pycache__/getids.cpython-310.pyc
+-rw-r--r--   0        0        0     1927 2023-06-09 16:25:01.577587 maptasker-2.0.5/maptasker/src/__pycache__/getputarg.cpython-310.pyc
+-rw-r--r--   0        0        0     1099 2023-06-16 18:00:07.569780 maptasker-2.0.5/maptasker/src/__pycache__/initparg.cpython-310.pyc
+-rw-r--r--   0        0        0     1259 2023-05-25 18:58:04.869004 maptasker-2.0.5/maptasker/src/__pycache__/kidapp.cpython-310.pyc
+-rw-r--r--   0        0        0     5942 2023-06-07 18:35:45.951818 maptasker-2.0.5/maptasker/src/__pycache__/lineout.cpython-310.pyc
+-rw-r--r--   0        0        0     6430 2023-06-18 18:59:49.351979 maptasker-2.0.5/maptasker/src/__pycache__/mapit.cpython-310.pyc
+-rw-r--r--   0        0        0     2879 2023-05-25 18:58:04.841682 maptasker-2.0.5/maptasker/src/__pycache__/migrate.cpython-310.pyc
+-rw-r--r--   0        0        0     5229 2023-06-18 17:34:29.724102 maptasker-2.0.5/maptasker/src/__pycache__/parsearg.cpython-310.pyc
+-rw-r--r--   0        0        0     4813 2023-05-26 17:35:25.585117 maptasker-2.0.5/maptasker/src/__pycache__/prefers.cpython-310.pyc
+-rw-r--r--   0        0        0     2298 2023-06-14 18:52:04.201292 maptasker-2.0.5/maptasker/src/__pycache__/proclist.cpython-310.pyc
+-rw-r--r--   0        0        0     4962 2023-06-18 14:49:54.659332 maptasker-2.0.5/maptasker/src/__pycache__/profiles.cpython-310.pyc
+-rw-r--r--   0        0        0      704 2023-06-12 16:38:06.347136 maptasker-2.0.5/maptasker/src/__pycache__/progargs.cpython-310.pyc
+-rw-r--r--   0        0        0     7710 2023-06-18 17:38:58.133027 maptasker-2.0.5/maptasker/src/__pycache__/proginit.cpython-310.pyc
+-rw-r--r--   0        0        0     8577 2023-06-18 18:50:10.924294 maptasker-2.0.5/maptasker/src/__pycache__/projects.cpython-310.pyc
+-rw-r--r--   0        0        0     4964 2023-06-12 18:39:32.522025 maptasker-2.0.5/maptasker/src/__pycache__/runcli.cpython-310.pyc
+-rw-r--r--   0        0        0     1908 2023-06-19 17:25:35.194237 maptasker-2.0.5/maptasker/src/__pycache__/rungui.cpython-310.pyc
+-rw-r--r--   0        0        0     5101 2023-06-16 18:00:07.648767 maptasker-2.0.5/maptasker/src/__pycache__/scenes.cpython-310.pyc
+-rw-r--r--   0        0        0     8098 2023-03-23 17:49:08.215471 maptasker-2.0.5/maptasker/src/__pycache__/servicec.cpython-310.pyc
+-rw-r--r--   0        0        0     2565 2023-06-11 15:40:38.257691 maptasker-2.0.5/maptasker/src/__pycache__/share.cpython-310.pyc
+-rw-r--r--   0        0        0      998 2023-03-23 17:49:08.120911 maptasker-2.0.5/maptasker/src/__pycache__/shellsort.cpython-310.pyc
+-rw-r--r--   0        0        0     2601 2023-06-19 15:57:38.279724 maptasker-2.0.5/maptasker/src/__pycache__/sysconst.cpython-310.pyc
+-rw-r--r--   0        0        0     2329 2023-05-23 17:42:23.066794 maptasker-2.0.5/maptasker/src/__pycache__/taskactn.cpython-310.pyc
+-rw-r--r--   0        0        0     2091 2023-06-16 17:25:33.824919 maptasker-2.0.5/maptasker/src/__pycache__/taskerd.cpython-310.pyc
+-rw-r--r--   0        0        0     1699 2023-05-23 19:26:14.226538 maptasker-2.0.5/maptasker/src/__pycache__/taskflag.cpython-310.pyc
+-rw-r--r--   0        0        0     7928 2023-06-16 19:23:46.264837 maptasker-2.0.5/maptasker/src/__pycache__/tasks.cpython-310.pyc
+-rw-r--r--   0        0        0     5594 2023-06-16 18:35:42.813632 maptasker-2.0.5/maptasker/src/__pycache__/taskuniq.cpython-310.pyc
+-rw-r--r--   0        0        0      579 2023-06-12 15:13:02.654321 maptasker-2.0.5/maptasker/src/__pycache__/twisty.cpython-310.pyc
+-rw-r--r--   0        0        0    18411 2023-06-19 17:17:28.999546 maptasker-2.0.5/maptasker/src/__pycache__/userintr.cpython-310.pyc
+-rw-r--r--   0        0        0     2674 2023-06-05 17:48:06.086421 maptasker-2.0.5/maptasker/src/__pycache__/xmldata.cpython-310.pyc
+-rw-r--r--   0        0        0     7414 2023-06-04 16:15:59.477019 maptasker-2.0.5/maptasker/src/actargs.py
+-rw-r--r--   0        0        0    18949 2023-06-02 16:53:30.423052 maptasker-2.0.5/maptasker/src/action.py
+-rw-r--r--   0        0        0   154233 2023-06-18 15:37:16.462602 maptasker-2.0.5/maptasker/src/actionc.py
+-rw-r--r--   0        0        0     7036 2023-05-24 19:01:58.258828 maptasker-2.0.5/maptasker/src/actiond.py
+-rw-r--r--   0        0        0    10560 2023-06-09 17:35:02.599552 maptasker-2.0.5/maptasker/src/actione.py
+-rw-r--r--   0        0        0     8224 2023-06-18 15:36:44.590639 maptasker-2.0.5/maptasker/src/actionr.py
+-rw-r--r--   0        0        0    17569 2023-06-02 17:39:56.913511 maptasker-2.0.5/maptasker/src/actiont.py
+-rw-r--r--   0        0        0     3488 2023-06-12 16:06:29.576743 maptasker-2.0.5/maptasker/src/caveats.py
+-rw-r--r--   0        0        0     8244 2023-05-23 17:29:37.974990 maptasker-2.0.5/maptasker/src/colors.py
+-rw-r--r--   0        0        0     3242 2023-05-09 16:40:21.806291 maptasker-2.0.5/maptasker/src/colrmode.py
+-rw-r--r--   0        0        0     9332 2023-05-24 19:04:05.075671 maptasker-2.0.5/maptasker/src/condition.py
+-rw-r--r--   0        0        0     3372 2023-06-19 18:05:45.645749 maptasker-2.0.5/maptasker/src/config.py
+-rw-r--r--   0        0        0     2643 2023-06-12 18:45:06.646868 maptasker-2.0.5/maptasker/src/debug.py
+-rw-r--r--   0        0        0      417 2023-05-31 19:09:27.920155 maptasker-2.0.5/maptasker/src/depricated.py
+-rw-r--r--   0        0        0     1671 2023-06-01 15:32:00.745212 maptasker-2.0.5/maptasker/src/error.py
+-rw-r--r--   0        0        0     2221 2023-05-22 19:21:46.589160 maptasker-2.0.5/maptasker/src/frmthtml.py
+-rw-r--r--   0        0        0     5145 2023-06-06 19:08:23.863491 maptasker-2.0.5/maptasker/src/getbakup.py
+-rw-r--r--   0        0        0     2532 2023-06-16 17:19:30.793740 maptasker-2.0.5/maptasker/src/getids.py
+-rw-r--r--   0        0        0     3819 2023-06-09 16:19:09.335881 maptasker-2.0.5/maptasker/src/getputarg.py
+-rw-r--r--   0        0        0     3413 2023-06-16 17:58:14.740698 maptasker-2.0.5/maptasker/src/initparg.py
+-rw-r--r--   0        0        0     2435 2023-05-25 18:00:06.894522 maptasker-2.0.5/maptasker/src/kidapp.py
+-rw-r--r--   0        0        0    11973 2023-06-07 18:33:07.116619 maptasker-2.0.5/maptasker/src/lineout.py
+-rw-r--r--   0        0        0    18170 2023-06-18 18:59:49.282569 maptasker-2.0.5/maptasker/src/mapit.py
+-rw-r--r--   0        0        0     5145 2023-05-25 18:00:06.900647 maptasker-2.0.5/maptasker/src/migrate.py
+-rw-r--r--   0        0        0     9266 2023-06-18 17:06:55.237399 maptasker-2.0.5/maptasker/src/parsearg.py
+-rw-r--r--   0        0        0     9205 2023-05-26 17:34:12.026105 maptasker-2.0.5/maptasker/src/prefers.py
+-rw-r--r--   0        0        0     5580 2023-06-14 18:52:04.000202 maptasker-2.0.5/maptasker/src/proclist.py
+-rw-r--r--   0        0        0    11551 2023-06-16 19:27:33.527686 maptasker-2.0.5/maptasker/src/profiles.py
+-rw-r--r--   0        0        0     1985 2023-06-12 16:37:07.347333 maptasker-2.0.5/maptasker/src/progargs.py
+-rw-r--r--   0        0        0    14103 2023-06-18 17:38:58.060239 maptasker-2.0.5/maptasker/src/proginit.py
+-rw-r--r--   0        0        0    18468 2023-06-18 18:50:10.766540 maptasker-2.0.5/maptasker/src/projects.py
+-rw-r--r--   0        0        0    11239 2023-06-12 18:39:32.427057 maptasker-2.0.5/maptasker/src/runcli.py
+-rw-r--r--   0        0        0     4657 2023-06-19 17:25:35.128929 maptasker-2.0.5/maptasker/src/rungui.py
+-rw-r--r--   0        0        0     9629 2023-06-16 18:00:07.508159 maptasker-2.0.5/maptasker/src/scenes.py
+-rw-r--r--   0        0        0    14219 2023-03-23 17:42:41.454000 maptasker-2.0.5/maptasker/src/servicec.py
+-rw-r--r--   0        0        0     5496 2023-06-11 15:40:38.119559 maptasker-2.0.5/maptasker/src/share.py
+-rw-r--r--   0        0        0     3354 2023-03-23 17:42:41.454000 maptasker-2.0.5/maptasker/src/shellsort.py
+-rw-r--r--   0        0        0     4396 2023-06-19 15:56:41.084615 maptasker-2.0.5/maptasker/src/sysconst.py
+-rw-r--r--   0        0        0     5837 2023-05-23 17:29:37.959325 maptasker-2.0.5/maptasker/src/taskactn.py
+-rw-r--r--   0        0        0     4066 2023-06-16 17:14:13.317736 maptasker-2.0.5/maptasker/src/taskerd.py
+-rw-r--r--   0        0        0     2673 2023-05-23 19:05:18.026922 maptasker-2.0.5/maptasker/src/taskflag.py
+-rw-r--r--   0        0        0    15856 2023-06-16 19:23:46.121563 maptasker-2.0.5/maptasker/src/tasks.py
+-rw-r--r--   0        0        0    12325 2023-06-16 18:35:42.669791 maptasker-2.0.5/maptasker/src/taskuniq.py
+-rw-r--r--   0        0        0     1544 2023-06-12 15:13:02.513986 maptasker-2.0.5/maptasker/src/twisty.py
+-rw-r--r--   0        0        0    40771 2023-06-19 17:17:21.125734 maptasker-2.0.5/maptasker/src/userintr.py
+-rw-r--r--   0        0        0     7081 2023-06-05 17:44:34.728274 maptasker-2.0.5/maptasker/src/xmldata.py
+-rw-r--r--   0        0        0     1247 2023-06-19 15:56:41.089646 maptasker-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 maptasker-2.0.5/PKG-INFO
```

### Comparing `maptasker-2.0.4/LICENSE.txt` & `maptasker-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/.DS_Store` & `maptasker-2.0.5/maptasker/.DS_Store`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/main.py` & `maptasker-2.0.5/maptasker/main.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/.DS_Store` & `maptasker-2.0.5/maptasker/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/actargs.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/actargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/action.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/action.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/actionc.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/actionc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/actiond.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/actiond.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/actione.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/actione.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/actionr.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/actionr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/actiont.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/actiont.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/argsdict.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/argsdict.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/caveats.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/caveats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/colors.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/colors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/colrmode.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/colrmode.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/condition.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/condition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/debug.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/debug.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/error.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/error.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/frmthtml.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/frmthtml.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/getbakup.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/getbakup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/getids.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/getids.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/getputarg.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/getputarg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/initparg.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/initparg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/kidapp.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/kidapp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/lineout.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/lineout.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/mapit.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/mapit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/migrate.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/migrate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/parsearg.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/parsearg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/prefers.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/prefers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/proclist.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/proclist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/profiles.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/profiles.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/progargs.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/progargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/proginit.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/proginit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/projects.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/projects.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/runcli.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/runcli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/rungui.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/rungui.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 18:08:18 2023 UTC, .py size: 4530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 926a 8364 b211 0000  o........j.d....
+00000000: 6f0d 0d0a 0000 0000 8f8f 9064 3112 0000  o..........d1...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 8400 5a08 6407 6509 6408 650a 650b  d...Z.d.e.d.e.e.
 00000070: 650b 6602 1900 6604 6409 640a 8404 5a0c  e.f...f.d.d...Z.
@@ -26,92 +26,95 @@
 00000190: 2f4d 7920 4472 6976 652f 5079 7468 6f6e  /My Drive/Python
 000001a0: 2f6d 6170 7461 736b 6572 2f6d 6170 7461  /maptasker/mapta
 000001b0: 736b 6572 2f73 7263 2f72 756e 6775 692e  sker/src/rungui.
 000001c0: 7079 da0a 6465 6c65 7465 5f67 7569 1a00  py..delete_gui..
 000001d0: 0000 7308 0000 000a 020a 0202 0106 0172  ..s............r
 000001e0: 0c00 0000 da07 7573 655f 6775 69da 0672  ......use_gui..r
 000001f0: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
-00000200: 0000 0700 0000 0800 0000 4300 0000 7336  ..........C...s6
+00000200: 0000 0700 0000 0800 0000 4300 0000 7348  ..........C...sH
 00000210: 0100 007c 0172 0864 0164 026c 006d 0161  ...|.r.d.d.l.m.a
 00000220: 0101 0074 0183 007d 027c 02a0 02a1 0001  ...t...}.|......
 00000230: 007c 026a 0372 1774 0464 0364 0183 0201  .|.j.r.t.d.d....
 00000240: 007c 026a 0573 227c 026a 0673 2274 0464  .|.j.s"|.j.s"t.d
 00000250: 0464 0583 0201 0074 0783 007c 0064 063c  .d.....t...|.d.<
 00000260: 007a 0b74 087c 026a 0983 017c 0064 0619  .z.t.|.j...|.d..
 00000270: 0064 073c 0057 006e 0f04 0074 0a79 4101  .d.<.W.n...t.yA.
 00000280: 0001 0001 0064 087c 0064 0619 0064 073c  .....d.|.d...d.<
-00000290: 0059 006e 0177 0074 0b44 005d 207d 037c  .Y.n.w.t.D.] }.|
-000002a0: 0364 096b 0272 5b74 0c7c 027c 0383 0204  .d.k.r[t.|.|....
-000002b0: 007d 0472 5a64 0a7c 049b 009d 027c 0064  .}.rZd.|.....|.d
-000002c0: 0619 007c 033c 0071 4474 0c7c 027c 0383  ...|.<.qDt.|.|..
-000002d0: 027c 0064 0619 007c 033c 0071 4474 0d7c  .|.d...|.<.qDt.|
-000002e0: 0064 0619 0064 0719 0074 0e83 0272 7a74  .d...d...t...rzt
-000002f0: 087c 0064 0619 0064 0719 0083 017c 0064  .|.d...d.....|.d
-00000300: 0619 0064 073c 0074 0f7c 026a 1083 017d  ...d.<.t.|.j...}
-00000310: 057c 026a 1172 907c 026a 11a0 12a1 0044  .|.j.r.|.j.....D
-00000320: 005d 085c 027d 067d 037c 037c 057c 063c  .].\.}.}.|.|.|.<
-00000330: 0071 8774 1374 017c 0283 0201 007c 0064  .q.t.t.|.....|.d
-00000340: 0619 007c 0566 0253 0029 0b61 3b01 0000  ...|.f.S.).a;...
-00000350: 0a20 2020 2050 7265 7365 6e74 2074 6865  .    Present the
-00000360: 2047 5549 2061 6e64 2067 6574 2074 6865   GUI and get the
-00000370: 2072 756e 7469 6d65 2064 6574 6169 6c73   runtime details
-00000380: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000390: 7072 696d 6172 795f 6974 656d 733a 2064  primary_items: d
-000003a0: 6963 7469 6f6e 6172 7920 6f66 2074 6865  ictionary of the
-000003b0: 2070 7269 6d61 7279 2069 7465 6d73 2075   primary items u
-000003c0: 7365 6420 7468 726f 7567 686f 7574 2074  sed throughout t
-000003d0: 6865 206d 6f64 756c 652e 2020 5365 6520  he module.  See 
-000003e0: 6d61 7069 742e 7079 2066 6f72 2064 6574  mapit.py for det
-000003f0: 6169 6c73 0a20 2020 2020 2020 203a 7061  ails.        :pa
-00000400: 7261 6d20 7573 655f 6775 693a 2066 6c61  ram use_gui: fla
-00000410: 6720 6966 2075 7369 6a6e 6720 7468 6520  g if usijng the 
-00000420: 4755 492c 206d 616b 6520 7375 7265 2077  GUI, make sure w
-00000430: 6520 696d 706f 7274 2069 740a 2020 2020  e import it.    
-00000440: 2020 2020 3a72 6574 7572 6e3a 2070 726f      :return: pro
-00000450: 6772 616d 2072 756e 7469 6d65 2061 7267  gram runtime arg
-00000460: 756d 656e 7473 2061 6e64 2063 6f6c 6f72  uments and color
-00000470: 7320 746f 2075 7365 2069 6e20 7468 6520  s to use in the 
-00000480: 6f75 7470 7574 0a20 2020 2072 0100 0000  output.    r....
-00000490: 2901 7208 0000 007a 1850 726f 6772 616d  ).r....z.Program
-000004a0: 2065 7869 7465 642e 2047 6f6f 6462 7965   exited. Goodbye
-000004b0: 2e7a 2650 726f 6772 616d 2063 616e 6365  .z&Program cance
-000004c0: 6c6c 6564 2062 6520 7573 6572 2028 6b69  lled be user (ki
-000004d0: 6c6c 6564 2047 5549 29e9 6300 0000 da11  lled GUI).c.....
-000004e0: 7072 6f67 7261 6d5f 6172 6775 6d65 6e74  program_argument
-000004f0: 73da 1464 6973 706c 6179 5f64 6574 6169  s..display_detai
-00000500: 6c5f 6c65 7665 6ce9 0300 0000 da10 6261  l_level.......ba
-00000510: 636b 7570 5f66 696c 655f 6874 7470 7a07  ckup_file_httpz.
-00000520: 6874 7470 3a2f 2f29 145a 166d 6170 7461  http://).Z.mapta
-00000530: 736b 6572 2e73 7263 2e75 7365 7269 6e74  sker.src.userint
-00000540: 7272 0800 0000 da08 6d61 696e 6c6f 6f70  rr......mainloop
-00000550: da04 6578 6974 7204 0000 005a 0a67 6f5f  ..exitr....Z.go_
-00000560: 7072 6f67 7261 6dda 0572 6572 756e 7202  program..rerunr.
-00000570: 0000 00da 0369 6e74 7211 0000 00da 0954  .....intr......T
-00000580: 7970 6545 7272 6f72 7205 0000 00da 0767  ypeErrorr......g
-00000590: 6574 6174 7472 da0a 6973 696e 7374 616e  etattr..isinstan
-000005a0: 6365 da03 7374 7272 0300 0000 5a0f 6170  ce..strr....Z.ap
-000005b0: 7065 6172 616e 6365 5f6d 6f64 655a 0c63  pearance_modeZ.c
-000005c0: 6f6c 6f72 5f6c 6f6f 6b75 70da 0569 7465  olor_lookup..ite
-000005d0: 6d73 720c 0000 0029 07da 0d70 7269 6d61  msr....)...prima
-000005e0: 7279 5f69 7465 6d73 720d 0000 0072 0900  ry_itemsr....r..
-000005f0: 0000 da05 7661 6c75 655a 0968 7474 705f  ....valueZ.http_
-00000600: 696e 666f da08 636f 6c6f 726d 6170 da03  info..colormap..
-00000610: 6b65 7972 0a00 0000 720a 0000 0072 0b00  keyr....r....r..
-00000620: 0000 da0b 7072 6f63 6573 735f 6775 6926  ....process_gui&
-00000630: 0000 0073 4400 0000 0409 0c01 0603 0801  ...sD...........
-00000640: 0603 0a01 0c03 0a01 0a03 0203 0201 0401  ................
-00000650: 10ff 0c03 1001 02ff 0804 0801 0e01 1201  ................
-00000660: 0280 1402 1202 0201 0a01 0cff 0a05 0603  ................
-00000670: 1201 0a01 0a03 0603 0201 04fe 7221 0000  ............r!..
-00000680: 004e 290d da16 6d61 7074 6173 6b65 722e  .N)...maptasker.
-00000690: 7372 632e 696e 6974 7061 7267 7202 0000  src.initpargr...
-000006a0: 00da 166d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
-000006b0: 2e63 6f6c 726d 6f64 6572 0300 0000 da13  .colrmoder......
-000006c0: 6d61 7074 6173 6b65 722e 7372 632e 6572  maptasker.src.er
-000006d0: 726f 7272 0400 0000 da16 6d61 7074 6173  rorr......maptas
-000006e0: 6b65 722e 7372 632e 7379 7363 6f6e 7374  ker.src.sysconst
-000006f0: 7205 0000 0072 0c00 0000 da04 626f 6f6c  r....r......bool
-00000700: da05 7475 706c 65da 0464 6963 7472 2100  ..tuple..dictr!.
-00000710: 0000 720a 0000 0072 0a00 0000 720a 0000  ..r....r....r...
-00000720: 0072 0b00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000730: 0100 0000 730c 0000 000c 130c 010c 010c  ....s...........
-00000740: 0108 031e 0c                             .....
+00000290: 0059 006e 0177 007c 026a 0b72 4b7c 026a  .Y.n.w.|.j.rK|.j
+000002a0: 0b6a 0c7c 0064 093c 0074 0d44 005d 207d  .j.|.d.<.t.D.] }
+000002b0: 037c 0364 0a6b 0272 6474 0e7c 027c 0383  .|.d.k.rdt.|.|..
+000002c0: 0204 007d 0472 6364 0b7c 049b 009d 027c  ...}.rcd.|.....|
+000002d0: 0064 0619 007c 033c 0071 4d74 0e7c 027c  .d...|.<.qMt.|.|
+000002e0: 0383 027c 0064 0619 007c 033c 0071 4d74  ...|.d...|.<.qMt
+000002f0: 0f7c 0064 0619 0064 0719 0074 1083 0272  .|.d...d...t...r
+00000300: 8374 087c 0064 0619 0064 0719 0083 017c  .t.|.d...d.....|
+00000310: 0064 0619 0064 073c 0074 117c 026a 1283  .d...d.<.t.|.j..
+00000320: 017d 057c 026a 1372 997c 026a 13a0 14a1  .}.|.j.r.|.j....
+00000330: 0044 005d 085c 027d 067d 037c 037c 057c  .D.].\.}.}.|.|.|
+00000340: 063c 0071 9074 1574 017c 0283 0201 007c  .<.q.t.t.|.....|
+00000350: 0064 0619 007c 0566 0253 0029 0c61 3b01  .d...|.f.S.).a;.
+00000360: 0000 0a20 2020 2050 7265 7365 6e74 2074  ...    Present t
+00000370: 6865 2047 5549 2061 6e64 2067 6574 2074  he GUI and get t
+00000380: 6865 2072 756e 7469 6d65 2064 6574 6169  he runtime detai
+00000390: 6c73 0a20 2020 2020 2020 203a 7061 7261  ls.        :para
+000003a0: 6d20 7072 696d 6172 795f 6974 656d 733a  m primary_items:
+000003b0: 2064 6963 7469 6f6e 6172 7920 6f66 2074   dictionary of t
+000003c0: 6865 2070 7269 6d61 7279 2069 7465 6d73  he primary items
+000003d0: 2075 7365 6420 7468 726f 7567 686f 7574   used throughout
+000003e0: 2074 6865 206d 6f64 756c 652e 2020 5365   the module.  Se
+000003f0: 6520 6d61 7069 742e 7079 2066 6f72 2064  e mapit.py for d
+00000400: 6574 6169 6c73 0a20 2020 2020 2020 203a  etails.        :
+00000410: 7061 7261 6d20 7573 655f 6775 693a 2066  param use_gui: f
+00000420: 6c61 6720 6966 2075 7369 6a6e 6720 7468  lag if usijng th
+00000430: 6520 4755 492c 206d 616b 6520 7375 7265  e GUI, make sure
+00000440: 2077 6520 696d 706f 7274 2069 740a 2020   we import it.  
+00000450: 2020 2020 2020 3a72 6574 7572 6e3a 2070        :return: p
+00000460: 726f 6772 616d 2072 756e 7469 6d65 2061  rogram runtime a
+00000470: 7267 756d 656e 7473 2061 6e64 2063 6f6c  rguments and col
+00000480: 6f72 7320 746f 2075 7365 2069 6e20 7468  ors to use in th
+00000490: 6520 6f75 7470 7574 0a20 2020 2072 0100  e output.    r..
+000004a0: 0000 2901 7208 0000 007a 1850 726f 6772  ..).r....z.Progr
+000004b0: 616d 2065 7869 7465 642e 2047 6f6f 6462  am exited. Goodb
+000004c0: 7965 2e7a 2650 726f 6772 616d 2063 616e  ye.z&Program can
+000004d0: 6365 6c6c 6564 2062 6520 7573 6572 2028  celled be user (
+000004e0: 6b69 6c6c 6564 2047 5549 29e9 6300 0000  killed GUI).c...
+000004f0: da11 7072 6f67 7261 6d5f 6172 6775 6d65  ..program_argume
+00000500: 6e74 73da 1464 6973 706c 6179 5f64 6574  nts..display_det
+00000510: 6169 6c5f 6c65 7665 6ce9 0300 0000 da0b  ail_level.......
+00000520: 6669 6c65 5f74 6f5f 6765 74da 1062 6163  file_to_get..bac
+00000530: 6b75 705f 6669 6c65 5f68 7474 707a 0768  kup_file_httpz.h
+00000540: 7474 703a 2f2f 2916 5a16 6d61 7074 6173  ttp://).Z.maptas
+00000550: 6b65 722e 7372 632e 7573 6572 696e 7472  ker.src.userintr
+00000560: 7208 0000 00da 086d 6169 6e6c 6f6f 70da  r......mainloop.
+00000570: 0465 7869 7472 0400 0000 5a0a 676f 5f70  .exitr....Z.go_p
+00000580: 726f 6772 616d da05 7265 7275 6e72 0200  rogram..rerunr..
+00000590: 0000 da03 696e 7472 1100 0000 da09 5479  ....intr......Ty
+000005a0: 7065 4572 726f 72da 0466 696c 65da 046e  peError..file..n
+000005b0: 616d 6572 0500 0000 da07 6765 7461 7474  amer......getatt
+000005c0: 72da 0a69 7369 6e73 7461 6e63 65da 0373  r..isinstance..s
+000005d0: 7472 7203 0000 005a 0f61 7070 6561 7261  trr....Z.appeara
+000005e0: 6e63 655f 6d6f 6465 5a0c 636f 6c6f 725f  nce_modeZ.color_
+000005f0: 6c6f 6f6b 7570 da05 6974 656d 7372 0c00  lookup..itemsr..
+00000600: 0000 2907 da0d 7072 696d 6172 795f 6974  ..)...primary_it
+00000610: 656d 7372 0d00 0000 7209 0000 00da 0576  emsr....r......v
+00000620: 616c 7565 5a09 6874 7470 5f69 6e66 6fda  alueZ.http_info.
+00000630: 0863 6f6c 6f72 6d61 70da 036b 6579 720a  .colormap..keyr.
+00000640: 0000 0072 0a00 0000 720b 0000 00da 0b70  ...r....r......p
+00000650: 726f 6365 7373 5f67 7569 2600 0000 7348  rocess_gui&...sH
+00000660: 0000 0004 090c 0106 0308 0106 030a 010c  ................
+00000670: 030a 010a 0302 0302 0104 0110 ff0c 0310  ................
+00000680: 0102 ff06 040c 0108 0308 010e 0112 0102  ................
+00000690: 8014 0212 0202 010a 010c ff0a 0506 0312  ................
+000006a0: 010a 010a 0306 0302 0104 fe72 2400 0000  ...........r$...
+000006b0: 4e29 0dda 166d 6170 7461 736b 6572 2e73  N)...maptasker.s
+000006c0: 7263 2e69 6e69 7470 6172 6772 0200 0000  rc.initpargr....
+000006d0: da16 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
+000006e0: 636f 6c72 6d6f 6465 7203 0000 00da 136d  colrmoder......m
+000006f0: 6170 7461 736b 6572 2e73 7263 2e65 7272  aptasker.src.err
+00000700: 6f72 7204 0000 00da 166d 6170 7461 736b  orr......maptask
+00000710: 6572 2e73 7263 2e73 7973 636f 6e73 7472  er.src.sysconstr
+00000720: 0500 0000 720c 0000 00da 0462 6f6f 6cda  ....r......bool.
+00000730: 0574 7570 6c65 da04 6469 6374 7224 0000  .tuple..dictr$..
+00000740: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
+00000750: 720b 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000760: 0000 0073 0c00 0000 0c13 0c01 0c01 0c01  ...s............
+00000770: 0803 1e0c                                ....
```

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/scenes.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/scenes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/servicec.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/servicec.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/share.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/share.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/shellsort.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/shellsort.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/sysconst.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/sysconst.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 13 16:28:51 2023 UTC, .py size: 4396 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4399 8864 2c11 0000  o.......C..d,...
+00000000: 6f0d 0d0a 0000 0000 b97a 9064 2c11 0000  o........z.d,...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6403 5a03 6404 5a04 6405 5a05 6406  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a06 6407 5a07 6408 5a08 6409 6501 9b00  Z.d.Z.d.Z.d.e...
 00000060: 9d02 5a09 640a 5a0a 6900 640b 640c 9301  ..Z.d.Z.i.d.d...
 00000070: 640d 640c 9301 640e 640f 9301 6410 640f  d.d...d.d...d.d.
@@ -26,15 +26,15 @@
 00000190: 9301 6437 6449 9301 643a 644a 9301 643d  ..d7dI..d:dJ..d=
 000001a0: 643b 6901 a501 5a0c 6700 644b a201 5a0d  d;i...Z.g.dK..Z.
 000001b0: 6502 a00e 644c a101 5a0f 644d 5a10 644d  e...dL..Z.dMZ.dM
 000001c0: 5a11 6402 5300 294e e900 0000 0029 01da  Z.d.S.)N.....)..
 000001d0: 0b4f 5554 5055 545f 464f 4e54 4e7a 1255  .OUTPUT_FONTNz.U
 000001e0: 6e6e 616d 6564 2f41 6e6f 6e79 6d6f 7573  nnamed/Anonymous
 000001f0: 2e7a 174d 6170 5461 736b 6572 2076 6572  .z.MapTasker ver
-00000200: 7369 6f6e 2032 2e30 2e34 7a34 474e 5520  sion 2.0.4z4GNU 
+00000200: 7369 6f6e 2032 2e30 2e35 7a34 474e 5520  sion 2.0.5z4GNU 
 00000210: 4745 4e45 5241 4c20 5055 424c 4943 204c  GENERAL PUBLIC L
 00000220: 4943 454e 5345 2028 5665 7273 696f 6e20  ICENSE (Version 
 00000230: 332c 2032 3920 4a75 6e65 2032 3030 3729  3, 29 June 2007)
 00000240: 7a0c 2d6e 6f6e 6520 666f 756e 642e 7a17  z.-none found.z.
 00000250: 2e4d 6170 5461 736b 6572 5f52 756e 436f  .MapTasker_RunCo
 00000260: 756e 742e 7478 747a 192e 4d61 7054 6173  unt.txtz..MapTas
 00000270: 6b65 725f 6172 6775 6d65 6e74 732e 6a73  ker_arguments.js
@@ -82,15 +82,15 @@
 00000510: 6173 6b65 724e 6574 2049 6e66 6f72 6d61  askerNet Informa
 00000520: 7469 6f6e 5a0f 7461 736b 6572 6e65 745f  tionZ.taskernet_
 00000530: 636f 6c6f 725a 0d54 6173 6b65 724e 6574  colorZ.TaskerNet
 00000540: 496e 666f 7a12 5461 736b 6572 2050 7265  Infoz.Tasker Pre
 00000550: 6665 7265 6e63 6573 5a11 7072 6566 6572  ferencesZ.prefer
 00000560: 656e 6365 735f 636f 6c6f 725a 0b50 7265  ences_colorZ.Pre
 00000570: 6665 7265 6e63 6573 7a11 5472 6169 6c69  ferencesz.Traili
-00000580: 6e67 2043 6f6d 6d65 6e74 735a 1774 7261  ng CommentsZ.tra
+00000580: 6e67 2043 6f6d 6d65 6e74 73da 1774 7261  ng Comments..tra
 00000590: 696c 696e 675f 636f 6d6d 656e 7473 5f63  iling_comments_c
 000005a0: 6f6c 6f72 5a10 5472 6169 6c69 6e67 436f  olorZ.TrailingCo
 000005b0: 6d6d 656e 7473 7a0e 5461 736b 2027 6163  mmentsz.Task 'ac
 000005c0: 7469 6f6e 7327 7a13 2764 6973 6162 6c65  tions'z.'disable
 000005d0: 6427 2050 726f 6669 6c65 737a 0f27 756e  d' Profilesz.'un
 000005e0: 6b6e 6f77 6e27 2054 6173 6b73 7a17 6469  known' Tasksz.di
 000005f0: 7361 626c 6564 2054 6173 6b20 2761 6374  sabled Task 'act
@@ -132,15 +132,15 @@
 00000830: 4f5f 5553 455a 0a4e 4f5f 5052 4f46 494c  O_USEZ.NO_PROFIL
 00000840: 455a 1454 5950 4553 5f4f 465f 434f 4c4f  EZ.TYPES_OF_COLO
 00000850: 525f 4e41 4d45 535a 0f54 5950 4553 5f4f  R_NAMESZ.TYPES_O
 00000860: 465f 434f 4c4f 5253 5a0e 4152 4755 4d45  F_COLORSZ.ARGUME
 00000870: 4e54 5f4e 414d 4553 5a09 6765 744c 6f67  NT_NAMESZ.getLog
 00000880: 6765 72da 066c 6f67 6765 72da 0964 6562  ger..logger..deb
 00000890: 7567 5f6f 7574 5a0d 4445 4255 475f 5052  ug_outZ.DEBUG_PR
-000008a0: 4f47 5241 4da9 0072 1800 0000 7218 0000  OGRAM..r....r...
+000008a0: 4f47 5241 4da9 0072 1900 0000 7219 0000  OGRAM..r....r...
 000008b0: 00fa 772f 5573 6572 732f 6d69 6b72 7562  ..w/Users/mikrub
 000008c0: 696e 2f4c 6962 7261 7279 2f43 6c6f 7564  in/Library/Cloud
 000008d0: 5374 6f72 6167 652f 476f 6f67 6c65 4472  Storage/GoogleDr
 000008e0: 6976 652d 6d69 6b72 7562 696e 4067 6d61  ive-mikrubin@gma
 000008f0: 696c 2e63 6f6d 2f4d 7920 4472 6976 652f  il.com/My Drive/
 00000900: 5079 7468 6f6e 2f6d 6170 7461 736b 6572  Python/maptasker
 00000910: 2f6d 6170 7461 736b 6572 2f73 7263 2f73  /maptasker/src/s
```

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/taskactn.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/taskactn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/taskerd.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/taskerd.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/taskflag.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/taskflag.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/tasks.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/tasks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/taskuniq.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/taskuniq.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/twisty.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/twisty.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/userintr.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/userintr.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 13 16:34:54 2023 UTC, .py size: 40418 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ae9a 8864 e29d 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 a18d 9064 439f 0000  o..........dC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
@@ -445,701 +445,707 @@
 00001bc0: 0104 0102 0102 0108 fb06 070a 0106 ff04  ................
 00001bd0: 050e 0108 ff14 0304 030c 0108 ff14 0304  ................
 00001be0: 010a 0106 0104 1108 ed14 1504 030a 0102  ................
 00001bf0: 0104 0102 0102 0108 fb0e 0710 010e 037a  ...............z
 00001c00: 0e4d 7947 7569 2e5f 5f69 6e69 745f 5fda  .MyGui.__init__.
 00001c10: 0a66 6972 7374 5f74 696d 6563 0200 0000  .first_timec....
 00001c20: 0000 0000 0000 0000 0200 0000 0800 0000  ................
-00001c30: 4300 0000 7302 0100 007c 006a 006a 0167  C...s....|.j.j.g
+00001c30: 4300 0000 7308 0100 007c 006a 006a 0167  C...s....|.j.j.g
 00001c40: 0064 01a2 0164 028d 0101 007c 006a 00a0  .d...d.....|.j..
 00001c50: 0264 03a1 0101 0064 047c 005f 0364 0504  .d.....d.|._.d..
 00001c60: 007c 005f 0404 007c 005f 0504 007c 005f  .|._...|._...|._
 00001c70: 0604 007c 005f 0704 007c 005f 0804 007c  ...|._...|._...|
 00001c80: 005f 0904 007c 005f 0a04 007c 005f 0b04  ._...|._...|._..
 00001c90: 007c 005f 0c7c 005f 0d64 0604 007c 005f  .|._.|._.d...|._
 00001ca0: 0e04 007c 005f 0f7c 005f 1064 077c 005f  ...|._.|._.d.|._
 00001cb0: 117c 006a 12a0 0264 08a1 0101 0067 007c  .|.j...d.....g.|
 00001cc0: 005f 1364 087c 005f 147c 0172 537c 006a  ._.d.|._.|.rS|.j
 00001cd0: 15a0 1664 0964 0a74 1717 00a1 0201 0069  ...d.d.t.......i
-00001ce0: 007c 005f 187a 067c 006a 1972 5b09 0057  .|._.z.|.j.r[..W
-00001cf0: 006e 0c04 0074 1a79 6801 0001 0001 0064  .n...t.yh......d
-00001d00: 067c 005f 1959 006e 0177 007a 0a7c 006a  .|._.Y.n.w.z.|.j
-00001d10: 1b72 7109 0057 0064 0053 0057 0064 0053  .rq..W.d.S.W.d.S
-00001d20: 0004 0074 1a79 8001 0001 0001 0064 067c  ...t.y.......d.|
-00001d30: 005f 1b59 0064 0053 0077 0029 0b4e 7222  ._.Y.d.S.w.).Nr"
-00001d40: 0000 0029 0172 2700 0000 7226 0000 0072  ...).r'...r&...r
-00001d50: 1000 0000 46da 0072 0f00 0000 720b 0000  ....F..r....r...
-00001d60: 00fa 0330 2e30 7a10 4d61 7054 6173 6b65  ...0.0z.MapTaske
-00001d70: 7220 4865 6c70 0a0a 291c 725a 0000 0072  r Help..).rZ...r
-00001d80: 6e00 0000 da03 7365 74da 1464 6973 706c  n.....set..displ
-00001d90: 6179 5f64 6574 6169 6c5f 6c65 7665 6cda  ay_detail_level.
-00001da0: 1a64 6973 706c 6179 5f70 726f 6669 6c65  .display_profile
-00001db0: 5f63 6f6e 6469 7469 6f6e 73da 1364 6973  _conditions..dis
-00001dc0: 706c 6179 5f70 7265 6665 7265 6e63 6573  play_preferences
-00001dd0: da11 6469 7370 6c61 795f 7461 736b 6572  ..display_tasker
-00001de0: 6e65 74da 0564 6562 7567 5a0e 636c 6561  net..debugZ.clea
-00001df0: 725f 7365 7474 696e 6773 da05 7265 7365  r_settings..rese
-00001e00: 74da 0465 7869 74da 0a67 6f5f 7072 6f67  t..exit..go_prog
-00001e10: 7261 6dda 0572 6572 756e da06 7477 6973  ram..rerun..twis
-00001e20: 7479 da13 7369 6e67 6c65 5f70 726f 6a65  ty..single_proje
-00001e30: 6374 5f6e 616d 65da 1373 696e 676c 655f  ct_name..single_
-00001e40: 7072 6f66 696c 655f 6e61 6d65 da10 7369  profile_name..si
-00001e50: 6e67 6c65 5f74 6173 6b5f 6e61 6d65 da0e  ngle_task_name..
-00001e60: 636f 6c6f 725f 7465 7874 5f72 6f77 7266  color_text_rowrf
-00001e70: 0000 00da 0c63 6f6c 6f72 5f6c 6162 656c  .....color_label
-00001e80: 73da 0f61 7070 6561 7261 6e63 655f 6d6f  s..appearance_mo
-00001e90: 6465 726d 0000 00da 0669 6e73 6572 74da  derm.....insert.
-00001ea0: 0949 4e46 4f5f 5445 5854 da0c 636f 6c6f  .INFO_TEXT..colo
-00001eb0: 725f 6c6f 6f6b 7570 da10 6261 636b 7570  r_lookup..backup
-00001ec0: 5f66 696c 655f 6874 7470 da0e 4174 7472  _file_http..Attr
-00001ed0: 6962 7574 6545 7272 6f72 da14 6261 636b  ibuteError..back
-00001ee0: 7570 5f66 696c 655f 6c6f 6361 7469 6f6e  up_file_location
-00001ef0: 2902 727e 0000 0072 8300 0000 7281 0000  ).r~...r....r...
-00001f00: 0072 8100 0000 7282 0000 0072 7c00 0000  .r....r....r|...
-00001f10: 6101 0000 7354 0000 0012 020c 0106 0102  a...sT..........
-00001f20: 0908 f804 0102 ff04 0302 fd04 0502 fb04  ................
-00001f30: 0702 f904 0802 f804 0802 f804 0802 f808  ................
-00001f40: 0812 0106 010c 0106 0106 0104 0112 0106  ................
-00001f50: 0102 0306 0102 0104 800c 010a 0102 ff02  ................
-00001f60: 0206 0108 0106 ff0c 020c 0102 ff7a 124d  .............z.M
-00001f70: 7947 7569 2e73 6574 5f64 6566 6175 6c74  yGui.set_default
-00001f80: 7363 0300 0000 0000 0000 0000 0000 0400  sc..............
-00001f90: 0000 0700 0000 4300 0000 7374 0000 007c  ......C...st...|
-00001fa0: 0272 0464 016e 0164 027d 037c 006a 00a0  .r.d.n.d.}.|.j..
-00001fb0: 0164 0364 04a1 0201 0074 026a 037c 0064  .d.d.....t.j.|.d
-00001fc0: 0564 0664 078d 037c 005f 007c 006a 006a  .d.d...|._.|.j.j
-00001fd0: 0464 0864 0964 0a64 0b64 0c64 0d8d 0501  .d.d.d.d.d.d....
-00001fe0: 007c 006a 00a0 0564 0e7c 019b 0064 0f9d  .|.j...d.|...d..
-00001ff0: 02a1 0201 007c 006a 006a 0664 107c 0364  .....|.j.j.d.|.d
-00002000: 118d 0201 007c 006a 00a0 07a1 0001 0064  .....|.j.......d
-00002010: 0053 0029 124e da05 4772 6565 6e72 3f00  .S.).N..Greenr?.
-00002020: 0000 fa03 312e 30da 0365 6e64 69f4 0100  ....1.0..endi...
-00002030: 0069 5802 0000 7242 0000 0072 0100 0000  .iX...rB...r....
-00002040: 720d 0000 0072 1900 0000 e928 0000 0072  r....r.....(...r
-00002050: 1400 0000 722b 0000 0072 8500 0000 da01  ....r+...r......
-00002060: 0ada 0864 6973 6162 6c65 6429 02da 0573  ...disabled)...s
-00002070: 7461 7465 723b 0000 0029 0872 6d00 0000  tater;...).rm...
-00002080: da06 6465 6c65 7465 7256 0000 0072 6c00  ..deleterV...rl.
-00002090: 0000 7257 0000 0072 9700 0000 726e 0000  ..rW...r....rn..
-000020a0: 00da 0966 6f63 7573 5f73 6574 2904 727e  ...focus_set).r~
-000020b0: 0000 00da 076d 6573 7361 6765 5a04 676f  .....messageZ.go
-000020c0: 6f64 da05 636f 6c6f 7272 8100 0000 7281  od..colorr....r.
-000020d0: 0000 0072 8200 0000 da13 6469 7370 6c61  ...r......displa
-000020e0: 795f 6d65 7373 6167 655f 626f 7887 0100  y_message_box...
-000020f0: 0073 1800 0000 0c02 0602 0201 0201 04fe  .s..............
-00002100: 1205 1601 1401 0601 0401 06ff 0e03 7a19  ..............z.
-00002110: 4d79 4775 692e 6469 7370 6c61 795f 6d65  MyGui.display_me
-00002120: 7373 6167 655f 626f 7863 0300 0000 0000  ssage_boxc......
-00002130: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
-00002140: 0000 73ba 0000 0064 017d 037c 0173 0d64  ..s....d.}.|.s.d
-00002150: 027c 0217 0064 0317 007d 0364 047c 005f  .|...d...}.d.|._
-00002160: 007c 0164 0075 0072 1364 057d 037c 006a  .|.d.u.r.d.}.|.j
-00002170: 0172 1c7c 006a 0272 1c64 067d 036e 217c  .r.|.j.r.d.}.n!|
-00002180: 006a 0172 257c 006a 0372 2564 077d 036e  .j.r%|.j.r%d.}.n
-00002190: 187c 006a 0272 2e7c 006a 0372 2e64 087d  .|.j.r.|.j.r.d.}
-000021a0: 036e 0f7c 00a0 047c 017c 02a1 0273 3d64  .n.|...|.|...s=d
-000021b0: 097c 019b 0064 0a7c 029b 0064 0b9d 057d  .|...d.|...d...}
-000021c0: 037c 0372 4f7c 00a0 057c 0364 0ca1 0201  .|.rO|...|.d....
-000021d0: 0064 0d5c 037c 005f 017c 005f 027c 005f  .d.\.|._.|._.|._
-000021e0: 0364 0053 007c 00a0 0564 0e7c 019b 0064  .d.S.|...d.|...d
-000021f0: 0f7c 029b 009d 0464 0ca1 0201 0064 0053  .|.....d.....d.S
-00002200: 0029 104e 7284 0000 007a 2145 7272 6f72  .).Nr....z!Error
-00002210: 3a0a 0a54 6865 206e 616d 6520 656e 7465  :..The name ente
-00002220: 7265 6420 666f 7220 7468 6520 7a16 2069  red for the z. i
-00002230: 7320 626c 616e 6b21 0a0a 5472 7920 6167  s blank!..Try ag
-00002240: 6169 6e2e 467a 2c4e 616d 6520 656e 7472  ain.Fz,Name entr
-00002250: 7920 6361 6e63 656c 6564 2e20 2041 6c6c  y canceled.  All
-00002260: 2077 696c 6c20 6265 2064 6973 706c 6179   will be display
-00002270: 6564 2e7a 5b45 7272 6f72 3a0a 0a59 6f75  ed.z[Error:..You
-00002280: 2068 6176 6520 656e 7465 7265 6420 626f   have entered bo
-00002290: 7468 2061 2050 726f 6a65 6374 2061 6e64  th a Project and
-000022a0: 2061 2050 726f 6669 6c65 206e 616d 6521   a Profile name!
-000022b0: 0a0a 5472 7920 6167 6169 6e20 616e 6420  ..Try again and 
-000022c0: 6f6e 6c79 2073 656c 6563 7420 6f6e 652e  only select one.
-000022d0: 7a58 4572 726f 723a 0a0a 596f 7520 6861  zXError:..You ha
-000022e0: 7665 2065 6e74 6572 6564 2062 6f74 6820  ve entered both 
-000022f0: 6120 5072 6f6a 6563 7420 616e 6420 6120  a Project and a 
-00002300: 5461 736b 206e 616d 6521 0a0a 5472 7920  Task name!..Try 
-00002310: 6167 6169 6e20 616e 6420 6f6e 6c79 2073  again and only s
-00002320: 656c 6563 7420 6f6e 652e 7a58 4572 726f  elect one.zXErro
-00002330: 723a 0a0a 596f 7520 6861 7665 2065 6e74  r:..You have ent
-00002340: 6572 6564 2062 6f74 6820 6120 5072 6f66  ered both a Prof
-00002350: 696c 6520 616e 6420 6120 5461 736b 206e  ile and a Task n
-00002360: 616d 6521 0a0a 5472 7920 6167 6169 6e20  ame!..Try again 
-00002370: 616e 6420 6f6e 6c79 2073 656c 6563 7420  and only select 
-00002380: 6f6e 652e 7a08 4572 726f 723a 2022 7a02  one.z.Error: "z.
-00002390: 2220 7a18 206e 6f74 2066 6f75 6e64 2121  " z. not found!!
-000023a0: 2020 5472 7920 6167 6169 6e2e 5429 0372    Try again.T).r
-000023b0: 8400 0000 7284 0000 0072 8400 0000 7a12  ....r....r....z.
-000023c0: 4469 7370 6c61 7920 6f6e 6c79 2074 6865  Display only the
-000023d0: 2027 7a02 2720 2906 5a0a 6e61 6d65 645f   'z.' ).Z.named_
-000023e0: 6974 656d 7291 0000 0072 9200 0000 7293  itemr....r....r.
-000023f0: 0000 00da 0a76 616c 6964 5f69 7465 6d72  .....valid_itemr
-00002400: a800 0000 2904 727e 0000 00da 0874 6865  ....).r~.....the
-00002410: 5f6e 616d 65da 0c65 6c65 6d65 6e74 5f6e  _name..element_n
-00002420: 616d 65da 0d65 7272 6f72 5f6d 6573 7361  ame..error_messa
-00002430: 6765 7281 0000 0072 8100 0000 7282 0000  ger....r....r...
-00002440: 00da 0a63 6865 636b 5f6e 616d 659b 0100  ...check_name...
-00002450: 0073 4200 0000 0401 0402 0202 0201 02ff  .sB.............
-00002460: 0202 02fe 02ff 0605 0801 0401 0c03 0202  ................
-00002470: 04ff 0c04 0202 04ff 0c04 0202 04ff 0c05  ................
-00002480: 1002 02ff 0405 0c01 0205 02fc 0401 0401  ................
-00002490: 0801 0403 1001 08ff 7a10 4d79 4775 692e  ........z.MyGui.
-000024a0: 6368 6563 6b5f 6e61 6d65 6303 0000 0000  check_namec.....
-000024b0: 0000 0000 0000 0008 0000 0009 0000 0043  ...............C
-000024c0: 0000 0073 0601 0000 6401 7400 8300 6901  ...s....d.t...i.
-000024d0: 7d03 7c00 6a01 7c03 6401 1900 6402 3c00  }.|.j.|.d...d.<.
-000024e0: 7c00 6a01 7211 6403 6e01 6404 7c03 6405  |.j.r.d.n.d.|.d.
-000024f0: 3c00 7402 7c00 6a03 8301 7c03 6406 3c00  <.t.|.j...|.d.<.
-00002500: 7404 8300 7c03 6407 3c00 7405 7c03 8301  t...|.d.<.t.|...
-00002510: 7d03 7c03 6407 3d00 6700 7d04 7c02 0400  }.|.d.=.g.}.|...
-00002520: 6408 6b02 7239 0100 7c03 6409 1900 640a  d.k.r9..|.d...d.
-00002530: 1900 7d04 6900 7d05 6e19 0400 640b 6b02  ..}.i.}.n...d.k.
-00002540: 7245 0100 7c03 640c 1900 7d04 640c 7d05  rE..|.d...}.d.}.
-00002550: 6e0d 640d 6b02 724f 7c03 640e 1900 7d04  n.d.k.rO|.d...}.
-00002560: 640e 7d05 6e03 0900 6900 7d05 7c04 4400  d.}.n...i.}.|.D.
-00002570: 5d2c 7d06 7a1f 7c02 6408 6b02 7262 7c06  ],}.z.|.d.k.rb|.
-00002580: a006 640f a101 6a07 7d07 6e0a 7c03 7c05  ..d...j.}.n.|.|.
-00002590: 1900 7c06 1900 a006 6410 a101 6a07 7d07  ..|.....d...j.}.
-000025a0: 7c01 7c07 6b02 7274 5700 0100 6411 5300  |.|.k.rtW...d.S.
-000025b0: 5700 7154 0400 7408 7980 0100 0100 0100  W.qT..t.y.......
-000025c0: 6404 7d07 5900 7154 7700 6412 5300 2913  d.}.Y.qTw.d.S.).
-000025d0: 4eda 1170 726f 6772 616d 5f61 7267 756d  N..program_argum
-000025e0: 656e 7473 728b 0000 00fa 0a62 6163 6b75  entsr......backu
-000025f0: 702e 786d 6c72 8400 0000 da0b 6669 6c65  p.xmlr......file
-00002600: 5f74 6f5f 6765 74da 0d63 6f6c 6f72 735f  _to_get..colors_
-00002610: 746f 5f75 7365 da0c 6f75 7470 7574 5f6c  to_use..output_l
-00002620: 696e 6573 da07 5072 6f6a 6563 74da 1474  ines..Project..t
-00002630: 6173 6b65 725f 726f 6f74 5f65 6c65 6d65  asker_root_eleme
-00002640: 6e74 73da 0c61 6c6c 5f70 726f 6a65 6374  nts..all_project
-00002650: 73da 0750 726f 6669 6c65 da0c 616c 6c5f  s..Profile..all_
-00002660: 7072 6f66 696c 6573 da04 5461 736b da09  profiles..Task..
-00002670: 616c 6c5f 7461 736b 73da 046e 616d 65da  all_tasks..name.
-00002680: 036e 6d65 5446 2909 7206 0000 0072 8b00  .nmeTF).r....r..
-00002690: 0000 7209 0000 0072 9600 0000 720a 0000  ..r....r....r...
-000026a0: 0072 0500 0000 da04 6669 6e64 721b 0000  .r......findr...
-000026b0: 0072 9b00 0000 2908 727e 0000 0072 aa00  .r....).r~...r..
-000026c0: 0000 72ab 0000 005a 1274 656d 705f 7072  ..r....Z.temp_pr
-000026d0: 696d 6172 795f 6974 656d 73da 0c72 6f6f  imary_items..roo
-000026e0: 745f 656c 656d 656e 745a 0b64 6963 745f  t_elementZ.dict_
-000026f0: 746f 5f75 7365 da04 6974 656d 5a09 6974  to_use..itemZ.it
-00002700: 656d 5f6e 616d 6572 8100 0000 7281 0000  em_namer....r...
-00002710: 0072 8200 0000 72a9 0000 00ce 0100 0073  .r....r........s
-00002720: 4400 0000 0a02 0e01 1201 0e01 0a01 0801  D...............
-00002730: 0601 0402 0203 0a01 0601 0201 04ff 0603  ................
-00002740: 0a01 0801 0601 0601 0801 0601 0201 0401  ................
-00002750: 0803 0201 0801 0e01 1402 0801 0801 04ff  ................
-00002760: 0c02 0801 02ff 0403 7a10 4d79 4775 692e  ........z.MyGui.
-00002770: 7661 6c69 645f 6974 656d 6301 0000 0000  valid_itemc.....
-00002780: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00002790: 0000 00f3 5200 0000 7c00 6a00 a001 6401  ....R...|.j...d.
-000027a0: 6402 a102 0100 7c00 6a02 a003 a100 0100  d.....|.j.......
-000027b0: 7c00 6a04 a003 a100 0100 7405 6a06 6403  |.j.......t.j.d.
-000027c0: 7407 9b00 9d02 6404 6405 8d02 7d01 7c01  t.....d.d...}.|.
-000027d0: a008 a100 7c00 5f09 7c00 a00a 7c00 6a09  ....|._.|...|.j.
-000027e0: 6406 a102 0100 6400 5300 2907 4e72 9e00  d.....d.S.).Nr..
-000027f0: 0000 729f 0000 007a 1345 6e74 6572 2050  ..r....z.Enter P
-00002800: 726f 6a65 6374 206e 616d 653a 7a18 4469  roject name:z.Di
-00002810: 7370 6c61 7920 5370 6563 6966 6963 2050  splay Specific P
-00002820: 726f 6a65 6374 a902 721b 0000 0072 5200  roject..r....rR.
-00002830: 0000 72b3 0000 0029 0b72 6d00 0000 72a4  ..r....).rm...r.
-00002840: 0000 0072 7500 0000 da08 6465 7365 6c65  ...ru.....desele
-00002850: 6374 7277 0000 0072 5600 0000 da0e 4354  ctrw...rV.....CT
-00002860: 6b49 6e70 7574 4469 616c 6f67 da11 6361  kInputDialog..ca
-00002870: 6e63 656c 5f62 7574 746f 6e5f 6d73 67da  ncel_button_msg.
-00002880: 0967 6574 5f69 6e70 7574 7291 0000 0072  .get_inputr....r
-00002890: ad00 0000 a902 727e 0000 00da 0664 6961  ......r~.....dia
-000028a0: 6c6f 6772 8100 0000 7281 0000 0072 8200  logr....r....r..
-000028b0: 0000 7272 0000 00fb 0100 00f3 1200 0000  ..rr............
-000028c0: 0e02 0a03 0a01 0402 0801 0201 06fe 0a05  ................
-000028d0: 1202 7a1f 4d79 4775 692e 7369 6e67 6c65  ..z.MyGui.single
-000028e0: 5f70 726f 6a65 6374 5f6e 616d 655f 6576  _project_name_ev
-000028f0: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
-00002900: 0200 0000 0400 0000 4300 0000 72bf 0000  ........C...r...
-00002910: 0029 074e 729e 0000 0072 9f00 0000 7a13  .).Nr....r....z.
-00002920: 456e 7465 7220 5072 6f66 696c 6520 6e61  Enter Profile na
-00002930: 6d65 3a7a 1844 6973 706c 6179 2053 7065  me:z.Display Spe
-00002940: 6369 6669 6320 5072 6f66 696c 6572 c000  cific Profiler..
-00002950: 0000 72b6 0000 0029 0b72 6d00 0000 72a4  ..r....).rm...r.
-00002960: 0000 0072 7300 0000 72c1 0000 0072 7700  ...rs...r....rw.
-00002970: 0000 7256 0000 0072 c200 0000 72c3 0000  ..rV...r....r...
-00002980: 0072 c400 0000 7292 0000 0072 ad00 0000  .r....r....r....
-00002990: 72c5 0000 0072 8100 0000 7281 0000 0072  r....r....r....r
-000029a0: 8200 0000 7274 0000 000f 0200 0072 c700  ....rt.......r..
-000029b0: 0000 7a1f 4d79 4775 692e 7369 6e67 6c65  ..z.MyGui.single
-000029c0: 5f70 726f 6669 6c65 5f6e 616d 655f 6576  _profile_name_ev
-000029d0: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
-000029e0: 0200 0000 0400 0000 4300 0000 72bf 0000  ........C...r...
-000029f0: 0029 074e 729e 0000 0072 9f00 0000 7a10  .).Nr....r....z.
-00002a00: 456e 7465 7220 5461 736b 206e 616d 653a  Enter Task name:
-00002a10: 7a15 4469 7370 6c61 7920 5370 6563 6966  z.Display Specif
-00002a20: 6963 2054 6173 6b72 c000 0000 72b8 0000  ic Taskr....r...
-00002a30: 0029 0b72 6d00 0000 72a4 0000 0072 7300  .).rm...r....rs.
-00002a40: 0000 72c1 0000 0072 7500 0000 7256 0000  ..r....ru...rV..
-00002a50: 0072 c200 0000 72c3 0000 0072 c400 0000  .r....r....r....
-00002a60: 7293 0000 0072 ad00 0000 72c5 0000 0072  r....r....r....r
-00002a70: 8100 0000 7281 0000 0072 8200 0000 7276  ....r....r....rv
-00002a80: 0000 0023 0200 0072 c700 0000 7a1c 4d79  ...#...r....z.My
-00002a90: 4775 692e 7369 6e67 6c65 5f74 6173 6b5f  Gui.single_task_
-00002aa0: 6e61 6d65 5f65 7665 6e74 da13 6e65 775f  name_event..new_
-00002ab0: 6170 7065 6172 616e 6365 5f6d 6f64 6563  appearance_modec
-00002ac0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00002ad0: 0300 0000 4300 0000 7314 0000 0074 00a0  ....C...s....t..
-00002ae0: 017c 01a1 0101 007c 017c 005f 0264 0053  .|.....|.|._.d.S
-00002af0: 00a9 014e 2903 7256 0000 00da 1373 6574  ...N).rV.....set
-00002b00: 5f61 7070 6561 7261 6e63 655f 6d6f 6465  _appearance_mode
-00002b10: 7296 0000 0029 0272 7e00 0000 72c8 0000  r....).r~...r...
-00002b20: 0072 8100 0000 7281 0000 0072 8200 0000  .r....r....r....
-00002b30: 7265 0000 0037 0200 0073 0400 0000 0a01  re...7...s......
-00002b40: 0a01 7a22 4d79 4775 692e 6368 616e 6765  ..z"MyGui.change
-00002b50: 5f61 7070 6561 7261 6e63 655f 6d6f 6465  _appearance_mode
-00002b60: 5f65 7665 6e74 da0e 6469 7370 6c61 795f  _event..display_
-00002b70: 6465 7461 696c 6302 0000 0000 0000 0000  detailc.........
-00002b80: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00002b90: 1600 0000 7c01 7c00 5f00 7c00 6a01 a002  ....|.|._.|.j...
-00002ba0: 7c01 a101 0100 6400 5300 72c9 0000 0029  |.....d.S.r....)
-00002bb0: 0372 8700 0000 725a 0000 0072 8600 0000  .r....rZ...r....
-00002bc0: 2902 727e 0000 0072 cb00 0000 7281 0000  ).r~...r....r...
-00002bd0: 0072 8100 0000 7282 0000 0072 5900 0000  .r....r....rY...
-00002be0: 3e02 0000 7304 0000 0006 0110 017a 1b4d  >...s........z.M
-00002bf0: 7947 7569 2e64 6574 6169 6c5f 7365 6c65  yGui.detail_sele
-00002c00: 6374 6564 5f65 7665 6e74 da13 636f 6c6f  cted_event..colo
-00002c10: 725f 7365 6c65 6374 6564 5f69 7465 6d63  r_selected_itemc
-00002c20: 0200 0000 0000 0000 0000 0000 0800 0000  ................
-00002c30: 0800 0000 4300 0000 73d6 0000 0067 0064  ....C...s....g.d
-00002c40: 01a2 017d 027c 006a 007c 006a 007c 006a  ...}.|.j.|.j.|.j
-00002c50: 017c 006a 0267 047d 0374 03a0 0474 05a1  .|.j.g.}.t...t..
-00002c60: 018f 3001 007c 02a0 067c 01a1 017d 047c  ..0..|...|...}.|
-00002c70: 037c 0419 0073 3c7c 01a0 0764 0264 03a1  .|...s<|...d.d..
-00002c80: 027d 057c 05a0 0764 0464 03a1 027d 057c  .}.|...d.d...}.|
-00002c90: 00a0 0864 057c 059b 0064 069d 0364 07a1  ...d.|...d...d..
-00002ca0: 0201 0009 0057 0064 0004 0004 0083 0301  .....W.d........
-00002cb0: 0064 0053 0057 0064 0004 0004 0083 0301  .d.S.W.d........
-00002cc0: 006e 0831 0073 4677 0101 0001 0001 0059  .n.1.sFw.......Y
-00002cd0: 0001 0074 0983 007d 067c 06a0 0aa1 007d  ...t...}.|.....}
-00002ce0: 077c 0764 0075 0172 697c 00a0 087c 019b  .|.d.u.ri|...|..
-00002cf0: 0064 087c 079b 009d 0364 07a1 0201 007c  .d.|.....d.....|
-00002d00: 00a0 0b7c 077c 01a1 0201 0064 0053 0064  ...|.|.....d.S.d
-00002d10: 0053 0029 094e 2904 7248 0000 0072 4a00  .S.).N).rH...rJ.
-00002d20: 0000 724e 0000 0072 4f00 0000 7a08 5072  ..rN...rO...z.Pr
-00002d30: 6f66 696c 6520 7284 0000 007a 0741 6374  ofile r....z.Act
-00002d40: 696f 6e20 7a08 4469 7370 6c61 7920 7a17  ion z.Display z.
-00002d50: 2069 7320 6e6f 7420 7365 7420 746f 2064   is not set to d
-00002d60: 6973 706c 6179 2146 fa12 2063 6f6c 6f72  isplay!F.. color
-00002d70: 2063 6861 6e67 6564 2074 6f20 290c 7288   changed to ).r.
-00002d80: 0000 0072 8a00 0000 7289 0000 00da 0a63  ...r....r......c
-00002d90: 6f6e 7465 7874 6c69 62da 0873 7570 7072  ontextlib..suppr
-00002da0: 6573 73da 0945 7863 6570 7469 6f6e da05  ess..Exception..
-00002db0: 696e 6465 78da 0772 6570 6c61 6365 72a8  index..replacer.
-00002dc0: 0000 0072 0300 0000 da03 6765 74da 1865  ...r......get..e
-00002dd0: 7874 7261 6374 5f63 6f6c 6f72 5f66 726f  xtract_color_fro
-00002de0: 6d5f 6576 656e 7429 0872 7e00 0000 72cc  m_event).r~...r.
-00002df0: 0000 005a 0d77 6172 6e69 6e67 5f63 6865  ...Z.warning_che
-00002e00: 636b 5a0d 6368 6563 6b5f 6167 6169 6e73  ckZ.check_agains
-00002e10: 745a 0974 6865 5f69 6e64 6578 5a12 7468  tZ.the_indexZ.th
-00002e20: 655f 6f75 7470 7574 5f6d 6573 7361 6765  e_output_message
-00002e30: 5a0a 7069 636b 5f63 6f6c 6f72 72a7 0000  Z.pick_colorr...
-00002e40: 0072 8100 0000 7281 0000 0072 8200 0000  .r....r....r....
-00002e50: 7278 0000 0045 0200 0073 3400 0000 0801  rx...E...s4.....
-00002e60: 0407 0401 0401 0401 04fc 0c09 0a01 0801  ................
-00002e70: 0c01 0c01 0401 0c01 04ff 0203 10f8 0202  ................
-00002e80: 1cfe 060a 0801 0801 0401 0e01 04ff 1005  ................
-00002e90: 04fa 7a12 4d79 4775 692e 636f 6c6f 7273  ..z.MyGui.colors
-00002ea0: 5f65 7665 6e74 6303 0000 0000 0000 0000  _eventc.........
-00002eb0: 0000 0003 0000 0007 0000 0043 0000 0073  ...........C...s
-00002ec0: 7600 0000 7c01 7c00 6a00 7401 7c02 1900  v...|.|.j.t.|...
-00002ed0: 3c00 7c00 6a02 a003 7404 6a05 7c00 6a06  <.|.j...t.j.|.j.
-00002ee0: a007 6401 a101 7c02 9b00 6402 9d02 7c01  ..d...|...d...|.
-00002ef0: 6403 8d03 a101 0100 7c00 6a02 6404 1900  d.......|.j.d...
-00002f00: 6a08 7c00 6a09 6405 6405 6405 6406 8d04  j.|.j.d.d.d.d...
-00002f10: 0100 7c00 0400 6a09 6407 3700 0200 5f09  ..|...j.d.7..._.
-00002f20: 7c00 a00a 7c02 9b00 6408 7c01 9b00 9d03  |...|...d.|.....
-00002f30: 6409 a102 0100 6400 5300 290a 4e72 4400  d.....d.S.).NrD.
-00002f40: 0000 7a09 203c 3c20 636f 6c6f 7229 0272  ..z. << color).r
-00002f50: 1b00 0000 723b 0000 00e9 ffff ffff 7201  ....r;........r.
-00002f60: 0000 0072 1d00 0000 720d 0000 0072 cd00  ...r....r....r..
-00002f70: 0000 5429 0b72 9900 0000 7207 0000 0072  ..T).r....r....r
-00002f80: 9500 0000 da06 6170 7065 6e64 7256 0000  ......appendrV..
-00002f90: 0072 5800 0000 726f 0000 0072 7100 0000  .rX...ro...rq...
-00002fa0: 7257 0000 0072 9400 0000 72a8 0000 0029  rW...r....r....)
-00002fb0: 0372 7e00 0000 72a7 0000 0072 cc00 0000  .r~...r....r....
-00002fc0: 7281 0000 0072 8100 0000 7282 0000 0072  r....r....r....r
-00002fd0: d400 0000 6c02 0000 731c 0000 0002 030c  ....l...s.......
-00002fe0: ff06 0304 010a 0108 0102 0104 fd04 ff1a  ................
-00002ff0: 070e 0104 010e 0108 ff7a 1e4d 7947 7569  .........z.MyGui
-00003000: 2e65 7874 7261 6374 5f63 6f6c 6f72 5f66  .extract_color_f
-00003010: 726f 6d5f 6576 656e 7463 0100 0000 0000  rom_eventc......
-00003020: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00003030: 0000 f310 0000 007c 006a 00a0 01a1 007c  .......|.j.....|
-00003040: 005f 0264 0053 0072 c900 0000 2903 725c  ._.d.S.r....).r\
-00003050: 0000 0072 d300 0000 7288 0000 0072 7d00  ...r....r....r}.
-00003060: 0000 7281 0000 0072 8100 0000 7282 0000  ..r....r....r...
-00003070: 0072 5b00 0000 8102 0000 f302 0000 0010  .r[.............
-00003080: 017a 154d 7947 7569 2e63 6f6e 6469 7469  .z.MyGui.conditi
-00003090: 6f6e 5f65 7665 6e74 6301 0000 0000 0000  on_eventc.......
-000030a0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-000030b0: 0072 d700 0000 72c9 0000 0029 0372 6000  .r....r....).r`.
-000030c0: 0000 72d3 0000 0072 8900 0000 727d 0000  ..r....r....r}..
-000030d0: 0072 8100 0000 7281 0000 0072 8200 0000  .r....r....r....
-000030e0: 725f 0000 0087 0200 0072 d800 0000 7a1f  r_.......r....z.
-000030f0: 4d79 4775 692e 6469 7370 6c61 795f 7072  MyGui.display_pr
-00003100: 6566 6572 656e 6365 735f 6576 656e 7463  eferences_eventc
-00003110: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00003120: 0200 0000 4300 0000 72d7 0000 0072 c900  ....C...r....r..
-00003130: 0000 2903 7262 0000 0072 d300 0000 7290  ..).rb...r....r.
-00003140: 0000 0072 7d00 0000 7281 0000 0072 8100  ...r}...r....r..
-00003150: 0000 7282 0000 0072 6100 0000 8e02 0000  ..r....ra.......
-00003160: 72d8 0000 007a 124d 7947 7569 2e74 7769  r....z.MyGui.twi
-00003170: 7374 795f 6576 656e 7463 0100 0000 0000  sty_eventc......
-00003180: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00003190: 0000 72d7 0000 0072 c900 0000 2903 725e  ..r....r....).r^
-000031a0: 0000 0072 d300 0000 728a 0000 0072 7d00  ...r....r....r}.
-000031b0: 0000 7281 0000 0072 8100 0000 7282 0000  ..r....r....r...
-000031c0: 0072 5d00 0000 9402 0000 72d8 0000 007a  .r].......r....z
-000031d0: 1d4d 7947 7569 2e64 6973 706c 6179 5f74  .MyGui.display_t
-000031e0: 6173 6b65 726e 6574 5f65 7665 6e74 6301  askernet_eventc.
-000031f0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00003200: 0000 0003 0000 0073 3600 0000 8700 6601  .......s6.....f.
-00003210: 6401 6402 8408 7400 4400 8301 7d01 7401  d.d...t.D...}.t.
-00003220: 7c01 8800 6a02 6403 8303 5c02 7d01 8800  |...j.d...\.}...
-00003230: 5f02 8800 a003 6404 6403 a102 0100 6400  _.....d.d.....d.
-00003240: 5300 2905 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00003250: 0000 0200 0000 0600 0000 1300 0000 7318  ..............s.
-00003260: 0000 0069 007c 005d 087d 017c 0174 0088  ...i.|.].}.|.t..
-00003270: 007c 0183 0293 0271 0253 0072 8100 0000  .|.....q.S.r....
-00003280: 2901 da07 6765 7461 7474 7229 02da 022e  )...getattr)....
-00003290: 30da 0576 616c 7565 727d 0000 0072 8100  0..valuer}...r..
-000032a0: 0000 7282 0000 00da 0a3c 6469 6374 636f  ..r......<dictco
-000032b0: 6d70 3e9c 0200 0073 0200 0000 1800 7a2d  mp>....s......z-
-000032c0: 4d79 4775 692e 7361 7665 5f73 6574 7469  MyGui.save_setti
-000032d0: 6e67 735f 6576 656e 742e 3c6c 6f63 616c  ngs_event.<local
-000032e0: 733e 2e3c 6469 6374 636f 6d70 3e54 7a0f  s>.<dictcomp>Tz.
-000032f0: 5365 7474 696e 6773 2073 6176 6564 2e29  Settings saved.)
-00003300: 0472 0800 0000 7204 0000 0072 9900 0000  .r....r....r....
-00003310: 72a8 0000 00a9 0272 7e00 0000 da09 7465  r......r~.....te
-00003320: 6d70 5f61 7267 7372 8100 0000 727d 0000  mp_argsr....r}..
-00003330: 0072 8200 0000 7263 0000 009a 0200 0073  .r....rc.......s
-00003340: 0a00 0000 1202 0203 0801 0aff 1003 7a19  ..............z.
-00003350: 4d79 4775 692e 7361 7665 5f73 6574 7469  MyGui.save_setti
-00003360: 6e67 735f 6576 656e 7463 0300 0000 0000  ngs_eventc......
-00003370: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
-00003380: 0000 73fc 0100 0064 017d 037c 0104 0064  ..s....d.}.|...d
-00003390: 026b 0272 1f01 007c 0272 107c 006a 00a0  .k.r...|.r.|.j..
-000033a0: 01a1 0001 006e 057c 006a 00a0 02a1 0001  .....n.|.j......
-000033b0: 0064 0374 037c 0283 019b 0064 049d 037d  .d.t.|.....d...}
-000033c0: 037c 0353 0004 0064 056b 0272 3601 007c  .|.S...d.k.r6..|
-000033d0: 006a 04a0 0574 037c 0283 01a1 0101 0064  .j...t.|.......d
-000033e0: 0674 037c 0283 019b 0064 049d 037d 037c  .t.|.....d...}.|
-000033f0: 0353 0004 0064 076b 0272 5001 007c 0272  .S...d.k.rP..|.r
-00003400: 437c 006a 06a0 01a1 0001 006e 057c 006a  C|.j.......n.|.j
-00003410: 06a0 02a1 0001 0064 087c 029b 0064 049d  .......d.|...d..
-00003420: 037d 037c 0353 0004 0064 096b 0272 6a01  .}.|.S...d.k.rj.
-00003430: 007c 0272 5d7c 006a 07a0 01a1 0001 006e  .|.r]|.j.......n
-00003440: 057c 006a 07a0 02a1 0001 0064 0a7c 029b  .|.j.......d.|..
-00003450: 0064 049d 037d 037c 0353 0004 0064 0b6b  .d...}.|.S...d.k
-00003460: 0272 8401 007c 0272 777c 006a 08a0 01a1  .r...|.rw|.j....
-00003470: 0001 006e 057c 006a 08a0 02a1 0001 0064  ...n.|.j.......d
-00003480: 0c7c 029b 0064 049d 037d 037c 0353 0004  .|...d...}.|.S..
-00003490: 0064 0d6b 0272 9301 007c 0272 9164 0e7c  .d.k.r...|.r.d.|
-000034a0: 029b 0064 049d 037d 037c 0353 0004 0064  ...d...}.|.S...d
-000034b0: 0f6b 0272 a201 007c 0272 a064 107c 029b  .k.r...|.r.d.|..
-000034c0: 0064 049d 037d 037c 0353 0004 0064 116b  .d...}.|.S...d.k
-000034d0: 0272 b101 007c 0272 af64 127c 029b 0064  .r...|.r.d.|...d
-000034e0: 049d 037d 037c 0353 0004 0064 136b 0272  ...}.|.S...d.k.r
-000034f0: c001 007c 0272 be64 147c 029b 0064 159d  ...|.r.d.|...d..
-00003500: 037d 037c 0353 0004 0064 166b 0272 cf01  .}.|.S...d.k.r..
-00003510: 007c 0272 cd64 177c 029b 0064 159d 037d  .|.r.d.|...d...}
-00003520: 037c 0353 0004 0064 186b 0272 e901 007c  .|.S...d.k.r...|
-00003530: 0272 dc7c 006a 09a0 01a1 0001 006e 057c  .r.|.j.......n.|
-00003540: 006a 09a0 02a1 0001 0064 197c 029b 0064  .j.......d.|...d
-00003550: 159d 037d 037c 0353 0064 1a6b 0272 ef09  ...}.|.S.d.k.r..
-00003560: 007c 0353 0009 007c 00a0 0a64 1b7c 019b  .|.S...|...d.|..
-00003570: 0064 1c7c 029b 009d 0464 1da1 0201 007c  .d.|.....d.....|
-00003580: 0353 0029 1e4e 7284 0000 0072 8b00 0000  .S.).Nr....r....
-00003590: 7a0d 4465 6275 6720 7365 7420 746f 207a  z.Debug set to z
-000035a0: 022e 0a72 8700 0000 7a1c 4469 7370 6c61  ...r....z.Displa
-000035b0: 7920 4465 7461 696c 204c 6576 656c 2073  y Detail Level s
-000035c0: 6574 2074 6f20 7288 0000 007a 1a44 6973  et to r....z.Dis
-000035d0: 706c 6179 2043 6f6e 6469 7469 6f6e 7320  play Conditions 
-000035e0: 7365 7420 746f 2072 8900 0000 7a22 4469  set to r....z"Di
-000035f0: 7370 6c61 7920 5461 736b 6572 2050 7265  splay Tasker Pre
-00003600: 6665 7265 6e63 6573 2073 6574 2074 6f20  ferences set to 
-00003610: 728a 0000 007a 1944 6973 706c 6179 2054  r....z.Display T
-00003620: 6173 6b65 724e 6574 2073 6574 2074 6f20  askerNet set to 
-00003630: 7291 0000 007a 0f50 726f 6a65 6374 2073  r....z.Project s
-00003640: 6574 2074 6f20 7292 0000 007a 0f50 726f  et to r....z.Pro
-00003650: 6669 6c65 2073 6574 2074 6f20 7293 0000  file set to r...
-00003660: 007a 0c54 6173 6b20 7365 7420 746f 2072  .z.Task set to r
-00003670: 9a00 0000 7a1d 4765 7420 4261 636b 7570  ....z.Get Backup
-00003680: 2049 5020 4164 6472 6573 7320 7365 7420   IP Address set 
-00003690: 746f 2072 a100 0000 729c 0000 007a 2047  to r....r....z G
-000036a0: 6574 2042 6163 6b75 7020 4669 6c65 204c  et Backup File L
-000036b0: 6f63 6174 696f 6e20 7365 7420 746f 2072  ocation set to r
-000036c0: 9000 0000 7a0e 5477 6973 7479 2073 6574  ....z.Twisty set
-000036d0: 2074 6f20 728f 0000 007a 2152 7574 726f   to r....z!Rutro
-000036e0: 6821 2020 556e 6465 6669 6e65 6420 6172  h!  Undefined ar
-000036f0: 6775 6d65 6e74 3a20 6b65 793d 7a07 2076  gument: key=z. v
-00003700: 616c 7565 3d46 290b 727a 0000 00da 0673  alue=F).rz.....s
-00003710: 656c 6563 7472 c100 0000 da03 7374 7272  electr......strr
-00003720: 5a00 0000 7286 0000 0072 5c00 0000 7260  Z...r....r\...r`
-00003730: 0000 0072 5e00 0000 7262 0000 0072 a800  ...r^...rb...r..
-00003740: 0000 2904 727e 0000 00da 036b 6579 72db  ..).r~.....keyr.
-00003750: 0000 0072 a600 0000 7281 0000 0072 8100  ...r....r....r..
-00003760: 0000 7282 0000 00da 0f72 6573 746f 7265  ..r......restore
-00003770: 5f64 6973 706c 6179 a702 0000 7380 0000  _display....s...
-00003780: 0004 0102 010a 0104 010c 010a 0210 0104  ................
-00003790: 310a d010 0110 0104 2e0a d304 010c 010a  1...............
-000037a0: 020c 0104 280a d904 010c 010a 020c 0104  ....(...........
-000037b0: 220a df04 010c 010a 020c 0104 1c0a e504  "...............
-000037c0: 010c 0104 190a e804 010c 0104 160a eb04  ................
-000037d0: 010c 0104 130a ee04 010c 0104 100a f104  ................
-000037e0: 010c 0104 0d0a f404 010c 010a 020c 0104  ................
-000037f0: 0706 fa02 0104 0502 fc04 0110 0104 ff04  ................
-00003800: 037a 154d 7947 7569 2e72 6573 746f 7265  .z.MyGui.restore
-00003810: 5f64 6973 706c 6179 6301 0000 0000 0000  _displayc.......
-00003820: 0000 0000 0002 0000 0008 0000 0043 0000  .............C..
-00003830: 0073 ac00 0000 7c00 a000 6401 a101 0100  .s....|...d.....
-00003840: 6900 0400 7d01 7c00 5f01 7402 7c01 7c00  i...}.|._.t.|.|.
-00003850: 6a01 6401 8303 5c02 7d01 7c00 5f01 7403  j.d...\.}.|._.t.
-00003860: a004 7405 a101 8f21 0100 7c01 6402 1900  ..t....!..|.d...
-00003870: 7233 7c00 a006 7c01 6402 1900 6401 a102  r3|...|.d...d...
-00003880: 0100 6403 7c01 6402 3c00 0900 5700 6400  ..d.|.d.<...W.d.
-00003890: 0400 0400 8303 0100 6400 5300 5700 6400  ........d.S.W.d.
-000038a0: 0400 0400 8303 0100 6e08 3100 733d 7701  ........n.1.s=w.
-000038b0: 0100 0100 0100 5900 0100 7c01 7347 7c00  ......Y...|.sG|.
-000038c0: 6a01 724e 7c00 a007 7c01 a101 0100 6400  j.rN|...|.....d.
-000038d0: 5300 7c00 a006 6404 6401 a102 0100 6400  S.|...d.d.....d.
-000038e0: 5300 2905 4e46 da03 6d73 6772 8400 0000  S.).NF..msgr....
-000038f0: 7a17 4e6f 2073 6574 7469 6e67 7320 6669  z.No settings fi
-00003900: 6c65 2066 6f75 6e64 2e29 0872 7c00 0000  le found.).r|...
-00003910: 7299 0000 0072 0400 0000 72ce 0000 0072  r....r....r....r
-00003920: cf00 0000 da08 4b65 7945 7272 6f72 72a8  ......KeyErrorr.
-00003930: 0000 00da 1065 7874 7261 6374 5f73 6574  .....extract_set
-00003940: 7469 6e67 7372 dd00 0000 7281 0000 0072  tingsr....r....r
-00003950: 8100 0000 7282 0000 0072 6400 0000 e502  ....r....rd.....
-00003960: 0000 7320 0000 000a 010a 0102 0208 010a  ..s ............
-00003970: ff0c 0408 0110 0108 0102 0110 fc02 011c  ................
-00003980: ff0a 060e 0110 027a 1c4d 7947 7569 2e72  .......z.MyGui.r
-00003990: 6573 746f 7265 5f73 6574 7469 6e67 735f  estore_settings_
-000039a0: 6576 656e 7472 de00 0000 da06 7265 7475  eventr......retu
-000039b0: 726e 4e63 0200 0000 0000 0000 0000 0000  rnNc............
-000039c0: 0700 0000 0700 0000 4300 0000 73b6 0000  ........C...s...
-000039d0: 0064 015c 027d 027d 037c 01a0 00a1 0044  .d.\.}.}.|.....D
-000039e0: 005d 1a5c 027d 047d 057c 0464 0075 0172  .].\.}.}.|.d.u.r
-000039f0: 2274 017c 007c 047c 0583 0301 007c 00a0  "t.|.|.|.....|..
-00003a00: 027c 047c 05a1 0204 007d 0372 227c 027c  .|.|.....}.r"|.|
-00003a10: 0317 007d 0271 0864 0264 0384 0074 03a0  ...}.q.d.d...t..
-00003a20: 00a1 0044 0083 017d 067c 006a 04a0 00a1  ...D...}.|.j....
-00003a30: 0044 005d 1e5c 027d 047d 057c 0464 0075  .D.].\.}.}.|.d.u
-00003a40: 0172 4f7c 0464 046b 0272 4264 057c 067c  .rO|.d.k.rBd.|.|
-00003a50: 043c 0071 317c 029b 0064 067c 067c 0419  .<.q1|...d.|.|..
-00003a60: 009b 0064 077c 059b 0064 089d 067d 0271  ...d.|...d...}.q
-00003a70: 317c 00a0 057c 029b 0064 099d 0264 0aa1  1|...|...d...d..
-00003a80: 0201 0064 0053 0029 0b4e 2902 7284 0000  ...d.S.).N).r...
-00003a90: 0072 8400 0000 6301 0000 0000 0000 0000  .r....c.........
-00003aa0: 0000 0003 0000 0004 0000 0053 0000 0073  ...........S...s
-00003ab0: 1600 0000 6900 7c00 5d07 5c02 7d01 7d02  ....i.|.].\.}.}.
-00003ac0: 7c02 7c01 9302 7102 5300 7281 0000 0072  |.|...q.S.r....r
-00003ad0: 8100 0000 2903 72da 0000 00da 016b da01  ....).r......k..
-00003ae0: 7672 8100 0000 7281 0000 0072 8200 0000  vr....r....r....
-00003af0: 72dc 0000 0003 0300 0073 0200 0000 1600  r........s......
-00003b00: 7a2a 4d79 4775 692e 6578 7472 6163 745f  z*MyGui.extract_
-00003b10: 7365 7474 696e 6773 2e3c 6c6f 6361 6c73  settings.<locals
-00003b20: 3e2e 3c64 6963 7463 6f6d 703e 72e3 0000  >.<dictcomp>r...
-00003b30: 0072 8400 0000 da01 207a 0e20 636f 6c6f  .r...... z. colo
-00003b40: 7220 7365 7420 746f 2072 a100 0000 7a13  r set to r....z.
-00003b50: 0a53 6574 7469 6e67 7320 7265 7374 6f72  .Settings restor
-00003b60: 6564 2e54 2906 da05 6974 656d 73da 0773  ed.T)...items..s
-00003b70: 6574 6174 7472 72e2 0000 0072 0700 0000  etattrr....r....
-00003b80: 7299 0000 0072 a800 0000 2907 727e 0000  r....r....).r~..
-00003b90: 0072 de00 0000 5a0c 616c 6c5f 6d65 7373  .r....Z.all_mess
-00003ba0: 6167 6573 5a0b 6e65 775f 6d65 7373 6167  agesZ.new_messag
-00003bb0: 6572 e100 0000 72db 0000 005a 0f69 6e76  er....r....Z.inv
-00003bc0: 5f63 6f6c 6f72 5f6e 616d 6573 7281 0000  _color_namesr...
-00003bd0: 0072 8100 0000 7282 0000 0072 e500 0000  .r....r....r....
-00003be0: fb02 0000 7320 0000 0008 0110 0108 010c  ....s ..........
-00003bf0: 0110 0108 0102 8012 0212 0108 0108 010a  ................
-00003c00: 0118 0302 ff02 8016 057a 164d 7947 7569  .........z.MyGui
-00003c10: 2e65 7874 7261 6374 5f73 6574 7469 6e67  .extract_setting
-00003c20: 7363 0100 0000 0000 0000 0000 0000 0700  sc..............
-00003c30: 0000 0600 0000 4300 0000 7356 0100 007c  ......C...sV...|
-00003c40: 006a 0064 016b 0272 0864 027c 005f 007c  .j.d.k.r.d.|._.|
-00003c50: 006a 0173 0e64 037c 005f 0174 026a 0364  .j.s.d.|._.t.j.d
-00003c60: 047c 006a 009b 0064 057c 006a 019b 009d  .|.j...d.|.j....
-00003c70: 0464 0664 078d 027d 017c 01a0 04a1 0004  .d.d...}.|......
-00003c80: 007d 0273 2b7c 00a0 0564 0864 09a1 0201  .}.s+|...d.d....
-00003c90: 0064 0053 007c 0264 0a6b 0372 9b7c 02a0  .d.S.|.d.k.r.|..
-00003ca0: 0664 05a1 017d 037c 0364 0b19 00a0 0664  .d...}.|.d.....d
-00003cb0: 0ca1 017d 047c 0464 0b19 00a0 0664 0da1  ...}.|.d.....d..
-00003cc0: 017d 0574 077c 0583 0164 0e6b 0072 567c  .}.t.|...d.k.rV|
-00003cd0: 00a0 0564 0f7c 0464 0b19 009b 0064 109d  ...d.|.d.....d..
-00003ce0: 0364 09a1 0201 0064 0053 007c 0564 0b19  .d.....d.S.|.d..
-00003cf0: 0044 005d 157d 067c 06a0 08a1 0073 6f7c  .D.].}.|.....so|
-00003d00: 00a0 0564 0f7c 0464 0b19 009b 0064 109d  ...d.|.d.....d..
-00003d10: 0364 09a1 0201 0001 0064 0053 0071 5a7c  .d.......d.S.qZ|
-00003d20: 0564 1119 006a 0873 837c 00a0 0564 127c  .d...j.s.|...d.|
-00003d30: 0564 1119 009b 0064 109d 0364 09a1 0201  .d.....d...d....
-00003d40: 0064 0053 0074 077c 0383 0164 136b 0072  .d.S.t.|...d.k.r
-00003d50: 917c 00a0 0564 1464 09a1 0201 0064 0053  .|...d.d.....d.S
-00003d60: 007c 0364 0b19 007c 005f 007c 0364 1119  .|.d...|._.|.d..
-00003d70: 007c 005f 017c 00a0 0564 157c 006a 009b  .|._.|...d.|.j..
-00003d80: 0064 167c 006a 019b 009d 0464 17a1 0201  .d.|.j.....d....
-00003d90: 0064 0053 0029 184e 7284 0000 007a 1231  .d.S.).Nr....z.1
-00003da0: 3932 2e31 3638 2e30 2e32 3130 3a31 3832  92.168.0.210:182
-00003db0: 317a 1f2f 5461 736b 6572 2f63 6f6e 6669  1z./Tasker/confi
-00003dc0: 6773 2f75 7365 722f 6261 636b 7570 2e78  gs/user/backup.x
-00003dd0: 6d6c 7a80 456e 7465 7220 4950 2041 6464  mlz.Enter IP Add
-00003de0: 7265 7373 2c20 506f 7274 204e 756d 6265  ress, Port Numbe
-00003df0: 7220 616e 6420 4669 6c65 204c 6f63 6174  r and File Locat
-00003e00: 696f 6e2c 2069 6e20 7468 6520 666f 6c6c  ion, in the foll
-00003e10: 6f77 696e 6720 666f 726d 6174 3a20 6970  owing format: ip
-00003e20: 5f61 6464 7265 7373 3a70 6f72 742c 6669  _address:port,fi
-00003e30: 6c65 5f6c 6f63 6174 696f 6e0a 456e 7465  le_location.Ente
-00003e40: 7220 272a 2720 666f 7220 6465 6661 756c  r '*' for defaul
-00003e50: 7473 3a20 fa01 2c72 3a00 0000 72c0 0000  ts: ..,r:...r...
-00003e60: 007a 3847 6574 2042 6163 6b75 7020 5365  .z8Get Backup Se
-00003e70: 7474 696e 6773 2e2e 2e6e 6f74 6869 6e67  ttings...nothing
-00003e80: 2065 6e74 6572 6564 2e20 204e 6f20 6163   entered.  No ac
-00003e90: 7469 6f6e 2074 616b 656e 2e46 da01 2a72  tion taken.F..*r
-00003ea0: 0100 0000 fa01 3ada 012e 722c 0000 007a  ......:...r,...z
-00003eb0: 1449 6e76 616c 6964 2049 5020 4164 6472  .Invalid IP Addr
-00003ec0: 6573 733a 207a 0d2e 2020 5472 7920 6167  ess: z..  Try ag
-00003ed0: 6169 6e2e 720d 0000 007a 1549 6e76 616c  ain.r....z.Inval
-00003ee0: 6964 2070 6f72 7420 6e75 6d62 6572 3a20  id port number: 
-00003ef0: 720f 0000 007a 2546 696c 6520 6c6f 6361  r....z%File loca
-00003f00: 7469 6f6e 2069 7320 6d69 7373 696e 672e  tion is missing.
-00003f10: 2020 5472 7920 6167 6169 6e2e 7a1e 4765    Try again.z.Ge
-00003f20: 7420 4261 636b 7570 2049 5020 4164 6472  t Backup IP Addr
-00003f30: 6573 7320 7365 7420 746f 3a20 7a16 0a47  ess set to: z..G
-00003f40: 6574 204c 6f63 6174 696f 6e20 7365 7420  et Location set 
-00003f50: 746f 3a20 5429 0972 9a00 0000 729c 0000  to: T).r....r...
-00003f60: 0072 5600 0000 72c2 0000 0072 c400 0000  .rV...r....r....
-00003f70: 72a8 0000 00da 0573 706c 6974 da03 6c65  r......split..le
-00003f80: 6eda 0769 7364 6967 6974 2907 727e 0000  n..isdigit).r~..
-00003f90: 0072 c600 0000 5a0b 6261 636b 7570 5f69  .r....Z.backup_i
-00003fa0: 6e66 6f5a 0974 656d 705f 696e 666f 5a07  nfoZ.temp_infoZ.
-00003fb0: 7465 6d70 5f69 705a 0b74 656d 705f 6970  temp_ipZ.temp_ip
-00003fc0: 6164 6472 72be 0000 0072 8100 0000 7281  addrr....r....r.
-00003fd0: 0000 0072 8200 0000 7268 0000 0013 0300  ...r....rh......
-00003fe0: 0073 7000 0000 0a02 0601 0601 0601 0402  .sp.............
-00003ff0: 0202 0403 04fd 0403 04fd 0205 06f9 0c0b  ................
-00004000: 0401 0201 0201 04fe 0404 0803 0a02 0e01  ................
-00004010: 0e03 0c01 0401 0e01 0201 04fe 0404 0c01  ................
-00004020: 0801 0401 0e01 0201 04fe 0604 02fb 0a08  ................
-00004030: 0401 0e01 0201 04fe 0404 0c03 0401 0201  ................
-00004040: 0201 04fe 0404 0a03 0a01 0402 0a02 0401  ................
-00004050: 04ff 0203 08fb 7a16 4d79 4775 692e 6765  ......z.MyGui.ge
-00004060: 745f 6261 636b 7570 5f65 7665 6e74 6301  t_backup_eventc.
-00004070: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00004080: 0000 0043 0000 0073 9800 0000 7c00 6a00  ...C...s....|.j.
-00004090: a001 6401 a101 0100 7c00 6a02 a003 a100  ..d.....|.j.....
-000040a0: 0100 7c00 6a04 a003 a100 0100 7c00 6a05  ..|.j.......|.j.
-000040b0: a003 a100 0100 7c00 6a06 a001 6402 a101  ......|.j...d...
-000040c0: 0100 7407 a008 6402 a101 0100 7c00 6a09  ..t...d.....|.j.
-000040d0: a003 a100 0100 7c00 a00a 6403 6404 a102  ......|...d.d...
-000040e0: 0100 7c00 6a0b a003 a100 0100 6405 0400  ..|.j.......d...
-000040f0: 7c00 5f0c 7c00 5f0d 7c00 6a0e 7245 7c00  |._.|._.|.j.rE|.
-00004100: 6a0e 4400 5d08 7d01 7c01 6a0f 6405 6406  j.D.].}.|.j.d.d.
-00004110: 8d01 0100 713c 7c00 a010 6407 a101 0100  ....q<|...d.....
-00004120: 6400 5300 2908 4e72 2400 0000 720b 0000  d.S.).Nr$...r...
-00004130: 007a 0f53 6574 7469 6e67 7320 7265 7365  .z.Settings rese
-00004140: 742e 5472 8400 0000 7245 0000 0046 2911  t.Tr....rE...F).
-00004150: 725a 0000 0072 8600 0000 725c 0000 0072  rZ...r....r\...r
-00004160: c100 0000 7260 0000 0072 5e00 0000 7266  ....r`...r^...rf
-00004170: 0000 0072 5600 0000 72ca 0000 0072 7a00  ...rV...r....rz.
-00004180: 0000 72a8 0000 0072 6200 0000 729c 0000  ..r....rb...r...
-00004190: 0072 9a00 0000 7295 0000 0072 6e00 0000  .r....r....rn...
-000041a0: 727c 0000 0029 0272 7e00 0000 da05 6c61  r|...).r~.....la
-000041b0: 6265 6c72 8100 0000 7281 0000 0072 8200  belr....r....r..
-000041c0: 0000 7267 0000 0061 0300 0073 1c00 0000  ..rg...a...s....
-000041d0: 0c01 0a01 0a01 0a01 0c01 0a01 0a01 0c01  ................
-000041e0: 0a01 0c01 0601 0a01 0e01 0e01 7a1a 4d79  ............z.My
-000041f0: 4775 692e 7265 7365 745f 7365 7474 696e  Gui.reset_settin
-00004200: 6773 5f65 7665 6e74 6301 0000 0000 0000  gs_eventc.......
-00004210: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00004220: 0073 5400 0000 7c00 6a00 a001 a100 7c00  .sT...|.j.....|.
-00004230: 5f02 7c00 6a02 7222 7403 6401 8301 a004  _.|.j.r"t.d.....
-00004240: a100 7217 7c00 a005 6402 6403 a102 0100  ..r.|...d.d.....
-00004250: 6400 5300 7c00 a005 6404 6405 a102 0100  d.S.|...d.d.....
-00004260: 6405 7c00 5f02 6400 5300 7c00 a005 6406  d.|._.d.S.|...d.
-00004270: 6403 a102 0100 6400 5300 2907 4e72 af00  d.....d.S.).Nr..
-00004280: 0000 7a13 4465 6275 6720 6d6f 6465 2065  ..z.Debug mode e
-00004290: 6e61 626c 6564 2e54 7a53 4465 6275 6720  nabled.TzSDebug 
-000042a0: 6d6f 6465 2072 6571 7569 7265 7320 5461  mode requires Ta
-000042b0: 736b 6572 2062 6163 6b75 7020 6669 6c65  sker backup file
-000042c0: 2074 6f20 6265 206e 616d 6564 3a20 2762   to be named: 'b
-000042d0: 6163 6b75 702e 786d 6c27 2c20 7768 6963  ackup.xml', whic
-000042e0: 6820 6973 206d 6973 7369 6e67 2146 7a14  h is missing!Fz.
-000042f0: 4465 6275 6720 6d6f 6465 2064 6973 6162  Debug mode disab
-00004300: 6c65 642e 2906 727a 0000 0072 d300 0000  led.).rz...r....
-00004310: 728b 0000 0072 0200 0000 da07 6973 5f66  r....r......is_f
-00004320: 696c 6572 a800 0000 727d 0000 0072 8100  iler....r}...r..
-00004330: 0000 7281 0000 0072 8200 0000 7279 0000  ..r....r....ry..
-00004340: 0074 0300 0073 1400 0000 0c01 0601 0c01  .t...s..........
-00004350: 1001 0402 0202 0203 04fb 0a07 1002 7a1a  ..............z.
-00004360: 4d79 4775 692e 6465 6275 675f 6368 6563  MyGui.debug_chec
-00004370: 6b62 6f78 5f65 7665 6e74 6301 0000 0000  kbox_eventc.....
-00004380: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00004390: 0000 00f3 1200 0000 6401 7c00 5f00 7c00  ........d.|._.|.
-000043a0: a001 a100 0100 6400 5300 a902 4e54 2902  ......d.S...NT).
-000043b0: 728e 0000 00da 0471 7569 7472 7d00 0000  r......quitr}...
-000043c0: 7281 0000 0072 8100 0000 7282 0000 0072  r....r....r....r
-000043d0: 6900 0000 8803 0000 f304 0000 0006 010c  i...............
-000043e0: 017a 114d 7947 7569 2e72 756e 5f70 726f  .z.MyGui.run_pro
-000043f0: 6772 616d 6301 0000 0000 0000 0000 0000  gramc...........
-00004400: 0001 0000 0002 0000 0043 0000 0073 1a00  .........C...s..
-00004410: 0000 6401 7c00 5f00 7c00 a001 a100 0100  ..d.|._.|.......
-00004420: 7c00 a002 a100 0100 6400 5300 72f6 0000  |.......d.S.r...
-00004430: 0029 0372 8f00 0000 da08 7769 7468 6472  .).r......withdr
-00004440: 6177 72f7 0000 0072 7d00 0000 7281 0000  awr....r}...r...
-00004450: 0072 8100 0000 7282 0000 0072 6a00 0000  .r....r....rj...
-00004460: 8f03 0000 7306 0000 0006 0108 020c 017a  ....s..........z
-00004470: 174d 7947 7569 2e72 6572 756e 5f74 6865  .MyGui.rerun_the
-00004480: 5f70 726f 6772 616d 6301 0000 0000 0000  _programc.......
-00004490: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-000044a0: 0072 f500 0000 72f6 0000 0029 0272 8d00  .r....r....).r..
-000044b0: 0000 72f7 0000 0072 7d00 0000 7281 0000  ..r....r}...r...
-000044c0: 0072 8100 0000 7282 0000 0072 6b00 0000  .r....r....rk...
-000044d0: 9803 0000 72f8 0000 007a 124d 7947 7569  ....r....z.MyGui
-000044e0: 2e65 7869 745f 7072 6f67 7261 6d29 21da  .exit_program)!.
-000044f0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00004500: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00004510: 655f 5f72 5100 0000 da04 626f 6f6c 727c  e__rQ.....boolr|
-00004520: 0000 0072 a800 0000 72ad 0000 0072 a900  ...r....r....r..
-00004530: 0000 7272 0000 0072 7400 0000 7276 0000  ..rr...rt...rv..
-00004540: 0072 e000 0000 7265 0000 0072 5900 0000  .r....re...rY...
-00004550: 7278 0000 0072 d400 0000 725b 0000 0072  rx...r....r[...r
-00004560: 5f00 0000 7261 0000 0072 5d00 0000 7263  _...ra...r]...rc
-00004570: 0000 0072 e200 0000 7264 0000 00da 0464  ...r....rd.....d
-00004580: 6963 7472 e500 0000 7268 0000 0072 6700  ictr....rh...rg.
-00004590: 0000 7279 0000 0072 6900 0000 726a 0000  ..ry...ri...rj..
-000045a0: 0072 6b00 0000 da0d 5f5f 636c 6173 7363  .rk.....__classc
-000045b0: 656c 6c5f 5f72 8100 0000 7281 0000 0072  ell__r....r....r
-000045c0: 7f00 0000 7282 0000 0072 0c00 0000 4600  ....r....r....F.
-000045d0: 0000 733a 0000 0008 000c 0100 7f00 7f0e  ..s:............
-000045e0: 1c08 2608 1408 3308 2d08 1408 140e 140e  ..&...3.-.......
-000045f0: 070e 0708 2708 1508 0608 0708 0608 0608  ....'...........
-00004600: 0d08 3e12 1608 1808 4e08 1308 1408 0710  ..>.....N.......
-00004610: 0972 0c00 0000 2919 72ce 0000 0072 5600  .r....).r....rV.
-00004620: 0000 da07 7061 7468 6c69 6272 0200 0000  ....pathlibr....
-00004630: 5a1f 4354 6b43 6f6c 6f72 5069 636b 6572  Z.CTkColorPicker
-00004640: 2e63 746b 5f63 6f6c 6f72 5f70 6963 6b65  .ctk_color_picke
-00004650: 7272 0300 0000 da17 6d61 7074 6173 6b65  rr......maptaske
-00004660: 722e 7372 632e 6765 7470 7574 6172 6772  r.src.getputargr
-00004670: 0400 0000 da16 6d61 7074 6173 6b65 722e  ......maptasker.
-00004680: 7372 632e 7072 6f67 696e 6974 7205 0000  src.proginitr...
-00004690: 00da 166d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
-000046a0: 2e69 6e69 7470 6172 6772 0600 0000 da16  .initpargr......
-000046b0: 6d61 7074 6173 6b65 722e 7372 632e 7379  maptasker.src.sy
-000046c0: 7363 6f6e 7374 7207 0000 0072 0800 0000  sconstr....r....
-000046d0: da16 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
-000046e0: 636f 6c72 6d6f 6465 7209 0000 00da 156d  colrmoder......m
-000046f0: 6170 7461 736b 6572 2e73 7263 2e6c 696e  aptasker.src.lin
-00004700: 656f 7574 720a 0000 0072 ca00 0000 5a17  eoutr....r....Z.
-00004710: 7365 745f 6465 6661 756c 745f 636f 6c6f  set_default_colo
-00004720: 725f 7468 656d 6572 9800 0000 72c3 0000  r_themer....r...
-00004730: 005a 0343 546b 720c 0000 0072 8100 0000  .Z.CTkr....r....
-00004740: 7281 0000 0072 8100 0000 7282 0000 00da  r....r....r.....
-00004750: 083c 6d6f 6475 6c65 3e01 0000 0073 2200  .<module>....s".
-00004760: 0000 0812 0801 0c01 0c01 0c01 0c01 0c01  ................
-00004770: 0c01 0c01 0c01 0c01 0a03 0a02 0203 02ff  ................
-00004780: 041c 1606                                ....
+00001ce0: 007c 005f 1864 007c 005f 197a 067c 006a  .|._.d.|._.z.|.j
+00001cf0: 1a72 5e09 0057 006e 0c04 0074 1b79 6b01  .r^..W.n...t.yk.
+00001d00: 0001 0001 0064 067c 005f 1a59 006e 0177  .....d.|._.Y.n.w
+00001d10: 007a 0a7c 006a 1c72 7409 0057 0064 0053  .z.|.j.rt..W.d.S
+00001d20: 0057 0064 0053 0004 0074 1b79 8301 0001  .W.d.S...t.y....
+00001d30: 0001 0064 067c 005f 1c59 0064 0053 0077  ...d.|._.Y.d.S.w
+00001d40: 0029 0b4e 7222 0000 0029 0172 2700 0000  .).Nr"...).r'...
+00001d50: 7226 0000 0072 1000 0000 46da 0072 0f00  r&...r....F..r..
+00001d60: 0000 720b 0000 00fa 0330 2e30 7a10 4d61  ..r......0.0z.Ma
+00001d70: 7054 6173 6b65 7220 4865 6c70 0a0a 291d  pTasker Help..).
+00001d80: 725a 0000 0072 6e00 0000 da03 7365 74da  rZ...rn.....set.
+00001d90: 1464 6973 706c 6179 5f64 6574 6169 6c5f  .display_detail_
+00001da0: 6c65 7665 6cda 1a64 6973 706c 6179 5f70  level..display_p
+00001db0: 726f 6669 6c65 5f63 6f6e 6469 7469 6f6e  rofile_condition
+00001dc0: 73da 1364 6973 706c 6179 5f70 7265 6665  s..display_prefe
+00001dd0: 7265 6e63 6573 da11 6469 7370 6c61 795f  rences..display_
+00001de0: 7461 736b 6572 6e65 74da 0564 6562 7567  taskernet..debug
+00001df0: 5a0e 636c 6561 725f 7365 7474 696e 6773  Z.clear_settings
+00001e00: da05 7265 7365 74da 0465 7869 74da 0a67  ..reset..exit..g
+00001e10: 6f5f 7072 6f67 7261 6dda 0572 6572 756e  o_program..rerun
+00001e20: da06 7477 6973 7479 da13 7369 6e67 6c65  ..twisty..single
+00001e30: 5f70 726f 6a65 6374 5f6e 616d 65da 1373  _project_name..s
+00001e40: 696e 676c 655f 7072 6f66 696c 655f 6e61  ingle_profile_na
+00001e50: 6d65 da10 7369 6e67 6c65 5f74 6173 6b5f  me..single_task_
+00001e60: 6e61 6d65 da0e 636f 6c6f 725f 7465 7874  name..color_text
+00001e70: 5f72 6f77 7266 0000 00da 0c63 6f6c 6f72  _rowrf.....color
+00001e80: 5f6c 6162 656c 73da 0f61 7070 6561 7261  _labels..appeara
+00001e90: 6e63 655f 6d6f 6465 726d 0000 00da 0669  nce_moderm.....i
+00001ea0: 6e73 6572 74da 0949 4e46 4f5f 5445 5854  nsert..INFO_TEXT
+00001eb0: da0c 636f 6c6f 725f 6c6f 6f6b 7570 da04  ..color_lookup..
+00001ec0: 6669 6c65 da10 6261 636b 7570 5f66 696c  file..backup_fil
+00001ed0: 655f 6874 7470 da0e 4174 7472 6962 7574  e_http..Attribut
+00001ee0: 6545 7272 6f72 da14 6261 636b 7570 5f66  eError..backup_f
+00001ef0: 696c 655f 6c6f 6361 7469 6f6e 2902 727e  ile_location).r~
+00001f00: 0000 0072 8300 0000 7281 0000 0072 8100  ...r....r....r..
+00001f10: 0000 7282 0000 0072 7c00 0000 6101 0000  ..r....r|...a...
+00001f20: 7356 0000 0012 020c 0106 0102 0908 f804  sV..............
+00001f30: 0102 ff04 0302 fd04 0502 fb04 0702 f904  ................
+00001f40: 0802 f804 0802 f804 0802 f808 0812 0106  ................
+00001f50: 010c 0106 0106 0104 0112 0106 0106 0102  ................
+00001f60: 0306 0102 0104 800c 010a 0102 ff02 0206  ................
+00001f70: 0108 0106 ff0c 020c 0102 ff7a 124d 7947  ...........z.MyG
+00001f80: 7569 2e73 6574 5f64 6566 6175 6c74 7363  ui.set_defaultsc
+00001f90: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+00001fa0: 0700 0000 4300 0000 7374 0000 007c 0272  ....C...st...|.r
+00001fb0: 0464 016e 0164 027d 037c 006a 00a0 0164  .d.n.d.}.|.j...d
+00001fc0: 0364 04a1 0201 0074 026a 037c 0064 0564  .d.....t.j.|.d.d
+00001fd0: 0664 078d 037c 005f 007c 006a 006a 0464  .d...|._.|.j.j.d
+00001fe0: 0864 0964 0a64 0b64 0c64 0d8d 0501 007c  .d.d.d.d.d.....|
+00001ff0: 006a 00a0 0564 0e7c 019b 0064 0f9d 02a1  .j...d.|...d....
+00002000: 0201 007c 006a 006a 0664 107c 0364 118d  ...|.j.j.d.|.d..
+00002010: 0201 007c 006a 00a0 07a1 0001 0064 0053  ...|.j.......d.S
+00002020: 0029 124e da05 4772 6565 6e72 3f00 0000  .).N..Greenr?...
+00002030: fa03 312e 30da 0365 6e64 69f4 0100 0069  ..1.0..endi....i
+00002040: 5802 0000 7242 0000 0072 0100 0000 720d  X...rB...r....r.
+00002050: 0000 0072 1900 0000 e928 0000 0072 1400  ...r.....(...r..
+00002060: 0000 722b 0000 0072 8500 0000 da01 0ada  ..r+...r........
+00002070: 0864 6973 6162 6c65 6429 02da 0573 7461  .disabled)...sta
+00002080: 7465 723b 0000 0029 0872 6d00 0000 da06  ter;...).rm.....
+00002090: 6465 6c65 7465 7256 0000 0072 6c00 0000  deleterV...rl...
+000020a0: 7257 0000 0072 9700 0000 726e 0000 00da  rW...r....rn....
+000020b0: 0966 6f63 7573 5f73 6574 2904 727e 0000  .focus_set).r~..
+000020c0: 00da 076d 6573 7361 6765 5a04 676f 6f64  ...messageZ.good
+000020d0: da05 636f 6c6f 7272 8100 0000 7281 0000  ..colorr....r...
+000020e0: 0072 8200 0000 da13 6469 7370 6c61 795f  .r......display_
+000020f0: 6d65 7373 6167 655f 626f 7888 0100 0073  message_box....s
+00002100: 1800 0000 0c02 0602 0201 0201 04fe 1205  ................
+00002110: 1601 1401 0601 0401 06ff 0e03 7a19 4d79  ............z.My
+00002120: 4775 692e 6469 7370 6c61 795f 6d65 7373  Gui.display_mess
+00002130: 6167 655f 626f 7863 0300 0000 0000 0000  age_boxc........
+00002140: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+00002150: 73b6 0000 0064 017d 037c 0173 1164 027c  s....d.}.|.s.d.|
+00002160: 029b 0064 037c 029b 0064 049d 057d 0364  ...d.|...d...}.d
+00002170: 057c 005f 006e 2a7c 006a 0172 1a7c 006a  .|._.n*|.j.r.|.j
+00002180: 0272 1a64 067d 036e 217c 006a 0172 237c  .r.d.}.n!|.j.r#|
+00002190: 006a 0372 2364 077d 036e 187c 006a 0272  .j.r#d.}.n.|.j.r
+000021a0: 2c7c 006a 0372 2c64 087d 036e 0f7c 00a0  ,|.j.r,d.}.n.|..
+000021b0: 047c 017c 02a1 0273 3b64 097c 019b 0064  .|.|...s;d.|...d
+000021c0: 0a7c 029b 0064 0b9d 057d 037c 0372 4d7c  .|...d...}.|.rM|
+000021d0: 00a0 057c 0364 0ca1 0201 0064 0d5c 037c  ...|.d.....d.\.|
+000021e0: 005f 017c 005f 027c 005f 0364 0053 007c  ._.|._.|._.d.S.|
+000021f0: 00a0 0564 0e7c 019b 0064 0f7c 029b 009d  ...d.|...d.|....
+00002200: 0464 0ca1 0201 0064 0053 0029 104e 7284  .d.....d.S.).Nr.
+00002210: 0000 007a 220a 0a45 6974 6865 7220 7468  ...z"..Either th
+00002220: 6520 6e61 6d65 2065 6e74 6572 6564 2066  e name entered f
+00002230: 6f72 2074 6865 207a 3320 6973 2062 6c61  or the z3 is bla
+00002240: 6e6b 206f 7220 7468 6520 2743 616e 6365  nk or the 'Cance
+00002250: 6c27 2062 7574 746f 6e20 7761 7320 636c  l' button was cl
+00002260: 6963 6b65 642e 0a0a 416c 6c20 7a14 7320  icked...All z.s 
+00002270: 7769 6c6c 2062 6520 6469 7370 6c61 7965  will be displaye
+00002280: 642e 467a 5b45 7272 6f72 3a0a 0a59 6f75  d.Fz[Error:..You
+00002290: 2068 6176 6520 656e 7465 7265 6420 626f   have entered bo
+000022a0: 7468 2061 2050 726f 6a65 6374 2061 6e64  th a Project and
+000022b0: 2061 2050 726f 6669 6c65 206e 616d 6521   a Profile name!
+000022c0: 0a0a 5472 7920 6167 6169 6e20 616e 6420  ..Try again and 
+000022d0: 6f6e 6c79 2073 656c 6563 7420 6f6e 652e  only select one.
+000022e0: 7a58 4572 726f 723a 0a0a 596f 7520 6861  zXError:..You ha
+000022f0: 7665 2065 6e74 6572 6564 2062 6f74 6820  ve entered both 
+00002300: 6120 5072 6f6a 6563 7420 616e 6420 6120  a Project and a 
+00002310: 5461 736b 206e 616d 6521 0a0a 5472 7920  Task name!..Try 
+00002320: 6167 6169 6e20 616e 6420 6f6e 6c79 2073  again and only s
+00002330: 656c 6563 7420 6f6e 652e 7a58 4572 726f  elect one.zXErro
+00002340: 723a 0a0a 596f 7520 6861 7665 2065 6e74  r:..You have ent
+00002350: 6572 6564 2062 6f74 6820 6120 5072 6f66  ered both a Prof
+00002360: 696c 6520 616e 6420 6120 5461 736b 206e  ile and a Task n
+00002370: 616d 6521 0a0a 5472 7920 6167 6169 6e20  ame!..Try again 
+00002380: 616e 6420 6f6e 6c79 2073 656c 6563 7420  and only select 
+00002390: 6f6e 652e 7a08 4572 726f 723a 2022 7a02  one.z.Error: "z.
+000023a0: 2220 7a18 206e 6f74 2066 6f75 6e64 2121  " z. not found!!
+000023b0: 2020 5472 7920 6167 6169 6e2e 5429 0372    Try again.T).r
+000023c0: 8400 0000 7284 0000 0072 8400 0000 7a12  ....r....r....z.
+000023d0: 4469 7370 6c61 7920 6f6e 6c79 2074 6865  Display only the
+000023e0: 2027 7a02 2720 2906 5a0a 6e61 6d65 645f   'z.' ).Z.named_
+000023f0: 6974 656d 7291 0000 0072 9200 0000 7293  itemr....r....r.
+00002400: 0000 00da 0a76 616c 6964 5f69 7465 6d72  .....valid_itemr
+00002410: a900 0000 2904 727e 0000 00da 0874 6865  ....).r~.....the
+00002420: 5f6e 616d 65da 0c65 6c65 6d65 6e74 5f6e  _name..element_n
+00002430: 616d 65da 0d65 7272 6f72 5f6d 6573 7361  ame..error_messa
+00002440: 6765 7281 0000 0072 8100 0000 7282 0000  ger....r....r...
+00002450: 00da 0a63 6865 636b 5f6e 616d 659c 0100  ...check_name...
+00002460: 0073 3a00 0000 0401 0402 0802 0201 06ff  .s:.............
+00002470: 02ff 0805 0c02 0202 04ff 0c04 0202 04ff  ................
+00002480: 0c04 0202 04ff 0c05 1002 02ff 0405 0c01  ................
+00002490: 0205 02fc 0401 0401 0801 0403 1001 08ff  ................
+000024a0: 7a10 4d79 4775 692e 6368 6563 6b5f 6e61  z.MyGui.check_na
+000024b0: 6d65 6303 0000 0000 0000 0000 0000 0008  mec.............
+000024c0: 0000 0009 0000 0043 0000 0073 2c01 0000  .......C...s,...
+000024d0: 6401 7400 8300 6901 7d03 7c00 6a01 7c03  d.t...i.}.|.j.|.
+000024e0: 6401 1900 6402 3c00 7c00 6a01 7211 6403  d...d.<.|.j.r.d.
+000024f0: 6e01 6404 7c03 6405 3c00 7402 7c00 6a03  n.d.|.d.<.t.|.j.
+00002500: 8301 7c03 6406 3c00 7404 8300 7c03 6407  ..|.d.<.t...|.d.
+00002510: 3c00 7405 7c03 8301 7d03 7c03 6407 3d00  <.t.|...}.|.d.=.
+00002520: 6700 7d04 7c02 0400 6408 6b02 7239 0100  g.}.|...d.k.r9..
+00002530: 7c03 6409 1900 640a 1900 7d04 6900 7d05  |.d...d...}.i.}.
+00002540: 6e1d 0400 640b 6b02 7247 0100 7c03 6409  n...d.k.rG..|.d.
+00002550: 1900 640c 1900 7d04 640c 7d05 6e0f 640d  ..d...}.d.}.n.d.
+00002560: 6b02 7253 7c03 6409 1900 640e 1900 7d04  k.rS|.d...d...}.
+00002570: 640e 7d05 6e03 0900 6900 7d05 7c04 4400  d.}.n...i.}.|.D.
+00002580: 5d3b 7d06 7a2e 7c02 6408 6b02 7266 7c06  ];}.z.|.d.k.rf|.
+00002590: a006 640f a101 6a07 7d07 6e0c 7c03 6409  ..d...j.}.n.|.d.
+000025a0: 1900 7c05 1900 7c06 1900 a006 6410 a101  ..|...|.....d...
+000025b0: 6a07 7d07 7c07 6411 6b02 727a 7408 6412  j.}.|.d.k.rzt.d.
+000025c0: 8301 0100 7c01 7c07 6b02 7287 7c03 6405  ....|.|.k.r.|.d.
+000025d0: 1900 7c00 5f09 5700 0100 6413 5300 5700  ..|._.W...d.S.W.
+000025e0: 7158 0400 740a 7993 0100 0100 0100 6404  qX..t.y.......d.
+000025f0: 7d07 5900 7158 7700 6414 5300 2915 4eda  }.Y.qXw.d.S.).N.
+00002600: 1170 726f 6772 616d 5f61 7267 756d 656e  .program_argumen
+00002610: 7473 728b 0000 00fa 0a62 6163 6b75 702e  tsr......backup.
+00002620: 786d 6c72 8400 0000 da0b 6669 6c65 5f74  xmlr......file_t
+00002630: 6f5f 6765 74da 0d63 6f6c 6f72 735f 746f  o_get..colors_to
+00002640: 5f75 7365 da0c 6f75 7470 7574 5f6c 696e  _use..output_lin
+00002650: 6573 da07 5072 6f6a 6563 74da 1474 6173  es..Project..tas
+00002660: 6b65 725f 726f 6f74 5f65 6c65 6d65 6e74  ker_root_element
+00002670: 73da 0c61 6c6c 5f70 726f 6a65 6374 73da  s..all_projects.
+00002680: 0750 726f 6669 6c65 da0c 616c 6c5f 7072  .Profile..all_pr
+00002690: 6f66 696c 6573 da04 5461 736b da09 616c  ofiles..Task..al
+000026a0: 6c5f 7461 736b 73da 046e 616d 65da 036e  l_tasks..name..n
+000026b0: 6d65 7a15 4368 6563 6b20 446f 776e 7374  mez.Check Downst
+000026c0: 6169 7273 2048 6561 74da 046b 616b 6154  airs Heat..kakaT
+000026d0: 4629 0b72 0600 0000 728b 0000 0072 0900  F).r....r....r..
+000026e0: 0000 7296 0000 0072 0a00 0000 7205 0000  ..r....r....r...
+000026f0: 00da 0466 696e 6472 1b00 0000 da05 7072  ...findr......pr
+00002700: 696e 7472 9a00 0000 729c 0000 0029 0872  intr....r....).r
+00002710: 7e00 0000 72ab 0000 0072 ac00 0000 5a12  ~...r....r....Z.
+00002720: 7465 6d70 5f70 7269 6d61 7279 5f69 7465  temp_primary_ite
+00002730: 6d73 da0c 726f 6f74 5f65 6c65 6d65 6e74  ms..root_element
+00002740: 5a0b 6469 6374 5f74 6f5f 7573 65da 0469  Z.dict_to_use..i
+00002750: 7465 6d5a 0969 7465 6d5f 6e61 6d65 7281  temZ.item_namer.
+00002760: 0000 0072 8100 0000 7282 0000 0072 aa00  ...r....r....r..
+00002770: 0000 cc01 0000 7354 0000 000a 020e 0112  ......sT........
+00002780: 010e 010a 0108 0106 0104 0202 030a 0106  ................
+00002790: 0102 0104 ff06 030a 0106 0102 0104 ff06  ................
+000027a0: 0306 010c 0106 0102 0104 0108 0302 0108  ................
+000027b0: 010e 010e 0306 0102 0102 fd08 0508 0108  ................
+000027c0: 010a 0108 0104 fe0c 0308 0102 ff04 037a  ...............z
+000027d0: 104d 7947 7569 2e76 616c 6964 5f69 7465  .MyGui.valid_ite
+000027e0: 6d63 0100 0000 0000 0000 0000 0000 0200  mc..............
+000027f0: 0000 0400 0000 4300 0000 f352 0000 007c  ......C....R...|
+00002800: 006a 00a0 0164 0164 02a1 0201 007c 006a  .j...d.d.....|.j
+00002810: 02a0 03a1 0001 007c 006a 04a0 03a1 0001  .......|.j......
+00002820: 0074 056a 0664 0374 079b 009d 0264 0464  .t.j.d.t.....d.d
+00002830: 058d 027d 017c 01a0 08a1 007c 005f 097c  ...}.|.....|._.|
+00002840: 00a0 0a7c 006a 0964 06a1 0201 0064 0053  ...|.j.d.....d.S
+00002850: 0029 074e 729f 0000 0072 a000 0000 7a13  .).Nr....r....z.
+00002860: 456e 7465 7220 5072 6f6a 6563 7420 6e61  Enter Project na
+00002870: 6d65 3a7a 1844 6973 706c 6179 2053 7065  me:z.Display Spe
+00002880: 6369 6669 6320 5072 6f6a 6563 74a9 0272  cific Project..r
+00002890: 1b00 0000 7252 0000 0072 b400 0000 290b  ....rR...r....).
+000028a0: 726d 0000 0072 a500 0000 7275 0000 00da  rm...r....ru....
+000028b0: 0864 6573 656c 6563 7472 7700 0000 7256  .deselectrw...rV
+000028c0: 0000 00da 0e43 546b 496e 7075 7444 6961  .....CTkInputDia
+000028d0: 6c6f 67da 1163 616e 6365 6c5f 6275 7474  log..cancel_butt
+000028e0: 6f6e 5f6d 7367 da09 6765 745f 696e 7075  on_msg..get_inpu
+000028f0: 7472 9100 0000 72ae 0000 00a9 0272 7e00  tr....r......r~.
+00002900: 0000 da06 6469 616c 6f67 7281 0000 0072  ....dialogr....r
+00002910: 8100 0000 7282 0000 0072 7200 0000 0202  ....r....rr.....
+00002920: 0000 f312 0000 000e 020a 030a 0104 0208  ................
+00002930: 0102 0106 fe0a 0512 027a 1f4d 7947 7569  .........z.MyGui
+00002940: 2e73 696e 676c 655f 7072 6f6a 6563 745f  .single_project_
+00002950: 6e61 6d65 5f65 7665 6e74 6301 0000 0000  name_eventc.....
+00002960: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00002970: 0000 0072 c200 0000 2907 4e72 9f00 0000  ...r....).Nr....
+00002980: 72a0 0000 007a 1345 6e74 6572 2050 726f  r....z.Enter Pro
+00002990: 6669 6c65 206e 616d 653a 7a18 4469 7370  file name:z.Disp
+000029a0: 6c61 7920 5370 6563 6966 6963 2050 726f  lay Specific Pro
+000029b0: 6669 6c65 72c3 0000 0072 b700 0000 290b  filer....r....).
+000029c0: 726d 0000 0072 a500 0000 7273 0000 0072  rm...r....rs...r
+000029d0: c400 0000 7277 0000 0072 5600 0000 72c5  ....rw...rV...r.
+000029e0: 0000 0072 c600 0000 72c7 0000 0072 9200  ...r....r....r..
+000029f0: 0000 72ae 0000 0072 c800 0000 7281 0000  ..r....r....r...
+00002a00: 0072 8100 0000 7282 0000 0072 7400 0000  .r....r....rt...
+00002a10: 1602 0000 72ca 0000 007a 1f4d 7947 7569  ....r....z.MyGui
+00002a20: 2e73 696e 676c 655f 7072 6f66 696c 655f  .single_profile_
+00002a30: 6e61 6d65 5f65 7665 6e74 6301 0000 0000  name_eventc.....
+00002a40: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00002a50: 0000 0072 c200 0000 2907 4e72 9f00 0000  ...r....).Nr....
+00002a60: 72a0 0000 007a 1045 6e74 6572 2054 6173  r....z.Enter Tas
+00002a70: 6b20 6e61 6d65 3a7a 1544 6973 706c 6179  k name:z.Display
+00002a80: 2053 7065 6369 6669 6320 5461 736b 72c3   Specific Taskr.
+00002a90: 0000 0072 b900 0000 290b 726d 0000 0072  ...r....).rm...r
+00002aa0: a500 0000 7273 0000 0072 c400 0000 7275  ....rs...r....ru
+00002ab0: 0000 0072 5600 0000 72c5 0000 0072 c600  ...rV...r....r..
+00002ac0: 0000 72c7 0000 0072 9300 0000 72ae 0000  ..r....r....r...
+00002ad0: 0072 c800 0000 7281 0000 0072 8100 0000  .r....r....r....
+00002ae0: 7282 0000 0072 7600 0000 2a02 0000 72ca  r....rv...*...r.
+00002af0: 0000 007a 1c4d 7947 7569 2e73 696e 676c  ...z.MyGui.singl
+00002b00: 655f 7461 736b 5f6e 616d 655f 6576 656e  e_task_name_even
+00002b10: 74da 136e 6577 5f61 7070 6561 7261 6e63  t..new_appearanc
+00002b20: 655f 6d6f 6465 6302 0000 0000 0000 0000  e_modec.........
+00002b30: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+00002b40: 1400 0000 7400 a001 7c01 a101 0100 7c01  ....t...|.....|.
+00002b50: 7c00 5f02 6400 5300 a901 4e29 0372 5600  |._.d.S...N).rV.
+00002b60: 0000 da13 7365 745f 6170 7065 6172 616e  ....set_appearan
+00002b70: 6365 5f6d 6f64 6572 9600 0000 2902 727e  ce_moder....).r~
+00002b80: 0000 0072 cb00 0000 7281 0000 0072 8100  ...r....r....r..
+00002b90: 0000 7282 0000 0072 6500 0000 3e02 0000  ..r....re...>...
+00002ba0: 7304 0000 000a 010a 017a 224d 7947 7569  s........z"MyGui
+00002bb0: 2e63 6861 6e67 655f 6170 7065 6172 616e  .change_appearan
+00002bc0: 6365 5f6d 6f64 655f 6576 656e 74da 0e64  ce_mode_event..d
+00002bd0: 6973 706c 6179 5f64 6574 6169 6c63 0200  isplay_detailc..
+00002be0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00002bf0: 0000 4300 0000 7316 0000 007c 017c 005f  ..C...s....|.|._
+00002c00: 007c 006a 01a0 027c 01a1 0101 0064 0053  .|.j...|.....d.S
+00002c10: 0072 cc00 0000 2903 7287 0000 0072 5a00  .r....).r....rZ.
+00002c20: 0000 7286 0000 0029 0272 7e00 0000 72ce  ..r....).r~...r.
+00002c30: 0000 0072 8100 0000 7281 0000 0072 8200  ...r....r....r..
+00002c40: 0000 7259 0000 0045 0200 0073 0400 0000  ..rY...E...s....
+00002c50: 0601 1001 7a1b 4d79 4775 692e 6465 7461  ....z.MyGui.deta
+00002c60: 696c 5f73 656c 6563 7465 645f 6576 656e  il_selected_even
+00002c70: 74da 1363 6f6c 6f72 5f73 656c 6563 7465  t..color_selecte
+00002c80: 645f 6974 656d 6302 0000 0000 0000 0000  d_itemc.........
+00002c90: 0000 0008 0000 0008 0000 0043 0000 0073  ...........C...s
+00002ca0: d600 0000 6700 6401 a201 7d02 7c00 6a00  ....g.d...}.|.j.
+00002cb0: 7c00 6a00 7c00 6a01 7c00 6a02 6704 7d03  |.j.|.j.|.j.g.}.
+00002cc0: 7403 a004 7405 a101 8f30 0100 7c02 a006  t...t....0..|...
+00002cd0: 7c01 a101 7d04 7c03 7c04 1900 733c 7c01  |...}.|.|...s<|.
+00002ce0: a007 6402 6403 a102 7d05 7c05 a007 6404  ..d.d...}.|...d.
+00002cf0: 6403 a102 7d05 7c00 a008 6405 7c05 9b00  d...}.|...d.|...
+00002d00: 6406 9d03 6407 a102 0100 0900 5700 6400  d...d.......W.d.
+00002d10: 0400 0400 8303 0100 6400 5300 5700 6400  ........d.S.W.d.
+00002d20: 0400 0400 8303 0100 6e08 3100 7346 7701  ........n.1.sFw.
+00002d30: 0100 0100 0100 5900 0100 7409 8300 7d06  ......Y...t...}.
+00002d40: 7c06 a00a a100 7d07 7c07 6400 7501 7269  |.....}.|.d.u.ri
+00002d50: 7c00 a008 7c01 9b00 6408 7c07 9b00 9d03  |...|...d.|.....
+00002d60: 6407 a102 0100 7c00 a00b 7c07 7c01 a102  d.....|...|.|...
+00002d70: 0100 6400 5300 6400 5300 2909 4e29 0472  ..d.S.d.S.).N).r
+00002d80: 4800 0000 724a 0000 0072 4e00 0000 724f  H...rJ...rN...rO
+00002d90: 0000 007a 0850 726f 6669 6c65 2072 8400  ...z.Profile r..
+00002da0: 0000 7a07 4163 7469 6f6e 207a 0844 6973  ..z.Action z.Dis
+00002db0: 706c 6179 207a 1720 6973 206e 6f74 2073  play z. is not s
+00002dc0: 6574 2074 6f20 6469 7370 6c61 7921 46fa  et to display!F.
+00002dd0: 1220 636f 6c6f 7220 6368 616e 6765 6420  . color changed 
+00002de0: 746f 2029 0c72 8800 0000 728a 0000 0072  to ).r....r....r
+00002df0: 8900 0000 da0a 636f 6e74 6578 746c 6962  ......contextlib
+00002e00: da08 7375 7070 7265 7373 da09 4578 6365  ..suppress..Exce
+00002e10: 7074 696f 6eda 0569 6e64 6578 da07 7265  ption..index..re
+00002e20: 706c 6163 6572 a900 0000 7203 0000 00da  placer....r.....
+00002e30: 0367 6574 da18 6578 7472 6163 745f 636f  .get..extract_co
+00002e40: 6c6f 725f 6672 6f6d 5f65 7665 6e74 2908  lor_from_event).
+00002e50: 727e 0000 0072 cf00 0000 5a0d 7761 726e  r~...r....Z.warn
+00002e60: 696e 675f 6368 6563 6b5a 0d63 6865 636b  ing_checkZ.check
+00002e70: 5f61 6761 696e 7374 5a09 7468 655f 696e  _againstZ.the_in
+00002e80: 6465 785a 1274 6865 5f6f 7574 7075 745f  dexZ.the_output_
+00002e90: 6d65 7373 6167 655a 0a70 6963 6b5f 636f  messageZ.pick_co
+00002ea0: 6c6f 7272 a800 0000 7281 0000 0072 8100  lorr....r....r..
+00002eb0: 0000 7282 0000 0072 7800 0000 4c02 0000  ..r....rx...L...
+00002ec0: 7334 0000 0008 0104 0704 0104 0104 0104  s4..............
+00002ed0: fc0c 090a 0108 010c 010c 0104 010c 0104  ................
+00002ee0: ff02 0310 f802 021c fe06 0a08 0108 0104  ................
+00002ef0: 010e 0104 ff10 0504 fa7a 124d 7947 7569  .........z.MyGui
+00002f00: 2e63 6f6c 6f72 735f 6576 656e 7463 0300  .colors_eventc..
+00002f10: 0000 0000 0000 0000 0000 0300 0000 0700  ................
+00002f20: 0000 4300 0000 7376 0000 007c 017c 006a  ..C...sv...|.|.j
+00002f30: 0074 017c 0219 003c 007c 006a 02a0 0374  .t.|...<.|.j...t
+00002f40: 046a 057c 006a 06a0 0764 01a1 017c 029b  .j.|.j...d...|..
+00002f50: 0064 029d 027c 0164 038d 03a1 0101 007c  .d...|.d.......|
+00002f60: 006a 0264 0419 006a 087c 006a 0964 0564  .j.d...j.|.j.d.d
+00002f70: 0564 0564 068d 0401 007c 0004 006a 0964  .d.d.....|...j.d
+00002f80: 0737 0002 005f 097c 00a0 0a7c 029b 0064  .7..._.|...|...d
+00002f90: 087c 019b 009d 0364 09a1 0201 0064 0053  .|.....d.....d.S
+00002fa0: 0029 0a4e 7244 0000 007a 0920 3c3c 2063  .).NrD...z. << c
+00002fb0: 6f6c 6f72 2902 721b 0000 0072 3b00 0000  olor).r....r;...
+00002fc0: e9ff ffff ff72 0100 0000 721d 0000 0072  .....r....r....r
+00002fd0: 0d00 0000 72d0 0000 0054 290b 7299 0000  ....r....T).r...
+00002fe0: 0072 0700 0000 7295 0000 00da 0661 7070  .r....r......app
+00002ff0: 656e 6472 5600 0000 7258 0000 0072 6f00  endrV...rX...ro.
+00003000: 0000 7271 0000 0072 5700 0000 7294 0000  ..rq...rW...r...
+00003010: 0072 a900 0000 2903 727e 0000 0072 a800  .r....).r~...r..
+00003020: 0000 72cf 0000 0072 8100 0000 7281 0000  ..r....r....r...
+00003030: 0072 8200 0000 72d7 0000 0073 0200 0073  .r....r....s...s
+00003040: 1c00 0000 0203 0cff 0603 0401 0a01 0801  ................
+00003050: 0201 04fd 04ff 1a07 0e01 0401 0e01 08ff  ................
+00003060: 7a1e 4d79 4775 692e 6578 7472 6163 745f  z.MyGui.extract_
+00003070: 636f 6c6f 725f 6672 6f6d 5f65 7665 6e74  color_from_event
+00003080: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00003090: 0002 0000 0043 0000 00f3 1000 0000 7c00  .....C........|.
+000030a0: 6a00 a001 a100 7c00 5f02 6400 5300 72cc  j.....|._.d.S.r.
+000030b0: 0000 0029 0372 5c00 0000 72d6 0000 0072  ...).r\...r....r
+000030c0: 8800 0000 727d 0000 0072 8100 0000 7281  ....r}...r....r.
+000030d0: 0000 0072 8200 0000 725b 0000 0088 0200  ...r....r[......
+000030e0: 00f3 0200 0000 1001 7a15 4d79 4775 692e  ........z.MyGui.
+000030f0: 636f 6e64 6974 696f 6e5f 6576 656e 7463  condition_eventc
+00003100: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00003110: 0200 0000 4300 0000 72da 0000 0072 cc00  ....C...r....r..
+00003120: 0000 2903 7260 0000 0072 d600 0000 7289  ..).r`...r....r.
+00003130: 0000 0072 7d00 0000 7281 0000 0072 8100  ...r}...r....r..
+00003140: 0000 7282 0000 0072 5f00 0000 8e02 0000  ..r....r_.......
+00003150: 72db 0000 007a 1f4d 7947 7569 2e64 6973  r....z.MyGui.dis
+00003160: 706c 6179 5f70 7265 6665 7265 6e63 6573  play_preferences
+00003170: 5f65 7665 6e74 6301 0000 0000 0000 0000  _eventc.........
+00003180: 0000 0001 0000 0002 0000 0043 0000 0072  ...........C...r
+00003190: da00 0000 72cc 0000 0029 0372 6200 0000  ....r....).rb...
+000031a0: 72d6 0000 0072 9000 0000 727d 0000 0072  r....r....r}...r
+000031b0: 8100 0000 7281 0000 0072 8200 0000 7261  ....r....r....ra
+000031c0: 0000 0095 0200 0072 db00 0000 7a12 4d79  .......r....z.My
+000031d0: 4775 692e 7477 6973 7479 5f65 7665 6e74  Gui.twisty_event
+000031e0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000031f0: 0002 0000 0043 0000 0072 da00 0000 72cc  .....C...r....r.
+00003200: 0000 0029 0372 5e00 0000 72d6 0000 0072  ...).r^...r....r
+00003210: 8a00 0000 727d 0000 0072 8100 0000 7281  ....r}...r....r.
+00003220: 0000 0072 8200 0000 725d 0000 009b 0200  ...r....r]......
+00003230: 0072 db00 0000 7a1d 4d79 4775 692e 6469  .r....z.MyGui.di
+00003240: 7370 6c61 795f 7461 736b 6572 6e65 745f  splay_taskernet_
+00003250: 6576 656e 7463 0100 0000 0000 0000 0000  eventc..........
+00003260: 0000 0200 0000 0400 0000 0300 0000 7336  ..............s6
+00003270: 0000 0087 0066 0164 0164 0284 0874 0044  .....f.d.d...t.D
+00003280: 0083 017d 0174 017c 0188 006a 0264 0383  ...}.t.|...j.d..
+00003290: 035c 027d 0188 005f 0288 00a0 0364 0464  .\.}..._.....d.d
+000032a0: 03a1 0201 0064 0053 0029 054e 6301 0000  .....d.S.).Nc...
+000032b0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+000032c0: 0013 0000 0073 1800 0000 6900 7c00 5d08  .....s....i.|.].
+000032d0: 7d01 7c01 7400 8800 7c01 8302 9302 7102  }.|.t...|.....q.
+000032e0: 5300 7281 0000 0029 01da 0767 6574 6174  S.r....)...getat
+000032f0: 7472 2902 da02 2e30 da05 7661 6c75 6572  tr)....0..valuer
+00003300: 7d00 0000 7281 0000 0072 8200 0000 da0a  }...r....r......
+00003310: 3c64 6963 7463 6f6d 703e a302 0000 7302  <dictcomp>....s.
+00003320: 0000 0018 007a 2d4d 7947 7569 2e73 6176  .....z-MyGui.sav
+00003330: 655f 7365 7474 696e 6773 5f65 7665 6e74  e_settings_event
+00003340: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00003350: 6f6d 703e 547a 0f53 6574 7469 6e67 7320  omp>Tz.Settings 
+00003360: 7361 7665 642e 2904 7208 0000 0072 0400  saved.).r....r..
+00003370: 0000 7299 0000 0072 a900 0000 a902 727e  ..r....r......r~
+00003380: 0000 00da 0974 656d 705f 6172 6773 7281  .....temp_argsr.
+00003390: 0000 0072 7d00 0000 7282 0000 0072 6300  ...r}...r....rc.
+000033a0: 0000 a102 0000 730a 0000 0012 0202 0308  ......s.........
+000033b0: 010a ff10 037a 194d 7947 7569 2e73 6176  .....z.MyGui.sav
+000033c0: 655f 7365 7474 696e 6773 5f65 7665 6e74  e_settings_event
+000033d0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+000033e0: 0006 0000 0043 0000 0073 fc01 0000 6401  .....C...s....d.
+000033f0: 7d03 7c01 0400 6402 6b02 721f 0100 7c02  }.|...d.k.r...|.
+00003400: 7210 7c00 6a00 a001 a100 0100 6e05 7c00  r.|.j.......n.|.
+00003410: 6a00 a002 a100 0100 6403 7403 7c02 8301  j.......d.t.|...
+00003420: 9b00 6404 9d03 7d03 7c03 5300 0400 6405  ..d...}.|.S...d.
+00003430: 6b02 7236 0100 7c00 6a04 a005 7403 7c02  k.r6..|.j...t.|.
+00003440: 8301 a101 0100 6406 7403 7c02 8301 9b00  ......d.t.|.....
+00003450: 6404 9d03 7d03 7c03 5300 0400 6407 6b02  d...}.|.S...d.k.
+00003460: 7250 0100 7c02 7243 7c00 6a06 a001 a100  rP..|.rC|.j.....
+00003470: 0100 6e05 7c00 6a06 a002 a100 0100 6408  ..n.|.j.......d.
+00003480: 7c02 9b00 6404 9d03 7d03 7c03 5300 0400  |...d...}.|.S...
+00003490: 6409 6b02 726a 0100 7c02 725d 7c00 6a07  d.k.rj..|.r]|.j.
+000034a0: a001 a100 0100 6e05 7c00 6a07 a002 a100  ......n.|.j.....
+000034b0: 0100 640a 7c02 9b00 6404 9d03 7d03 7c03  ..d.|...d...}.|.
+000034c0: 5300 0400 640b 6b02 7284 0100 7c02 7277  S...d.k.r...|.rw
+000034d0: 7c00 6a08 a001 a100 0100 6e05 7c00 6a08  |.j.......n.|.j.
+000034e0: a002 a100 0100 640c 7c02 9b00 6404 9d03  ......d.|...d...
+000034f0: 7d03 7c03 5300 0400 640d 6b02 7293 0100  }.|.S...d.k.r...
+00003500: 7c02 7291 640e 7c02 9b00 6404 9d03 7d03  |.r.d.|...d...}.
+00003510: 7c03 5300 0400 640f 6b02 72a2 0100 7c02  |.S...d.k.r...|.
+00003520: 72a0 6410 7c02 9b00 6404 9d03 7d03 7c03  r.d.|...d...}.|.
+00003530: 5300 0400 6411 6b02 72b1 0100 7c02 72af  S...d.k.r...|.r.
+00003540: 6412 7c02 9b00 6404 9d03 7d03 7c03 5300  d.|...d...}.|.S.
+00003550: 0400 6413 6b02 72c0 0100 7c02 72be 6414  ..d.k.r...|.r.d.
+00003560: 7c02 9b00 6415 9d03 7d03 7c03 5300 0400  |...d...}.|.S...
+00003570: 6416 6b02 72cf 0100 7c02 72cd 6417 7c02  d.k.r...|.r.d.|.
+00003580: 9b00 6415 9d03 7d03 7c03 5300 0400 6418  ..d...}.|.S...d.
+00003590: 6b02 72e9 0100 7c02 72dc 7c00 6a09 a001  k.r...|.r.|.j...
+000035a0: a100 0100 6e05 7c00 6a09 a002 a100 0100  ....n.|.j.......
+000035b0: 6419 7c02 9b00 6415 9d03 7d03 7c03 5300  d.|...d...}.|.S.
+000035c0: 641a 6b02 72ef 0900 7c03 5300 0900 7c00  d.k.r...|.S...|.
+000035d0: a00a 641b 7c01 9b00 641c 7c02 9b00 9d04  ..d.|...d.|.....
+000035e0: 641d a102 0100 7c03 5300 291e 4e72 8400  d.....|.S.).Nr..
+000035f0: 0000 728b 0000 007a 0d44 6562 7567 2073  ..r....z.Debug s
+00003600: 6574 2074 6f20 7a02 2e0a 7287 0000 007a  et to z...r....z
+00003610: 1c44 6973 706c 6179 2044 6574 6169 6c20  .Display Detail 
+00003620: 4c65 7665 6c20 7365 7420 746f 2072 8800  Level set to r..
+00003630: 0000 7a1a 4469 7370 6c61 7920 436f 6e64  ..z.Display Cond
+00003640: 6974 696f 6e73 2073 6574 2074 6f20 7289  itions set to r.
+00003650: 0000 007a 2244 6973 706c 6179 2054 6173  ...z"Display Tas
+00003660: 6b65 7220 5072 6566 6572 656e 6365 7320  ker Preferences 
+00003670: 7365 7420 746f 2072 8a00 0000 7a19 4469  set to r....z.Di
+00003680: 7370 6c61 7920 5461 736b 6572 4e65 7420  splay TaskerNet 
+00003690: 7365 7420 746f 2072 9100 0000 7a0f 5072  set to r....z.Pr
+000036a0: 6f6a 6563 7420 7365 7420 746f 2072 9200  oject set to r..
+000036b0: 0000 7a0f 5072 6f66 696c 6520 7365 7420  ..z.Profile set 
+000036c0: 746f 2072 9300 0000 7a0c 5461 736b 2073  to r....z.Task s
+000036d0: 6574 2074 6f20 729b 0000 007a 1d47 6574  et to r....z.Get
+000036e0: 2042 6163 6b75 7020 4950 2041 6464 7265   Backup IP Addre
+000036f0: 7373 2073 6574 2074 6f20 72a2 0000 0072  ss set to r....r
+00003700: 9d00 0000 7a20 4765 7420 4261 636b 7570  ....z Get Backup
+00003710: 2046 696c 6520 4c6f 6361 7469 6f6e 2073   File Location s
+00003720: 6574 2074 6f20 7290 0000 007a 0e54 7769  et to r....z.Twi
+00003730: 7374 7920 7365 7420 746f 2072 8f00 0000  sty set to r....
+00003740: 7a21 5275 7472 6f68 2120 2055 6e64 6566  z!Rutroh!  Undef
+00003750: 696e 6564 2061 7267 756d 656e 743a 206b  ined argument: k
+00003760: 6579 3d7a 0720 7661 6c75 653d 4629 0b72  ey=z. value=F).r
+00003770: 7a00 0000 da06 7365 6c65 6374 72c4 0000  z.....selectr...
+00003780: 00da 0373 7472 725a 0000 0072 8600 0000  ...strrZ...r....
+00003790: 725c 0000 0072 6000 0000 725e 0000 0072  r\...r`...r^...r
+000037a0: 6200 0000 72a9 0000 0029 0472 7e00 0000  b...r....).r~...
+000037b0: da03 6b65 7972 de00 0000 72a7 0000 0072  ..keyr....r....r
+000037c0: 8100 0000 7281 0000 0072 8200 0000 da0f  ....r....r......
+000037d0: 7265 7374 6f72 655f 6469 7370 6c61 79ae  restore_display.
+000037e0: 0200 0073 8000 0000 0401 0201 0a01 0401  ...s............
+000037f0: 0c01 0a02 1001 0431 0ad0 1001 1001 042e  .......1........
+00003800: 0ad3 0401 0c01 0a02 0c01 0428 0ad9 0401  ...........(....
+00003810: 0c01 0a02 0c01 0422 0adf 0401 0c01 0a02  ......."........
+00003820: 0c01 041c 0ae5 0401 0c01 0419 0ae8 0401  ................
+00003830: 0c01 0416 0aeb 0401 0c01 0413 0aee 0401  ................
+00003840: 0c01 0410 0af1 0401 0c01 040d 0af4 0401  ................
+00003850: 0c01 0a02 0c01 0407 06fa 0201 0405 02fc  ................
+00003860: 0401 1001 04ff 0403 7a15 4d79 4775 692e  ........z.MyGui.
+00003870: 7265 7374 6f72 655f 6469 7370 6c61 7963  restore_displayc
+00003880: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003890: 0800 0000 4300 0000 73ac 0000 007c 00a0  ....C...s....|..
+000038a0: 0064 01a1 0101 0069 0004 007d 017c 005f  .d.....i...}.|._
+000038b0: 0174 027c 017c 006a 0164 0183 035c 027d  .t.|.|.j.d...\.}
+000038c0: 017c 005f 0174 03a0 0474 05a1 018f 2101  .|._.t...t....!.
+000038d0: 007c 0164 0219 0072 337c 00a0 067c 0164  .|.d...r3|...|.d
+000038e0: 0219 0064 01a1 0201 0064 037c 0164 023c  ...d.....d.|.d.<
+000038f0: 0009 0057 0064 0004 0004 0083 0301 0064  ...W.d.........d
+00003900: 0053 0057 0064 0004 0004 0083 0301 006e  .S.W.d.........n
+00003910: 0831 0073 3d77 0101 0001 0001 0059 0001  .1.s=w.......Y..
+00003920: 007c 0173 477c 006a 0172 4e7c 00a0 077c  .|.sG|.j.rN|...|
+00003930: 01a1 0101 0064 0053 007c 00a0 0664 0464  .....d.S.|...d.d
+00003940: 01a1 0201 0064 0053 0029 054e 46da 036d  .....d.S.).NF..m
+00003950: 7367 7284 0000 007a 174e 6f20 7365 7474  sgr....z.No sett
+00003960: 696e 6773 2066 696c 6520 666f 756e 642e  ings file found.
+00003970: 2908 727c 0000 0072 9900 0000 7204 0000  ).r|...r....r...
+00003980: 0072 d100 0000 72d2 0000 00da 084b 6579  .r....r......Key
+00003990: 4572 726f 7272 a900 0000 da10 6578 7472  Errorr......extr
+000039a0: 6163 745f 7365 7474 696e 6773 72e0 0000  act_settingsr...
+000039b0: 0072 8100 0000 7281 0000 0072 8200 0000  .r....r....r....
+000039c0: 7264 0000 00ec 0200 0073 2000 0000 0a01  rd.......s .....
+000039d0: 0a01 0202 0801 0aff 0c04 0801 1001 0801  ................
+000039e0: 0201 10fc 0201 1cff 0a06 0e01 1002 7a1c  ..............z.
+000039f0: 4d79 4775 692e 7265 7374 6f72 655f 7365  MyGui.restore_se
+00003a00: 7474 696e 6773 5f65 7665 6e74 72e1 0000  ttings_eventr...
+00003a10: 00da 0672 6574 7572 6e4e 6302 0000 0000  ...returnNc.....
+00003a20: 0000 0000 0000 0007 0000 0007 0000 0043  ...............C
+00003a30: 0000 0073 b600 0000 6401 5c02 7d02 7d03  ...s....d.\.}.}.
+00003a40: 7c01 a000 a100 4400 5d1a 5c02 7d04 7d05  |.....D.].\.}.}.
+00003a50: 7c04 6400 7501 7222 7401 7c00 7c04 7c05  |.d.u.r"t.|.|.|.
+00003a60: 8303 0100 7c00 a002 7c04 7c05 a102 0400  ....|...|.|.....
+00003a70: 7d03 7222 7c02 7c03 1700 7d02 7108 6402  }.r"|.|...}.q.d.
+00003a80: 6403 8400 7403 a000 a100 4400 8301 7d06  d...t.....D...}.
+00003a90: 7c00 6a04 a000 a100 4400 5d1e 5c02 7d04  |.j.....D.].\.}.
+00003aa0: 7d05 7c04 6400 7501 724f 7c04 6404 6b02  }.|.d.u.rO|.d.k.
+00003ab0: 7242 6405 7c06 7c04 3c00 7131 7c02 9b00  rBd.|.|.<.q1|...
+00003ac0: 6406 7c06 7c04 1900 9b00 6407 7c05 9b00  d.|.|.....d.|...
+00003ad0: 6408 9d06 7d02 7131 7c00 a005 7c02 9b00  d...}.q1|...|...
+00003ae0: 6409 9d02 640a a102 0100 6400 5300 290b  d...d.....d.S.).
+00003af0: 4e29 0272 8400 0000 7284 0000 0063 0100  N).r....r....c..
+00003b00: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00003b10: 0000 5300 0000 7316 0000 0069 007c 005d  ..S...s....i.|.]
+00003b20: 075c 027d 017d 027c 027c 0193 0271 0253  .\.}.}.|.|...q.S
+00003b30: 0072 8100 0000 7281 0000 0029 0372 dd00  .r....r....).r..
+00003b40: 0000 da01 6bda 0176 7281 0000 0072 8100  ....k..vr....r..
+00003b50: 0000 7282 0000 0072 df00 0000 0a03 0000  ..r....r........
+00003b60: 7302 0000 0016 007a 2a4d 7947 7569 2e65  s......z*MyGui.e
+00003b70: 7874 7261 6374 5f73 6574 7469 6e67 732e  xtract_settings.
+00003b80: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+00003b90: 6d70 3e72 e600 0000 7284 0000 00da 0120  mp>r....r...... 
+00003ba0: 7a0e 2063 6f6c 6f72 2073 6574 2074 6f20  z. color set to 
+00003bb0: 72a2 0000 007a 130a 5365 7474 696e 6773  r....z..Settings
+00003bc0: 2072 6573 746f 7265 642e 5429 06da 0569   restored.T)...i
+00003bd0: 7465 6d73 da07 7365 7461 7474 7272 e500  tems..setattrr..
+00003be0: 0000 7207 0000 0072 9900 0000 72a9 0000  ..r....r....r...
+00003bf0: 0029 0772 7e00 0000 72e1 0000 005a 0c61  .).r~...r....Z.a
+00003c00: 6c6c 5f6d 6573 7361 6765 735a 0b6e 6577  ll_messagesZ.new
+00003c10: 5f6d 6573 7361 6765 72e4 0000 0072 de00  _messager....r..
+00003c20: 0000 5a0f 696e 765f 636f 6c6f 725f 6e61  ..Z.inv_color_na
+00003c30: 6d65 7372 8100 0000 7281 0000 0072 8200  mesr....r....r..
+00003c40: 0000 72e8 0000 0002 0300 0073 2000 0000  ..r........s ...
+00003c50: 0801 1001 0801 0c01 1001 0801 0280 1202  ................
+00003c60: 1201 0801 0801 0a01 1803 02ff 0280 1605  ................
+00003c70: 7a16 4d79 4775 692e 6578 7472 6163 745f  z.MyGui.extract_
+00003c80: 7365 7474 696e 6773 6301 0000 0000 0000  settingsc.......
+00003c90: 0000 0000 0007 0000 0006 0000 0043 0000  .............C..
+00003ca0: 0073 5601 0000 7c00 6a00 6401 6b02 7208  .sV...|.j.d.k.r.
+00003cb0: 6402 7c00 5f00 7c00 6a01 730e 6403 7c00  d.|._.|.j.s.d.|.
+00003cc0: 5f01 7402 6a03 6404 7c00 6a00 9b00 6405  _.t.j.d.|.j...d.
+00003cd0: 7c00 6a01 9b00 9d04 6406 6407 8d02 7d01  |.j.....d.d...}.
+00003ce0: 7c01 a004 a100 0400 7d02 732b 7c00 a005  |.......}.s+|...
+00003cf0: 6408 6409 a102 0100 6400 5300 7c02 640a  d.d.....d.S.|.d.
+00003d00: 6b03 729b 7c02 a006 6405 a101 7d03 7c03  k.r.|...d...}.|.
+00003d10: 640b 1900 a006 640c a101 7d04 7c04 640b  d.....d...}.|.d.
+00003d20: 1900 a006 640d a101 7d05 7407 7c05 8301  ....d...}.t.|...
+00003d30: 640e 6b00 7256 7c00 a005 640f 7c04 640b  d.k.rV|...d.|.d.
+00003d40: 1900 9b00 6410 9d03 6409 a102 0100 6400  ....d...d.....d.
+00003d50: 5300 7c05 640b 1900 4400 5d15 7d06 7c06  S.|.d...D.].}.|.
+00003d60: a008 a100 736f 7c00 a005 640f 7c04 640b  ....so|...d.|.d.
+00003d70: 1900 9b00 6410 9d03 6409 a102 0100 0100  ....d...d.......
+00003d80: 6400 5300 715a 7c05 6411 1900 6a08 7383  d.S.qZ|.d...j.s.
+00003d90: 7c00 a005 6412 7c05 6411 1900 9b00 6410  |...d.|.d.....d.
+00003da0: 9d03 6409 a102 0100 6400 5300 7407 7c03  ..d.....d.S.t.|.
+00003db0: 8301 6413 6b00 7291 7c00 a005 6414 6409  ..d.k.r.|...d.d.
+00003dc0: a102 0100 6400 5300 7c03 640b 1900 7c00  ....d.S.|.d...|.
+00003dd0: 5f00 7c03 6411 1900 7c00 5f01 7c00 a005  _.|.d...|._.|...
+00003de0: 6415 7c00 6a00 9b00 6416 7c00 6a01 9b00  d.|.j...d.|.j...
+00003df0: 9d04 6417 a102 0100 6400 5300 2918 4e72  ..d.....d.S.).Nr
+00003e00: 8400 0000 7a12 3139 322e 3136 382e 302e  ....z.192.168.0.
+00003e10: 3231 303a 3138 3231 7a1f 2f54 6173 6b65  210:1821z./Taske
+00003e20: 722f 636f 6e66 6967 732f 7573 6572 2f62  r/configs/user/b
+00003e30: 6163 6b75 702e 786d 6c7a 8045 6e74 6572  ackup.xmlz.Enter
+00003e40: 2049 5020 4164 6472 6573 732c 2050 6f72   IP Address, Por
+00003e50: 7420 4e75 6d62 6572 2061 6e64 2046 696c  t Number and Fil
+00003e60: 6520 4c6f 6361 7469 6f6e 2c20 696e 2074  e Location, in t
+00003e70: 6865 2066 6f6c 6c6f 7769 6e67 2066 6f72  he following for
+00003e80: 6d61 743a 2069 705f 6164 6472 6573 733a  mat: ip_address:
+00003e90: 706f 7274 2c66 696c 655f 6c6f 6361 7469  port,file_locati
+00003ea0: 6f6e 0a45 6e74 6572 2027 2a27 2066 6f72  on.Enter '*' for
+00003eb0: 2064 6566 6175 6c74 733a 20fa 012c 723a   defaults: ..,r:
+00003ec0: 0000 0072 c300 0000 7a38 4765 7420 4261  ...r....z8Get Ba
+00003ed0: 636b 7570 2053 6574 7469 6e67 732e 2e2e  ckup Settings...
+00003ee0: 6e6f 7468 696e 6720 656e 7465 7265 642e  nothing entered.
+00003ef0: 2020 4e6f 2061 6374 696f 6e20 7461 6b65    No action take
+00003f00: 6e2e 46da 012a 7201 0000 00fa 013a da01  n.F..*r......:..
+00003f10: 2e72 2c00 0000 7a14 496e 7661 6c69 6420  .r,...z.Invalid 
+00003f20: 4950 2041 6464 7265 7373 3a20 7a0d 2e20  IP Address: z.. 
+00003f30: 2054 7279 2061 6761 696e 2e72 0d00 0000   Try again.r....
+00003f40: 7a15 496e 7661 6c69 6420 706f 7274 206e  z.Invalid port n
+00003f50: 756d 6265 723a 2072 0f00 0000 7a25 4669  umber: r....z%Fi
+00003f60: 6c65 206c 6f63 6174 696f 6e20 6973 206d  le location is m
+00003f70: 6973 7369 6e67 2e20 2054 7279 2061 6761  issing.  Try aga
+00003f80: 696e 2e7a 1e47 6574 2042 6163 6b75 7020  in.z.Get Backup 
+00003f90: 4950 2041 6464 7265 7373 2073 6574 2074  IP Address set t
+00003fa0: 6f3a 207a 160a 4765 7420 4c6f 6361 7469  o: z..Get Locati
+00003fb0: 6f6e 2073 6574 2074 6f3a 2054 2909 729b  on set to: T).r.
+00003fc0: 0000 0072 9d00 0000 7256 0000 0072 c500  ...r....rV...r..
+00003fd0: 0000 72c7 0000 0072 a900 0000 da05 7370  ..r....r......sp
+00003fe0: 6c69 74da 036c 656e da07 6973 6469 6769  lit..len..isdigi
+00003ff0: 7429 0772 7e00 0000 72c9 0000 005a 0b62  t).r~...r....Z.b
+00004000: 6163 6b75 705f 696e 666f 5a09 7465 6d70  ackup_infoZ.temp
+00004010: 5f69 6e66 6f5a 0774 656d 705f 6970 5a0b  _infoZ.temp_ipZ.
+00004020: 7465 6d70 5f69 7061 6464 7272 c100 0000  temp_ipaddrr....
+00004030: 7281 0000 0072 8100 0000 7282 0000 0072  r....r....r....r
+00004040: 6800 0000 1a03 0000 7370 0000 000a 0206  h.......sp......
+00004050: 0106 0106 0104 0202 0204 0304 fd04 0304  ................
+00004060: fd02 0506 f90c 0b04 0102 0102 0104 fe04  ................
+00004070: 0408 030a 020e 010e 030c 0104 010e 0102  ................
+00004080: 0104 fe04 040c 0108 0104 010e 0102 0104  ................
+00004090: fe06 0402 fb0a 0804 010e 0102 0104 fe04  ................
+000040a0: 040c 0304 0102 0102 0104 fe04 040a 030a  ................
+000040b0: 0104 020a 0204 0104 ff02 0308 fb7a 164d  .............z.M
+000040c0: 7947 7569 2e67 6574 5f62 6163 6b75 705f  yGui.get_backup_
+000040d0: 6576 656e 7463 0100 0000 0000 0000 0000  eventc..........
+000040e0: 0000 0200 0000 0400 0000 4300 0000 7398  ..........C...s.
+000040f0: 0000 007c 006a 00a0 0164 01a1 0101 007c  ...|.j...d.....|
+00004100: 006a 02a0 03a1 0001 007c 006a 04a0 03a1  .j.......|.j....
+00004110: 0001 007c 006a 05a0 03a1 0001 007c 006a  ...|.j.......|.j
+00004120: 06a0 0164 02a1 0101 0074 07a0 0864 02a1  ...d.....t...d..
+00004130: 0101 007c 006a 09a0 03a1 0001 007c 00a0  ...|.j.......|..
+00004140: 0a64 0364 04a1 0201 007c 006a 0ba0 03a1  .d.d.....|.j....
+00004150: 0001 0064 0504 007c 005f 0c7c 005f 0d7c  ...d...|._.|._.|
+00004160: 006a 0e72 457c 006a 0e44 005d 087d 017c  .j.rE|.j.D.].}.|
+00004170: 016a 0f64 0564 068d 0101 0071 3c7c 00a0  .j.d.d.....q<|..
+00004180: 1064 07a1 0101 0064 0053 0029 084e 7224  .d.....d.S.).Nr$
+00004190: 0000 0072 0b00 0000 7a0f 5365 7474 696e  ...r....z.Settin
+000041a0: 6773 2072 6573 6574 2e54 7284 0000 0072  gs reset.Tr....r
+000041b0: 4500 0000 4629 1172 5a00 0000 7286 0000  E...F).rZ...r...
+000041c0: 0072 5c00 0000 72c4 0000 0072 6000 0000  .r\...r....r`...
+000041d0: 725e 0000 0072 6600 0000 7256 0000 0072  r^...rf...rV...r
+000041e0: cd00 0000 727a 0000 0072 a900 0000 7262  ....rz...r....rb
+000041f0: 0000 0072 9d00 0000 729b 0000 0072 9500  ...r....r....r..
+00004200: 0000 726e 0000 0072 7c00 0000 2902 727e  ..rn...r|...).r~
+00004210: 0000 00da 056c 6162 656c 7281 0000 0072  .....labelr....r
+00004220: 8100 0000 7282 0000 0072 6700 0000 6803  ....r....rg...h.
+00004230: 0000 731c 0000 000c 010a 010a 010a 010c  ..s.............
+00004240: 010a 010a 010c 010a 010c 0106 010a 010e  ................
+00004250: 010e 017a 1a4d 7947 7569 2e72 6573 6574  ...z.MyGui.reset
+00004260: 5f73 6574 7469 6e67 735f 6576 656e 7463  _settings_eventc
+00004270: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00004280: 0400 0000 4300 0000 7354 0000 007c 006a  ....C...sT...|.j
+00004290: 00a0 01a1 007c 005f 027c 006a 0272 2274  .....|._.|.j.r"t
+000042a0: 0364 0183 01a0 04a1 0072 177c 00a0 0564  .d.......r.|...d
+000042b0: 0264 03a1 0201 0064 0053 007c 00a0 0564  .d.....d.S.|...d
+000042c0: 0464 05a1 0201 0064 057c 005f 0264 0053  .d.....d.|._.d.S
+000042d0: 007c 00a0 0564 0664 03a1 0201 0064 0053  .|...d.d.....d.S
+000042e0: 0029 074e 72b0 0000 007a 1344 6562 7567  .).Nr....z.Debug
+000042f0: 206d 6f64 6520 656e 6162 6c65 642e 547a   mode enabled.Tz
+00004300: 5344 6562 7567 206d 6f64 6520 7265 7175  SDebug mode requ
+00004310: 6972 6573 2054 6173 6b65 7220 6261 636b  ires Tasker back
+00004320: 7570 2066 696c 6520 746f 2062 6520 6e61  up file to be na
+00004330: 6d65 643a 2027 6261 636b 7570 2e78 6d6c  med: 'backup.xml
+00004340: 272c 2077 6869 6368 2069 7320 6d69 7373  ', which is miss
+00004350: 696e 6721 467a 1444 6562 7567 206d 6f64  ing!Fz.Debug mod
+00004360: 6520 6469 7361 626c 6564 2e29 0672 7a00  e disabled.).rz.
+00004370: 0000 72d6 0000 0072 8b00 0000 7202 0000  ..r....r....r...
+00004380: 00da 0769 735f 6669 6c65 72a9 0000 0072  ...is_filer....r
+00004390: 7d00 0000 7281 0000 0072 8100 0000 7282  }...r....r....r.
+000043a0: 0000 0072 7900 0000 7b03 0000 7314 0000  ...ry...{...s...
+000043b0: 000c 0106 010c 0110 0104 0202 0202 0304  ................
+000043c0: fb0a 0710 027a 1a4d 7947 7569 2e64 6562  .....z.MyGui.deb
+000043d0: 7567 5f63 6865 636b 626f 785f 6576 656e  ug_checkbox_even
+000043e0: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+000043f0: 0000 0200 0000 4300 0000 f312 0000 0064  ......C........d
+00004400: 017c 005f 007c 00a0 01a1 0001 0064 0053  .|._.|.......d.S
+00004410: 00a9 024e 5429 0272 8e00 0000 da04 7175  ...NT).r......qu
+00004420: 6974 727d 0000 0072 8100 0000 7281 0000  itr}...r....r...
+00004430: 0072 8200 0000 7269 0000 008f 0300 00f3  .r....ri........
+00004440: 0400 0000 0601 0c01 7a11 4d79 4775 692e  ........z.MyGui.
+00004450: 7275 6e5f 7072 6f67 7261 6d63 0100 0000  run_programc....
+00004460: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00004470: 4300 0000 731a 0000 0064 017c 005f 007c  C...s....d.|._.|
+00004480: 00a0 01a1 0001 007c 00a0 02a1 0001 0064  .......|.......d
+00004490: 0053 0072 f900 0000 2903 728f 0000 00da  .S.r....).r.....
+000044a0: 0877 6974 6864 7261 7772 fa00 0000 727d  .withdrawr....r}
+000044b0: 0000 0072 8100 0000 7281 0000 0072 8200  ...r....r....r..
+000044c0: 0000 726a 0000 0096 0300 0073 0600 0000  ..rj.......s....
+000044d0: 0601 0802 0c01 7a17 4d79 4775 692e 7265  ......z.MyGui.re
+000044e0: 7275 6e5f 7468 655f 7072 6f67 7261 6d63  run_the_programc
+000044f0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00004500: 0200 0000 4300 0000 72f8 0000 0072 f900  ....C...r....r..
+00004510: 0000 2902 728d 0000 0072 fa00 0000 727d  ..).r....r....r}
+00004520: 0000 0072 8100 0000 7281 0000 0072 8200  ...r....r....r..
+00004530: 0000 726b 0000 009f 0300 0072 fb00 0000  ..rk.......r....
+00004540: 7a12 4d79 4775 692e 6578 6974 5f70 726f  z.MyGui.exit_pro
+00004550: 6772 616d 2921 da08 5f5f 6e61 6d65 5f5f  gram)!..__name__
+00004560: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00004570: 7175 616c 6e61 6d65 5f5f 7251 0000 00da  qualname__rQ....
+00004580: 0462 6f6f 6c72 7c00 0000 72a9 0000 0072  .boolr|...r....r
+00004590: ae00 0000 72aa 0000 0072 7200 0000 7274  ....r....rr...rt
+000045a0: 0000 0072 7600 0000 72e3 0000 0072 6500  ...rv...r....re.
+000045b0: 0000 7259 0000 0072 7800 0000 72d7 0000  ..rY...rx...r...
+000045c0: 0072 5b00 0000 725f 0000 0072 6100 0000  .r[...r_...ra...
+000045d0: 725d 0000 0072 6300 0000 72e5 0000 0072  r]...rc...r....r
+000045e0: 6400 0000 da04 6469 6374 72e8 0000 0072  d.....dictr....r
+000045f0: 6800 0000 7267 0000 0072 7900 0000 7269  h...rg...ry...ri
+00004600: 0000 0072 6a00 0000 726b 0000 00da 0d5f  ...rj...rk....._
+00004610: 5f63 6c61 7373 6365 6c6c 5f5f 7281 0000  _classcell__r...
+00004620: 0072 8100 0000 727f 0000 0072 8200 0000  .r....r....r....
+00004630: 720c 0000 0046 0000 0073 3a00 0000 0800  r....F...s:.....
+00004640: 0c01 007f 007f 0e1c 0827 0814 0830 0836  .........'...0.6
+00004650: 0814 0814 0e14 0e07 0e07 0827 0815 0806  ...........'....
+00004660: 0807 0806 0806 080d 083e 1216 0818 084e  .........>.....N
+00004670: 0813 0814 0807 1009 720c 0000 0029 1972  ........r....).r
+00004680: d100 0000 7256 0000 00da 0770 6174 686c  ....rV.....pathl
+00004690: 6962 7202 0000 005a 1f43 546b 436f 6c6f  ibr....Z.CTkColo
+000046a0: 7250 6963 6b65 722e 6374 6b5f 636f 6c6f  rPicker.ctk_colo
+000046b0: 725f 7069 636b 6572 7203 0000 00da 176d  r_pickerr......m
+000046c0: 6170 7461 736b 6572 2e73 7263 2e67 6574  aptasker.src.get
+000046d0: 7075 7461 7267 7204 0000 00da 166d 6170  putargr......map
+000046e0: 7461 736b 6572 2e73 7263 2e70 726f 6769  tasker.src.progi
+000046f0: 6e69 7472 0500 0000 da16 6d61 7074 6173  nitr......maptas
+00004700: 6b65 722e 7372 632e 696e 6974 7061 7267  ker.src.initparg
+00004710: 7206 0000 00da 166d 6170 7461 736b 6572  r......maptasker
+00004720: 2e73 7263 2e73 7973 636f 6e73 7472 0700  .src.sysconstr..
+00004730: 0000 7208 0000 00da 166d 6170 7461 736b  ..r......maptask
+00004740: 6572 2e73 7263 2e63 6f6c 726d 6f64 6572  er.src.colrmoder
+00004750: 0900 0000 da15 6d61 7074 6173 6b65 722e  ......maptasker.
+00004760: 7372 632e 6c69 6e65 6f75 7472 0a00 0000  src.lineoutr....
+00004770: 72cd 0000 005a 1773 6574 5f64 6566 6175  r....Z.set_defau
+00004780: 6c74 5f63 6f6c 6f72 5f74 6865 6d65 7298  lt_color_themer.
+00004790: 0000 0072 c600 0000 5a03 4354 6b72 0c00  ...r....Z.CTkr..
+000047a0: 0000 7281 0000 0072 8100 0000 7281 0000  ..r....r....r...
+000047b0: 0072 8200 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000047c0: 0100 0000 7322 0000 0008 1208 010c 010c  ....s"..........
+000047d0: 010c 010c 010c 010c 010c 010c 010c 010a  ................
+000047e0: 030a 0202 0302 ff04 1c16 06              ...........
```

### Comparing `maptasker-2.0.4/maptasker/src/__pycache__/xmldata.cpython-310.pyc` & `maptasker-2.0.5/maptasker/src/__pycache__/xmldata.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/actargs.py` & `maptasker-2.0.5/maptasker/src/actargs.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/action.py` & `maptasker-2.0.5/maptasker/src/action.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/actionc.py` & `maptasker-2.0.5/maptasker/src/actionc.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/actiond.py` & `maptasker-2.0.5/maptasker/src/actiond.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/actione.py` & `maptasker-2.0.5/maptasker/src/actione.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/actionr.py` & `maptasker-2.0.5/maptasker/src/actionr.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/actiont.py` & `maptasker-2.0.5/maptasker/src/actiont.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/caveats.py` & `maptasker-2.0.5/maptasker/src/caveats.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/colors.py` & `maptasker-2.0.5/maptasker/src/colors.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/colrmode.py` & `maptasker-2.0.5/maptasker/src/colrmode.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/condition.py` & `maptasker-2.0.5/maptasker/src/condition.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/config.py` & `maptasker-2.0.5/maptasker/src/config.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/debug.py` & `maptasker-2.0.5/maptasker/src/debug.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/error.py` & `maptasker-2.0.5/maptasker/src/error.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/frmthtml.py` & `maptasker-2.0.5/maptasker/src/frmthtml.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/getbakup.py` & `maptasker-2.0.5/maptasker/src/getbakup.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/getids.py` & `maptasker-2.0.5/maptasker/src/getids.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/getputarg.py` & `maptasker-2.0.5/maptasker/src/getputarg.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/initparg.py` & `maptasker-2.0.5/maptasker/src/initparg.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/kidapp.py` & `maptasker-2.0.5/maptasker/src/kidapp.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/lineout.py` & `maptasker-2.0.5/maptasker/src/lineout.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/mapit.py` & `maptasker-2.0.5/maptasker/src/mapit.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/migrate.py` & `maptasker-2.0.5/maptasker/src/migrate.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/parsearg.py` & `maptasker-2.0.5/maptasker/src/parsearg.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/prefers.py` & `maptasker-2.0.5/maptasker/src/prefers.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/proclist.py` & `maptasker-2.0.5/maptasker/src/proclist.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/profiles.py` & `maptasker-2.0.5/maptasker/src/profiles.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/progargs.py` & `maptasker-2.0.5/maptasker/src/progargs.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/proginit.py` & `maptasker-2.0.5/maptasker/src/proginit.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/projects.py` & `maptasker-2.0.5/maptasker/src/projects.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/runcli.py` & `maptasker-2.0.5/maptasker/src/runcli.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/rungui.py` & `maptasker-2.0.5/maptasker/src/rungui.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,14 +66,18 @@
     try:
         primary_items["program_arguments"]["display_detail_level"] = int(
             user_input.display_detail_level
         )
     except TypeError:
         primary_items["program_arguments"]["display_detail_level"] = 3
 
+    # Do we already have the file object?
+    if user_input.file:
+        primary_items["file_to_get"] = user_input.file.name
+
     # Get the program arguments and save them in our dictionary
     for value in ARGUMENT_NAMES:
         if value == "backup_file_http":
             if http_info := getattr(user_input, value):
                 primary_items["program_arguments"][value] = f"http://{http_info}"
         else:
             primary_items["program_arguments"][value] = getattr(user_input, value)
```

### Comparing `maptasker-2.0.4/maptasker/src/scenes.py` & `maptasker-2.0.5/maptasker/src/scenes.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/servicec.py` & `maptasker-2.0.5/maptasker/src/servicec.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/share.py` & `maptasker-2.0.5/maptasker/src/share.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/shellsort.py` & `maptasker-2.0.5/maptasker/src/shellsort.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/sysconst.py` & `maptasker-2.0.5/maptasker/src/sysconst.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #                                                                                            #
 # ########################################################################################## #
 from maptasker.src.config import OUTPUT_FONT
 import logging
 
 # Global constants
 UNKNOWN_TASK_NAME = "Unnamed/Anonymous."
-MY_VERSION = "MapTasker version 2.0.4"
+MY_VERSION = "MapTasker version 2.0.5"
 MY_LICENSE = "GNU GENERAL PUBLIC LICENSE (Version 3, 29 June 2007)"
 NO_PROJECT = "-none found."
 COUNTER_FILE = ".MapTasker_RunCount.txt"
 ARGUMENTS_FILE = ".MapTasker_arguments.json"
 FONT_TO_USE = f';font-family:{OUTPUT_FONT}'
 NO_PROFILE = "None or unnamed!"
```

### Comparing `maptasker-2.0.4/maptasker/src/taskactn.py` & `maptasker-2.0.5/maptasker/src/taskactn.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/taskerd.py` & `maptasker-2.0.5/maptasker/src/taskerd.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/taskflag.py` & `maptasker-2.0.5/maptasker/src/taskflag.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/tasks.py` & `maptasker-2.0.5/maptasker/src/tasks.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/taskuniq.py` & `maptasker-2.0.5/maptasker/src/taskuniq.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/twisty.py` & `maptasker-2.0.5/maptasker/src/twisty.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/maptasker/src/userintr.py` & `maptasker-2.0.5/maptasker/src/userintr.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,14 +368,15 @@
         self.color_text_row = 2
         self.appearance_mode_optionemenu.set("System")
         self.color_labels = []
         self.appearance_mode = "System"
         if first_time:
             self.textbox.insert("0.0", "MapTasker Help\n\n" + INFO_TEXT)
         self.color_lookup = {}  # Setup default dictionary as empty list
+        self.file = None
         # We only want to initialize the next two variables only if they have not yet been defined.
         #  Ignore sourcery recommendation to reformat these.
         try:  # The following will fail with an attribute error if it does not already exist
             if self.backup_file_http:
                 pass
         except AttributeError:
             self.backup_file_http = ""
@@ -409,24 +410,21 @@
     # Validate name entered
     # #######################################################################################
     def check_name(self, the_name, element_name):
         error_message = ""
         # Check for missing name
         if not the_name:
             error_message = (
-                "Error:\n\nThe name entered for the "
-                + element_name
-                + " is blank!\n\nTry again."
+                f"\n\nEither the name entered for the {element_name} is blank or the"
+                f" 'Cancel' button was clicked.\n\nAll {element_name}s will be"
+                " displayed."
             )
             self.named_item = False
-        if the_name is None:
-            error_message = "Name entry canceled.  All will be displayed."
-
         # Check to make sure only one named item has been entered
-        if self.single_project_name and self.single_profile_name:
+        elif self.single_project_name and self.single_profile_name:
             error_message = (
                 "Error:\n\nYou have entered both a Project and a Profile name!\n\n"
                 "Try again and only select one."
             )
         elif self.single_project_name and self.single_task_name:
             error_message = (
                 "Error:\n\nYou have entered both a Project and a Task name!\n\n"
@@ -475,30 +473,39 @@
         match element_name:
             case "Project":
                 root_element = temp_primary_items["tasker_root_elements"][
                     "all_projects"
                 ]
                 dict_to_use = {}
             case "Profile":
-                root_element = temp_primary_items["all_profiles"]
+                root_element = temp_primary_items["tasker_root_elements"][
+                    "all_profiles"
+                ]
                 dict_to_use = "all_profiles"
             case "Task":
-                root_element = temp_primary_items["all_tasks"]
+                root_element = temp_primary_items["tasker_root_elements"]["all_tasks"]
                 dict_to_use = "all_tasks"
             case _:
                 dict_to_use = {}
 
         # See if the item exists
         for item in root_element:
             try:
                 if element_name == "Project":
                     item_name = item.find("name").text
                 else:
-                    item_name = temp_primary_items[dict_to_use][item].find("nme").text
+                    item_name = (
+                        temp_primary_items["tasker_root_elements"][dict_to_use][item]
+                        .find("nme")
+                        .text
+                    )
+                if item_name == "Check Downstairs Heat":
+                    print("kaka")
                 if the_name == item_name:
+                    self.file = temp_primary_items["file_to_get"]
                     return True
             except AttributeError:
                 item_name = ""
 
         return False
 
     # #######################################################################################
```

### Comparing `maptasker-2.0.4/maptasker/src/xmldata.py` & `maptasker-2.0.5/maptasker/src/xmldata.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.0.4/pyproject.toml` & `maptasker-2.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maptasker"
-version = "2.0.4"
+version = "2.0.5"
 description = "Utility to display your entire Android 'Tasker' configuration on your MAC."
 authors = ["Michael Rubin <mikrubin@gmail.com>"]
 readme = "README_PyPl.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/mctinker/Map-Tasker"
 keywords = ["tasker", "Tasker", "map tasker"]
 packages = [
```

### Comparing `maptasker-2.0.4/PKG-INFO` & `maptasker-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maptasker
-Version: 2.0.4
+Version: 2.0.5
 Summary: Utility to display your entire Android 'Tasker' configuration on your MAC.
 Home-page: https://github.com/mctinker/Map-Tasker
 License: GPL-3.0-or-later
 Keywords: tasker,Tasker,map tasker
 Author: Michael Rubin
 Author-email: mikrubin@gmail.com
 Requires-Python: >=3.10,<4.0
```

