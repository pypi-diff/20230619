# Comparing `tmp/QPUIQ-0.2.3.tar.gz` & `tmp/QPUIQ-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.2.3.tar", last modified: Thu Jun  8 11:30:04 2023, max compression
+gzip compressed data, was "QPUIQ-0.2.4.tar", last modified: Mon Jun 19 04:17:46 2023, max compression
```

## Comparing `QPUIQ-0.2.3.tar` & `QPUIQ-0.2.4.tar`

### file list

```diff
@@ -1,83 +1,87 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.387673 QPUIQ-0.2.3/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     6129 2023-06-08 11:30:04.387538 QPUIQ-0.2.3/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.376302 QPUIQ-0.2.3/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.380125 QPUIQ-0.2.3/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)     1245 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      498 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     5469 2023-06-05 21:20:44.000000 QPUIQ-0.2.3/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      563 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2767 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      752 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     2331 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/combobox.py
--rw-r--r--   0 Bug        (504) staff       (20)      710 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      905 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      805 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/mdi.py
--rw-r--r--   0 Bug        (504) staff       (20)     2782 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/menu.py
--rw-r--r--   0 Bug        (504) staff       (20)      481 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      772 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     3806 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     1351 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/splitter.py
--rw-r--r--   0 Bug        (504) staff       (20)     1532 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/text.py
--rw-r--r--   0 Bug        (504) staff       (20)     1287 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     2239 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/PySide6/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      557 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      432 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     3607 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.382182 QPUIQ-0.2.3/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      703 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      588 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      848 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      549 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2067 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      634 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)      679 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1205 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      621 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      825 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     1665 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     1460 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      839 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      751 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     5588 2023-06-05 21:20:44.000000 QPUIQ-0.2.3/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)    13532 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/state.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.384901 QPUIQ-0.2.3/PUI/textual/
--rw-r--r--   0 Bug        (504) staff       (20)      955 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     1952 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/textual/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     2952 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      437 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      519 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     1300 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1501 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      502 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      622 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     1612 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      388 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      742 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      381 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/textual/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.386847 QPUIQ-0.2.3/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      692 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      729 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     2416 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      469 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1129 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      746 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)      538 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     2704 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      490 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      699 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     3671 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      391 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      860 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1550 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/tkinter/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      505 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/PUI/utils.py
--rw-r--r--   0 Bug        (504) staff       (20)     2929 2023-06-08 11:30:01.000000 QPUIQ-0.2.3/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-08 11:30:04.387348 QPUIQ-0.2.3/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     6129 2023-06-08 11:30:04.000000 QPUIQ-0.2.3/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1579 2023-06-08 11:30:04.000000 QPUIQ-0.2.3/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-06-08 11:30:04.000000 QPUIQ-0.2.3/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-06-08 11:30:04.000000 QPUIQ-0.2.3/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     5869 2023-06-05 21:20:44.000000 QPUIQ-0.2.3/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-06-08 11:30:04.387714 QPUIQ-0.2.3/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-06-05 21:02:12.000000 QPUIQ-0.2.3/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.499378 QPUIQ-0.2.4/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     7141 2023-06-19 04:17:46.499244 QPUIQ-0.2.4/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.488068 QPUIQ-0.2.4/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.491257 QPUIQ-0.2.4/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)      860 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      496 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5105 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      561 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2765 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2327 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/combobox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      708 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1561 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      801 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/mdi.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2780 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/menu.py
+-rw-r--r--   0 Bug        (504) staff       (20)      479 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      770 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2903 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      793 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/splitter.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1192 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1418 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1286 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1899 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/PySide6/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      557 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      432 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3705 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.493844 QPUIQ-0.2.4/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      421 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      587 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      848 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      540 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2066 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      633 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      678 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1201 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      620 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      830 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1664 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1003 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1457 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      838 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5593 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)    13538 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/state.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.496247 QPUIQ-0.2.4/PUI/textual/
+-rw-r--r--   0 Bug        (504) staff       (20)      685 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2144 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2950 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      436 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      518 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1548 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      501 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      621 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1611 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2280 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)      473 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      785 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      380 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/textual/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.498522 QPUIQ-0.2.4/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      495 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      951 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2416 2023-06-08 11:30:01.000000 QPUIQ-0.2.4/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      467 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1127 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      741 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      536 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2698 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      488 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3669 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1743 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)      475 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      862 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1548 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/PUI/tkinter/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      505 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/PUI/utils.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2929 2023-06-08 11:30:01.000000 QPUIQ-0.2.4/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-06-19 04:17:46.499053 QPUIQ-0.2.4/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     7141 2023-06-19 04:17:46.000000 QPUIQ-0.2.4/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1652 2023-06-19 04:17:46.000000 QPUIQ-0.2.4/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-06-19 04:17:46.000000 QPUIQ-0.2.4/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-06-19 04:17:46.000000 QPUIQ-0.2.4/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     6881 2023-06-19 04:17:18.000000 QPUIQ-0.2.4/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-06-19 04:17:46.499414 QPUIQ-0.2.4/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-06-05 21:02:12.000000 QPUIQ-0.2.4/setup.py
```

### Comparing `QPUIQ-0.2.3/LICENSE.txt` & `QPUIQ-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.3/PUI/PySide6/base.py` & `QPUIQ-0.2.4/PUI/PySide6/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     StyleSheet = node.qt_params.get("StyleSheet", {})
     for k,v in StyleSheet.items():
         styles[k] = v
 
     if hasattr(ui, "setStyleSheet"):
         ui.setStyleSheet("".join([f"{k}:{v};" for k,v in styles.items()]))
 
+    if node.layout_padding:
+        ui.setContentsMargins(*trbl2ltrb(node.layout_padding))
+
 class QPUIView(PUIView):
     def __init__(self):
         super().__init__()
         self.qt_params = {}
         self.signal = QtViewSignal()
         self.signal.redraw.connect(self.update)
 
@@ -92,92 +95,82 @@
         return self
 
 class QtBaseLayout(PUINode):
     def __init__(self):
         super().__init__()
         self.qt_params = {}
 
+    @property
+    def outer(self):
+        return self.ui
+
+    @property
+    def inner(self):
+        return self.layout
+
     def destroy(self, direct):
         if direct:
+            self.layout.setParent(None)
+            self.layout.deleteLater()
             self.ui.deleteLater()
+        self.layout = None
         self.ui = None
         super().destroy(direct)
 
     def update(self, prev=None):
         super().update(prev)
         _apply_params(self.ui, self)
 
     def addChild(self, idx, child):
-        from .layout import QtSpacerItem
-        if isinstance(child, QtBaseLayout):
-            params = {}
-            if not child.layout_weight is None:
-                params["stretch"] = child.layout_weight
-            self.ui.insertLayout(idx, child.outer, **params)
-        elif isinstance(child, QtSpacerItem):
-            self.ui.insertItem(idx, child.outer)
-        elif isinstance(child, QtBaseWidget):
+        from .layout import Spacer
+        if isinstance(child, Spacer):
+            self.layout.insertItem(idx, child.outer)
+        elif isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             params = {}
             if not child.layout_weight is None:
                 params["stretch"] = child.layout_weight
-            self.ui.insertWidget(idx, child.ui, **params)
+            self.layout.insertWidget(idx, child.outer, **params)
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
-        from .layout import QtSpacerItem
-        if isinstance(child, QtBaseLayout):
-            self.ui.removeItem(child.outer)
-        elif isinstance(child, QtSpacerItem):
-            self.ui.removeItem(child.outer)
-        elif isinstance(child, QtBaseWidget):
-            child.ui.setParent(None)
+        from .layout import Spacer
+        if isinstance(child, Spacer):
+            self.layout.removeItem(child.outer)
+        elif isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
+            child.outer.setParent(None)
         elif child.children:
             self.removeChild(idx, child.children[0])
 
     def qt(self, **kwargs):
         for k,v in kwargs.items():
             self.qt_params[k] = v
         return self
 
 class QtBaseFrame(QtBaseWidget):
     terminal = False
 
