# Comparing `tmp/FuncsForSPO-5.3.0.tar.gz` & `tmp/FuncsForSPO-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.3.0.tar", last modified: Fri Jun  9 21:35:39 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.0.0.tar", last modified: Sun Jun 18 22:38:05 2023, max compression
```

## Comparing `FuncsForSPO-5.3.0.tar` & `FuncsForSPO-6.0.0.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:39.308973 FuncsForSPO-5.3.0/
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.581817 FuncsForSPO-5.3.0/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.695940 FuncsForSPO-5.3.0/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.3.0/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.3.0/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.717177 FuncsForSPO-5.3.0/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.3.0/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.3.0/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.741762 FuncsForSPO-5.3.0/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.3.0/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.3.0/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.754940 FuncsForSPO-5.3.0/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.3.0/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.764289 FuncsForSPO-5.3.0/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.3.0/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.3.0/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.788779 FuncsForSPO-5.3.0/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.3.0/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.3.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.800135 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.869172 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     8122 2023-06-09 21:34:32.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-09 19:06:51.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.912732 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.942313 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.956903 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.994349 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9646 2023-06-06 20:32:25.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5303 2023-06-06 20:31:18.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:39.012525 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     1217 2023-06-07 11:50:52.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:39.028756 FuncsForSPO-5.3.0/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:39.054007 FuncsForSPO-5.3.0/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.3.0/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:39.072584 FuncsForSPO-5.3.0/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.3.0/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.3.0/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:39.090170 FuncsForSPO-5.3.0/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.3.0/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-5.3.0/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:39.114356 FuncsForSPO-5.3.0/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.3.0/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.3.0/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:39.128564 FuncsForSPO-5.3.0/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.3.0/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.3.0/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:39.140667 FuncsForSPO-5.3.0/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.3.0/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:35:38.675924 FuncsForSPO-5.3.0/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-09 21:35:38.000000 FuncsForSPO-5.3.0/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1815 2023-06-09 21:35:38.000000 FuncsForSPO-5.3.0/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 21:35:38.000000 FuncsForSPO-5.3.0/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      194 2023-06-09 21:35:38.000000 FuncsForSPO-5.3.0/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      458 2023-06-09 21:35:38.000000 FuncsForSPO-5.3.0/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.3.0/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-09 21:35:39.301240 FuncsForSPO-5.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 21:35:39.309491 FuncsForSPO-5.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2506 2023-06-09 21:35:26.000000 FuncsForSPO-5.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.534116 FuncsForSPO-6.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.154902 FuncsForSPO-6.0.0/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.219958 FuncsForSPO-6.0.0/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.0.0/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.0.0/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.228119 FuncsForSPO-6.0.0/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.0/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.0.0/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.238381 FuncsForSPO-6.0.0/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.0/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.0.0/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.243449 FuncsForSPO-6.0.0/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.0.0/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.246465 FuncsForSPO-6.0.0/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.0.0/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-6.0.0/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.256393 FuncsForSPO-6.0.0/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.0/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.0.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.260659 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.289684 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     8120 2023-06-17 20:27:58.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-17 20:27:40.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.309339 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.325324 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.328841 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.355827 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0     9014 2023-06-18 21:43:31.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.363883 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.375093 FuncsForSPO-6.0.0/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.386691 FuncsForSPO-6.0.0/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-6.0.0/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.395114 FuncsForSPO-6.0.0/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.0/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-6.0.0/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.406375 FuncsForSPO-6.0.0/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.0/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-6.0.0/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.415003 FuncsForSPO-6.0.0/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.0.0/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.0.0/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.424010 FuncsForSPO-6.0.0/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.0.0/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.0.0/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.462265 FuncsForSPO-6.0.0/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-6.0.0/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 22:38:05.208981 FuncsForSPO-6.0.0/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-18 22:38:04.000000 FuncsForSPO-6.0.0/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1886 2023-06-18 22:38:04.000000 FuncsForSPO-6.0.0/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 22:38:04.000000 FuncsForSPO-6.0.0/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-06-18 22:38:04.000000 FuncsForSPO-6.0.0/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      458 2023-06-18 22:38:04.000000 FuncsForSPO-6.0.0/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.0.0/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-18 22:38:05.530579 FuncsForSPO-6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-6.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-18 22:38:05.535090 FuncsForSPO-6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2611 2023-06-18 22:37:57.000000 FuncsForSPO-6.0.0/setup.py
```

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.0.0/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.0.0/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
             return text
         except Exception as e:
             faz_log(repr(e), 'c*')
             faz_log(self.DRIVER.get_screenshot_as_base64(), 'i*')
             self.DRIVER.quit()
             raise ErroPDFAIException
 
-
 class GPTPDFV2(BotMain):    
     def __init__(self, content_txt: str, prompt:str, headless: bool=True) -> str:
         cria_dir_no_dir_de_trabalho_atual('tempdir')
         faz_log('Criando arquivo em uma pasta temporária')
         self.TXT_CONTENT = arquivo_com_caminho_absoluto('tempdir', 'temp.txt')
         with open(self.TXT_CONTENT, 'w', encoding='utf-8') as f:
             f.write(content_txt)
```

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,22 +18,21 @@
 from FuncsForSPO.fpython.functions_for_py import *
 from FuncsForSPO.fselenium.functions_selenium import *
 from FuncsForSPO.fexceptions.exceptions import FalhaAoRecuperarOcr
 import json
 import os
 
 class GetTextPDF:    
