# Comparing `tmp/perun.proxygui-1.8.3.tar.gz` & `tmp/perun.proxygui-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxygui-1.8.3.tar", last modified: Thu Jun 15 10:41:37 2023, max compression
+gzip compressed data, was "perun.proxygui-1.8.4.tar", last modified: Mon Jun 19 10:44:02 2023, max compression
```

## Comparing `perun.proxygui-1.8.3.tar` & `perun.proxygui-1.8.4.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.494279 perun.proxygui-1.8.3/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-15 10:41:37.494279 perun.proxygui-1.8.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6779 2023-06-15 10:33:43.000000 perun.proxygui-1.8.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/api/backchannel_logout_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4178 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/api/ban_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/proxygui/api/consent_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2815 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/api/kerberos_auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-06-15 09:44:59.000000 perun.proxygui-1.8.3/perun/proxygui/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3756 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/proxygui/gui/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
--rw-rw-rw-   0 root         (0) root         (0)   141520 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
--rw-rw-rw-   0 root         (0) root         (0)     1451 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
--rw-rw-rw-   0 root         (0) root         (0)     3089 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
--rw-rw-rw-   0 root         (0) root         (0)     1617 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
--rw-rw-rw-   0 root         (0) root         (0)     2945 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
--rw-rw-rw-   0 root         (0) root         (0)     2758 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.546256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
--rw-rw-rw-   0 root         (0) root         (0)    29997 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.582257 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
--rw-rw-rw-   0 root         (0) root         (0)    22637 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
--rw-rw-rw-   0 root         (0) root         (0)    21057 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
--rw-rw-rw-   0 root         (0) root         (0)    22481 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
--rw-rw-rw-   0 root         (0) root         (0)    35533 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
--rw-rw-rw-   0 root         (0) root         (0)    34805 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
--rw-rw-rw-   0 root         (0) root         (0)    28733 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
--rw-rw-rw-   0 root         (0) root         (0)    20267 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
--rw-rw-rw-   0 root         (0) root         (0)    28025 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
--rw-rw-rw-   0 root         (0) root         (0)    25884 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
--rw-rw-rw-   0 root         (0) root         (0)   363233 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
--rw-rw-rw-   0 root         (0) root         (0)    27013 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
--rw-rw-rw-   0 root         (0) root         (0)    33321 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
--rw-rw-rw-   0 root         (0) root         (0)    31511 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
--rw-rw-rw-   0 root         (0) root         (0)    34010 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
--rw-rw-rw-   0 root         (0) root         (0)    28152 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
--rw-rw-rw-   0 root         (0) root         (0)    36726 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
--rw-rw-rw-   0 root         (0) root         (0)    28663 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
--rw-rw-rw-   0 root         (0) root         (0)    22030 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.694260 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.170271 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/
--rw-rw-rw-   0 root         (0) root         (0)   125046 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
--rw-rw-rw-   0 root         (0) root         (0)   252563 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1052500 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1125125 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1125144 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1125123 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1125121 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1125119 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1125120 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1125147 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1125545 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1125121 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
--rw-rw-rw-   0 root         (0) root         (0)  1126098 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
--rw-rw-rw-   0 root         (0) root         (0)   139176 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/documentation.css
--rw-rw-rw-   0 root         (0) root         (0)    48080 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/print.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.234272 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
--rw-rw-rw-   0 root         (0) root         (0)    46987 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
--rw-rw-rw-   0 root         (0) root         (0)   303728 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
--rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
--rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
--rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
--rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
--rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
--rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
--rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
--rw-rw-rw-   0 root         (0) root         (0)   332353 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
--rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
--rw-rw-rw-   0 root         (0) root         (0)   332557 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
--rw-rw-rw-   0 root         (0) root         (0)     5778 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
--rw-rw-rw-   0 root         (0) root         (0)   312236 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
--rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
--rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
--rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
--rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
--rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-law.css
--rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-med.css
--rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
--rw-rw-rw-   0 root         (0) root         (0)   341456 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
--rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
--rw-rw-rw-   0 root         (0) root         (0)   341664 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style.css
--rw-rw-rw-   0 root         (0) root         (0)     5772 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.250273 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    87048 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
--rw-rw-rw-   0 root         (0) root         (0)    74284 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)   208892 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
--rw-rw-rw-   0 root         (0) root         (0)   159376 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
--rw-rw-rw-   0 root         (0) root         (0)     1632 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
--rw-rw-rw-   0 root         (0) root         (0)     1837 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
--rw-rw-rw-   0 root         (0) root         (0)     1484 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
--rw-rw-rw-   0 root         (0) root         (0)    12252 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
--rw-rw-rw-   0 root         (0) root         (0)     9596 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.250273 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.310274 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/
--rw-rw-rw-   0 root         (0) root         (0)    70841 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
--rw-rw-rw-   0 root         (0) root         (0)     7406 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     4426 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.362275 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/
--rw-rw-rw-   0 root         (0) root         (0)   218591 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/app.js
--rw-rw-rw-   0 root         (0) root         (0)   659454 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/app.js.map
--rw-rw-rw-   0 root         (0) root         (0)   337945 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/d3.js
--rw-rw-rw-   0 root         (0) root         (0)     2707 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/documentation.js
--rw-rw-rw-   0 root         (0) root         (0)     8806 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/graphs.js
--rw-rw-rw-   0 root         (0) root         (0)    26171 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
--rw-rw-rw-   0 root         (0) root         (0)     4075 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
--rw-rw-rw-   0 root         (0) root         (0)   284394 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)   610160 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.430277 perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/css/
--rw-rw-rw-   0 root         (0) root         (0)   155845 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0 root         (0) root         (0)   431289 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.450277 perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/js/
--rw-rw-rw-   0 root         (0) root         (0)    78743 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0 root         (0) root         (0)   325834 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/campus-idp-muni.js
--rw-rw-rw-   0 root         (0) root         (0)     7336 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/campus-idp.css
--rw-rw-rw-   0 root         (0) root         (0)     4859 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/campus-idp.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.450277 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/css/
--rw-rw-rw-   0 root         (0) root         (0)    73577 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/css/all.css
--rw-rw-rw-   0 root         (0) root         (0)    59305 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/css/all.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.482278 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/
--rw-rw-rw-   0 root         (0) root         (0)   134294 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
--rw-rw-rw-   0 root         (0) root         (0)   747927 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
--rw-rw-rw-   0 root         (0) root         (0)   133988 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)    89988 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
--rw-rw-rw-   0 root         (0) root         (0)    76736 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)    34034 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
--rw-rw-rw-   0 root         (0) root         (0)   144714 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
--rw-rw-rw-   0 root         (0) root         (0)    33736 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0 root         (0) root         (0)    16276 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
--rw-rw-rw-   0 root         (0) root         (0)    13224 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0 root         (0) root         (0)   203030 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
--rw-rw-rw-   0 root         (0) root         (0)   918991 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
--rw-rw-rw-   0 root         (0) root         (0)   202744 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0 root         (0) root         (0)   101648 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
--rw-rw-rw-   0 root         (0) root         (0)    78268 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
--rw-rw-rw-   0 root         (0) root         (0)    89501 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/jquery-3.6.0.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.486278 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/
--rw-rw-rw-   0 root         (0) root         (0)    15836 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
--rw-rw-rw-   0 root         (0) root         (0)     8266 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
--rw-rw-rw-   0 root         (0) root         (0)     8862 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
--rw-rw-rw-   0 root         (0) root         (0)     8873 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
--rw-rw-rw-   0 root         (0) root         (0)     7692 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.css
--rw-rw-rw-   0 root         (0) root         (0)     8344 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.default.css
--rw-rw-rw-   0 root         (0) root         (0)    11438 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.486278 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/js/standalone/
--rw-rw-rw-   0 root         (0) root         (0)    64906 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.486278 perun.proxygui-1.8.3/perun/proxygui/gui/templates/
--rw-rw-rw-   0 root         (0) root         (0)    15205 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/proxygui/gui/templates/ConsentRegistration.html
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/templates/IsTestingSP.html
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/templates/SPAuthorization.html
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/templates/_footer.html
--rw-rw-rw-   0 root         (0) root         (0)     8047 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/templates/_header.html
--rw-rw-rw-   0 root         (0) root         (0)     1175 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/templates/authorization.html
--rw-rw-rw-   0 root         (0) root         (0)     2226 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/gui/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/translations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun/proxygui/gui/translations/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.490278 perun.proxygui-1.8.3/perun/proxygui/gui/translations/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2973 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
--rw-rw-rw-   0 root         (0) root         (0)     5815 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.490278 perun.proxygui-1.8.3/perun/proxygui/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/tests/shared_test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7166 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/tests/test_ban_api.py
--rw-rw-rw-   0 root         (0) root         (0)     3105 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/proxygui/tests/test_consent_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/proxygui/tests/test_consent_db.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/proxygui/tests/test_consent_request_db.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/tests/test_gui.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/tests/test_kerberos_auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5509 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/proxygui/user_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.490278 perun.proxygui-1.8.3/perun/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1273 2023-06-04 07:37:17.000000 perun.proxygui-1.8.3/perun/utils/ConfigStore.py
--rw-rw-rw-   0 root         (0) root         (0)     2642 2023-06-04 07:50:33.000000 perun.proxygui-1.8.3/perun/utils/CustomRPHandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:37.494279 perun.proxygui-1.8.3/perun/utils/consent_framework/
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/utils/consent_framework/consent.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/utils/consent_framework/consent_db.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/utils/consent_framework/consent_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/utils/consent_framework/consent_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-06-05 14:34:11.000000 perun.proxygui-1.8.3/perun/utils/consent_framework/consent_request_db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:41:36.542256 perun.proxygui-1.8.3/perun.proxygui.egg-info/
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-15 10:41:36.000000 perun.proxygui-1.8.3/perun.proxygui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11250 2023-06-15 10:41:36.000000 perun.proxygui-1.8.3/perun.proxygui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 10:41:36.000000 perun.proxygui-1.8.3/perun.proxygui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-15 10:41:36.000000 perun.proxygui-1.8.3/perun.proxygui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-15 10:41:36.000000 perun.proxygui-1.8.3/perun.proxygui.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-15 10:41:37.494279 perun.proxygui-1.8.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      863 2023-06-15 10:33:43.000000 perun.proxygui-1.8.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6779 2023-06-15 10:33:43.000000 perun.proxygui-1.8.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.230429 perun.proxygui-1.8.4/perun/proxygui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.230429 perun.proxygui-1.8.4/perun/proxygui/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/api/backchannel_logout_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4178 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/api/ban_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/proxygui/api/consent_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2815 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/api/kerberos_auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-06-15 09:44:59.000000 perun.proxygui-1.8.4/perun/proxygui/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.230429 perun.proxygui-1.8.4/perun/proxygui/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3756 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/proxygui/gui/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.246430 perun.proxygui-1.8.4/perun/proxygui/gui/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.250430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.250430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
+-rw-rw-rw-   0 root         (0) root         (0)   141520 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.250430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.250430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.254430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
+-rw-rw-rw-   0 root         (0) root         (0)      437 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2945 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.254430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.258430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.258430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
+-rw-rw-rw-   0 root         (0) root         (0)    29997 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.262430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
+-rw-rw-rw-   0 root         (0) root         (0)    22637 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    21057 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    22481 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    35533 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    34805 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    28733 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    20267 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    28025 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    25884 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
+-rw-rw-rw-   0 root         (0) root         (0)   363233 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    27013 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    33321 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    31511 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    34010 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    28152 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    36726 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    28663 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    22030 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.274430 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.290431 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/
+-rw-rw-rw-   0 root         (0) root         (0)   125046 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
+-rw-rw-rw-   0 root         (0) root         (0)   252563 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1052500 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1125125 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1125144 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1125123 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1125121 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1125119 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1125120 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1125147 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1125545 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1125121 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
+-rw-rw-rw-   0 root         (0) root         (0)  1126098 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
+-rw-rw-rw-   0 root         (0) root         (0)   139176 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/documentation.css
+-rw-rw-rw-   0 root         (0) root         (0)    48080 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/print.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.294431 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
+-rw-rw-rw-   0 root         (0) root         (0)    46987 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
+-rw-rw-rw-   0 root         (0) root         (0)   303728 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
+-rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
+-rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
+-rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
+-rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
+-rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
+-rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
+-rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
+-rw-rw-rw-   0 root         (0) root         (0)   332353 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
+-rw-rw-rw-   0 root         (0) root         (0)   332243 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
+-rw-rw-rw-   0 root         (0) root         (0)   332557 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
+-rw-rw-rw-   0 root         (0) root         (0)     5778 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
+-rw-rw-rw-   0 root         (0) root         (0)   312236 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
+-rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
+-rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
+-rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
+-rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
+-rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-law.css
+-rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-med.css
+-rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
+-rw-rw-rw-   0 root         (0) root         (0)   341456 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
+-rw-rw-rw-   0 root         (0) root         (0)   341340 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
+-rw-rw-rw-   0 root         (0) root         (0)   341664 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style.css
+-rw-rw-rw-   0 root         (0) root         (0)     5772 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.298431 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    87048 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
+-rw-rw-rw-   0 root         (0) root         (0)    74284 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   208892 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
+-rw-rw-rw-   0 root         (0) root         (0)   159376 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
+-rw-rw-rw-   0 root         (0) root         (0)     1632 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
+-rw-rw-rw-   0 root         (0) root         (0)    12252 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
+-rw-rw-rw-   0 root         (0) root         (0)     9596 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.298431 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.298431 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/
+-rw-rw-rw-   0 root         (0) root         (0)    70841 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
+-rw-rw-rw-   0 root         (0) root         (0)     7406 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.302431 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/
+-rw-rw-rw-   0 root         (0) root         (0)   218591 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/app.js
+-rw-rw-rw-   0 root         (0) root         (0)   659454 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/app.js.map
+-rw-rw-rw-   0 root         (0) root         (0)   337945 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/d3.js
+-rw-rw-rw-   0 root         (0) root         (0)     2707 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/documentation.js
+-rw-rw-rw-   0 root         (0) root         (0)     8806 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/graphs.js
+-rw-rw-rw-   0 root         (0) root         (0)    26171 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
+-rw-rw-rw-   0 root         (0) root         (0)     4075 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
+-rw-rw-rw-   0 root         (0) root         (0)   284394 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)   610160 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.302431 perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/css/
+-rw-rw-rw-   0 root         (0) root         (0)   155845 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   431289 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.302431 perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/js/
+-rw-rw-rw-   0 root         (0) root         (0)    78743 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0 root         (0) root         (0)   325834 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/campus-idp-muni.js
+-rw-rw-rw-   0 root         (0) root         (0)     7336 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/campus-idp.css
+-rw-rw-rw-   0 root         (0) root         (0)     4859 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/campus-idp.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.302431 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/css/
+-rw-rw-rw-   0 root         (0) root         (0)    73577 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/css/all.css
+-rw-rw-rw-   0 root         (0) root         (0)    59305 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/css/all.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.306431 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/
+-rw-rw-rw-   0 root         (0) root         (0)   134294 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0 root         (0) root         (0)   747927 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0 root         (0) root         (0)   133988 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    89988 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0 root         (0) root         (0)    76736 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    34034 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0 root         (0) root         (0)   144714 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33736 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    16276 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0 root         (0) root         (0)    13224 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   203030 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0 root         (0) root         (0)   918991 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0 root         (0) root         (0)   202744 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   101648 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0 root         (0) root         (0)    78268 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
+-rw-rw-rw-   0 root         (0) root         (0)    89501 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/jquery-3.6.0.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/
+-rw-rw-rw-   0 root         (0) root         (0)    15836 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
+-rw-rw-rw-   0 root         (0) root         (0)     8266 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
+-rw-rw-rw-   0 root         (0) root         (0)     8862 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
+-rw-rw-rw-   0 root         (0) root         (0)     8873 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
+-rw-rw-rw-   0 root         (0) root         (0)     7692 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.css
+-rw-rw-rw-   0 root         (0) root         (0)     8344 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.default.css
+-rw-rw-rw-   0 root         (0) root         (0)    11438 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/js/standalone/
+-rw-rw-rw-   0 root         (0) root         (0)    64906 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/perun/proxygui/gui/templates/
+-rw-rw-rw-   0 root         (0) root         (0)    15205 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/proxygui/gui/templates/ConsentRegistration.html
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/templates/IsTestingSP.html
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/templates/SPAuthorization.html
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/templates/_footer.html
+-rw-rw-rw-   0 root         (0) root         (0)     8047 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/templates/_header.html
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/templates/authorization.html
+-rw-rw-rw-   0 root         (0) root         (0)     2226 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/gui/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/translations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.194429 perun.proxygui-1.8.4/perun/proxygui/gui/translations/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/perun/proxygui/gui/translations/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2973 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
+-rw-rw-rw-   0 root         (0) root         (0)     5815 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/perun/proxygui/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/tests/shared_test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7166 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/tests/test_ban_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/proxygui/tests/test_consent_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/proxygui/tests/test_consent_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/proxygui/tests/test_consent_request_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/tests/test_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/proxygui/tests/test_kerberos_auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2023-06-19 10:23:19.000000 perun.proxygui-1.8.4/perun/proxygui/user_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/perun/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2023-06-04 07:37:17.000000 perun.proxygui-1.8.4/perun/utils/ConfigStore.py
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2023-06-04 07:50:33.000000 perun.proxygui-1.8.4/perun/utils/CustomRPHandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/perun/utils/consent_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/utils/consent_framework/consent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/utils/consent_framework/consent_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/utils/consent_framework/consent_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/utils/consent_framework/consent_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-06-05 14:34:11.000000 perun.proxygui-1.8.4/perun/utils/consent_framework/consent_request_db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:44:02.210429 perun.proxygui-1.8.4/perun.proxygui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-19 10:44:02.000000 perun.proxygui-1.8.4/perun.proxygui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11250 2023-06-19 10:44:02.000000 perun.proxygui-1.8.4/perun.proxygui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:44:02.000000 perun.proxygui-1.8.4/perun.proxygui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-19 10:44:02.000000 perun.proxygui-1.8.4/perun.proxygui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-19 10:44:02.000000 perun.proxygui-1.8.4/perun.proxygui.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-19 10:44:02.310431 perun.proxygui-1.8.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      863 2023-06-19 10:23:19.000000 perun.proxygui-1.8.4/setup.py
```

### Comparing `perun.proxygui-1.8.3/LICENSE` & `perun.proxygui-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/README.md` & `perun.proxygui-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/api/backchannel_logout_api.py` & `perun.proxygui-1.8.4/perun/proxygui/api/backchannel_logout_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/api/ban_api.py` & `perun.proxygui-1.8.4/perun/proxygui/api/ban_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/api/consent_api.py` & `perun.proxygui-1.8.4/perun/proxygui/api/consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/api/kerberos_auth_api.py` & `perun.proxygui-1.8.4/perun/proxygui/api/kerberos_auth_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/app.py` & `perun.proxygui-1.8.4/perun/proxygui/app.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/gui.py` & `perun.proxygui-1.8.4/perun/proxygui/gui/gui.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/documentation.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/print.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-custom.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-econ.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-fi.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-fss.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-law.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-med.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-ped.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-phil.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style-sci.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/style.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/favicon.ico` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/app.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/app.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/app.js.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/app.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/d3.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/documentation.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/documentation.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/graphs.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/graphs.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/jquery.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/jquery.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/campus-idp.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/campus-idp.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/campus-idp.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/campus-idp.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/css/all.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/css/all.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/css/all.min.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/jquery-3.6.0.min.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.default.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.default.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/css/selectize.legacy.css` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/css/selectize.legacy.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js` & `perun.proxygui-1.8.4/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/templates/ConsentRegistration.html` & `perun.proxygui-1.8.4/perun/proxygui/gui/templates/ConsentRegistration.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/templates/IsTestingSP.html` & `perun.proxygui-1.8.4/perun/proxygui/gui/templates/IsTestingSP.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/templates/SPAuthorization.html` & `perun.proxygui-1.8.4/perun/proxygui/gui/templates/SPAuthorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/templates/_footer.html` & `perun.proxygui-1.8.4/perun/proxygui/gui/templates/_footer.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/templates/_header.html` & `perun.proxygui-1.8.4/perun/proxygui/gui/templates/_header.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/templates/authorization.html` & `perun.proxygui-1.8.4/perun/proxygui/gui/templates/authorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/templates/base.html` & `perun.proxygui-1.8.4/perun/proxygui/gui/templates/base.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo` & `perun.proxygui-1.8.4/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po` & `perun.proxygui-1.8.4/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/tests/test_ban_api.py` & `perun.proxygui-1.8.4/perun/proxygui/tests/test_ban_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/tests/test_consent_api.py` & `perun.proxygui-1.8.4/perun/proxygui/tests/test_consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/tests/test_consent_db.py` & `perun.proxygui-1.8.4/perun/proxygui/tests/test_consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/tests/test_consent_request_db.py` & `perun.proxygui-1.8.4/perun/proxygui/tests/test_consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/tests/test_gui.py` & `perun.proxygui-1.8.4/perun/proxygui/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/tests/test_kerberos_auth_api.py` & `perun.proxygui-1.8.4/perun/proxygui/tests/test_kerberos_auth_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/proxygui/user_manager.py` & `perun.proxygui-1.8.4/perun/proxygui/user_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,51 +48,52 @@
         engine = sqlalchemy.create_engine(connection_string)
 
         return engine
 
     def _get_mitre_delete_statements(self, user_id: str, engine: Engine) -> list[Any]:
         meta_data = sqlalchemy.MetaData(bind=engine)
         sqlalchemy.MetaData.reflect(meta_data)