-    def __init__(self):
-        self.widget = None
-        super().__init__()
-
     def destroy(self, direct):
         if direct:
             if self.ui:
                 self.ui.deleteLater()
                 self.ui = None
-            if self.widget:
-                self.widget.deleteLater()
-                self.widget = None
 
     def addChild(self, idx, child):
         if idx != 0:
             return
-        if isinstance(child, QtBaseLayout):
-            self.widget = QtWidgets.QWidget()
-            self.ui.setWidget(self.widget)
-            self.widget.setLayout(child.outer)
-        elif isinstance(child, QtBaseWidget):
+        if isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             self.ui.setWidget(child.outer)
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if idx != 0:
             return
-        if isinstance(child, QtBaseLayout):
-            child.outer.setParent(None)
-            self.widget.setParent(None)
-        elif isinstance(child, QtBaseWidget):
+        if isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             child.outer.setParent(None)
         elif child.children:
             self.removeChild(idx, child.children[0])
 
 class QtWrapper(QtBaseWidget):
     def __init__(self, widget, *args):
         super().__init__(*args)
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/button.py` & `QPUIQ-0.2.4/PUI/PySide6/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class QtButton(QtBaseWidget):
+class Button(QtBaseWidget):
     def __init__(self, text):
         super().__init__()
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/canvas.py` & `QPUIQ-0.2.4/PUI/PySide6/canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             self.node.qpainter.fillRect(rect, bgBrush)
 
         self.node.painter(self.node, *self.node.args)
 
         self.node.qpainter.end()
         self.node.qpainter = None
 
-class QtCanvas(QtBaseWidget):
+class Canvas(QtBaseWidget):
     def __init__(self, painter, *args):
         super().__init__()
         self.ui = None
         self.painter = painter
         self.args = args
 
     def update(self, prev):
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/checkbox.py` & `QPUIQ-0.2.4/PUI/PySide6/checkbox.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .. import *
 from .base import *
 from ..utils import *
 from PySide6.QtWidgets import QSizePolicy
 
-class QtCheckbox(QtBaseWidget):
+class Checkbox(QtBaseWidget):
     def __init__(self, text, model):
         super().__init__()
         self.text = text
         self.model = model
 
     def update(self, prev):
         if prev and prev.ui:
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/combobox.py` & `QPUIQ-0.2.4/PUI/PySide6/combobox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class QtComboBox(QtBaseWidget):
+class ComboBox(QtBaseWidget):
     terminal = False
     def __init__(self, editable=False, index_model=None, text_model=None):
         super().__init__()
         self.editable = editable
         if index_model is None:
             index_model = DummyBinding(0)
         if text_model is None:
@@ -59,11 +59,11 @@
 
     def addChild(self, idx, child):
         self.ui.insertItem(idx, child.text)
 
     def removeChild(self, idx, child):
         self.ui.removeItem(idx)
 
-class QtComboBoxItem(PUINode):
+class ComboBoxItem(PUINode):
     def __init__(self, text):
         super().__init__()
         self.text = text
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/label.py` & `QPUIQ-0.2.4/PUI/PySide6/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class ClickableQLabel(QtWidgets.QLabel):
     clicked  = QtCore.Signal()
 
     def mousePressEvent(self, ev):
         self.clicked.emit()
 
-class QtLabel(QtBaseWidget):
+class Label(QtBaseWidget):
     def __init__(self, text):
         super().__init__()
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/layout.py` & `QPUIQ-0.2.4/PUI/flet/button.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,20 @@
 from .. import *
 from .base import *
 
-class QtHBox(QtBaseLayout):
-    def update(self, prev):
-        if prev and prev.ui:
-            self.ui = prev.ui
-        else:
-            self.ui = QtWidgets.QHBoxLayout()
-        super().update(prev)
+class Button(FBase):
+    def __init__(self, text):
+        super().__init__()
+        self.text = text
 
-class QtVBox(QtBaseLayout):
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
+            self.ui.text = self.text
+            self.ui.on_click = self._clicked
+            try:
+                self.ui.update()
+            except:
+                pass
         else:
-            self.ui = QtWidgets.QVBoxLayout()
-        super().update(prev)
-
-class QtSpacerItem(PUINode):
-    terminal = True
-
-    def update(self, prev):
-        if prev and prev.ui:
-            self.ui = prev.ui
-        else:
-            self.ui = QtWidgets.QSpacerItem(0, 0, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        super().update(prev)
-
-    def destroy(self, direct):
-        # self.ui.deleteLater() # QSpacerItem doesn't have .deleteLater()
-        self.ui = None
-        super().destroy(direct)
+            self.ui = ft.ElevatedButton(text=self.text, on_click=self._clicked)
+        self.ui.expand = self.layout_weight
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/mdi.py` & `QPUIQ-0.2.4/PUI/PySide6/mdi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class QtMdiArea(QtBaseWidget):
+class MdiArea(QtBaseWidget):
     terminal = False
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QMdiArea()
 
@@ -19,15 +19,15 @@
 
     def addSubWindow(self, child):
         self.ui.addSubWindow(child.outer)
 
     def removeSubWindow(self, child):
         self.ui.removeSubWindow(child.outer)
 
-class QtMdiSubWindow(QtBaseFrame):
+class MdiSubWindow(QtBaseFrame):
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QMdiSubWindow()
 
         super().update(prev)
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/menu.py` & `QPUIQ-0.2.4/PUI/PySide6/menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from .. import *
 from .base import *
 
-class QtMenuBar(PUINode):
+class MenuBar(PUINode):
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
             self.actions = prev.actions
         else:
             self.ui = QtWidgets.QMenuBar()
             self.actions = []
 
         super().update(prev)
 
     def addChild(self, idx, child):
         if idx < len(self.actions):
-            if isinstance(child, QtMenu):
+            if isinstance(child, Menu):
                 self.actions.insert(idx, self.ui.insertMenu(self.actions[idx], child.outer))
-            elif isinstance(child, QtAction):
+            elif isinstance(child, MenuAction):
                 self.actions.insert(idx, self.ui.insertAction(self.actions[idx], child.outer))
         else:
-            if isinstance(child, QtMenu):
+            if isinstance(child, Menu):
                 self.actions.append(self.ui.addMenu(child.outer))
-            elif isinstance(child, QtAction):
+            elif isinstance(child, MenuAction):
                 self.actions.append(self.ui.addAction(child.outer))
 
     def removeChild(self, idx, child):
         self.ui.removeAction(self.actions[idx])
 
-class QtMenu(PUINode):
+class Menu(PUINode):
     def __init__(self, text):
         super().__init__()
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
@@ -41,28 +41,28 @@
             self.ui = QtWidgets.QMenu(self.text)
             self.actions = []
 
         super().update(prev)
 
     def addChild(self, idx, child):
         if idx < len(self.actions):
-            if isinstance(child, QtMenu):
+            if isinstance(child, Menu):
                 self.actions.insert(idx, self.ui.insertMenu(self.actions[idx], child.outer))
-            elif isinstance(child, QtAction):
+            elif isinstance(child, MenuAction):
                 self.actions.insert(idx, self.ui.insertAction(self.actions[idx], child.outer))
         else:
-            if isinstance(child, QtMenu):
+            if isinstance(child, Menu):
                 self.actions.append(self.ui.addMenu(child.outer))
-            elif isinstance(child, QtAction):
+            elif isinstance(child, MenuAction):
                 self.actions.append(self.ui.addAction(child.outer))
 
     def removeChild(self, idx, child):
         self.ui.removeAction(self.actions[idx])
 
-class QtAction(PUINode):
+class MenuAction(PUINode):
     def __init__(self, text):
         super().__init__()
         self.text = text
         self.onTriggered = None
 
     def update(self, prev):
         if prev and prev.ui:
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/radiobutton.py` & `QPUIQ-0.2.4/PUI/PySide6/radiobutton.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .. import *
 from .base import *
 from ..utils import *
 from PySide6.QtWidgets import QSizePolicy
 
-class QtRadioButton(QtBaseWidget):
+class RadioButton(QtBaseWidget):
     def __init__(self, text, value, model):
         super().__init__()
         self.text = text
         self.value = value
         self.model = model
 
     def update(self, prev):
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/scroll.py` & `QPUIQ-0.2.4/PUI/PySide6/scroll.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 from .. import *
 from .base import *
 from PySide6.QtWidgets import QSizePolicy
 
-class QtScrollArea(QtBaseWidget):
+class Scroll(QtBaseWidget):
     terminal = False
 
     def __init__(self, vertical=None, horizontal=False):
         self.vertical = vertical
         self.horizontal = horizontal
         super().__init__()
 
-    def destroy(self, direct):
-        if direct:
-            if self.widget:
-                self.widget.deleteLater()
-                self.widget = None
-        super().destroy(direct)
-
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
-            self.widget = prev.widget
         else:
             self.ui = QtWidgets.QScrollArea()
             self.ui.setWidgetResizable(True)
-            self.widget = None
             if self.vertical is None:
                 self.ui.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAsNeeded)
             elif self.vertical:
                 self.ui.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOn)
             else:
                 self.ui.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
             if self.horizontal is None:
@@ -38,56 +29,40 @@
             else:
                 self.ui.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
         super().update(prev)
 
     def addChild(self, idx, child):
         if idx != 0:
             return
-        if isinstance(child, QtBaseLayout):
-            self.widget = QtWidgets.QWidget()
-            self.ui.setWidget(self.widget)
-            self.widget.setLayout(child.outer)
-            if not hasattr(self.widget, "origResizeEvent"):
-                self.widget.origResizeEvent = self.widget.resizeEvent
-            self.widget.resizeEvent = self.onUiResized
-        elif isinstance(child, QtBaseWidget):
+        if isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             self.ui.setWidget(child.outer)
             if not hasattr(child.outer, "origResizeEvent"):
                 child.outer.origResizeEvent = child.outer.resizeEvent
             child.outer.resizeEvent = self.onUiResized
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if idx != 0:
             return
-        if isinstance(child, QtBaseLayout):
-            child.outer.setParent(None)
-            self.widget.setParent(None)
-            self.widget.deleteLater()
-            self.widget = None
-        elif isinstance(child, QtBaseWidget):
+        if isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             child.outer.setParent(None)
         elif child.children:
             self.removeChild(idx, child.children[0])
 
     def onUiResized(self, event):
         node = self.get_node()
         if node.destroyed:
             return
-        if node.widget:
-            node.widget.origResizeEvent(event)
-            node.widget.resizeEvent = self.onUiResized
-        else:
-            node.children[0].outer.origResizeEvent(event)
-            node.children[0].outer.resizeEvent = self.onUiResized
+        node.children[0].outer.origResizeEvent(event)
+        node.children[0].outer.resizeEvent = self.onUiResized
         if node.horizontal is False:
             if isinstance(node.children[0], QtBaseLayout):
                 node.outer.setMinimumWidth(node.children[0].outer.sizeHint().width())
             elif isinstance(node.children[0], QtBaseWidget):
                 node.outer.setMinimumWidth(node.children[0].outer.sizeHint().width())
 
         if node.vertical is False:
             if isinstance(node.children[0], QtBaseLayout):
                 node.outer.setMinimumHeight(node.children[0].outer.sizeHint().height())
             elif isinstance(node.children[0], QtBaseWidget):
-                self.outer.setMinimumHeight(self.children[0].outer.sizeHint().height())
+                self.outer.setMinimumHeight(node.children[0].outer.sizeHint().height())
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/splitter.py` & `QPUIQ-0.2.4/PUI/flet/scroll.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,60 @@
 from .. import *
 from .base import *
 
-class QtSplitter(QtBaseWidget):
-    terminal = False
-    def __init__(self, vertical=False):
-        super().__init__()
+class Scroll(FBase):
+    def __init__(self, vertical=None, horizontal=False):
         self.vertical = vertical
-
-    def destroy(self, direct):
-        if direct:
-            for frame in self.frame:
-                if frame:
-                    frame.deleteLater()
-        super().destroy(direct)
+        self.horizontal = horizontal
+        self.widget = None
+        super().__init__()
+        self.layout_weight = 1
 
     def update(self, prev):
-        if prev and prev.ui:
-            self.ui = prev.ui
-            self.frame = prev.frame
+        if prev and hasattr(prev, "hframe"):
+            self.vframe = prev.vframe
+            self.hframe = prev.hframe
+        else:
+            self.vframe = ft.Column() # outer
+            self.hframe = ft.Row() # inner
+            self.vframe.controls.append(self.hframe)
+        self.vframe.expand = self.layout_weight
+        if self.vertical is None:
+            self.vframe.scroll = ft.ScrollMode.AUTO
+        elif self.vertical:
+            self.vframe.scroll = ft.ScrollMode.ADAPTIVE
+        else:
+            self.vframe.scroll = None
+        if self.horizontal is None:
+            self.hframe.scroll = ft.ScrollMode.AUTO
+        elif self.horizontal:
+            self.hframe.scroll = ft.ScrollMode.ADAPTIVE
         else:
-            self.ui = QtWidgets.QSplitter()
-            self.frame = []
-        self.ui.setOrientation(QtCore.Qt.Orientation.Vertical if self.vertical else QtCore.Qt.Orientation.Horizontal)
+            self.hframe.scroll = None
+        try:
+            self.vframe.update()
+        except:
+            pass
         super().update(prev)
 
     def addChild(self, idx, child):
-        if isinstance(child, QtBaseLayout):
-            frame = QtWidgets.QWidget()
-            frame.setLayout(child.outer)
-            self.frame.insert(idx, frame)
-            self.ui.insertWidget(idx, frame)
-        elif isinstance(child, QtBaseWidget):
-            self.ui.insertWidget(idx, child.outer)
-            self.frame.insert(idx, None)
-        else:
-            self.addChild(idx, child.children[0])
-    
+        if idx != 0:
+            return
+        self.hframe.controls.insert(idx, child.outer)
+        try:
+            self.hframe.update()
+        except:
+            pass
+
     def removeChild(self, idx, child):
-        child.outer.setParent(None)
-        frame = self.frame.pop(idx)
-        if frame:
-            frame.deleteLater()
+        if idx != 0:
+            return
+        self.hframe.controls.pop(idx)
+        self.hframe.update()
+
+    @property
+    def outer(self):
+        return self.vframe
+
+    @property
+    def inner(self):
+        return self.hframe
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/text.py` & `QPUIQ-0.2.4/PUI/PySide6/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return QtCore.QSize(*self._sizehint)
     
     def setSizeHint(self, sizeHint):
         if sizeHint != self._sizehint:
             self._sizehint = sizeHint
             self.adjustSize()
 
-class QtText(QtBaseWidget):
+class Text(QtBaseWidget):
     textformat = QtCore.Qt.TextFormat.PlainText
     def __init__(self, text, sizeHint=(120,320)):
         super().__init__()
         self.text = text
         self.sizeHint = sizeHint
 
     def update(self, prev):
@@ -33,18 +33,16 @@
             self.ui.setSizeHint(self.sizeHint)
         else:
             self.ui = QText(self.text, self.sizeHint)
             self.ui.setTextFormat(self.textformat)
             self.ui.setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
             self.ui.setWordWrap(True)
             self.ui.setSizePolicy(QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Ignored))
-        if self.layout_padding:
-            self.ui.setContentsMargins(*trbl2ltrb(self.layout_padding))
 
         super().update(prev)
 
 
