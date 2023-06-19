# Comparing `tmp/customtkinter-5.1.3.tar.gz` & `tmp/customtkinter-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tomschimansky/Documents/Projekte/CustomTkinter/dist/.tmp-g81nkl_2/customtkinter-5.1.3.tar", last modified: Fri May  5 17:12:37 2023, max compression
+gzip compressed data, was "/Users/tomschimansky/Documents/Projekte/CustomTkinter/dist/.tmp-v9i4m_f9/customtkinter-5.2.0.tar", last modified: Mon Jun 19 12:01:18 2023, max compression
```

## Comparing `customtkinter-5.1.3.tar` & `customtkinter-5.2.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.901600 customtkinter-5.1.3/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1071 2023-02-06 12:16:00.000000 customtkinter-5.1.3/LICENSE
--rw-r--r--   0 tomschimansky   (501) staff       (20)      187 2023-02-06 12:16:00.000000 customtkinter-5.1.3/MANIFEST.in
--rw-r--r--   0 tomschimansky   (501) staff       (20)      592 2023-05-05 17:12:37.901909 customtkinter-5.1.3/PKG-INFO
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.868297 customtkinter-5.1.3/customtkinter/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2739 2023-05-05 16:55:53.000000 customtkinter-5.1.3/customtkinter/__init__.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.871190 customtkinter-5.1.3/customtkinter/assets/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2023-04-20 16:40:50.000000 customtkinter-5.1.3/customtkinter/assets/.DS_Store
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.871666 customtkinter-5.1.3/customtkinter/assets/fonts/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     3528 2022-11-30 22:56:26.000000 customtkinter-5.1.3/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.873519 customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/
--rw-r--r--   0 tomschimansky   (501) staff       (20)   168644 2022-11-30 22:56:26.000000 customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 tomschimansky   (501) staff       (20)   168260 2022-11-30 22:56:26.000000 customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.875515 customtkinter-5.1.3/customtkinter/assets/icons/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2022-12-11 00:44:28.000000 customtkinter-5.1.3/customtkinter/assets/icons/.DS_Store
--rw-r--r--   0 tomschimansky   (501) staff       (20)    13238 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.877528 customtkinter-5.1.3/customtkinter/assets/themes/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4520 2023-04-23 09:36:19.000000 customtkinter-5.1.3/customtkinter/assets/themes/blue.json
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4514 2023-04-23 09:36:19.000000 customtkinter-5.1.3/customtkinter/assets/themes/dark-blue.json
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4515 2023-04-23 09:36:19.000000 customtkinter-5.1.3/customtkinter/assets/themes/green.json
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.879545 customtkinter-5.1.3/customtkinter/windows/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      107 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     5532 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/ctk_input_dialog.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    15580 2023-03-26 14:22:30.000000 customtkinter-5.1.3/customtkinter/windows/ctk_tk.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    14727 2023-04-20 23:43:47.000000 customtkinter-5.1.3/customtkinter/windows/ctk_toplevel.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.888855 customtkinter-5.1.3/customtkinter/windows/widgets/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      622 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/__init__.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.890708 customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      172 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2602 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     4097 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.892130 customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      324 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     5894 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/ctk_canvas.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    91030 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/draw_engine.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.893662 customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/
--rw-r--r--   0 tomschimansky   (501) staff       (20)       81 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    15788 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     8516 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    27663 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_button.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    22074 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_checkbox.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    20598 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_combobox.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    17893 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_entry.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     9510 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_frame.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    12136 2023-05-05 16:54:04.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_label.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    19456 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_optionmenu.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    14115 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_progressbar.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    20211 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_radiobutton.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    15116 2023-04-26 08:52:31.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_scrollable_frame.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    13856 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_scrollbar.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    19712 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_segmented_button.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    18308 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_slider.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    23416 2023-04-24 11:44:24.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_switch.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    17700 2023-04-26 09:33:02.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_tabview.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)    24566 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/ctk_textbox.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.895072 customtkinter-5.1.3/customtkinter/windows/widgets/font/
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1302 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/font/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     3764 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/font/ctk_font.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2268 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/font/font_manager.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.895969 customtkinter-5.1.3/customtkinter/windows/widgets/image/
--rw-r--r--   0 tomschimansky   (501) staff       (20)       32 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/image/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     5306 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/image/ctk_image.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.897782 customtkinter-5.1.3/customtkinter/windows/widgets/scaling/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      287 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/scaling/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     7060 2023-02-06 12:16:01.000000 customtkinter-5.1.3/customtkinter/windows/widgets/scaling/scaling_base_class.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     8745 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/scaling/scaling_tracker.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.899354 customtkinter-5.1.3/customtkinter/windows/widgets/theme/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      471 2023-04-24 11:36:20.000000 customtkinter-5.1.3/customtkinter/windows/widgets/theme/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1906 2023-04-24 11:32:27.000000 customtkinter-5.1.3/customtkinter/windows/widgets/theme/theme_manager.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.900920 customtkinter-5.1.3/customtkinter/windows/widgets/utility/
--rw-r--r--   0 tomschimansky   (501) staff       (20)       72 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/utility/__init__.py
--rw-r--r--   0 tomschimansky   (501) staff       (20)      766 2022-11-30 23:02:26.000000 customtkinter-5.1.3/customtkinter/windows/widgets/utility/utility_functions.py
-drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-05-05 17:12:37.870598 customtkinter-5.1.3/customtkinter.egg-info/
--rw-r--r--   0 tomschimansky   (501) staff       (20)      592 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/PKG-INFO
--rw-r--r--   0 tomschimansky   (501) staff       (20)     2793 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/SOURCES.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)        1 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/dependency_links.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)       57 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/requires.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)       14 2023-05-05 17:12:37.000000 customtkinter-5.1.3/customtkinter.egg-info/top_level.txt
--rw-r--r--   0 tomschimansky   (501) staff       (20)      757 2023-05-05 16:55:53.000000 customtkinter-5.1.3/pyproject.toml
--rw-r--r--   0 tomschimansky   (501) staff       (20)     1355 2023-05-05 17:12:37.903208 customtkinter-5.1.3/setup.cfg
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.679157 customtkinter-5.2.0/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1071 2023-02-06 12:16:00.000000 customtkinter-5.2.0/LICENSE
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      187 2023-02-06 12:16:00.000000 customtkinter-5.2.0/MANIFEST.in
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      567 2023-06-19 12:01:18.679425 customtkinter-5.2.0/PKG-INFO
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.613267 customtkinter-5.2.0/customtkinter/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2739 2023-06-19 11:54:51.000000 customtkinter-5.2.0/customtkinter/__init__.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.618029 customtkinter-5.2.0/customtkinter/assets/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2023-04-20 16:40:50.000000 customtkinter-5.2.0/customtkinter/assets/.DS_Store
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.619161 customtkinter-5.2.0/customtkinter/assets/fonts/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     3528 2022-11-30 22:56:26.000000 customtkinter-5.2.0/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.622577 customtkinter-5.2.0/customtkinter/assets/fonts/Roboto/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)   168644 2022-11-30 22:56:26.000000 customtkinter-5.2.0/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 tomschimansky   (501) staff       (20)   168260 2022-11-30 22:56:26.000000 customtkinter-5.2.0/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.627339 customtkinter-5.2.0/customtkinter/assets/icons/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     6148 2022-12-11 00:44:28.000000 customtkinter-5.2.0/customtkinter/assets/icons/.DS_Store
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    13238 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.630512 customtkinter-5.2.0/customtkinter/assets/themes/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4520 2023-05-27 11:07:00.000000 customtkinter-5.2.0/customtkinter/assets/themes/blue.json
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4514 2023-05-27 11:07:33.000000 customtkinter-5.2.0/customtkinter/assets/themes/dark-blue.json
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4515 2023-05-27 11:07:33.000000 customtkinter-5.2.0/customtkinter/assets/themes/green.json
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.634647 customtkinter-5.2.0/customtkinter/windows/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      107 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     5536 2023-06-19 11:00:42.000000 customtkinter-5.2.0/customtkinter/windows/ctk_input_dialog.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    15580 2023-03-26 14:22:30.000000 customtkinter-5.2.0/customtkinter/windows/ctk_tk.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    14727 2023-04-20 23:43:47.000000 customtkinter-5.2.0/customtkinter/windows/ctk_toplevel.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.655109 customtkinter-5.2.0/customtkinter/windows/widgets/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      622 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/__init__.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.658121 customtkinter-5.2.0/customtkinter/windows/widgets/appearance_mode/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      172 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/appearance_mode/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2602 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     4097 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.660614 customtkinter-5.2.0/customtkinter/windows/widgets/core_rendering/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      324 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/core_rendering/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     5894 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/core_rendering/ctk_canvas.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    91030 2023-06-15 20:07:56.000000 customtkinter-5.2.0/customtkinter/windows/widgets/core_rendering/draw_engine.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.664370 customtkinter-5.2.0/customtkinter/windows/widgets/core_widget_classes/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       81 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/core_widget_classes/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    15788 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     8516 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    27695 2023-06-19 11:19:59.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_button.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    22416 2023-05-27 11:04:37.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_checkbox.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    20598 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_combobox.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    17893 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_entry.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     9510 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_frame.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    13101 2023-05-27 10:47:43.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_label.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    19633 2023-05-08 17:10:54.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_optionmenu.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    14115 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_progressbar.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    20211 2023-05-27 11:04:37.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_radiobutton.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    15116 2023-04-26 08:52:31.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_scrollable_frame.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    13856 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_scrollbar.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    20788 2023-05-27 13:00:56.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_segmented_button.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    18308 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_slider.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    23416 2023-04-24 11:44:24.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_switch.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    17807 2023-05-27 13:20:02.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_tabview.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)    24566 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/ctk_textbox.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.667536 customtkinter-5.2.0/customtkinter/windows/widgets/font/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1302 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/font/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     3825 2023-06-15 10:47:09.000000 customtkinter-5.2.0/customtkinter/windows/widgets/font/ctk_font.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2268 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/font/font_manager.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.669871 customtkinter-5.2.0/customtkinter/windows/widgets/image/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       32 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/image/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     5306 2023-05-27 10:17:42.000000 customtkinter-5.2.0/customtkinter/windows/widgets/image/ctk_image.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.673525 customtkinter-5.2.0/customtkinter/windows/widgets/scaling/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      287 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/scaling/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     7060 2023-02-06 12:16:01.000000 customtkinter-5.2.0/customtkinter/windows/widgets/scaling/scaling_base_class.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     8745 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/scaling/scaling_tracker.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.676021 customtkinter-5.2.0/customtkinter/windows/widgets/theme/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      471 2023-04-24 11:36:20.000000 customtkinter-5.2.0/customtkinter/windows/widgets/theme/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2179 2023-05-27 11:05:58.000000 customtkinter-5.2.0/customtkinter/windows/widgets/theme/theme_manager.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.678191 customtkinter-5.2.0/customtkinter/windows/widgets/utility/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       72 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/utility/__init__.py
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      766 2022-11-30 23:02:26.000000 customtkinter-5.2.0/customtkinter/windows/widgets/utility/utility_functions.py
+drwxr-xr-x   0 tomschimansky   (501) staff       (20)        0 2023-06-19 12:01:18.617234 customtkinter-5.2.0/customtkinter.egg-info/
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      567 2023-06-19 12:01:18.000000 customtkinter-5.2.0/customtkinter.egg-info/PKG-INFO
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     2793 2023-06-19 12:01:18.000000 customtkinter-5.2.0/customtkinter.egg-info/SOURCES.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)        1 2023-06-19 12:01:18.000000 customtkinter-5.2.0/customtkinter.egg-info/dependency_links.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       57 2023-06-19 12:01:18.000000 customtkinter-5.2.0/customtkinter.egg-info/requires.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)       14 2023-06-19 12:01:18.000000 customtkinter-5.2.0/customtkinter.egg-info/top_level.txt
+-rw-r--r--   0 tomschimansky   (501) staff       (20)      757 2023-06-19 11:54:51.000000 customtkinter-5.2.0/pyproject.toml
+-rw-r--r--   0 tomschimansky   (501) staff       (20)     1330 2023-06-19 12:01:18.681749 customtkinter-5.2.0/setup.cfg
```

### Comparing `customtkinter-5.1.3/LICENSE` & `customtkinter-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/PKG-INFO` & `customtkinter-5.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: customtkinter
-Version: 5.1.3
+Version: 5.2.0
 Summary: Create modern looking GUIs with Python
 Home-page: https://customtkinter.tomschimansky.com
 Author: Tom Schimansky
 License: Creative Commons Zero v1.0 Universal
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A modern and customizable python UI-library based on Tkinter: https://customtkinter.tomschimansky.com
```

### Comparing `customtkinter-5.1.3/customtkinter/__init__.py` & `customtkinter-5.2.0/customtkinter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "5.1.3"
+__version__ = "5.2.0"
 
 import os
 import sys
 from tkinter import Variable, StringVar, IntVar, DoubleVar, BooleanVar
 from tkinter.constants import *
 import tkinter.filedialog as filedialog
