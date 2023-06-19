# Comparing `tmp/nionui-0.6.8.tar.gz` & `tmp/nionui-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nionui-0.6.8.tar", last modified: Thu Oct  6 20:13:15 2022, max compression
+gzip compressed data, was "nionui-0.6.9.tar", last modified: Fri Nov  4 20:51:25 2022, max compression
```

## Comparing `nionui-0.6.8.tar` & `nionui-0.6.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.509872 nionui-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-10-06 20:13:03.000000 nionui-0.6.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10503 2022-10-06 20:13:15.509872 nionui-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-10-06 20:13:03.000000 nionui-0.6.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.501872 nionui-0.6.8/nion/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.505872 nionui-0.6.8/nion/ui/
--rw-r--r--   0 runner    (1001) docker     (121)    10634 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/Application.py
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/Bitmap.py
--rw-r--r--   0 runner    (1001) docker     (121)   229992 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/CanvasItem.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    94439 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/Declarative.py
--rw-r--r--   0 runner    (1001) docker     (121)    11768 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/Dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)    40761 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/DrawingContext.py
--rw-r--r--   0 runner    (1001) docker     (121)    20122 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/GridCanvasItem.py
--rw-r--r--   0 runner    (1001) docker     (121)    18964 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/ListCanvasItem.py
--rw-r--r--   0 runner    (1001) docker     (121)     5273 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/MouseTrackingCanvasItem.py
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/PreferencesDialog.py
--rw-r--r--   0 runner    (1001) docker     (121)   173553 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/PyQtProxy.py
--rw-r--r--   0 runner    (1001) docker     (121)   101295 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/QtUserInterface.py
--rw-r--r--   0 runner    (1001) docker     (121)    56595 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/TestUI.py
--rw-r--r--   0 runner    (1001) docker     (121)     8578 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/TreeCanvasItem.py
--rw-r--r--   0 runner    (1001) docker     (121)   137805 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/UserInterface.py
--rw-r--r--   0 runner    (1001) docker     (121)    52836 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/Widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    45438 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/Window.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/command.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.505872 nionui-0.6.8/nion/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/resources/stylesheet.qss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.505872 nionui-0.6.8/nion/ui/test/
--rw-r--r--   0 runner    (1001) docker     (121)   114129 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/test/CanvasItem_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/test/Declarative_test.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/test/Dialog_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/test/DrawingContext_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/test/GridCanvasItem_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/test/ListCanvasItem_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/test/TestUI_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/test/Widgets_test.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-06 20:13:03.000000 nionui-0.6.8/nion/ui/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.509872 nionui-0.6.8/nionui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10503 2022-10-06 20:13:15.000000 nionui-0.6.8/nionui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-10-06 20:13:15.000000 nionui-0.6.8/nionui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 20:13:15.000000 nionui-0.6.8/nionui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-06 20:13:15.000000 nionui-0.6.8/nionui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-06 20:13:15.000000 nionui-0.6.8/nionui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-06 20:13:15.000000 nionui-0.6.8/nionui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.501872 nionui-0.6.8/nionui_app/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.501872 nionui-0.6.8/nionui_app/nionui_examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.509872 nionui-0.6.8/nionui_app/nionui_examples/hello_world/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/hello_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/hello_world/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.509872 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Buttons.py
--rw-r--r--   0 runner    (1001) docker     (121)     2859 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/CheckBoxes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComboBoxes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComponentContent.py
--rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComponentLayout.py
--rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComponentPolymorphic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6975 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComponentStack.py
--rw-r--r--   0 runner    (1001) docker     (121)     3337 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Compositions.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Converters.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/LineEdits.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ProgressBars.py
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/RadioButtons.py
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Sections.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Sliders.py
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Stacks.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/StatusBar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/nionui_examples/ui_demo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:15.509872 nionui-0.6.8/nionui_app/none/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 20:13:03.000000 nionui-0.6.8/nionui_app/none/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-06 20:13:03.000000 nionui-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-10-06 20:13:15.509872 nionui-0.6.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       69 2022-10-06 20:13:03.000000 nionui-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.542058 nionui-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-11-04 20:51:13.000000 nionui-0.6.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10710 2022-11-04 20:51:25.542058 nionui-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-04 20:51:13.000000 nionui-0.6.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.530057 nionui-0.6.9/nion/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.538057 nionui-0.6.9/nion/ui/
+-rw-r--r--   0 runner    (1001) docker     (121)    11005 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/Application.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/Bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)   230188 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/CanvasItem.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    94439 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/Declarative.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11768 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/Dialog.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40761 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/DrawingContext.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20122 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/GridCanvasItem.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18964 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/ListCanvasItem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5273 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/MouseTrackingCanvasItem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/PreferencesDialog.py
+-rw-r--r--   0 runner    (1001) docker     (121)   173553 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/PyQtProxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)   101309 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/QtUserInterface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56667 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/TestUI.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8578 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/TreeCanvasItem.py
+-rw-r--r--   0 runner    (1001) docker     (121)   138885 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/UserInterface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52843 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45480 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/Window.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.538057 nionui-0.6.9/nion/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/resources/stylesheet.qss
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.538057 nionui-0.6.9/nion/ui/test/
+-rw-r--r--   0 runner    (1001) docker     (121)   114129 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/test/CanvasItem_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/test/Declarative_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/test/Dialog_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/test/DrawingContext_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/test/GridCanvasItem_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/test/ListCanvasItem_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/test/TestUI_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/test/Widgets_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-04 20:51:13.000000 nionui-0.6.9/nion/ui/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.538057 nionui-0.6.9/nionui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10710 2022-11-04 20:51:25.000000 nionui-0.6.9/nionui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-11-04 20:51:25.000000 nionui-0.6.9/nionui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 20:51:25.000000 nionui-0.6.9/nionui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-04 20:51:25.000000 nionui-0.6.9/nionui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-04 20:51:25.000000 nionui-0.6.9/nionui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-04 20:51:25.000000 nionui-0.6.9/nionui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.530057 nionui-0.6.9/nionui_app/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.530057 nionui-0.6.9/nionui_app/nionui_examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.538057 nionui-0.6.9/nionui_app/nionui_examples/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/hello_world/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.542058 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/
+-rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Buttons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2859 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/CheckBoxes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComboBoxes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComponentContent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComponentLayout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComponentPolymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6975 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComponentStack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3337 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Compositions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Converters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/LineEdits.py
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ProgressBars.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/RadioButtons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Sections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Sliders.py
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Stacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/StatusBar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Tabs.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/nionui_examples/ui_demo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:25.542058 nionui-0.6.9/nionui_app/none/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 20:51:13.000000 nionui-0.6.9/nionui_app/none/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-04 20:51:13.000000 nionui-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2022-11-04 20:51:25.542058 nionui-0.6.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)       69 2022-11-04 20:51:13.000000 nionui-0.6.9/setup.py
```

### Comparing `nionui-0.6.8/LICENSE.txt` & `nionui-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/PKG-INFO` & `nionui-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nionui
-Version: 0.6.8
+Version: 0.6.9
 Summary: Nion UI framework.
 Home-page: https://github.com/nion-software/nionui
 Author: Nion Software
 Author-email: swift@nion.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,14 +17,20 @@
 Introduction
 ============
 This is a UI library that can run with a pyqt, PySide2, or nionui-tool backend.
 
 Changelog (nionui)
 ==================
 