-class QtHtml(QtText):
+class Html(Text):
     textformat = QtCore.Qt.TextFormat.RichText
 
-class QtMarkDown(QtText):
+class MarkDown(Text):
     textformat = QtCore.Qt.TextFormat.MarkdownText
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/textfield.py` & `QPUIQ-0.2.4/PUI/PySide6/textfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class QtLineEdit(QtBaseWidget):
+class TextField(QtBaseWidget):
     def __init__(self, model):
         super().__init__()
         self.model = model
         self.editing = False
 
     def update(self, prev):
         value = self.model.value
```

### Comparing `QPUIQ-0.2.3/PUI/PySide6/window.py` & `QPUIQ-0.2.4/PUI/PySide6/window.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .. import *
 from .base import *
 from .menu import *
 
-class QtWindow(QtBaseWidget):
+class Window(QtBaseWidget):
     terminal = False
 
     def __init__(self, title=None, size=None, maximize=None, fullscreen=None):
         super().__init__()
         self.title = title
         self.size = size
         self.curr_size = None
@@ -14,22 +14,20 @@
         self.curr_maximize = None
         self.fullscreen = fullscreen
         self.curr_fullscreen = None
 
     def update(self, prev=None):
         if prev and prev.ui:
             self.ui = prev.ui
-            self.frame = prev.frame
             self.curr_size = prev.curr_size
             self.curr_maximize = prev.curr_maximize
             self.curr_fullscreen = prev.curr_fullscreen
         else:
             from PySide6 import QtWidgets
             self.ui = QtWidgets.QMainWindow()
-            self.frame = None
 
         if self.curr_size != self.size:
             self.curr_size = self.size
             self.ui.resize(*self.size)
         if self.curr_maximize !=  self.maximize:
             self.curr_maximize = self.maximize
             self.ui.showMaximized()
@@ -37,29 +35,21 @@
             self.curr_fullscreen = self.fullscreen
             self.ui.showFullScreen()
         if not self.title is None:
             self.ui.setWindowTitle(self.title)
         super().update(prev)
 
     def addChild(self, idx, child):
-        if isinstance(child, QtMenuBar):
+        if isinstance(child, MenuBar):
             self.ui.setMenuBar(child.outer)
-        elif isinstance(child, QtBaseLayout):
-            self.frame = QtWidgets.QWidget()
-            self.ui.setCentralWidget(self.frame)
-            self.frame.setLayout(child.outer)
-        elif isinstance(child, QtBaseWidget):
+        elif isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             self.ui.setCentralWidget(child.outer)
         else:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
-        if isinstance(child, QtMenuBar):
+        if isinstance(child, MenuBar):
             child.outer.close()
-        elif isinstance(child, QtBaseLayout):
-            self.frame.setParent(None)
-            self.frame.deleteLater()
-            self.frame = None
-        elif isinstance(child, QtBaseWidget):
+        elif isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             child.outer.setParent(None)
         else:
             self.removeChild(idx, child.children[0])
```

### Comparing `QPUIQ-0.2.3/PUI/__init__.py` & `QPUIQ-0.2.4/PUI/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 from .node import *
 from .view import *
 from .state import *
 from .timeline import *
 from .decorator import *
```

### Comparing `QPUIQ-0.2.3/PUI/dom.py` & `QPUIQ-0.2.4/PUI/dom.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,32 @@
                 trimmed = True
 
             if trimmed:
                 continue # restart
 
             try: # node exists
                 idx = oldMap[i+1:].index(new.key)+i+1
+            except ValueError:
+                idx = None
+            if idx is None: # new node
+                try:
+                    new.update(None)
+                except:
+                    import traceback
+                    print("## <ERROR OF update() >")
+                    print(new.key)
+                    traceback.print_exc()
+                    print("## </ERROR OF update()>")
+                if not new.terminal:
+                    sync(new, [], new.children)
+                node.addChild(i, new)
+                oldDOM.insert(i, None) # placeholder
+                oldMap.insert(i, new.key)
+
+            else: # existed node
                 if idx==i+1: # move wrong node
                     oldMap.pop(i)
                     old = oldDOM.pop(i)
                     node.removeChild(i, old)
 
                     node.addChild(len(oldDOM), old)
                     oldMap.append(old.key)
@@ -81,30 +99,14 @@
 
                     if not new.terminal:
                         sync(new, old.children, new.children)
 
                     node.addChild(i, new)
                     oldDOM.insert(i, None) # placeholder
                     oldMap.insert(i, new.key)
-
-            except: # new node
-                try:
-                    new.update(None)
-                except:
-                    import traceback
-                    print("## <ERROR OF update() >")
-                    print(new.key)
-                    traceback.print_exc()
-                    print("## </ERROR OF update()>")
-                if not new.terminal:
-                    sync(new, [], new.children)
-                node.addChild(i, new)
-                oldDOM.insert(i, None) # placeholder
-                oldMap.insert(i, new.key)
-
             break # finish
 
     nl = len(newDOM)
     while len(oldDOM) > nl:
         old = oldDOM.pop(nl)
         oldMap.pop(nl)
         node.removeChild(nl, old)
```

### Comparing `QPUIQ-0.2.3/PUI/flet/__init__.py` & `QPUIQ-0.2.4/PUI/textual/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from .application import *
 from .button import *
-from .canvas import *
 from .checkbox import *
 from .label import *
 from .layout import *
 from .progressbar import *
 from .radiobutton import *
 from .scroll import *
+from .tab import *
 from .text import *
 from .textfield import *
 from .window import *
 from .. import NotImplementedNode
 
-Application = FApplication
-Window = FWindow
-HBox = FRow
-VBox = FColumn
-Label = FLabel
-Button = FElevatedButton
-Checkbox = FCheckbox
-RadioButton = FRadio
-Canvas = FCanvas
-TextField = FTextField
-ProgressBar = FProgressBar
-Scroll = FScroll
-Spacer = FSpacer
-Text = FText
-Html = FHtml
-MarkDown = FMarkDown
-Combobox = NotImplementedNode
-ComboboxItem = NotImplementedNode
+class DummyWidget(TBase):
+    supported = False
+    def __init__(self, *args, **kwrgas):
+        super().__init__()
 
-PUI_BACKEND = "flet"
+    def update(self, prev):
+        if prev and prev.ui:
+            self.ui = prev.ui
+        else:
+            self.ui = widgets.Label("Not Implemented")
+
+
+
+Canvas = DummyWidget
+Combobox = DummyWidget
+ComboboxItem = DummyWidget
+
+PUI_BACKEND = "textual"
```

### Comparing `QPUIQ-0.2.3/PUI/flet/application.py` & `QPUIQ-0.2.4/PUI/flet/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class FApplication(PUIView):
+class Application(PUIView):
     def __init__(self):
         super().__init__()
         self.ready = False
 
     def update(self, prev=None):
         if not self.ready:
             return
```

### Comparing `QPUIQ-0.2.3/PUI/flet/base.py` & `QPUIQ-0.2.4/PUI/flet/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.3/PUI/flet/button.py` & `QPUIQ-0.2.4/PUI/flet/label.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from .. import *
 from .base import *
 
-class FElevatedButton(FBase):
-    def __init__(self, text):
-        super().__init__()
+class Label(FBase):
+    def __init__(self, text, **kwargs):
+        super().__init__(**kwargs)
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
-            self.ui.text = self.text
-            self.ui.on_click = self._clicked
-            try:
-                self.ui.update()
-            except:
-                pass
         else:
-            self.ui = ft.ElevatedButton(text=self.text, on_click=self._clicked)
+            self.ui = ft.Text(spans=[])
         self.ui.expand = self.layout_weight
+        if self.onClicked:
+            self.ui.spans = [
+                ft.TextSpan(self.text, on_click=self._clicked)
+            ]
+        else:
+            self.ui.spans = [
+                ft.TextSpan(self.text)
+            ]
+        try:
+            self.ui.update()
+        except:
+            pass
+        super().update(prev)
```

### Comparing `QPUIQ-0.2.3/PUI/flet/canvas.py` & `QPUIQ-0.2.4/PUI/flet/canvas.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .. import *
 from .base import *
 import flet.canvas as cv
 