-    def __init__(self, file_pdf: str, type_extract='text', dir_exit: str='output', get_text_into_code: bool=True, headless: bool=True, prints: bool=False, create_driver: bool=True) -> str:
+    def __init__(self, file_pdf: str, dir_exit: str='output', headless: bool=True, prints: bool=False, create_driver: bool=True) -> str:
         """Init
 
         Args:
             file_pdf (str): Caminho do arquivo
             dir_exit (str, optional): Local de saída do arquivo TXT. Defaults to 'output'.
             headless (bool, optional): executa como headless. Defaults to True.
-            get_text_into_code (bool, optional): Retorna o texto do pdf no código. Defaults to True.
             create_driver (bool, optional): Cria um driver. Defaults to True.
         """
         if isinstance(headless, (bool, int)):
             self.HEADLESS = headless
         else:
             print('Adicione True ou False para Headless')
         
@@ -43,21 +42,17 @@
             self.MESCLAR_EM_UMA_LINHA = False
         else:
             print('Envie, uma string como caminho do parâmetro file_pdf')
             
         # --- CHROME OPTIONS --- #
         self._options = ChromeOptions()
         
-        # --- PATH BASE DIR --- #
-        self.get_text_into_code = get_text_into_code
-        
-        if get_text_into_code:
-            self.DOWNLOAD_DIR = cria_dir_no_dir_de_trabalho_atual('tempdir')
-        else:
-            self.DOWNLOAD_DIR =  cria_dir_no_dir_de_trabalho_atual(dir=dir_exit, print_value=False, criar_diretorio=True)
+        # --- PATH BASE DIR --- #        
+        self.DOWNLOAD_DIR = cria_dir_no_dir_de_trabalho_atual('tempdir')
+        limpa_diretorio('tempdir')
             
         self._SETTINGS_SAVE_AS_PDF = {
                     "recentDestinations": [
                         {
                             "id": "Save as PDF",
                             "origin": "local",
                             "account": ""
@@ -127,33 +122,29 @@
         self.WDW = WebDriverWait(self.DRIVER, timeout=3)
         self.WDW3 = WebDriverWait(self.DRIVER, timeout=3)
         self.WDW30 = WebDriverWait(self.DRIVER, timeout=30)
         self.WDW60 = WebDriverWait(self.DRIVER, timeout=60)
         self.WDW180 = WebDriverWait(self.DRIVER, timeout=180)
         self.DRIVER.maximize_window()
     
-    
+    # ----------------------------------------------------------------- #
         try:
             if prints:
                 print('Acessando o site...')
             self.DRIVER.get('https://online2pdf.com/pt/converter-pdf-para-txt-com-ocr')
             
             if prints:
                 print('Convertendo arquivo...')
 
             # Espera pelo elemento de enviar o arquivo
             self.WDW3.until(EC.presence_of_element_located((By.CSS_SELECTOR, '#input_file0')))
 
             # Envia o arquivo
             self.DRIVER.find_element(By.CSS_SELECTOR, '#input_file0').send_keys(self.FILE_PDF)
-                
-            if type_extract == 'docx':
-                espera_elemento_disponivel_e_clica(self.WDW3, (By.CSS_SELECTOR, '#selectbox_2 span'))
-                espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, '#selectbox_content[style*="display: block"] img[src*="word"]~span'))
-            
+
             # Clica em OCR Profundo
             try:
                 espera_elemento_disponivel_e_clica(self.WDW3, (By.CSS_SELECTOR, '#export_fullocr_box > label'))
             except (TimeoutException, NoSuchElementException):
                 pass
 
             # Clica em Converter
@@ -164,32 +155,26 @@
             
             # espera o elemento de completo
             try:
                 espera_elemento(self.WDW180, (By.CSS_SELECTOR, '#completed_window'))
             except TimeoutException:
                 raise Exception('Não foi possível fazer o OCR... Provavelmenten não encontrou nenhum texto.')
 
-            if type_extract == 'docx':
-                verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.docx')            
-            elif type_extract == 'text':
-                verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.txt')            
+            verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.txt')            
+            self.DRIVER.close()
         except Exception as e:
             print('Ocorreu um erro!')
             print(str(e))
             
 
             
     def recupera_texto(self) -> str:
-        if self.get_text_into_code:
-            try:
-                file_txts = arquivos_com_caminho_absoluto_do_arquivo(self.DOWNLOAD_DIR)
-                file_txt = file_txts[-1]
-                text = None
-                with open(file_txt, mode='r', encoding='utf-16-le') as f:
-                    text = f.read()
-                shutil.rmtree(self.DOWNLOAD_DIR)
-                return text
-            except IndexError:
-                raise FalhaAoRecuperarOcr('Ocorreu um erro na recuperação que causou um IndexError, provavelmente não baixou o arquivo.')
-
-    def retorna_o_docx(self) -> str:
-        return arquivos_com_caminho_absoluto_do_arquivo(self.DOWNLOAD_DIR)[-1]
+        try:
+            file_txts = arquivos_com_caminho_absoluto_do_arquivo(self.DOWNLOAD_DIR)
+            file_txt = file_txts[-1]
+            text = None
+            with open(file_txt, mode='r', encoding='utf-16-le') as f:
+                text = f.read()
+            shutil.rmtree(self.DOWNLOAD_DIR)
+            return text
+        except IndexError:
+            raise FalhaAoRecuperarOcr('Ocorreu um erro na recuperação que causou um IndexError, provavelmente não baixou o arquivo.')
```

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.0.0/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.0.0/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.0.0/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.3.0
+Version: 6.0.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.3.0/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.0.0/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 FuncsForSPO/fpdf/fcompress/compress.py
 FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
 FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
 FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
 FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
 FuncsForSPO/fpdf/focr/__init__.py
 FuncsForSPO/fpdf/focr/__ocr_online.py
+FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+FuncsForSPO/fpdf/focr/base.py
 FuncsForSPO/fpdf/focr/orc.py
 FuncsForSPO/fpdf/pdfutils/__init__.py
 FuncsForSPO/fpdf/pdfutils/pdfutils.py
 FuncsForSPO/fpysimplegui/__init__.py
 FuncsForSPO/fpysimplegui/functions_for_sg.py
 FuncsForSPO/fpython/__init__.py
 FuncsForSPO/fpython/functions_for_py.py
```

### Comparing `FuncsForSPO-5.3.0/LICENSE` & `FuncsForSPO-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/PKG-INFO` & `FuncsForSPO-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.3.0
+Version: 6.0.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.3.0/README.md` & `FuncsForSPO-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.3.0/setup.py` & `FuncsForSPO-6.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.3.0'
+version = '6.0.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
@@ -51,16 +51,20 @@
             'webdriver-manager',
             'requests',
             'pretty_html_table',
             'packaging',
             'PySimpleGUI',
             'macholib',
             'wget',
+            'alive-progress',
             'winotify',
             'pypdf',
             'pywin32',
+            'gdown',
+            'pytesseract',
+            'pymupdf',
             'PyPDF2',
             'sqlalchemy',
             'rich==12.6.0',
             'pyinstaller==5.6.2',
         ],
         )
```