+0.6.9 (2022-11-04)
+------------------
+- Automatically activate windows when showing them.
+- Use alternate low level asyncio on Windows to avoid crash/bug in default.
+- Fix race condition in binding helper.
+
 0.6.8 (2022-10-06)
 ------------------
 - Introduce a Bitmap object to optionally replace uses of NDArray/uint32 bitmaps.
 
 0.6.6 (2022-10-03)
 ------------------
 - Fix regression where line edits not using latest text when still focused.
```

### Comparing `nionui-0.6.8/nion/ui/Application.py` & `nionui-0.6.9/nion/ui/Application.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,18 @@
         self.__event_loop: asyncio.AbstractEventLoop = typing.cast(asyncio.AbstractEventLoop, None)
         # Python 3.9+: typing.List[weakref.ReferenceType[Dialog]]
         self.__dialogs : typing.List[typing.Any] = list()
 
     def initialize(self) -> None:
         """Initialize. Separate from __init__ so that overridden methods can be called."""
         # configure the event loop, which can be used for non-window clients. for backwards compatibility only.
+        if sys.platform == "win32":
+            # hopefully resolves issue with async from a thread (run_coroutine_threadsafe) crashing on Windows.
+            # see https://stackoverflow.com/questions/69833208/runtimeerror-overlapped-overlapped-object-still-has-pending-operation-at-de
+            asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
         self.__event_loop = asyncio.get_event_loop()
 
     def deinitialize(self) -> None:
         self._close_dialogs()
         Process.sync_event_loop(self.__event_loop)
         self.__event_loop = typing.cast(asyncio.AbstractEventLoop, None)
         with open(os.path.join(self.ui.get_data_location(), "PythonConfig.ini"), 'w') as f:
```

### Comparing `nionui-0.6.8/nion/ui/Bitmap.py` & `nionui-0.6.9/nion/ui/Bitmap.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/CanvasItem.py` & `nionui-0.6.9/nion/ui/CanvasItem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1940,14 +1940,18 @@
             layout_sizing._preferred_width = 0
             layout_sizing._maximum_width = 0
             layout_sizing._minimum_height = 0
             layout_sizing._preferred_height = 0
             layout_sizing._maximum_height = 0
         return layout_sizing
 
+    def size_to_content(self) -> None:
+        # I'm not sure if this is the right implementation. It works for now.
+        self.update_sizing(self.layout.get_sizing(self.visible_canvas_items))
+
     def canvas_item_layout_sizing_changed(self, canvas_item: AbstractCanvasItem) -> None:
         """ Contained canvas items call this when their layout_sizing changes. """
         self.refresh_layout()
 
     def _insert_canvas_item_direct(self, before_index: int, canvas_item: AbstractCanvasItem,
                                    pos: typing.Optional[Geometry.IntPoint] = None) -> None:
         self.insert_canvas_item(before_index, canvas_item, pos)
```

### Comparing `nionui-0.6.8/nion/ui/Declarative.py` & `nionui-0.6.9/nion/ui/Declarative.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/Dialog.py` & `nionui-0.6.9/nion/ui/Dialog.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/DrawingContext.py` & `nionui-0.6.9/nion/ui/DrawingContext.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/GridCanvasItem.py` & `nionui-0.6.9/nion/ui/GridCanvasItem.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/ListCanvasItem.py` & `nionui-0.6.9/nion/ui/ListCanvasItem.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/MouseTrackingCanvasItem.py` & `nionui-0.6.9/nion/ui/MouseTrackingCanvasItem.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/PreferencesDialog.py` & `nionui-0.6.9/nion/ui/PreferencesDialog.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/PyQtProxy.py` & `nionui-0.6.9/nion/ui/PyQtProxy.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/QtUserInterface.py` & `nionui-0.6.9/nion/ui/QtUserInterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
 
     def set_property(self, key: str, value: typing.Any) -> None:
         self.proxy.Widget_setWidgetProperty(self.widget, key, self.proxy.encode_variant(value))
 
     def periodic(self) -> None:
         pass
 
-    def _set_root_container(self, window: typing.Optional[Window.Window]) -> None:
+    def _set_root_container(self, window: typing.Optional[UserInterface.Window]) -> None:
         pass
 
     def _get_content_widget(self) -> typing.Optional[UserInterface.Widget]:
         return None
 
     def _register_ui_activity(self) -> None:
         if callable(self.on_ui_activity):
@@ -629,15 +629,15 @@
 
     def close(self) -> None:
         pass
 
     def periodic(self) -> None:
         pass
 
-    def _set_root_container(self, window: typing.Optional[Window.Window]) -> None:
+    def _set_root_container(self, window: typing.Optional[UserInterface.Window]) -> None:
         pass
 
     def _get_content_widget(self) -> typing.Optional[UserInterface.Widget]:
         return None
 
     def set_property(self, key: str, value: typing.Any) -> None:
         pass