-class FCanvas(FBase):
+class Canvas(FBase):
     def __init__(self, painter, *args):
         super().__init__()
         self.ui = None
         self.painter = painter
         self.args = args
 
     def update(self, prev):
```

### Comparing `QPUIQ-0.2.3/PUI/flet/checkbox.py` & `QPUIQ-0.2.4/PUI/flet/checkbox.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class FCheckbox(FBase):
+class Checkbox(FBase):
     def __init__(self, text, model):
         super().__init__()
         self.text = text
         self.model = model
 
     def update(self, prev):
         if prev and prev.ui:
```

### Comparing `QPUIQ-0.2.3/PUI/flet/layout.py` & `QPUIQ-0.2.4/PUI/flet/layout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class FRow(FBase):
+class HBox(FBase):
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = ft.Row()
         self.ui.expand = self.layout_weight
         super().update(prev)
@@ -17,15 +17,15 @@
         except:
             pass
 
     def removeChild(self, idx, child):
         self.ui.controls.pop(idx)
         self.ui.update()
 
-class FColumn(FBase):
+class VBox(FBase):
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = ft.Column()
         self.ui.expand = self.layout_weight
         super().update(prev)
@@ -37,14 +37,14 @@
         except:
             pass
 
     def removeChild(self, idx, child):
         self.ui.controls.pop(idx)
         self.ui.update()
 
-class FSpacer(FBase):
+class Spacer(FBase):
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = ft.Container()
         super().update(prev)
```

### Comparing `QPUIQ-0.2.3/PUI/flet/progressbar.py` & `QPUIQ-0.2.4/PUI/flet/progressbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class FProgressBar(FBase):
+class ProgressBar(FBase):
     def __init__(self, progress, maximum=100):
         super().__init__()
         self.progress = progress
         self.maximum = maximum
 
     def update(self, prev):
         if prev and prev.ui:
```

### Comparing `QPUIQ-0.2.3/PUI/flet/radiobutton.py` & `QPUIQ-0.2.4/PUI/flet/radiobutton.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class FRadio(FBase):
+class RadioButton(FBase):
     def __init__(self, text, value, model):
         super().__init__()
         self.text = text
         self.value = value
         self.model = model
 
     def update(self, prev):
```

### Comparing `QPUIQ-0.2.3/PUI/flet/scroll.py` & `QPUIQ-0.2.4/PUI/flet/text.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 from .. import *
 from .base import *
 
-class FScroll(FBase):
-    def __init__(self, vertical=None, horizontal=False):
-        self.vertical = vertical
-        self.horizontal = horizontal
-        self.widget = None
-        super().__init__()
-        self.layout_weight = 1
+class Text(FBase):
+    def __init__(self, text, **kwargs):
+        super().__init__(**kwargs)
+        self.text = text
 
     def update(self, prev):
-        if prev and hasattr(prev, "hframe"):
-            self.vframe = prev.vframe
-            self.hframe = prev.hframe
+        if prev and prev.ui:
+            self.ui = prev.ui
+            self.ui.value = self.text
+            try:
+                self.ui.update()
+            except:
+                pass
         else:
-            self.vframe = ft.Column() # outer
-            self.hframe = ft.Row() # inner
-            self.vframe.controls.append(self.hframe)
-        self.vframe.expand = self.layout_weight
-        if self.vertical is None:
-            self.vframe.scroll = ft.ScrollMode.AUTO
-        elif self.vertical:
-            self.vframe.scroll = ft.ScrollMode.ADAPTIVE
-        else:
-            self.vframe.scroll = None
-        if self.horizontal is None:
-            self.hframe.scroll = ft.ScrollMode.AUTO
-        elif self.horizontal:
-            self.hframe.scroll = ft.ScrollMode.ADAPTIVE
+            self.ui = ft.Text(self.text, expand=self.layout_weight)
+        super().update(prev)
+
+class Html(FBase):
+    supported = False
+    def __init__(self, text, **kwargs):
+        super().__init__(**kwargs)
+        self.text = text
+
+    def update(self, prev):
+        if prev and prev.ui:
+            self.ui = prev.ui
+            self.ui.value = self.text
+            try:
+                self.ui.update()
+            except:
+                pass
         else:
-            self.hframe.scroll = None
-        try:
-            self.vframe.update()
-        except:
-            pass
+            self.ui = ft.Text(self.text, expand=self.layout_weight)
         super().update(prev)
 
-    def addChild(self, idx, child):
-        if idx != 0:
-            return
-        self.hframe.controls.insert(idx, child.outer)
-        try:
-            self.hframe.update()
-        except:
-            pass
-
-    def removeChild(self, idx, child):
-        if idx != 0:
-            return
-        self.hframe.controls.pop(idx)
-        self.hframe.update()
-
-    @property
-    def outer(self):
-        return self.vframe
-
-    @property
-    def inner(self):
-        return self.hframe
+class MarkDown(FBase):
+    supported = False
+    def __init__(self, text, **kwargs):
+        super().__init__(**kwargs)
+        self.text = text
+
+    def update(self, prev):
+        if prev and prev.ui:
+            self.ui = prev.ui
+            self.ui.value = self.text
+            try:
+                self.ui.update()
+            except:
+                pass
+        else:
+            self.ui = ft.Markdown(self.text, expand=self.layout_weight, auto_follow_links=True)
+        super().update(prev)
```

### Comparing `QPUIQ-0.2.3/PUI/flet/textfield.py` & `QPUIQ-0.2.4/PUI/flet/textfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class FTextField(FBase):
+class TextField(FBase):
     def __init__(self, model, label="", **kwargs):
         super().__init__(**kwargs)
         self.model = model
         self.label = label
 
     def update(self, prev):
         value = self.model.value
```

### Comparing `QPUIQ-0.2.3/PUI/flet/window.py` & `QPUIQ-0.2.4/PUI/flet/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class FWindow(FBase):
+class Window(FBase):
     def __init__(self, title=None, size=None, maximize=None, fullscreen=None):
         super().__init__()
         self.title = title
         self.size = size
         self.curr_size = None
         self.maximize = maximize
         self.curr_maximize = None
```

### Comparing `QPUIQ-0.2.3/PUI/node.py` & `QPUIQ-0.2.4/PUI/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,12 +203,12 @@
 
     def flet(self, **kwargs):
         return self
 
     def textual(self, **kwargs):
         return self
 
-    def tk(self, **kwargs):
+    def tkinter(self, **kwargs):
         return self
 
     def qt(self, **kwargs):
         return self
```

### Comparing `QPUIQ-0.2.3/PUI/state.py` & `QPUIQ-0.2.4/PUI/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 def _notify(listeners):
     tbd = []
     for l in listeners:
         if l.retired_by:
             tbd.append(l)
     for l in tbd:
         listeners.remove(l)
-    for l in listeners:
+    for l in list(listeners):
         l.redraw()
 
 class BaseState():
     pass
 
 def State(data=None):
     if data is None:
```

### Comparing `QPUIQ-0.2.3/PUI/textual/application.py` & `QPUIQ-0.2.4/PUI/textual/application.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from typing import Type
 from textual.driver import Driver
 from .. import *
 from .base import *
 from textual.app import App, CSSPathType, ComposeResult
 from textual.containers import Vertical
-from textual.widgets import Button, Checkbox, Input, RadioButton
+from textual.widgets import Button, Checkbox, Input, RadioButton, Tabs
 
 class PUIApp(App):
 
     def __init__(self, puiview, driver_class: Type[Driver] | None = None, css_path: CSSPathType | None = None, watch_css: bool = False):
         super().__init__(driver_class, css_path, watch_css)
         self.puiview = puiview
 
     def on_mount(self) -> None:
         self.puiview.redraw()
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
-        event.button.puinode._clicked()
+        event.button.puinode.get_node()._clicked()
 
     def on_radio_button_changed(self, event: RadioButton.Changed) -> None:
-        event.radio_button.puinode._changed(event.value)
+        event.radio_button.puinode.get_node()._changed(event.value)
 
     def on_input_changed(self, event: Input.Changed) -> None:
-        event.input.puinode._changed(event.value)
+        event.input.puinode.get_node()._changed(event.value)
 
     def on_input_submitted(self, event: Input.Submitted) -> None:
-        event.input.puinode._submitted(event.value)
+        event.input.puinode.get_node()._submitted(event.value)
 
     def on_checkbox_changed(self, event: Checkbox.Changed) -> None:
-        event.checkbox.puinode._changed(event.value)
+        event.checkbox.puinode.get_node()._changed(event.value)
+
+    def on_tabs_tab_activated(self, event: Tabs.TabActivated) -> None:
+        event.tabs.puinode.get_node()._tab_activated(event)
 
     def compose(self) -> ComposeResult:
         yield Vertical(id="frame")
 
-class TApplication(PUIView):
+class Application(PUIView):
     def __init__(self):
         super().__init__()
         self.ui = PUIApp(self)
 
     def addChild(self, idx, child):
         if idx>0:
             raise RuntimeError("Textual backend only support single window")
```

### Comparing `QPUIQ-0.2.3/PUI/textual/base.py` & `QPUIQ-0.2.4/PUI/textual/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,14 @@
             if parent.expanding_y_children > 0:
                 self.weak_hug_y = True
 
         super().update(prev)
 
     def postUpdate(self):
         super().postUpdate()
-
-
         self.t_update_layout()
 
     @property
     def tparent(self):
         parent = self.parent
         while not isinstance(parent, TBase):
             if parent==parent.parent:
```

### Comparing `QPUIQ-0.2.3/PUI/textual/checkbox.py` & `QPUIQ-0.2.4/PUI/textual/checkbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class TCheckbox(TBase):
+class Checkbox(TBase):
     def __init__(self, text, model):
         super().__init__()
         self.text = text
         self.model = model
 
     def update(self, prev):
         if prev and prev.ui:
```

### Comparing `QPUIQ-0.2.3/PUI/textual/label.py` & `QPUIQ-0.2.4/PUI/textual/label.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class TLabel(TBase):
+class Label(TBase):
     def __init__(self, text, **kwargs):
         super().__init__(**kwargs)
         self.widget = None
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
```

### Comparing `QPUIQ-0.2.3/PUI/textual/layout.py` & `QPUIQ-0.2.4/PUI/textual/layout.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from .. import *
 from .base import *
 
-class TVertical(TBase):
+class VBox(TBase):
     container_y = True
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = containers.Vertical()
         super().update(prev)
 
     def addChild(self, idx, child):
         if isinstance(child, TBase):
             self.inner.mount(child.outer, before=idx)
-        else:
+        elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, TBase):
             child.tremove()
-        else:
+        elif child.children:
             self.removeChild(idx, child.children[0])
 
-class THorizontal(TBase):
+class HBox(TBase):
     container_x = True
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = containers.Horizontal()
         super().update(prev)
 
     def addChild(self, idx, child):
         if isinstance(child, TBase):
             self.inner.mount(child.outer, before=idx)
-        else:
+        elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, TBase):
             child.tremove()
-        else:
+        elif child.children:
             self.removeChild(idx, child.children[0])
 
-class TSpacer(TBase):
+class Spacer(TBase):
     def __init__(self, *args):
         super().__init__(*args)
         self.layout_weight = 1
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
```

### Comparing `QPUIQ-0.2.3/PUI/textual/radiobutton.py` & `QPUIQ-0.2.4/PUI/textual/radiobutton.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class TRadioButton(TBase):
+class RadioButton(TBase):
     def __init__(self, text, value, model):
         super().__init__()
         self.text = text
         self.value = value
         self.model = model
 
     def update(self, prev):
```

### Comparing `QPUIQ-0.2.3/PUI/textual/scroll.py` & `QPUIQ-0.2.4/PUI/textual/scroll.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class TScroll(TBase):
+class Scroll(TBase):
     weak_expand_x = True
     weak_expand_y = True
     def __init__(self, vertical=None, horizontal=False):
         self.vertical = vertical
         self.horizontal = horizontal
         super().__init__()
```

### Comparing `QPUIQ-0.2.3/PUI/textual/textfield.py` & `QPUIQ-0.2.4/PUI/textual/textfield.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .. import *
 from .base import *
 
-class TInput(TBase):
+class TextField(TBase):
     content_width = None
     def __init__(self, model):
         super().__init__()
         self.model = model
+        self.ui_text = self.model.value
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
             model_value = self.model.value
             if self.ui_text != model_value:
                 self.ui_text = model_value
```

### Comparing `QPUIQ-0.2.3/PUI/timeline.py` & `QPUIQ-0.2.4/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.3/PUI/tkinter/application.py` & `QPUIQ-0.2.4/PUI/tkinter/application.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 from .. import *
 from .base import *
 import functools
 
-class TkApplication(PUIView):
+class Application(PUIView):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.theme = None
+
     def redraw(self):
         if self.ui:
             self.ui.after(0, functools.partial(self.update))
         else:
             self.update()
 
+    def tkinter(self, theme=None, **kwargs):
+        super().tkinter(**kwargs)
+        if theme:
+            self.theme = theme
+        return self
+
     def update(self, prev=None):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = tk.Tk()
             ttkStyle = ttk.Style(self.ui)
-            ttkStyle.theme_use('classic') # macOS's aqua doesn't respect background setting for some widgets
+            if self.theme:
+                ttkStyle.theme_use(self.theme)
             self.ui.withdraw()
 
         super().update(prev)
 
     def addChild(self, idx, child):
         pass
```

### Comparing `QPUIQ-0.2.3/PUI/tkinter/base.py` & `QPUIQ-0.2.4/PUI/tkinter/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.3/PUI/tkinter/canvas.py` & `QPUIQ-0.2.4/PUI/tkinter/canvas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 import itertools
-class TkCanvas(TkBaseWidget):
+class Canvas(TkBaseWidget):
     terminal = True
     def __init__(self, painter, *args):
         super().__init__()
         self.painter = painter
         self.args = args
 
     def update(self, prev):
```

### Comparing `QPUIQ-0.2.3/PUI/tkinter/checkbox.py` & `QPUIQ-0.2.4/PUI/tkinter/checkbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class TkCheckbutton(TkBaseWidget):
+class Checkbox(TkBaseWidget):
     def __init__(self, text, model):
         super().__init__()
         self.text = text
         self.model = model
 
     def update(self, prev):
         if prev and prev.ui:
```

### Comparing `QPUIQ-0.2.3/PUI/tkinter/label.py` & `QPUIQ-0.2.4/PUI/tkinter/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .. import *
 from .base import *
-class TkLabel(TkBaseWidget):
+class Label(TkBaseWidget):
     def __init__(self, text):
         super().__init__()
         self.text = text
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
```

### Comparing `QPUIQ-0.2.3/PUI/tkinter/layout.py` & `QPUIQ-0.2.4/PUI/tkinter/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class TkHBox(TkBaseWidget):
+class HBox(TkBaseWidget):
     use_ttk = "TFrame"
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = ttk.Frame(self.tkparent.inner)
             self.ui.grid_rowconfigure(0, weight=1)
@@ -31,15 +31,15 @@
             self.removeChild(idx, child.children[0])
 
     def postSync(self):
         for i,child in enumerate(self.children):
             self.putChild(i, child)
         super().postSync()
 
-class TkVBox(TkBaseWidget):
+class VBox(TkBaseWidget):
     use_ttk = "TFrame"
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
             self.ui = ttk.Frame(self.tkparent.inner)
             self.ui.grid_columnconfigure(0, weight=1)