```

### Comparing `customtkinter-5.1.3/customtkinter/assets/.DS_Store` & `customtkinter-5.2.0/customtkinter/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf` & `customtkinter-5.2.0/customtkinter/assets/fonts/CustomTkinter_shapes_font.otf`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf` & `customtkinter-5.2.0/customtkinter/assets/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf` & `customtkinter-5.2.0/customtkinter/assets/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/assets/icons/.DS_Store` & `customtkinter-5.2.0/customtkinter/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico` & `customtkinter-5.2.0/customtkinter/assets/icons/CustomTkinter_icon_Windows.ico`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/assets/themes/blue.json` & `customtkinter-5.2.0/customtkinter/assets/themes/blue.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095238095238095%*

 * *Differences: {"'CTkCheckBox'": "OrderedDict([('corner_radius', 6), ('border_width', 3), ('fg_color', "*

 * *                  "['#3B8ED0', '#1F6AA5']), ('border_color', ['#3E454A', '#949A9F']), "*

 * *                  "('hover_color', ['#3B8ED0', '#1F6AA5']), ('checkmark_color', ['#DCE4EE', "*

 * *                  "'gray90']), ('text_color', ['gray10', '#DCE4EE']), ('text_color_disabled', "*

 * *                  "['gray60', 'gray45'])])",*

 * * "'CTkRadioButton'": "OrderedDict([('corner_radius', 1000), ('border_width_checked', 6), "*

 * *         […]*

```diff
@@ -25,15 +25,15 @@
             "#DCE4EE"
         ],
         "text_color_disabled": [
             "gray74",
             "gray60"
         ]
     },
-    "CTkCheckbox": {
+    "CTkCheckBox": {
         "border_color": [
             "#3E454A",
             "#949A9F"
         ],
         "border_width": 3,
         "checkmark_color": [
             "#DCE4EE",
@@ -181,15 +181,15 @@
             "#4A4D50"
         ],
         "progress_color": [
             "#3B8ED0",
             "#1F6AA5"
         ]
     },
-    "CTkRadiobutton": {
+    "CTkRadioButton": {
         "border_color": [
             "#3E454A",
             "#949A9F"
         ],
         "border_width_checked": 6,
         "border_width_unchecked": 3,
         "corner_radius": 1000,
```

### Comparing `customtkinter-5.1.3/customtkinter/assets/themes/dark-blue.json` & `customtkinter-5.2.0/customtkinter/assets/themes/dark-blue.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095238095238095%*

 * *Differences: {"'CTkCheckBox'": "OrderedDict([('corner_radius', 6), ('border_width', 3), ('fg_color', "*

 * *                  "['#3a7ebf', '#1f538d']), ('border_color', ['#3E454A', '#949A9F']), "*

 * *                  "('hover_color', ['#325882', '#14375e']), ('checkmark_color', ['#DCE4EE', "*

 * *                  "'gray90']), ('text_color', ['gray14', 'gray84']), ('text_color_disabled', "*

 * *                  "['gray60', 'gray45'])])",*

 * * "'CTkRadioButton'": "OrderedDict([('corner_radius', 1000), ('border_width_checked', 6), "*

 * *          […]*

```diff
@@ -25,15 +25,15 @@
             "#DCE4EE"
         ],
         "text_color_disabled": [
             "gray74",
             "gray60"
         ]
     },
-    "CTkCheckbox": {
+    "CTkCheckBox": {
         "border_color": [
             "#3E454A",
             "#949A9F"
         ],
         "border_width": 3,
         "checkmark_color": [
             "#DCE4EE",
@@ -181,15 +181,15 @@
             "#4A4D50"
         ],
         "progress_color": [
             "#3a7ebf",
             "#1f538d"
         ]
     },
-    "CTkRadiobutton": {
+    "CTkRadioButton": {
         "border_color": [
             "#3E454A",
             "#949A9F"
         ],
         "border_width_checked": 6,
         "border_width_unchecked": 3,
         "corner_radius": 1000,
```

### Comparing `customtkinter-5.1.3/customtkinter/assets/themes/green.json` & `customtkinter-5.2.0/customtkinter/assets/themes/green.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095238095238095%*

 * *Differences: {"'CTkCheckBox'": "OrderedDict([('corner_radius', 6), ('border_width', 3), ('fg_color', "*

 * *                  "['#2CC985', '#2FA572']), ('border_color', ['#3E454A', '#949A9F']), "*

 * *                  "('hover_color', ['#0C955A', '#106A43']), ('checkmark_color', ['#DCE4EE', "*

 * *                  "'gray90']), ('text_color', ['gray10', '#DCE4EE']), ('text_color_disabled', "*

 * *                  "['gray60', 'gray45'])])",*

 * * "'CTkRadioButton'": "OrderedDict([('corner_radius', 1000), ('border_width_checked', 6), "*

 * *         […]*

```diff
@@ -25,15 +25,15 @@
             "#DCE4EE"
         ],
         "text_color_disabled": [
             "gray78",
             "gray68"
         ]
     },
-    "CTkCheckbox": {
+    "CTkCheckBox": {
         "border_color": [
             "#3E454A",
             "#949A9F"
         ],
         "border_width": 3,
         "checkmark_color": [
             "#DCE4EE",
@@ -181,15 +181,15 @@
             "#4A4D50"
         ],
         "progress_color": [
             "#2CC985",
             "#2FA572"
         ]
     },
-    "CTkRadiobutton": {
+    "CTkRadioButton": {
         "border_color": [
             "#3E454A",
             "#949A9F"
         ],
         "border_width_checked": 6,
         "border_width_unchecked": 3,
         "corner_radius": 1000,
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/ctk_input_dialog.py` & `customtkinter-5.2.0/customtkinter/windows/ctk_input_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         self._cancel_button = CTkButton(master=self,
                                         width=100,
                                         border_width=0,
                                         fg_color=self._button_fg_color,
                                         hover_color=self._button_hover_color,
                                         text_color=self._button_text_color,
                                         text='Cancel',
-                                        command=self._ok_event)
+                                        command=self._cancel_event)
         self._cancel_button.grid(row=2, column=1, columnspan=1, padx=(10, 20), pady=(0, 20), sticky="ew")
 
         self.after(150, lambda: self._entry.focus())  # set focus to entry with slight delay, otherwise it won't work
         self._entry.bind("<Return>", self._ok_event)
 
     def _ok_event(self, event=None):
         self._user_input = self._entry.get()
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/ctk_tk.py` & `customtkinter-5.2.0/customtkinter/windows/ctk_tk.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/ctk_toplevel.py` & `customtkinter-5.2.0/customtkinter/windows/ctk_toplevel.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/__init__.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/appearance_mode/appearance_mode_base_class.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/appearance_mode/appearance_mode_tracker.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/ctk_canvas.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/core_rendering/ctk_canvas.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/core_rendering/draw_engine.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/core_rendering/draw_engine.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/core_widget_classes/ctk_base_class.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/core_widget_classes/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_button.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,14 +432,15 @@
 
         if "compound" in kwargs:
             self._compound = kwargs.pop("compound")
             require_redraw = True
 
         if "anchor" in kwargs:
             self._anchor = kwargs.pop("anchor")
+            self._create_grid()
             require_redraw = True
 
         super().configure(require_redraw=require_redraw, **kwargs)
 
     def cget(self, attribute_name: str) -> any:
         if attribute_name == "corner_radius":
             return self._corner_radius
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_checkbox.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_checkbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,28 +47,28 @@
         super().__init__(master=master, bg_color=bg_color, width=width, height=height, **kwargs)
 
         # dimensions
         self._checkbox_width = checkbox_width
         self._checkbox_height = checkbox_height
 
         # color
-        self._fg_color = ThemeManager.theme["CTkCheckbox"]["fg_color"] if fg_color is None else self._check_color_type(fg_color)
-        self._hover_color = ThemeManager.theme["CTkCheckbox"]["hover_color"] if hover_color is None else self._check_color_type(hover_color)
-        self._border_color = ThemeManager.theme["CTkCheckbox"]["border_color"] if border_color is None else self._check_color_type(border_color)
-        self._checkmark_color = ThemeManager.theme["CTkCheckbox"]["checkmark_color"] if checkmark_color is None else self._check_color_type(checkmark_color)
+        self._fg_color = ThemeManager.theme["CTkCheckBox"]["fg_color"] if fg_color is None else self._check_color_type(fg_color)
+        self._hover_color = ThemeManager.theme["CTkCheckBox"]["hover_color"] if hover_color is None else self._check_color_type(hover_color)
+        self._border_color = ThemeManager.theme["CTkCheckBox"]["border_color"] if border_color is None else self._check_color_type(border_color)
+        self._checkmark_color = ThemeManager.theme["CTkCheckBox"]["checkmark_color"] if checkmark_color is None else self._check_color_type(checkmark_color)
 
         # shape
-        self._corner_radius = ThemeManager.theme["CTkCheckbox"]["corner_radius"] if corner_radius is None else corner_radius
-        self._border_width = ThemeManager.theme["CTkCheckbox"]["border_width"] if border_width is None else border_width
+        self._corner_radius = ThemeManager.theme["CTkCheckBox"]["corner_radius"] if corner_radius is None else corner_radius
+        self._border_width = ThemeManager.theme["CTkCheckBox"]["border_width"] if border_width is None else border_width
 
         # text
         self._text = text
         self._text_label: Union[tkinter.Label, None] = None
-        self._text_color = ThemeManager.theme["CTkCheckbox"]["text_color"] if text_color is None else self._check_color_type(text_color)
-        self._text_color_disabled = ThemeManager.theme["CTkCheckbox"]["text_color_disabled"] if text_color_disabled is None else self._check_color_type(text_color_disabled)
+        self._text_color = ThemeManager.theme["CTkCheckBox"]["text_color"] if text_color is None else self._check_color_type(text_color)
+        self._text_color_disabled = ThemeManager.theme["CTkCheckBox"]["text_color_disabled"] if text_color_disabled is None else self._check_color_type(text_color_disabled)
 
         # font
         self._font = CTkFont() if font is None else self._check_font_type(font)
         if isinstance(self._font, CTkFont):
             self._font.add_size_configure_callback(self._update_font)
 
         # callback and hover functionality
@@ -261,20 +261,28 @@
             self._fg_color = self._check_color_type(kwargs.pop("fg_color"))
             require_redraw = True
 
         if "hover_color" in kwargs:
             self._hover_color = self._check_color_type(kwargs.pop("hover_color"))
             require_redraw = True
 
+        if "border_color" in kwargs:
+            self._border_color = self._check_color_type(kwargs.pop("border_color"))
+            require_redraw = True
+
+        if "checkmark_color" in kwargs:
+            self._checkmark_color = self._check_color_type(kwargs.pop("checkmark_color"))
+            require_redraw = True
+
         if "text_color" in kwargs:
             self._text_color = self._check_color_type(kwargs.pop("text_color"))
             require_redraw = True
 
-        if "border_color" in kwargs:
-            self._border_color = self._check_color_type(kwargs.pop("border_color"))
+        if "text_color_disabled" in kwargs:
+            self._text_color_disabled = self._check_color_type(kwargs.pop("text_color_disabled"))
             require_redraw = True
 
         if "hover" in kwargs:
             self._hover = kwargs.pop("hover")
 
         if "command" in kwargs:
             self._command = kwargs.pop("command")
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_combobox.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_combobox.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_entry.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_entry.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_frame.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_frame.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_label.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_label.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,15 @@
                  width: int = 0,
                  height: int = 28,
                  corner_radius: Optional[int] = None,
 
                  bg_color: Union[str, Tuple[str, str]] = "transparent",
                  fg_color: Optional[Union[str, Tuple[str, str]]] = None,
                  text_color: Optional[Union[str, Tuple[str, str]]] = None,
+                 text_color_disabled: Optional[Union[str, Tuple[str, str]]] = None,
 
                  text: str = "CTkLabel",
                  font: Optional[Union[tuple, CTkFont]] = None,
                  image: Union[CTkImage, None] = None,
                  compound: str = "center",
                  anchor: str = "center",  # label anchor: center, n, e, s, w
                  wraplength: int = 0,
@@ -43,14 +44,22 @@
         # transfer basic functionality (_bg_color, size, __appearance_mode, scaling) to CTkBaseClass
         super().__init__(master=master, bg_color=bg_color, width=width, height=height)
 
         # color
         self._fg_color = ThemeManager.theme["CTkLabel"]["fg_color"] if fg_color is None else self._check_color_type(fg_color, transparency=True)
         self._text_color = ThemeManager.theme["CTkLabel"]["text_color"] if text_color is None else self._check_color_type(text_color)
 
+        if text_color_disabled is None:
+            if "text_color_disabled" in ThemeManager.theme["CTkLabel"]:
+                self._text_color_disabled = ThemeManager.theme["CTkLabel"]["text_color"]
+            else:
+                self._text_color_disabled = self._text_color
+        else:
+            self._text_color_disabled = self._check_color_type(text_color_disabled)
+
         # shape
         self._corner_radius = ThemeManager.theme["CTkLabel"]["corner_radius"] if corner_radius is None else corner_radius
 
         # text
         self._anchor = anchor
         self._text = text
         self._wraplength = wraplength
@@ -157,21 +166,23 @@
         if no_color_updates is False or requires_recoloring:
             if self._apply_appearance_mode(self._fg_color) == "transparent":
                 self._canvas.itemconfig("inner_parts",
                                         fill=self._apply_appearance_mode(self._bg_color),
                                         outline=self._apply_appearance_mode(self._bg_color))
 
                 self._label.configure(fg=self._apply_appearance_mode(self._text_color),
+                                      disabledforeground=self._apply_appearance_mode(self._text_color_disabled),
                                       bg=self._apply_appearance_mode(self._bg_color))
             else:
                 self._canvas.itemconfig("inner_parts",
                                         fill=self._apply_appearance_mode(self._fg_color),
                                         outline=self._apply_appearance_mode(self._fg_color))
 
                 self._label.configure(fg=self._apply_appearance_mode(self._text_color),
+                                      disabledforeground=self._apply_appearance_mode(self._text_color_disabled),
                                       bg=self._apply_appearance_mode(self._fg_color))
 
             self._canvas.configure(bg=self._apply_appearance_mode(self._bg_color))
 
     def configure(self, require_redraw=False, **kwargs):
         if "corner_radius" in kwargs:
             self._corner_radius = kwargs.pop("corner_radius")
@@ -182,14 +193,18 @@
             self._fg_color = self._check_color_type(kwargs.pop("fg_color"), transparency=True)
             require_redraw = True
 
         if "text_color" in kwargs:
             self._text_color = self._check_color_type(kwargs.pop("text_color"))
             require_redraw = True
 
+        if "text_color_disabled" in kwargs:
+            self._text_color_disabled = self._check_color_type(kwargs.pop("text_color_disabled"))
+            require_redraw = True
+
         if "text" in kwargs:
             self._text = kwargs.pop("text")
             self._label.configure(text=self._text)
 
         if "font" in kwargs:
             if isinstance(self._font, CTkFont):
                 self._font.remove_size_configure_callback(self._update_font)
@@ -226,14 +241,16 @@
         if attribute_name == "corner_radius":
             return self._corner_radius
 
         elif attribute_name == "fg_color":
             return self._fg_color
         elif attribute_name == "text_color":
             return self._text_color
+        elif attribute_name == "text_color_disabled":
+            return self._text_color_disabled
 
         elif attribute_name == "text":
             return self._text
         elif attribute_name == "font":
             return self._font
         elif attribute_name == "image":
             return self._image
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_optionmenu.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_optionmenu.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,14 +239,18 @@
             self._button_hover_color = self._check_color_type(kwargs.pop("button_hover_color"))
             require_redraw = True
 
         if "text_color" in kwargs:
             self._text_color = self._check_color_type(kwargs.pop("text_color"))
             require_redraw = True
 
+        if "text_color_disabled" in kwargs:
+            self._text_color_disabled = self._check_color_type(kwargs.pop("text_color_disabled"))
+            require_redraw = True
+
         if "dropdown_fg_color" in kwargs:
             self._dropdown_menu.configure(fg_color=kwargs.pop("dropdown_fg_color"))
 
         if "dropdown_hover_color" in kwargs:
             self._dropdown_menu.configure(hover_color=kwargs.pop("dropdown_hover_color"))
 
         if "dropdown_text_color" in kwargs:
@@ -257,43 +261,43 @@
                 self._font.remove_size_configure_callback(self._update_font)
             self._font = self._check_font_type(kwargs.pop("font"))
             if isinstance(self._font, CTkFont):
                 self._font.add_size_configure_callback(self._update_font)
 
             self._update_font()
 
-        if "command" in kwargs:
-            self._command = kwargs.pop("command")
+        if "dropdown_font" in kwargs:
+            self._dropdown_menu.configure(font=kwargs.pop("dropdown_font"))
+
+        if "values" in kwargs:
+            self._values = kwargs.pop("values")
+            self._dropdown_menu.configure(values=self._values)
 
         if "variable" in kwargs:
             if self._variable is not None:  # remove old callback
                 self._variable.trace_remove("write", self._variable_callback_name)
 
             self._variable = kwargs.pop("variable")
 
             if self._variable is not None and self._variable != "":
                 self._variable_callback_name = self._variable.trace_add("write", self._variable_callback)
                 self._current_value = self._variable.get()
                 self._text_label.configure(text=self._current_value)
             else:
                 self._variable = None
 
-        if "values" in kwargs:
-            self._values = kwargs.pop("values")
-            self._dropdown_menu.configure(values=self._values)
-
-        if "dropdown_font" in kwargs:
-            self._dropdown_menu.configure(font=kwargs.pop("dropdown_font"))
+        if "state" in kwargs:
+            self._state = kwargs.pop("state")
+            require_redraw = True
 
         if "hover" in kwargs:
             self._hover = kwargs.pop("hover")
 
-        if "state" in kwargs:
-            self._state = kwargs.pop("state")
-            require_redraw = True
+        if "command" in kwargs:
+            self._command = kwargs.pop("command")
 
         if "dynamic_resizing" in kwargs:
             self._dynamic_resizing = kwargs.pop("dynamic_resizing")
             if not self._dynamic_resizing:
                 self.grid_propagate(0)
             else:
                 self.grid_propagate(1)
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_progressbar.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_progressbar.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_radiobutton.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_radiobutton.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,28 +46,28 @@
         super().__init__(master=master, bg_color=bg_color, width=width, height=height, **kwargs)
 
         # dimensions
         self._radiobutton_width = radiobutton_width
         self._radiobutton_height = radiobutton_height
 
         # color
-        self._fg_color = ThemeManager.theme["CTkRadiobutton"]["fg_color"] if fg_color is None else self._check_color_type(fg_color)
-        self._hover_color = ThemeManager.theme["CTkRadiobutton"]["hover_color"] if hover_color is None else self._check_color_type(hover_color)
-        self._border_color = ThemeManager.theme["CTkRadiobutton"]["border_color"] if border_color is None else self._check_color_type(border_color)
+        self._fg_color = ThemeManager.theme["CTkRadioButton"]["fg_color"] if fg_color is None else self._check_color_type(fg_color)
+        self._hover_color = ThemeManager.theme["CTkRadioButton"]["hover_color"] if hover_color is None else self._check_color_type(hover_color)
+        self._border_color = ThemeManager.theme["CTkRadioButton"]["border_color"] if border_color is None else self._check_color_type(border_color)
 
         # shape
-        self._corner_radius = ThemeManager.theme["CTkRadiobutton"]["corner_radius"] if corner_radius is None else corner_radius
-        self._border_width_unchecked = ThemeManager.theme["CTkRadiobutton"]["border_width_unchecked"] if border_width_unchecked is None else border_width_unchecked
-        self._border_width_checked = ThemeManager.theme["CTkRadiobutton"]["border_width_checked"] if border_width_checked is None else border_width_checked
+        self._corner_radius = ThemeManager.theme["CTkRadioButton"]["corner_radius"] if corner_radius is None else corner_radius
+        self._border_width_unchecked = ThemeManager.theme["CTkRadioButton"]["border_width_unchecked"] if border_width_unchecked is None else border_width_unchecked
+        self._border_width_checked = ThemeManager.theme["CTkRadioButton"]["border_width_checked"] if border_width_checked is None else border_width_checked
 
         # text
         self._text = text
         self._text_label: Union[tkinter.Label, None] = None
-        self._text_color = ThemeManager.theme["CTkRadiobutton"]["text_color"] if text_color is None else self._check_color_type(text_color)
-        self._text_color_disabled = ThemeManager.theme["CTkRadiobutton"]["text_color_disabled"] if text_color_disabled is None else self._check_color_type(text_color_disabled)
+        self._text_color = ThemeManager.theme["CTkRadioButton"]["text_color"] if text_color is None else self._check_color_type(text_color)
+        self._text_color_disabled = ThemeManager.theme["CTkRadioButton"]["text_color_disabled"] if text_color_disabled is None else self._check_color_type(text_color_disabled)
 
         # font
         self._font = CTkFont() if font is None else self._check_font_type(font)
         if isinstance(self._font, CTkFont):
             self._font.add_size_configure_callback(self._update_font)
 
         # callback and control variables
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_scrollable_frame.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_scrollable_frame.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_scrollbar.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_scrollbar.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_segmented_button.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_segmented_button.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 except ImportError:
     from typing_extensions import Literal
 
 from .theme import ThemeManager
 from .font import CTkFont
 from .ctk_button import CTkButton
 from .ctk_frame import CTkFrame
+from .utility import check_kwargs_empty
 
 
 class CTkSegmentedButton(CTkFrame):
     """
     Segmented button with corner radius, border width, variable support.
     For detailed information check out the documentation.
     """
@@ -36,18 +37,17 @@
                  background_corner_colors: Union[Tuple[Union[str, Tuple[str, str]]], None] = None,
 
                  font: Optional[Union[tuple, CTkFont]] = None,
                  values: Optional[list] = None,
                  variable: Union[tkinter.Variable, None] = None,
                  dynamic_resizing: bool = True,
                  command: Union[Callable[[str], None], None] = None,
-                 state: str = "normal",
-                 **kwargs):
+                 state: str = "normal"):
 
-        super().__init__(master=master, bg_color=bg_color, width=width, height=height, **kwargs)
+        super().__init__(master=master, bg_color=bg_color, width=width, height=height)
 
         self._sb_fg_color = ThemeManager.theme["CTkSegmentedButton"]["fg_color"] if fg_color is None else self._check_color_type(fg_color)
 
         self._sb_selected_color = ThemeManager.theme["CTkSegmentedButton"]["selected_color"] if selected_color is None else self._check_color_type(selected_color)
         self._sb_selected_hover_color = ThemeManager.theme["CTkSegmentedButton"]["selected_hover_color"] if selected_hover_color is None else self._check_color_type(selected_hover_color)
 
         self._sb_unselected_color = ThemeManager.theme["CTkSegmentedButton"]["unselected_color"] if unselected_color is None else self._check_color_type(unselected_color)
@@ -182,25 +182,42 @@
         number_of_columns, _ = self.grid_size()
         for n in range(number_of_columns):
             self.grid_columnconfigure(n, weight=1, minsize=0)
         self.grid_rowconfigure(0, weight=1)
 
         for index, value in enumerate(self._value_list):
             self.grid_columnconfigure(index, weight=1, minsize=self._current_height)
-            self._buttons_dict[value].grid(row=0, column=index, sticky="ew")
+            self._buttons_dict[value].grid(row=0, column=index, sticky="nsew")
 
     def _create_buttons_from_values(self):
         assert len(self._buttons_dict) == 0
         assert len(self._value_list) > 0
 
         for index, value in enumerate(self._value_list):
             self._buttons_dict[value] = self._create_button(index, value)
             self._configure_button_corners_for_index(index)
 
     def configure(self, **kwargs):
+        if "width" in kwargs:
+            super().configure(width=kwargs.pop("width"))
+
+        if "height" in kwargs:
+            super().configure(height=kwargs.pop("height"))
+
+        if "corner_radius" in kwargs:
+            self._sb_corner_radius = kwargs.pop("corner_radius")
+            super().configure(corner_radius=self._sb_corner_radius)
+            for button in self._buttons_dict.values():
+                button.configure(corner_radius=self._sb_corner_radius)
+
+        if "border_width" in kwargs:
+            self._sb_border_width = kwargs.pop("border_width")
+            for button in self._buttons_dict.values():
+                button.configure(border_width=self._sb_border_width)
+
         if "bg_color" in kwargs:
             super().configure(bg_color=kwargs.pop("bg_color"))
 
             if len(self._buttons_dict) > 0:
                 self._configure_button_corners_for_index(0)
             if len(self._buttons_dict) > 1:
                 max_index = len(self._buttons_dict) - 1
@@ -292,22 +309,28 @@
             self._command = kwargs.pop("command")
 
         if "state" in kwargs:
             self._state = kwargs.pop("state")
             for button in self._buttons_dict.values():
                 button.configure(state=self._state)
 
-        super().configure(**kwargs)
+        check_kwargs_empty(kwargs, raise_error=True)
 
     def cget(self, attribute_name: str) -> any:
-        if attribute_name == "corner_radius":
+        if attribute_name == "width":
+            return super().cget(attribute_name)
+        elif attribute_name == "height":
+            return super().cget(attribute_name)
+        elif attribute_name == "corner_radius":
             return self._sb_corner_radius
         elif attribute_name == "border_width":
             return self._sb_border_width
 
+        elif attribute_name == "bg_color":
+            return super().cget(attribute_name)
         elif attribute_name == "fg_color":
             return self._sb_fg_color
         elif attribute_name == "selected_color":
             return self._sb_selected_color
         elif attribute_name == "selected_hover_color":
             return self._sb_selected_hover_color
         elif attribute_name == "unselected_color":
@@ -327,15 +350,15 @@
             return self._variable
         elif attribute_name == "dynamic_resizing":
             return self._dynamic_resizing
         elif attribute_name == "command":
             return self._command
 
         else:
-            return super().cget(attribute_name)
+            raise ValueError(f"'{attribute_name}' is not a supported argument. Look at the documentation for supported arguments.")
 
     def set(self, value: str, from_variable_callback: bool = False, from_button_callback: bool = False):
         if value == self._current_value:
             return
         elif value in self._buttons_dict:
             self._select_button_by_value(value)
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_slider.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_slider.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_switch.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_switch.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_tabview.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_tabview.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,17 +167,18 @@
 
     def _set_grid_tab_by_name(self, name: str):
         """ needs to be called for changes in corner_radius, border_width """
         self._tab_dict[name].grid(row=3, column=0, sticky="nsew",
                                   padx=self._apply_widget_scaling(max(self._corner_radius, self._border_width)),
                                   pady=self._apply_widget_scaling(max(self._corner_radius, self._border_width)))
 
-    def _grid_forget_all_tabs(self):
-        for frame in self._tab_dict.values():
-            frame.grid_forget()
+    def _grid_forget_all_tabs(self, exclude_name=None):
+        for name, frame in self._tab_dict.items():
+            if name != exclude_name:
+                frame.grid_forget()
 
     def _create_tab(self) -> CTkFrame:
         new_tab = CTkFrame(self,
                            height=0,
                            width=0,
                            fg_color=self._fg_color,
                            border_width=0,
@@ -356,15 +357,15 @@
 
     def set(self, name: str):
         """ select tab by name """
 
         if name in self._tab_dict:
             self._current_name = name
             self._segmented_button.set(name)
-            self._grid_forget_all_tabs()
             self._set_grid_tab_by_name(name)
+            self.after(100, lambda: self._grid_forget_all_tabs(exclude_name=name))
         else:
             raise ValueError(f"CTkTabview has no tab named '{name}'")
 
     def get(self) -> str:
         """ returns name of selected tab, returns empty string if no tab selected """
         return self._current_name
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/ctk_textbox.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/ctk_textbox.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/font/__init__.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/font/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/font/ctk_font.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/font/ctk_font.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,18 @@
 
     def add_size_configure_callback(self, callback: Callable):
         """ add function, that gets called when font got configured """
         self._size_configure_callback_list.append(callback)
 
     def remove_size_configure_callback(self, callback: Callable):
         """ remove function, that gets called when font got configured """
-        self._size_configure_callback_list.remove(callback)
+        try:
+            self._size_configure_callback_list.remove(callback)
+        except ValueError:
+            pass
 
     def create_scaled_tuple(self, font_scaling: float) -> Tuple[str, int, str]:
         """ return scaled tuple representation of font in the form (family: str, size: int, style: str)"""
         return self._family, round(-abs(self._size) * font_scaling), self._tuple_style_string
 
     def config(self, *args, **kwargs):
         raise AttributeError("'config' is not implemented for CTk widgets. For consistency, always use 'configure' instead.")
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/font/font_manager.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/font/font_manager.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/image/ctk_image.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/image/ctk_image.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/scaling/scaling_base_class.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/scaling/scaling_base_class.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/scaling/scaling_tracker.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/scaling/scaling_tracker.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/theme/theme_manager.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/theme/theme_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,20 @@
                 if sys.platform == "darwin":
                     cls.theme[key] = cls.theme[key]["macOS"]
                 elif sys.platform.startswith("win"):
                     cls.theme[key] = cls.theme[key]["Windows"]
                 else:
                     cls.theme[key] = cls.theme[key]["Linux"]
 
+        # fix name inconsistencies
+        if "CTkCheckbox" in cls.theme.keys():
+            cls.theme["CTkCheckBox"] = cls.theme.pop("CTkCheckbox")
+        if "CTkRadiobutton" in cls.theme.keys():
+            cls.theme["CTkRadioButton"] = cls.theme.pop("CTkRadiobutton")
+
     @classmethod
     def save_theme(cls):
         if cls._currently_loaded_theme is not None:
             if cls._currently_loaded_theme not in cls._built_in_themes:
                 with open(cls._currently_loaded_theme, "r") as f:
                     json.dump(cls.theme, f, indent=2)
             else:
```

### Comparing `customtkinter-5.1.3/customtkinter/windows/widgets/utility/utility_functions.py` & `customtkinter-5.2.0/customtkinter/windows/widgets/utility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/customtkinter.egg-info/PKG-INFO` & `customtkinter-5.2.0/customtkinter.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: customtkinter
-Version: 5.1.3
+Version: 5.2.0
 Summary: Create modern looking GUIs with Python
 Home-page: https://customtkinter.tomschimansky.com
 Author: Tom Schimansky
 License: Creative Commons Zero v1.0 Universal
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A modern and customizable python UI-library based on Tkinter: https://customtkinter.tomschimansky.com
```

### Comparing `customtkinter-5.1.3/customtkinter.egg-info/SOURCES.txt` & `customtkinter-5.2.0/customtkinter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `customtkinter-5.1.3/pyproject.toml` & `customtkinter-5.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 github_url = "https://github.com/TomSchimansky/CustomTkinter"
 
 [tool.tbump.version]
-current = "5.1.3"
+current = "5.2.0"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `customtkinter-5.1.3/setup.cfg` & `customtkinter-5.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = customtkinter
-version = 5.1.3
+version = 5.2.0
 description = Create modern looking GUIs with Python
 long_description = A modern and customizable python UI-library based on Tkinter: https://customtkinter.tomschimansky.com
 long_description_content_type = text/markdown
 url = https://customtkinter.tomschimansky.com
 author = Tom Schimansky
 license = Creative Commons Zero v1.0 Universal
 license_file = LICENSE
 classifiers = 
-	License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 
 [project.urls]
 homepage = https://customtkinter.tomschimansky.com
 documentation = https://customtkinter.tomschimansky.com/documentation
 repository = https://github.com/tomschimansky/customtkinter
```