```

### Comparing `nionui-0.6.8/nion/ui/TestUI.py` & `nionui-0.6.9/nion/ui/TestUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
         self.children = list()
         self.content = None
         self.canvas_item = None
 
     def periodic(self) -> None:
         pass
 
-    def _set_root_container(self, window: typing.Optional[Window.Window]) -> None:
+    def _set_root_container(self, window: typing.Optional[UserInterfaceModule.Window]) -> None:
         pass
 
     def _get_content_widget(self) -> typing.Optional[UserInterfaceModule.Widget]:
         return None
 
     def _register_ui_activity(self) -> None:
         pass
@@ -590,15 +590,15 @@
 
     def close(self) -> None:
         pass
 
     def periodic(self) -> None:
         pass
 
-    def _set_root_container(self, window: typing.Optional[Window.Window]) -> None:
+    def _set_root_container(self, window: typing.Optional[UserInterfaceModule.Window]) -> None:
         pass
 
     def _get_content_widget(self) -> typing.Optional[UserInterfaceModule.Widget]:
         return None
 
     def set_property(self, key: str, value: typing.Any) -> None:
         pass
@@ -1184,14 +1184,17 @@
         menu = Menu(self, menu_id)
         self._menu_added(menu)
         return menu
 
     def show(self, size: typing.Optional[Geometry.IntSize] = None, position: typing.Optional[Geometry.IntPoint] = None) -> None:
         pass
 
+    def activate(self) -> None:
+        pass
+
     def restore(self, geometry: str, state: str) -> None:
         pass
 
     def _get_focus_widget(self) -> typing.Optional[UserInterfaceModule.Widget]:
         return None
         # wrong type. disabling.
         # global focused_widget
```

### Comparing `nionui-0.6.8/nion/ui/TreeCanvasItem.py` & `nionui-0.6.9/nion/ui/TreeCanvasItem.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/UserInterface.py` & `nionui-0.6.9/nion/ui/UserInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 # standard libraries
 import abc
 import asyncio
 import collections
 import concurrent.futures
 import copy
+import dataclasses
 import enum
 import functools
 import logging
 import numbers
 import operator
 import pathlib
 import threading
@@ -334,14 +335,35 @@
         ...
 
     @abc.abstractmethod
     def set_data_as_string(self, format: str, text: str) -> None:
         ...
 
 