@@ -65,15 +65,15 @@
             self.removeChild(idx, child.children[0])
 
     def postSync(self):
         for i,child in enumerate(self.children):
             self.putChild(i, child)
         super().postSync()
 
-class TkSpacer(TkBaseWidget):
+class Spacer(TkBaseWidget):
     use_ttk = "TFrame"
     def __init__(self, *args):
         super().__init__(*args)
         self.layout_weight = 1
 
     def update(self, prev):
         if prev and prev.ui:
```

### Comparing `QPUIQ-0.2.3/PUI/tkinter/radiobutton.py` & `QPUIQ-0.2.4/PUI/PySide6/splitter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from .. import *
 from .base import *
 
-class TkRadiobutton(TkBaseWidget):
-    def __init__(self, text, value, model):
+class Splitter(QtBaseWidget):
+    terminal = False
+    def __init__(self, vertical=False):
         super().__init__()
-        self.text = text
-        self.value = value
-        self.model = model
+        self.vertical = vertical
 
     def update(self, prev):
         if prev and prev.ui:
             self.ui = prev.ui
         else:
-            self.ui = tk.Radiobutton(self.tkparent.inner, text=self.text, anchor="w")
-        if self.value  == self.model.value:
-            self.ui.select()
-        else:
-            self.ui.deselect()
-        self.ui.configure(command=self._select)
+            self.ui = QtWidgets.QSplitter()
+        self.ui.setOrientation(QtCore.Qt.Orientation.Vertical if self.vertical else QtCore.Qt.Orientation.Horizontal)
         super().update(prev)
 
-    def _select(self):
-        node = self.get_node()
-        self.model.value = node.value
+    def addChild(self, idx, child):
+        if isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
+            self.ui.insertWidget(idx, child.outer)
+        else:
+            self.addChild(idx, child.children[0])
+    
+    def removeChild(self, idx, child):
+        child.outer.setParent(None)
```

### Comparing `QPUIQ-0.2.3/PUI/tkinter/scroll.py` & `QPUIQ-0.2.4/PUI/tkinter/scroll.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             delta = -1
         elif event.delta > 0:
             delta = 1
         elif event.delta < 0:
             delta = -1
         self.canvas.yview_scroll(delta, "units")
 
-class TkScroll(TkBaseWidget):
+class Scroll(TkBaseWidget):
     use_ttk = "TFrame"
     def __init__(self, vertical=None, horizontal=False):
         self.vertical = vertical
         self.horizontal = horizontal
         super().__init__()
         self.layout_weight = 1
```

### Comparing `QPUIQ-0.2.3/PUI/tkinter/textfield.py` & `QPUIQ-0.2.4/PUI/tkinter/textfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class TkEntry(TkBaseWidget):
+class TextField(TkBaseWidget):
     def __init__(self, model):
         super().__init__()
         self.model = model
 
     def update(self, prev):
         value = self.model.value
         if prev and prev.ui:
```

### Comparing `QPUIQ-0.2.3/PUI/tkinter/window.py` & `QPUIQ-0.2.4/PUI/tkinter/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .. import *
 from .base import *
 
-class TkWindow(TkBaseWidget):
+class Window(TkBaseWidget):
     def __init__(self, title=None, size=None, maximize=None, fullscreen=None):
         super().__init__()
         self.title = title
         self.size = size
         self.curr_size = None
         self.maximize = maximize
         self.curr_maximize = None
```

### Comparing `QPUIQ-0.2.3/PUI/view.py` & `QPUIQ-0.2.4/PUI/view.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.3/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.2.4/QPUIQ.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,55 +20,59 @@
 PUI/PySide6/layout.py
 PUI/PySide6/mdi.py
 PUI/PySide6/menu.py
 PUI/PySide6/progressbar.py
 PUI/PySide6/radiobutton.py
 PUI/PySide6/scroll.py
 PUI/PySide6/splitter.py
+PUI/PySide6/tab.py
 PUI/PySide6/text.py
 PUI/PySide6/textfield.py
 PUI/PySide6/window.py
 PUI/flet/__init__.py
 PUI/flet/application.py
 PUI/flet/base.py
 PUI/flet/button.py
 PUI/flet/canvas.py
 PUI/flet/checkbox.py
 PUI/flet/label.py
 PUI/flet/layout.py
 PUI/flet/progressbar.py
 PUI/flet/radiobutton.py
 PUI/flet/scroll.py
+PUI/flet/tab.py
 PUI/flet/text.py
 PUI/flet/textfield.py
 PUI/flet/window.py
 PUI/textual/__init__.py
 PUI/textual/application.py
 PUI/textual/base.py
 PUI/textual/button.py
 PUI/textual/checkbox.py
 PUI/textual/label.py
 PUI/textual/layout.py
 PUI/textual/progressbar.py
 PUI/textual/radiobutton.py
 PUI/textual/scroll.py
+PUI/textual/tab.py
 PUI/textual/text.py
 PUI/textual/textfield.py
 PUI/textual/window.py
 PUI/tkinter/__init__.py
 PUI/tkinter/application.py
 PUI/tkinter/base.py
 PUI/tkinter/button.py
 PUI/tkinter/canvas.py
 PUI/tkinter/checkbox.py
 PUI/tkinter/label.py
 PUI/tkinter/layout.py
 PUI/tkinter/progressbar.py
 PUI/tkinter/radiobutton.py
 PUI/tkinter/scroll.py
+PUI/tkinter/tab.py
 PUI/tkinter/text.py
 PUI/tkinter/textfield.py
 PUI/tkinter/window.py
 QPUIQ.egg-info/PKG-INFO
 QPUIQ.egg-info/SOURCES.txt
 QPUIQ.egg-info/dependency_links.txt
 QPUIQ.egg-info/top_level.txt
```

### Comparing `QPUIQ-0.2.3/README.md` & `QPUIQ-0.2.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -21,39 +21,40 @@
 root = Example()
 root.run()
 ```
 ![Hello World](https://github.com/buganini/PUI/raw/main/screenshots/hello_world.png)
 
 ## State & Data Binding
 ```python
-# example/pyside6_textfield.py
-
+# example/generic_textfield.py
 from PUI.PySide6 import *
 
 data = State()
-data.var = 0
+class Example(Application):
+    def __init__(self):
+        super().__init__()
+        data.var = 0
 
-class QtExample(QtApplication):
     def content(self):
-        with QtWindow(title="blah"):
-            with QtVBox():
-                with QtHBox():
-                    QtButton("-", self.on_minus)
-                    QtLabel(f"{data.var}")
-                    QtButton("+", self.on_plus)
+        with Window(title="blah"):
+            with VBox():
+                with HBox():
+                    Button("-").click(self.on_minus)
+                    Label(f"{data.var}")
+                    Button("+").click(self.on_plus)
 
-                QtLineEdit(data("var")) # binding
+                TextField(data("var")) # binding
 
     def on_minus(self):
         data.var -= 1
 
     def on_plus(self):
         data.var += 1
 
-root = QtExample()
+root = Example()
 root.run()
 ```
 ![State & Data Binding](https://github.com/buganini/PUI/raw/main/screenshots/pyside6_textfield.png)
 
 ## View Component
 ```python
 # example/bleak_list.py
@@ -95,143 +96,164 @@
                     Label(e.title).click(self.entry_selected, i)
                 Spacer()
 
         with Scroll().layout(weight=1): # Generic Layout Parameter
             if 0 <= selected and selected < len(entries):
                 (Text(entries[selected].description)
                     .layout(padding=10) # Generic Layout Parameter
-                    .qt(StyleSheet="background-color:white; color:black")) # QT-specific
+                    .qt(StyleSheet={"background-color":"white", "color":"black"})) # QT-specific
 ...
 ```
 ![Layout & Styling](https://github.com/buganini/PUI/raw/main/screenshots/feed_parser_padding.png)
 
 
 ## Canvas
 ```python