+        session = Session(bind=engine)
 
         AUTH_HOLDER_TBL = meta_data.tables["authentication_holder"]
         SAVED_USER_AUTH_TBL = meta_data.tables["saved_user_auth"]
 
         ACCESS_TOKEN_TBL = meta_data.tables["access_token"]
         delete_access_tokens_stmt = delete(ACCESS_TOKEN_TBL).where(
-            ACCESS_TOKEN_TBL.auth_holder_id.in_(
-                Session.query(AUTH_HOLDER_TBL.id).filter(
-                    AUTH_HOLDER_TBL.user_auth_id.in_(
-                        Session.query(SAVED_USER_AUTH_TBL.id).filter(
-                            SAVED_USER_AUTH_TBL.name == user_id
+            ACCESS_TOKEN_TBL.c.auth_holder_id.in_(
+                session.query(AUTH_HOLDER_TBL.c.id).filter(
+                    AUTH_HOLDER_TBL.c.user_auth_id.in_(
+                        session.query(SAVED_USER_AUTH_TBL.c.id).filter(
+                            SAVED_USER_AUTH_TBL.c.name == user_id
                         )
                     )
                 )
             )
         )
 
         AUTH_CODE_TBL = meta_data.tables["authorization_code"]
         delete_authorization_codes_stmt = delete(AUTH_CODE_TBL).where(
-            AUTH_CODE_TBL.auth_holder_id.in_(
-                Session.query(AUTH_HOLDER_TBL.id).filter(
-                    AUTH_HOLDER_TBL.user_auth_id.in_(
-                        Session.query(SAVED_USER_AUTH_TBL.id).filter(
-                            SAVED_USER_AUTH_TBL.name == user_id
+            AUTH_CODE_TBL.c.auth_holder_id.in_(
+                session.query(AUTH_HOLDER_TBL.c.id).filter(
+                    AUTH_HOLDER_TBL.c.user_auth_id.in_(
+                        session.query(SAVED_USER_AUTH_TBL.c.id).filter(
+                            SAVED_USER_AUTH_TBL.c.name == user_id
                         )
                     )
                 )
             )
         )
 
         DEVICE_CODE = meta_data.tables["device_code"]
         delete_device_codes_stmt = delete(DEVICE_CODE).where(
-            DEVICE_CODE.auth_holder_id.in_(
-                Session.query(AUTH_HOLDER_TBL.id).filter(
-                    AUTH_HOLDER_TBL.user_auth_id.in_(
-                        Session.query(SAVED_USER_AUTH_TBL.id).filter(
-                            SAVED_USER_AUTH_TBL.name == user_id
+            DEVICE_CODE.c.auth_holder_id.in_(
+                session.query(AUTH_HOLDER_TBL.c.id).filter(
+                    AUTH_HOLDER_TBL.c.user_auth_id.in_(
+                        session.query(SAVED_USER_AUTH_TBL.c.id).filter(
+                            SAVED_USER_AUTH_TBL.c.name == user_id
                         )
                     )
                 )
             )
         )
 
         return [
```

### Comparing `perun.proxygui-1.8.3/perun/utils/ConfigStore.py` & `perun.proxygui-1.8.4/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/utils/CustomRPHandler.py` & `perun.proxygui-1.8.4/perun/utils/CustomRPHandler.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/utils/consent_framework/consent.py` & `perun.proxygui-1.8.4/perun/utils/consent_framework/consent.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/utils/consent_framework/consent_db.py` & `perun.proxygui-1.8.4/perun/utils/consent_framework/consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/utils/consent_framework/consent_manager.py` & `perun.proxygui-1.8.4/perun/utils/consent_framework/consent_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/utils/consent_framework/consent_request.py` & `perun.proxygui-1.8.4/perun/utils/consent_framework/consent_request.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun/utils/consent_framework/consent_request_db.py` & `perun.proxygui-1.8.4/perun/utils/consent_framework/consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/perun.proxygui.egg-info/SOURCES.txt` & `perun.proxygui-1.8.4/perun.proxygui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perun.proxygui-1.8.3/setup.py` & `perun.proxygui-1.8.4/setup.py`

 * *Files identical despite different names*