+@dataclasses.dataclass
+class _TaskAndFuture:
+    task: typing.Optional[asyncio.Task[None]] = None
+    future: typing.Optional[concurrent.futures.Future[None]] = None
+    lock = threading.RLock()
+
+    def cancel(self) -> None:
+        with self.lock:
+            if self.task:
+                self.task.cancel()
+                self.task = None
+            if self.future:
+                self.future.cancel()
+                self.future = None
+
+    def clear(self) -> None:
+        with self.lock:
+            self.task = None
+            self.future = None
+
+
 T = typing.TypeVar('T')
 
 class BindablePropertyHelper(typing.Generic[T]):
     def __init__(self,
                  value_getter: typing.Optional[typing.Callable[[], T]],
                  value_setter: typing.Callable[[T], None],
                  value_validator: typing.Optional[typing.Callable[[T, T], T]] = None,
@@ -350,32 +372,27 @@
         self.__value = typing.cast(T, None)
         self.__pending_value = typing.cast(T, None)
         self.__value_getter = value_getter
         self.__value_setter = value_setter
         self.__value_validator = value_validator if callable(value_validator) else lambda x, y: x
         self.__value_cmp = value_cmp if callable(value_cmp) else typing.cast(typing.Callable[[T, T], bool], operator.eq)
         self.__binding: typing.Optional[Binding.Binding] = None
-        self.__task: typing.Optional[asyncio.Task[None]] = None
-        self.__future: typing.Optional[concurrent.futures.Future[None]] = None
 
-        def finalize(task: typing.Optional[asyncio.Task[None]], future: typing.Optional[concurrent.futures.Future[None]]) -> None:
-            if task:
-                task.cancel()
-            if future:
-                future.cancel()
-
-        weakref.finalize(self, finalize, self.__task, self.__future)
-
-    def close(self) -> None:
-        if self.__task:
-            self.__task.cancel()
-            self.__task = None
-        if self.__future:
-            self.__future.cancel()
-            self.__future = None
+        # in order that we can shut down properly in finalize without holding any reference to self, store
+        # both task and future in a single object that can be passed to finalize and will always hold the latest
+        # task and future. the lock will ensure everything shuts down cleanly.
+        self.__task_and_future = _TaskAndFuture()
+
+        def finalize(task_and_future: _TaskAndFuture) -> None:
+            task_and_future.cancel()
+
+        weakref.finalize(self, finalize, self.__task_and_future)
+
+    def close(self) -> None:
+        self.__task_and_future.cancel()
 
     @property
     def value(self) -> T:
         return self.__value_getter() if callable(self.__value_getter) else self.__value
 
     @value.setter
     def value(self, value: T) -> None:
@@ -419,40 +436,48 @@
         self.value = typing.cast(T, binding.get_target_value())
 
         # save the binding and configure the target setter
         # which will set the text when the binding changes
         self.__binding = binding
 
         async def update_value_inner(bph: typing.Any) -> None:
+            # this will always be called on the main thread. avoid holding any references to self so that
+            # dealloc works naturally.
             try:
                 self_ = typing.cast(typing.Optional[BindablePropertyHelper[T]], bph())
                 if self_:
                     try:
                         self_.set_value(self_.__pending_value)
                     finally:
-                        self_.__task = None
-                        self_.__future = None
+                        self_.__task_and_future.clear()
             except Exception as e:
                 import traceback
                 traceback.print_exc()
                 logging.debug(e)
 
         def update_value(bph: typing.Any, event_loop: asyncio.AbstractEventLoop, thread: threading.Thread, value: T) -> None:
+            # threadsafe. target setter may be called from a thread.
             # to avoid repeated cancel/new-task situations that starve the execution during tests,
             # update the pending value and only create a new task if required.
             self_ = typing.cast(typing.Optional[BindablePropertyHelper[T]], bph())
             if self_:
                 self_.__pending_value = value
                 if threading.current_thread() != thread:
-                    if not self_.__future:
-                        self_.__future = asyncio.run_coroutine_threadsafe(update_value_inner(bph), event_loop)
+                    with self_.__task_and_future.lock:
+                        if not self_.__task_and_future.future:
+                            self_.__task_and_future.future = asyncio.run_coroutine_threadsafe(update_value_inner(bph), event_loop)
                 else:
-                    if not self_.__task:
-                        self_.__task = event_loop.create_task(update_value_inner(bph))
-
+                    with self_.__task_and_future.lock:
+                        if not self_.__task_and_future.task:
+                            self_.__task_and_future.task = event_loop.create_task(update_value_inner(bph))
+
+        # the target setter may come in on a thread. call update_value, which is threadsafe. then either dispatch
+        # a future (different thread), a task (same thread), or just update the pending value (pending update).
+        # this ensures the value is updated in update_value_inner in all cases. be careful to use locks for anything
+        # that may have thread contention.
         self.__binding.target_setter = functools.partial(update_value, weakref.ref(self), asyncio.get_event_loop_policy().get_event_loop(), threading.current_thread())
 
     def unbind_value(self) -> None:
         if self.__binding:
             self.__binding.close()
             self.__binding = None
 
@@ -504,30 +529,30 @@
 
     # low level UI specific widget
     @property
     def widget(self) -> typing.Any: raise NotImplementedError()
 
     def close(self) -> None: ...
     def periodic(self) -> None: pass
-    def _set_root_container(self, window: typing.Optional[WindowModule.Window]) -> None: ...
+    def _set_root_container(self, window: typing.Optional[Window]) -> None: ...
     def _get_content_widget(self) -> typing.Optional[Widget]: return None
     def set_property(self, key: str, value: typing.Any) -> None: ...
     def map_to_global(self, p: Geometry.IntPoint) -> Geometry.IntPoint: ...
     def drag(self, mime_data: MimeData, thumbnail: typing.Optional[Bitmap.Bitmap] = None,
              hot_spot_x: typing.Optional[int] = None, hot_spot_y: typing.Optional[int] = None,
              drag_finished_fn: typing.Optional[typing.Callable[[str], None]] = None) -> None: ...
     def set_background_color(self, value: typing.Optional[typing.Union[str, DrawingContext.LinearGradient]]) -> None: ...
 
 
 class Widget:
 
     def __init__(self, widget_behavior: WidgetBehavior) -> None:
         self.__behavior = widget_behavior
         self.__behavior.on_ui_activity = self._register_ui_activity
-        self.__root_container: typing.Optional[WindowModule.Window] = None  # the document window
+        self.__root_container: typing.Optional[Window] = None  # the document window
         self.__pending_keyed_tasks: typing.List[typing.Tuple[str, typing.Callable[[], None]]] = list()
         self.__pending_queued_tasks: typing.List[typing.Callable[[], None]] = list()
         self.on_context_menu_event: typing.Optional[typing.Callable[[int, int, int, int], bool]] = None
         self.on_focus_changed: typing.Optional[typing.Callable[[bool], None]] = None
         self.widget_id: typing.Optional[str] = None
 
         def handle_context_menu_event(x: int, y: int, gx: int, gy: int) -> bool:
@@ -582,18 +607,18 @@
         self.__root_container = None
 
     @property
     def _behavior(self) -> WidgetBehavior:
         return self.__behavior
 
     @property
-    def root_container(self) -> typing.Optional[WindowModule.Window]:
+    def root_container(self) -> typing.Optional[Window]:
         return self.__root_container
 
-    def _set_root_container(self, root_container: typing.Optional[WindowModule.Window]) -> None:
+    def _set_root_container(self, root_container: typing.Optional[Window]) -> None:
         self.__root_container = root_container
         self._behavior._set_root_container(root_container)
         if self.__root_container:
             pending_keyed_tasks = self.__pending_keyed_tasks
             self.__pending_keyed_tasks = list()
             for key, task in pending_keyed_tasks:
                 self.add_task(key, task)
@@ -830,15 +855,15 @@
         self.children = typing.cast(typing.Any, None)
         super().close()
 
     @property
     def _behavior(self) -> BoxWidgetBehavior:
         return typing.cast(BoxWidgetBehavior, super()._behavior)
 
-    def _set_root_container(self, root_container: typing.Optional[WindowModule.Window]) -> None:
+    def _set_root_container(self, root_container: typing.Optional[Window]) -> None:
         super()._set_root_container(root_container)
         for child in self.children:
             child._set_root_container(root_container)
 
     @property
     def _contained_widgets(self) -> typing.List[Widget]:
         return super()._contained_widgets + copy.copy(self.children)
@@ -914,15 +939,15 @@
         self.children = typing.cast(typing.Any, None)
         super().close()
 
     @property
     def _behavior(self) -> SplitterWidgetBehavior:
         return typing.cast(SplitterWidgetBehavior, super()._behavior)
 
-    def _set_root_container(self, root_container: typing.Optional[WindowModule.Window]) -> None:
+    def _set_root_container(self, root_container: typing.Optional[Window]) -> None:
         super()._set_root_container(root_container)
         for child in self.children:
             child._set_root_container(root_container)
 
     @property
     def _contained_widgets(self) -> typing.List[Widget]:
         return super()._contained_widgets + copy.copy(self.children)
@@ -993,15 +1018,15 @@
         self.on_current_index_changed = None
         super().close()
 
     @property
     def _behavior(self) -> TabWidgetBehavior:
         return typing.cast(TabWidgetBehavior, super()._behavior)
 
-    def _set_root_container(self, root_container: typing.Optional[WindowModule.Window]) -> None:
+    def _set_root_container(self, root_container: typing.Optional[Window]) -> None:
         super()._set_root_container(root_container)
         for child in self.children:
             child._set_root_container(root_container)
 
     @property
     def _contained_widgets(self) -> typing.List[Widget]:
         return super()._contained_widgets + copy.copy(self.children)
@@ -1064,15 +1089,15 @@
         self.__current_index_binding_helper = typing.cast(typing.Any, None)
         super().close()
 
     @property
     def _behavior(self) -> StackWidgetBehavior:
         return typing.cast(StackWidgetBehavior, super()._behavior)
 
-    def _set_root_container(self, root_container: typing.Optional[WindowModule.Window]) -> None:
+    def _set_root_container(self, root_container: typing.Optional[Window]) -> None:
         super()._set_root_container(root_container)
         for child in self.children:
             child._set_root_container(root_container)
 
     @property
     def _contained_widgets(self) -> typing.List[Widget]:
         return super()._contained_widgets + copy.copy(self.children)
@@ -1149,15 +1174,15 @@
         self.children = typing.cast(typing.Any, None)
         super().close()
 
     @property
     def _behavior(self) -> GroupWidgetBehavior:
         return typing.cast(GroupWidgetBehavior, super()._behavior)
 
-    def _set_root_container(self, root_container: typing.Optional[WindowModule.Window]) -> None:
+    def _set_root_container(self, root_container: typing.Optional[Window]) -> None:
         super()._set_root_container(root_container)
         for child in self.children:
             child._set_root_container(root_container)
 
     @property
     def _contained_widgets(self) -> typing.List[Widget]:
         return super()._contained_widgets + copy.copy(self.children)
@@ -1236,15 +1261,15 @@
         self.on_viewport_changed = None
         super().close()
 
     @property
     def _behavior(self) -> ScrollAreaWidgetBehavior:
         return typing.cast(ScrollAreaWidgetBehavior, super()._behavior)
 
-    def _set_root_container(self, root_container: typing.Optional[WindowModule.Window]) -> None:
+    def _set_root_container(self, root_container: typing.Optional[Window]) -> None:
         super()._set_root_container(root_container)
         if self.__content:
             self.__content._set_root_container(root_container)
 
     @property
     def _contained_widgets(self) -> typing.List[Widget]:
         return super()._contained_widgets + ([self.__content] if self.__content else list())
@@ -2982,15 +3007,15 @@
 
 class DockWidget:
 
     def __init__(self, document_window: Window, widget: Widget, panel_id: str, title: str, positions: typing.Sequence[str], position: str) -> None:
         self.document_window = document_window
         self.document_window.register_dock_widget(self)
         self.widget = widget
-        self.widget._set_root_container(typing.cast("WindowModule.Window", self))
+        self.widget._set_root_container(typing.cast("Window", self))
         self.panel_id = panel_id
         self.title = title
         self.positions = positions
         self.position = position
         self.on_size_changed: typing.Optional[typing.Callable[[int, int], None]] = None
         self.on_focus_changed: typing.Optional[typing.Callable[[bool], None]] = None
         self.on_ui_activity: typing.Optional[typing.Callable[[], None]] = None
@@ -3157,15 +3182,15 @@
         if callable(self.on_ui_activity):
             self.on_ui_activity()
 
     # attach the root widget to this window
     # the root widget must respond to _set_root_container
     def attach(self, root_widget: Widget) -> None:
         self.root_widget = root_widget
-        self.root_widget._set_root_container(typing.cast("WindowModule.Window", self))
+        self.root_widget._set_root_container(self)
         self._attach_root_widget(root_widget)
 
     def _attach_root_widget(self, root_widget: typing.Optional[Widget]) -> None:
         raise NotImplementedError()
 
     def detach(self) -> None:
         assert self.root_widget is not None
```

### Comparing `nionui-0.6.8/nion/ui/Widgets.py` & `nionui-0.6.9/nion/ui/Widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     def periodic(self) -> None:
         self.content_widget.periodic()
 
     @property
     def widget(self) -> UserInterface.Widget:
         return self.content_widget
 
-    def _set_root_container(self, root_container: typing.Optional[Window.Window]) -> None:
+    def _set_root_container(self, root_container: typing.Optional[UserInterface.Window]) -> None:
         self.content_widget._set_root_container(root_container)
 
     def _get_content_widget(self) -> typing.Optional[UserInterface.Widget]:
         return self.content_widget
 
     def _set_focused(self, focused: bool) -> None:
         pass
```

### Comparing `nionui-0.6.8/nion/ui/Window.py` & `nionui-0.6.9/nion/ui/Window.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,14 +545,15 @@
 
     @property
     def dock_widgets(self) -> typing.Sequence[UserInterface.DockWidget]:
         return self.__document_window.dock_widgets
 
     def show(self, *, size: typing.Optional[Geometry.IntSize] = None, position: typing.Optional[Geometry.IntPoint] = None) -> None:
         self.__document_window.show(size=size, position=position)
+        self.__document_window.activate()
 
     def activate(self) -> None:
         self.__document_window.activate()
 
     def add_menu(self, title: str, menu_id: typing.Optional[str] = None) -> UserInterface.Menu:
         return self.__document_window.add_menu(title, menu_id)
```

### Comparing `nionui-0.6.8/nion/ui/command.py` & `nionui-0.6.9/nion/ui/command.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/resources/stylesheet.qss` & `nionui-0.6.9/nion/ui/resources/stylesheet.qss`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/test/CanvasItem_test.py` & `nionui-0.6.9/nion/ui/test/CanvasItem_test.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/test/Declarative_test.py` & `nionui-0.6.9/nion/ui/test/Declarative_test.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/test/DrawingContext_test.py` & `nionui-0.6.9/nion/ui/test/DrawingContext_test.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/test/GridCanvasItem_test.py` & `nionui-0.6.9/nion/ui/test/GridCanvasItem_test.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/test/ListCanvasItem_test.py` & `nionui-0.6.9/nion/ui/test/ListCanvasItem_test.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/test/TestUI_test.py` & `nionui-0.6.9/nion/ui/test/TestUI_test.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nion/ui/test/Widgets_test.py` & `nionui-0.6.9/nion/ui/test/Widgets_test.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui.egg-info/PKG-INFO` & `nionui-0.6.9/nionui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nionui
-Version: 0.6.8
+Version: 0.6.9
 Summary: Nion UI framework.
 Home-page: https://github.com/nion-software/nionui
 Author: Nion Software
 Author-email: swift@nion.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,14 +17,20 @@
 Introduction
 ============
 This is a UI library that can run with a pyqt, PySide2, or nionui-tool backend.
 
 Changelog (nionui)
 ==================
 
+0.6.9 (2022-11-04)
+------------------
+- Automatically activate windows when showing them.
+- Use alternate low level asyncio on Windows to avoid crash/bug in default.
+- Fix race condition in binding helper.
+
 0.6.8 (2022-10-06)
 ------------------
 - Introduce a Bitmap object to optionally replace uses of NDArray/uint32 bitmaps.
 
 0.6.6 (2022-10-03)
 ------------------
 - Fix regression where line edits not using latest text when still focused.
```

### Comparing `nionui-0.6.8/nionui.egg-info/SOURCES.txt` & `nionui-0.6.9/nionui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/hello_world/main.py` & `nionui-0.6.9/nionui_app/nionui_examples/hello_world/main.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Bindings.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Bindings.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Buttons.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Buttons.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/CheckBoxes.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/CheckBoxes.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComboBoxes.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComboBoxes.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComponentContent.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComponentContent.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComponentLayout.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComponentLayout.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComponentPolymorphic.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComponentPolymorphic.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ComponentStack.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ComponentStack.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Compositions.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Compositions.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Converters.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Converters.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Groups.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Groups.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/LineEdits.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/LineEdits.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/ProgressBars.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/ProgressBars.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/RadioButtons.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/RadioButtons.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Sections.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Sections.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Sliders.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Sliders.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Stacks.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Stacks.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/StatusBar.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/StatusBar.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/Tabs.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/Tabs.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/nionui_app/nionui_examples/ui_demo/main.py` & `nionui-0.6.9/nionui_app/nionui_examples/ui_demo/main.py`

 * *Files identical despite different names*

### Comparing `nionui-0.6.8/setup.cfg` & `nionui-0.6.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nionui
-version = 0.6.8
+version = 0.6.9
 author = Nion Software
 author_email = swift@nion.com
 description = Nion UI framework.
 long_description = file: README.rst, CHANGES.rst, LICENSE.txt
 url = https://github.com/nion-software/nionui
 license = Apache-2.0
 classifiers =
```