-# example/pyside6_canvas.py
+# example/generic_canvas.py
 
 from PUI.PySide6 import *
 
 data = State()
-data.var = 50
+class Example(Application):
+    def __init__(self):
+        super().__init__()
+        data.var = 50
 
-class QtExample(QtApplication):
     def content(self):
-        with QtWindow(title="blah", size=(640,480)):
-            with QtVBox():
-                QtCanvas(self.painter, data.var)
-                with QtHBox():
-                    QtButton("-", self.on_minus)
-                    QtLabel(f"{data.var}")
-                    QtButton("+", self.on_plus)
+        with Window(title="blah", size=(640,480)):
+            with VBox():
+                Canvas(self.painter, data.var)
+                with HBox():
+                    Button("-").click(self.on_minus)
+                    Label(f"{data.var}").layout(weight=1)
+                    Button("+").click(self.on_plus)
 
     @staticmethod
     def painter(canvas, var):
         canvas.drawText(var, var/2, f"blah {var}")
-        canvas.drawLine(var, var, var*2, var*3)
+        canvas.drawLine(var, var, var*2, var*3, color=0xFFFF00)
 
     def on_minus(self):
         data.var -= 1
 
     def on_plus(self):
         data.var += 1
 
-root = QtExample()
+root = Example()
 root.run()
 ```
 ![Canvas](https://github.com/buganini/PUI/raw/main/screenshots/pyside6_canvas.gif)
 
 ## Cookbook
 `python -m cookbook PySide6` (requires pygments for syntax highlight)
 
 ![Cookbook 1](https://github.com/buganini/PUI/raw/main/screenshots/cookbook1.png)
 ![Cookbook 2](https://github.com/buganini/PUI/raw/main/screenshots/cookbook2.png)
 
 `python -m cookbook textual`
 ![Cookbook textual](https://github.com/buganini/PUI/raw/main/screenshots/cookbook_textual.png)
 
+`python -m cookbook flet`
+![Cookbook flet](https://github.com/buganini/PUI/raw/main/screenshots/cookbook_flet.png)
+
+`python -m cookbook tkinter`
+![Cookbook tkinter](https://github.com/buganini/PUI/raw/main/screenshots/cookbook_tkinter.png)
+
+
 ## Hot-Reload with Reloadium
 [![Hot-Reload with Reloadium](https://img.youtube.com/vi/X716rwchPBM/0.jpg)](https://www.youtube.com/watch?v=X716rwchPBM)
 
 
 # Backends
 ## Tier-1
 * PySide6
 ## Lower Priority
 * tkinter
     * or https://github.com/rdbende/Sun-Valley-ttk-theme
 * flet
-    * no canvas before v0.6.0
 * textual (Text Mode)
     * no canvas
 
-# Generic Expression
-* Take a look at [PUI/PySide6/\_\_init__.py](https://github.com/buganini/PUI/blob/main/PUI/PySide6/__init__.py)
-## Elements
-* HBox()
-* VBox()
-* Spacer()
+# Components
+|Generic|PySide6|flet|tkinter|textual|
+|-------|-------|----|-------|-------|
+|Application|QApplication|Page|Tk|App|
+|Window|QMainWindow|✓(Single)|Toplevel|✓(Single)|
+|HBox|QHBoxLayout|Row|Frame(grid)|Horizontal|
+|VBox|QVBoxLayout|Column|Frame(grid)|Vertical|
+|Spacer|QSpacerItem|✓|✓|✓|
+|Label|QLabel|Text|Label|Label/Button|
+|Button|QPushButton|ElevatedButton|Button|Button|
+|Checkbox|QCheckBox|Checkbox|Checkbutton|Checkbox|
+|RadioButton|QRadioButton|Radio|Radiobutton|RadioButton|
+|Canvas|✓(QWidget)|Canvas|Canvas|-|
+|TextField|QLineEdit|TextField|Entry|Input|
+|ProgressBar|QProgressBar|ProgressBar|Progressbar|ProgressBar|
+|Scroll|QScrollArea|✓|✓|ScrollableContainer|
+|Text|QLabel|Text|Label|Text|
+|Html|QLabel|⚠ Text|⚠ Label|⚠ Text|
+|MarkDown|QLabel|Markdown|⚠ Label|⚠ Text|
+|Combobox|QComboBox|-|-|-|
+|ComboboxItem|✓|-|-|-|
+|Tabs|QTabWidget|Tabs|Notebook|Tabs|
+|Tab|✓|Tab|✓|✓|
+|MenuBar|QMenuBar|-|-|-|
+|Menu|QMenu|-|-|-|
+|MenuAction|QAction|-|-|-|
+|MdiArea|QMdiArea|-|-|-|
+|MdiSubWindow|QMdiSubWindow|-|-|-|
+|Splitter|QSplitter|-|-|-|
+|(Wrapper)|`QtWrapper`|-|-|-|
+
+## Interfaces
 * Button(text)
     * .click(callback, *cb_args, **cb_kwargs)
 * Label(text)
     * .click(callback, *cb_args, **cb_kwargs)
 * TextField(binding)
 * ProgressBar(progress `0-1`)
-* Scroll()
+* Checkbox(label, model)
+* RadioButton(label, value, model)
 * Canvas
     * .drawText(x, y, text)
     * .drawLine(x1, y1, x2, y2, color=0xFF0000, width=2)
     * .drawPolyline([x1, y2, ..., xn, yn], color=0xFF0000, width=2)
-## Layout
-* .layout(width=320, height=240, weight=1)
+## Modifiers
+* .layout(width=320, height=240, weight=1, padding=, margin=)
+* .style(color=0xFF0000, bgColor=0x0, fontSize=16, fontWeight="bold", fontFamily="Arial")
+* .qt(HorizontalPolicy=, VerticalPolicy=, SizeConstraint=, StyleSheet={})
+* .flet(k=v)
 
 # Hot Reload
 Add these lines to your view file and run with [reloadium](https://github.com/reloadware/reloadium)
 ```python
 import reloadium
 
 # reloadium: after_reload
 def after_reload(actions):
     PUIView.reload()
 ```
 
+
 # TODO
-* ~~Use threading.locals() instead of inspect~~
-* State
-    * ~~Update Trigger~~
-    * ~~Binding~~
-    * ~~StateList~~
-    * ~~StateDict~~
-    * Lazy UI?
+* Tabs(`tabposition`)
+* Lazy List
 * StateObject decorator
-* Adapters
-    * ~~Split Application/Window, multi-windows~~
-    * UI Flow
-        * Navigation Stack
-        * View Router
-        * Model Window/Dialog
-    * ~~Label~~
-    * ~~Button~~
-    * ~~TextField~~
-    * ~~TimelimeView~~
-    * Layout
-        * ~~HBox~~
-        * ~~VBox~~
-        * ZBox
-        * Grid
-            * Row
-            * Column
-        * SwiftUI style overlay ??
-    * Canvas
-        * ~~Text~~
-        * ~~Line~~
-        * Rect
-        * Arc
-        * Image
-        * ...
-    * Table
-    * Tree
-    * ~~Scrollbar (or as a layout setting)~~
-* Better DOM syncer
-    * Prevent unnecessary nested update
-    * Trace Event Source (TextField) and prevent update it DOM Sync
-* Pydantic State
+* UI Flow
+    * Navigation Stack
+    * View Router
+    * Model Window/Dialog
+* Layout
+    * ZBox
+    * Grid
+        * Row
+        * Column
+    * SwiftUI style overlay ??
+* Canvas
+    * Rect
+    * Arc
+    * Image
+    * ...
+* Table
+* Tree
+* Dialog
+* State with Pydantic support?
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `QPUIQ-0.2.3/setup.py` & `QPUIQ-0.2.4/setup.py`

 * *Files identical despite different names*

