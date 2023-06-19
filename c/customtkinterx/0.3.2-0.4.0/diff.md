# Comparing `tmp/customtkinterx-0.3.2.tar.gz` & `tmp/customtkinterx-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.3.2.tar", max compression
+gzip compressed data, was "customtkinterx-0.4.0.tar", max compression
```

## Comparing `customtkinterx-0.3.2.tar` & `customtkinterx-0.4.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.3.2/customtkinterx/__base64.py
--rw-r--r--   0        0        0     1036 2023-06-10 00:29:27.871591 customtkinterx-0.3.2/customtkinterx/__init__.py
--rw-r--r--   0        0        0      812 2023-06-04 13:04:43.345604 customtkinterx-0.3.2/customtkinterx/__main__.py
--rw-r--r--   0        0        0     8540 2023-06-03 22:47:50.802511 customtkinterx-0.3.2/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     6312 2023-06-03 22:39:55.190954 customtkinterx-0.3.2/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     6344 2023-06-04 13:04:43.403550 customtkinterx-0.3.2/customtkinterx/CTkGhostSharkTheme.py
--rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.3.2/customtkinterx/CTkInfoBar.py
--rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.3.2/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     2596 2023-06-04 02:13:08.630709 customtkinterx-0.3.2/customtkinterx/CTkMegaMenuBar.py
--rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__init__.py
--rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
--rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
--rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
--rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/dropdown_menu.py
--rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/menu_bar.py
--rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.3.2/customtkinterx/CTkMenuBar/title_menu_win.py
--rw-r--r--   0        0        0     6285 2023-06-03 22:42:43.931473 customtkinterx-0.3.2/customtkinterx/CTkMinimalTheme.py
--rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.3.2/customtkinterx/CTkOffice2019Theme.py
--rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/__init__.py
--rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
--rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
--rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.3.2/customtkinterx/CTkTable/__init__.py
--rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.3.2/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.3.2/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
--rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.3.2/customtkinterx/CTkTable/ctktable.py
--rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.3.2/customtkinterx/CTkToolTip/__init__.py
--rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.3.2/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.3.2/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
--rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.3.2/customtkinterx/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0        0        0     5690 2023-06-03 22:45:30.417651 customtkinterx-0.3.2/customtkinterx/Fluent.json
--rw-r--r--   0        0        0      113 2023-06-09 23:34:51.644065 customtkinterx-0.3.2/customtkinterx/fluent_android/__init__.py
--rw-r--r--   0        0        0      305 2023-06-09 23:34:52.417977 customtkinterx-0.3.2/customtkinterx/fluent_android/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7135 2023-06-09 23:42:37.438327 customtkinterx-0.3.2/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc
--rw-r--r--   0        0        0     6375 2023-06-09 23:42:02.599385 customtkinterx-0.3.2/customtkinterx/fluent_android/CTkFluentAndroidTheme.py
--rw-r--r--   0        0        0     1733 2023-06-10 00:34:11.681775 customtkinterx-0.3.2/customtkinterx/fluent_android/CTkFluentAppBar.py
--rw-r--r--   0        0        0     5680 2023-06-10 00:28:44.744869 customtkinterx-0.3.2/customtkinterx/fluent_android/FluentAndroid.json
--rw-r--r--   0        0        0     5437 2023-06-04 13:11:47.958728 customtkinterx-0.3.2/customtkinterx/GhostShark.json
--rw-r--r--   0        0        0    10030 2023-06-10 00:29:27.916591 customtkinterx-0.3.2/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0     5655 2023-06-03 22:45:30.423651 customtkinterx-0.3.2/customtkinterx/Minimal.json
--rw-r--r--   0        0        0     1377 2023-06-04 11:35:40.844283 customtkinterx-0.3.2/customtkinterx/Musix-Dark.png
--rw-r--r--   0        0        0     1039 2023-06-04 11:33:35.093179 customtkinterx-0.3.2/customtkinterx/Musix.png
--rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.3.2/customtkinterx/Office2019.json
--rw-r--r--   0        0        0     5435 2023-06-03 06:15:30.726312 customtkinterx-0.3.2/customtkinterx/tk_dragtool.py
--rw-r--r--   0        0        0      368 2023-06-11 07:35:54.646052 customtkinterx-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3686 2023-06-03 06:54:12.682589 customtkinterx-0.3.2/README.md
--rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 customtkinterx-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.4.0/customtkinterx/__base64.py
+-rw-r--r--   0        0        0     1036 2023-06-10 00:29:27.871591 customtkinterx-0.4.0/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-04 13:04:43.345604 customtkinterx-0.4.0/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     9391 2023-06-19 11:02:43.512474 customtkinterx-0.4.0/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     6312 2023-06-03 22:39:55.190954 customtkinterx-0.4.0/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     6344 2023-06-04 13:04:43.403550 customtkinterx-0.4.0/customtkinterx/CTkGhostSharkTheme.py
+-rw-r--r--   0        0        0     8443 2023-06-19 03:31:06.626442 customtkinterx-0.4.0/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.4.0/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     2596 2023-06-19 00:35:02.877216 customtkinterx-0.4.0/customtkinterx/CTkMegaMenuBar.py
+-rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
+-rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
+-rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/dropdown_menu.py
+-rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/menu_bar.py
+-rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/title_menu_win.py
+-rw-r--r--   0        0        0     6285 2023-06-03 22:42:43.931473 customtkinterx-0.4.0/customtkinterx/CTkMinimalTheme.py
+-rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.4.0/customtkinterx/CTkOffice2019Theme.py
+-rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
+-rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
+-rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.4.0/customtkinterx/CTkTable/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.4.0/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.4.0/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
+-rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.4.0/customtkinterx/CTkTable/ctktable.py
+-rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.4.0/customtkinterx/CTkToolTip/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.4.0/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.4.0/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.4.0/customtkinterx/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0        0        0     6122 2023-06-19 11:03:32.207624 customtkinterx-0.4.0/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0      113 2023-06-09 23:34:51.644065 customtkinterx-0.4.0/customtkinterx/fluent_android/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-09 23:34:52.417977 customtkinterx-0.4.0/customtkinterx/fluent_android/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7135 2023-06-09 23:42:37.438327 customtkinterx-0.4.0/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc
+-rw-r--r--   0        0        0     6375 2023-06-09 23:42:02.599385 customtkinterx-0.4.0/customtkinterx/fluent_android/CTkFluentAndroidTheme.py
+-rw-r--r--   0        0        0     1779 2023-06-19 00:59:49.124414 customtkinterx-0.4.0/customtkinterx/fluent_android/CTkFluentAppBar.py
+-rw-r--r--   0        0        0     5680 2023-06-10 00:28:44.744869 customtkinterx-0.4.0/customtkinterx/fluent_android/FluentAndroid.json
+-rw-r--r--   0        0        0     5437 2023-06-04 13:11:47.958728 customtkinterx-0.4.0/customtkinterx/GhostShark.json
+-rw-r--r--   0        0        0    10024 2023-06-19 11:03:46.583974 customtkinterx-0.4.0/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0     6141 2023-06-19 11:02:43.512474 customtkinterx-0.4.0/customtkinterx/Minimal.json
+-rw-r--r--   0        0        0     1377 2023-06-04 11:35:40.844283 customtkinterx-0.4.0/customtkinterx/Musix-Dark.png
+-rw-r--r--   0        0        0     1039 2023-06-04 11:33:35.093179 customtkinterx-0.4.0/customtkinterx/Musix.png
+-rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.4.0/customtkinterx/Office2019.json
+-rw-r--r--   0        0        0    84836 2022-04-30 00:01:08.000000 customtkinterx-0.4.0/customtkinterx/PublicSans-Regular.ttf
+-rw-r--r--   0        0        0    10586 2023-06-19 01:41:00.500221 customtkinterx-0.4.0/customtkinterx/test.py
+-rw-r--r--   0        0        0      368 2023-06-19 11:04:04.640070 customtkinterx-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3686 2023-06-03 06:54:12.682589 customtkinterx-0.4.0/README.md
+-rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 customtkinterx-0.4.0/PKG-INFO
```

### Comparing `customtkinterx-0.3.2/customtkinterx/__init__.py` & `customtkinterx-0.4.0/customtkinterx/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/__main__.py` & `customtkinterx-0.4.0/customtkinterx/__main__.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkCustom.py` & `customtkinterx-0.4.0/customtkinterx/CTkCustom.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from customtkinter import CTk, CTkToplevel, CTkFrame, CTkLabel, CTkButton, ThemeManager, get_appearance_mode
 from tkinter import ttk
 
 
 class CTkCustom(CTk):
-    def __init__(self, title: str = "", advanced: bool = True, **kwargs):
+    def __init__(self, title: str = "", advanced: bool = True, titlebar: bool = True,
+                 client_edge: bool = False, window_edge: bool = False, titlebar_layout: str = "pack", **kwargs):
         try:
             super().__init__(**kwargs)
         except:
             pass
         from sys import platform
         if advanced:
             if platform == "win32":
@@ -25,22 +26,30 @@
                 self.__transparent_color = '#000001'
 
         self.wm_overrideredirect(True)
 
         if advanced:
             if platform == "win32":
                 from ctypes import windll
+                windll.uxtheme
                 GWL_EXSTYLE = -20
                 WS_EX_APPWINDOW = 0x00040000
                 WS_EX_TOOLWINDOW = 0x00000080
+                WS_EX_CLIENTEDGE = 0x00000200
+                WS_EX_WINDOWEDGE = 0x00000100
                 hwnd = windll.user32.GetParent(self.winfo_id())
                 style = windll.user32.GetWindowLongW(hwnd, GWL_EXSTYLE)
                 style = style & ~WS_EX_TOOLWINDOW
                 style = style | WS_EX_APPWINDOW
+                if client_edge:
+                    style = style | WS_EX_CLIENTEDGE
+                if window_edge:
+                    style = style | WS_EX_WINDOWEDGE
                 res = windll.user32.SetWindowLongW(hwnd, GWL_EXSTYLE, style)
+                self.style32 = style
             else:
                 try:
                     self.wm_attributes("-topmost", True)
                 except:
                     pass
 
         self.minsize(150, 180)
@@ -51,64 +60,16 @@
                                            self.__transparent_color,
                                            self.__transparent_color,
                                            self.__transparent_color
                                        )
                                        )
         self.__frame_border.pack(fill="both", expand=True, padx=0, pady=0)
 
-        self.__frame_title = CTkFrame(self.__frame_border, border_width=0, corner_radius=ThemeManager.theme["CTkFrame"]["corner_radius"]/2+2)
-        self.__frame_title.pack(fill="x", side="top", padx=2, pady=2)
-        self.bind_move(self.__frame_title)
-
-        self.title(title)
-
-        self.maximized = False
-
-        if "CTkCustom" in ThemeManager.theme:
-            self.__frame_title._fg_color = ThemeManager.theme["CTkCustom"]["titlebar_color"]
-            self.__frame_title._draw()
-
-        self.__label_title = CTkLabel(self.__frame_title, text=title)
-        self.__label_title.pack(side="left", anchor="w", padx=10, pady=5)
-        self.bind_move(self.__label_title)
-
-        self.__button_close = CTkButton(self.__frame_title, text="✕", width=30, height=30,
-                                        command=lambda: self.destroy())
-        self.__button_close.pack(side="right", anchor="e", padx=5, pady=5)
-
-        self.__button_minimize = CTkButton(self.__frame_title, text="–", width=30, height=30,
-                                           command=lambda: self.minimize())
-        from sys import platform
-        if platform == "win32":
-            self.__button_minimize.pack(side="right", anchor="e", padx=5, pady=5)
-
-        if "CTkCustom" in ThemeManager.theme:
-
-            self.__label_title._text_color = ThemeManager.theme["CTkCustom"]["title_color"]
-            self.__label_title._draw()
-
-            self.__button_close._text_color = ThemeManager.theme["CTkCustom"]["closebutton_text_color"]
-            self.__button_close._fg_color = ThemeManager.theme["CTkCustom"]["closebutton_color"]
-            self.__button_close._hover_color = ThemeManager.theme["CTkCustom"]["closebutton_hover_color"]
-            self.__button_close._draw()
-
-            self.__button_minimize._text_color = ThemeManager.theme["CTkCustom"]["minimizebutton_text_color"]
-            self.__button_minimize._fg_color = ThemeManager.theme["CTkCustom"]["minimizebutton_color"]
-            self.__button_minimize._hover_color = ThemeManager.theme["CTkCustom"]["minimizebutton_hover_color"]
-            self.__button_minimize._draw()
-
-        if platform == "linux":
-            self.__frame_border.configure(corner_radius=0)
-
-        self.x, self.y = 0, 0
-
-        self.sg_x = 0
-        self.sg_y = 0
-        self.sg_width = 0
-        self.sg_height = 0
+        if titlebar:
+            self.create_titlebar(title)
 
     def minimize(self):
         try:
             from ctypes import windll
             hwnd = windll.user32.GetParent(self.winfo_id())
             windll.user32.ShowWindow(hwnd, 2)
         except:
@@ -147,15 +108,14 @@
             self.geometry(f"{self.sg_width + dx}x{self.sg_height + dy}+{self.sg_x}+{self.sg_y}")
         except TypeError:
             pass
 
     def create_sizegrip(self, custom: bool = False):
         from sys import platform
         if custom:
-            from customtkinterx.tk_dragtool import bind_resize
             self.sizegrip = CTkButton(self.__frame_border, width=32, height=32, text="⚪")
             self.sizegrip.configure(cursor="sizing")
 
             self.sizegrip.bind("<Button-1>", self._sizegrip_click)
             self.sizegrip.bind("<B1-Motion>", self._sizegrip_move)
             self.sizegrip._text_color = ThemeManager.theme["CTkLabel"]["text_color"]
             self.sizegrip._fg_color = self.sizegrip._hover_color = self.__frame_border._fg_color
@@ -166,14 +126,72 @@
                 ttk.Style().configure("CTkCustom.TSizegrip", background=ThemeManager.theme["CTkFrame"]["fg_color"][1])
             else:
                 ttk.Style().configure("CTkCustom.TSizegrip", background=ThemeManager.theme["CTkFrame"]["fg_color"][0])
             self.sizegrip = ttk.Sizegrip(self.__frame_border, style="CTkCustom.TSizegrip")
             self.sizegrip.pack(side="bottom", anchor="se", padx=5, pady=5, ipady=2)
         return self.sizegrip
 
+    def create_titlebar(self, title: str, titlebar_layout: str = "pack"):
+
+        self.__frame_title = CTkFrame(self.__frame_border, border_width=0, corner_radius=ThemeManager.theme["CTkFrame"]["corner_radius"]/2+2)
+        self.__frame_title.pack(fill="x", side="top", padx=2, pady=2)
+        self.bind_move(self.__frame_title)
+
+        self.title(title)
+
+        self.maximized = False
+
+        if "CTkCustom" in ThemeManager.theme:
+            self.__frame_title._fg_color = ThemeManager.theme["CTkCustom"]["titlebar_color"]
+            self.__frame_title._draw()
+
+        self.__label_title = CTkLabel(self.__frame_title, text=title)
+        self.__label_title.pack(side="left", anchor="w", padx=10, pady=5)
+        self.bind_move(self.__label_title)
+
+        self.__button_close = CTkButton(self.__frame_title, text="✕", width=30, height=30,
+                                        command=lambda: self.destroy())
+        self.__button_close.pack(side="right", anchor="e", padx=5, pady=5)
+
+        self.__button_minimize = CTkButton(self.__frame_title, text="–", width=30, height=30,
+                                           command=lambda: self.minimize())
+        from sys import platform
+        if platform == "win32":
+            self.__button_minimize.pack(side="right", anchor="e", padx=5, pady=5)
+
+        if "CTkCustom" in ThemeManager.theme:
+
+            self.__label_title._text_color = ThemeManager.theme["CTkCustom"]["title_color"]
+            self.__label_title._draw()
+
+            self.__button_close._text_color = ThemeManager.theme["CTkCustom"]["closebutton_text_color"]
+            self.__button_close._fg_color = ThemeManager.theme["CTkCustom"]["closebutton_color"]
+            self.__button_close._hover_color = ThemeManager.theme["CTkCustom"]["closebutton_hover_color"]
+            self.__button_close._border_width = ThemeManager.theme["CTkCustom"]["closebutton_border_width"]
+            self.__button_close._draw()
+
+            self.__button_minimize._text_color = ThemeManager.theme["CTkCustom"]["minimizebutton_text_color"]
+            self.__button_minimize._fg_color = ThemeManager.theme["CTkCustom"]["minimizebutton_color"]
+            self.__button_minimize._hover_color = ThemeManager.theme["CTkCustom"]["minimizebutton_hover_color"]
+            self.__button_minimize._border_width = ThemeManager.theme["CTkCustom"]["minimizebutton_border_width"]
+            self.__button_minimize._draw()
+
+        if platform == "linux":
+            self.__frame_border.configure(corner_radius=0)
+
+        self.x, self.y = 0, 0
+
+        self.sg_x = 0
+        self.sg_y = 0
+        self.sg_width = 0
+        self.sg_height = 0
+
+    def hide_titlebar(self):
+        self.__frame_title.forget()
+
     @property
     def titlebar(self):
         return self.__frame_title
 
     @property
     def titlebar_title(self):
         return self.__label_title
@@ -203,12 +221,12 @@
 
 
 class CTkCustomToplevel(CTkCustom, CTkToplevel):
     pass
 
 
 if __name__ == '__main__':
-    root = CTkCustom()
+    root = CTkCustom(window_edge=True)
     root.title("helloworld")
     root.titlebar_title.configure(text="helloworld")
 
     root.mainloop()
```

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.4.0/customtkinterx/CTkFluentTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkGhostSharkTheme.py` & `customtkinterx-0.4.0/customtkinterx/CTkGhostSharkTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkListBox.py` & `customtkinterx-0.4.0/customtkinterx/CTkListBox.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkMegaMenuBar.py` & `customtkinterx-0.4.0/customtkinterx/CTkMegaMenuBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc` & `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc` & `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc` & `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc` & `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/dropdown_menu.py` & `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/menu_bar.py` & `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkMenuBar/title_menu_win.py` & `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkMinimalTheme.py` & `customtkinterx-0.4.0/customtkinterx/CTkMinimalTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkOffice2019Theme.py` & `customtkinterx-0.4.0/customtkinterx/CTkOffice2019Theme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc` & `customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py` & `customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc` & `customtkinterx-0.4.0/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkTable/ctktable.py` & `customtkinterx-0.4.0/customtkinterx/CTkTable/ctktable.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc` & `customtkinterx-0.4.0/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/CTkToolTip/ctk_tooltip.py` & `customtkinterx-0.4.0/customtkinterx/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/Fluent.json` & `customtkinterx-0.4.0/customtkinterx/Fluent.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857503607503608%*

 * *Differences: {"'CTkCustom'": "{'closebutton_border_width': 0, 'minimizebutton_border_width': 0}",*

 * * "'CTkInfoBar'": "{'border_width': 1, 'text_color': ['#000000', '#ffffff'], 'success_text_color': "*

 * *                 "['#118d57', '#77ed8b'], 'success_border_color': ['#c8eed7', '#194331'], "*

 * *                 "'caution_text_color': ['#b76e00', '#fed566'], 'caution_border_color': "*

 * *                 "['#fae7c2', '#4b3c1c'], 'critical_text_color': ['#b71d18', '#ffac82'], "*

 * *                 "'critical_border_color': ['#fad5cd', […]*

```diff
@@ -82,26 +82,28 @@
         ],
         "text_color_disabled": [
             "gray50",
             "gray45"
         ]
     },
     "CTkCustom": {
+        "closebutton_border_width": 0,
         "closebutton_color": [
             "#ffffff",
             "#2c2c2c"
         ],
         "closebutton_hover_color": [
             "#b40d1b",
             "#b40d1b"
         ],
         "closebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
+        "minimizebutton_border_width": 0,
         "minimizebutton_color": [
             "#ffffff",
             "#2c2c2c"
         ],
         "minimizebutton_hover_color": [
             "#cccccc",
             "#282828"
@@ -174,47 +176,75 @@
         ]
     },
     "CTkInfoBar": {
         "border_color": [
             "#b0b2b2",
             "#424556"
         ],
-        "border_width": 0,
+        "border_width": 1,
+        "caution_border_color": [
+            "#fae7c2",
+            "#4b3c1c"
+        ],
         "caution_color": [
             "#fff4ce",
             "#433519"
         ],
         "caution_hover_color": [
             "#ccc3a4",
             "#695327"
         ],
+        "caution_text_color": [
+            "#b76e00",
+            "#fed566"
+        ],
         "corner_radius": 8,
+        "critical_border_color": [
+            "#fad5cd",
+            "#4b2927"
+        ],
         "critical_color": [
             "#fde7e9",
             "#442726"
         ],
         "critical_hover_color": [
             "#cab8ba",
             "#6a3c3b"
         ],
+        "critical_text_color": [
+            "#b71d18",
+            "#ffac82"
+        ],
         "fg_color": [
             "#f7f7f7",
             "#2f2f2f"
         ],
         "fg_hover_color": [
             "#c3c3c3",
             "#555555"
         ],
+        "success_border_color": [
+            "#c8eed7",
+            "#194331"
+        ],
         "success_color": [
             "#dff6dd",
             "#393d1b"
         ],
         "success_hover_color": [
             "#b0c3af",
             "#5c632b"
+        ],
+        "success_text_color": [
+            "#118d57",
+            "#77ed8b"
+        ],
+        "text_color": [
+            "#000000",
+            "#ffffff"
         ]
     },
     "CTkLabel": {
         "corner_radius": 0,
         "fg_color": "transparent",
         "text_color": [
             "gray10",
```

### Comparing `customtkinterx-0.3.2/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc` & `customtkinterx-0.4.0/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/fluent_android/CTkFluentAndroidTheme.py` & `customtkinterx-0.4.0/customtkinterx/fluent_android/CTkFluentAndroidTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/fluent_android/CTkFluentAppBar.py` & `customtkinterx-0.4.0/customtkinterx/fluent_android/CTkFluentAppBar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from customtkinter import CTkFrame, CTkLabel, CTkFont, CTkButton
 from customtkinterx.fluent_android import CTkFluentAndroidTheme
+from customtkinterx.CTkCustom import CTkCustom
 
 
 class CTkFluentAppBar(CTkFrame):
     def __init__(self, master=None, *args, width=360, height=80, title: str = "Title", subtitle: str = "Subtitle", bg_color="#ffffff", **kwargs):
         super().__init__(master, *args, width=width, height=height, bg_color=bg_color, **kwargs)
 
         self.__title = CTkLabel(self, text=title, font=CTkFont(family="Roboto", size=15, weight="bold"))
@@ -38,15 +39,15 @@
     CTkFluentAndroidTheme()
 
     root = CTkCustom()
     root.geometry("380x680")
 
     set_widget_scaling(1.2)
 
-    root.titlebar.forget()
+    root.hide_titlebar()
     root.create_sizegrip(False)
 
     appbar = CTkFluentAppBar(root.mainframe)
     root.bind_move(appbar)
     appbar.pack(fill="x", side="top", padx=1, pady=1)
 
     button1 = CTkButton(root.mainframe, width=90, height=38)
```

### Comparing `customtkinterx-0.3.2/customtkinterx/fluent_android/FluentAndroid.json` & `customtkinterx-0.4.0/customtkinterx/fluent_android/FluentAndroid.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/GhostShark.json` & `customtkinterx-0.4.0/customtkinterx/GhostShark.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/LaunchMusix.py` & `customtkinterx-0.4.0/customtkinterx/LaunchMusix.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             self.download = CTkButton(self, width=100, text="下载", command=download)
             self.download.pack(side="right", padx=5, pady=5)
 
             self.args = CTkComboBox(self, values=["standard", "higher", "exhigh", "lossless"])
             self.args.set("higher")
             self.args.pack(side="right", padx=5, pady=5)
 
-    CTkFluentAndroidTheme()
+    CTkMinimalTheme()
     set_appearance_mode("Light")
 
     root = CTkCustom(title="Musix")
     root.titlebar.configure(corner_radius=13)
     root.geometry("720x360")
 
     from sys import platform
```

### Comparing `customtkinterx-0.3.2/customtkinterx/Minimal.json` & `customtkinterx-0.4.0/customtkinterx/Office2019.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9038183707826565%*

 * *Differences: {"'CTk'": "{'fg_color': ['#ffffff', '#101010']}",*

 * * "'CTkButton'": "{'corner_radius': 0, 'border_width': 1, 'fg_color': ['#e5e5e5', '#3d3d3d'], "*

 * *                "'hover_color': ['#b2b2b2', '#151515'], 'text_color': {insert: [(1, '#ffffff')], "*

 * *                'delete: [0]}}',*

 * * "'CTkComboBox'": "{'corner_radius': 0, 'fg_color': ['#ffffff', '#2f2f2f'], 'border_color': "*

 * *                  "['#f3f3f3', '#949A9F'], 'button_color': ['#f2f2f2', '#565B5E'], "*

 * *                  "'button_hover_color': ['#f2f2f2', '#5 […]*

```diff
@@ -1,26 +1,32 @@
 {
     "CTk": {
         "fg_color": [
-            "#f9fafb",
-            "#161c24"
+            "#ffffff",
+            "#101010"
         ]
     },
     "CTkButton": {
         "border_color": [
             "#f3f3f3",
             "#949A9F"
         ],
-        "border_width": 0,
-        "corner_radius": 10,
-        "fg_color": "#00ab55",
-        "hover_color": "#007b55",
+        "border_width": 1,
+        "corner_radius": 0,
+        "fg_color": [
+            "#e5e5e5",
+            "#3d3d3d"
+        ],
+        "hover_color": [
+            "#b2b2b2",
+            "#151515"
+        ],
         "text_color": [
-            "#ffffff",
-            "#000000"
+            "#000000",
+            "#ffffff"
         ],
         "text_color_disabled": [
             "gray74",
             "gray60"
         ]
     },
     "CTkCheckbox": {
@@ -49,85 +55,85 @@
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkComboBox": {
         "border_color": [
-            "#c4cdd5",
-            "#637381"
+            "#f3f3f3",
+            "#949A9F"
         ],
         "border_width": 1,
         "button_color": [
-            "#c4cdd5",
-            "#637381"
+            "#f2f2f2",
+            "#565B5E"
         ],
         "button_hover_color": [
-            "#919eab",
-            "#919eab"
+            "#f2f2f2",
+            "#565B5E"
         ],
-        "corner_radius": 10,
+        "corner_radius": 0,
         "fg_color": [
-            "#dfe3e8",
-            "#454f5b"
+            "#ffffff",
+            "#2f2f2f"
         ],
         "text_color": [
             "gray10",
             "#ffffff"
         ],
         "text_color_disabled": [
             "gray50",
             "gray45"
         ]
     },
     "CTkCustom": {
         "closebutton_color": [
-            "#f4f6f8",
-            "#212b36"
+            "#ffffff",
+            "#2c2c2c"
         ],
         "closebutton_hover_color": [
             "#b40d1b",
             "#b40d1b"
         ],
         "closebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
         "minimizebutton_color": [
-            "#f4f6f8",
-            "#212b36"
+            "#ffffff",
+            "#2c2c2c"
         ],
         "minimizebutton_hover_color": [
-            "#dfe3e8",
-            "#454f5b"
+            "#cccccc",
+            "#282828"
         ],
         "minimizebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
         "title_color": [
-            "gray10",
-            "#DCE4EE"
+            "#ffffff",
+            "#ffffff"
         ],
         "titlebar_color": [
-            "#f4f6f8",
-            "#212b36"
+            "#106ebe",
+            "#106ebe"
         ],
         "transparent_color": "#101010"
     },
     "CTkEntry": {
         "border_color": [
-            "#c4cdd5",
-            "#637381"
+            "#f3f3f3",
+            "#949A9F"
         ],
         "border_width": 1,
-        "corner_radius": 10,
+        "corner_radius": 0,
         "fg_color": [
-            "#dfe3e8",
-            "#454f5b"
+            "#ffffff",
+            "#2f2f2f"
         ],
         "placeholder_text_color": [
             "gray52",
             "gray62"
         ],
         "text_color": [
             "#000000",
@@ -137,78 +143,78 @@
     "CTkFont": {
         "Linux": {
             "family": "Roboto",
             "size": 13,
             "weight": "normal"
         },
         "Windows": {
-            "family": "Roboto",
+            "family": "Segoe UI",
             "size": 13,
             "weight": "normal"
         },
         "macOS": {
             "family": "SF Display",
             "size": 13,
             "weight": "normal"
         }
     },
     "CTkFrame": {
         "border_color": [
-            "#edeff1",
-            "#212b36"
+            "#b0b2b2",
+            "#424556"
         ],
         "border_width": 1,
-        "corner_radius": 10,
+        "corner_radius": 0,
         "fg_color": [
-            "#f9fafb",
-            "#161c24"
+            "#ffffff",
+            "#1c1c1c"
         ],
         "top_fg_color": [
-            "#f4f6f8",
-            "#212b36"
+            "#ffffff",
+            "#2c2c2c"
         ]
     },
     "CTkInfoBar": {
         "border_color": [
             "#b0b2b2",
             "#424556"
         ],
         "border_width": 0,
         "caution_color": [
-            "#ffd666",
-            "#b76e00"
+            "#fff4ce",
+            "#433519"
         ],
         "caution_hover_color": [
-            "#fff5cc",
-            "#7a4100"
+            "#ccc3a4",
+            "#695327"
         ],
         "corner_radius": 8,
         "critical_color": [
-            "#ffac82",
-            "#b71d18"
+            "#fde7e9",
+            "#442726"
         ],
         "critical_hover_color": [
-            "#ffe9d5",
-            "#7a0916"
+            "#cab8ba",
+            "#6a3c3b"
         ],
         "fg_color": [
-            "#61f3f3",
-            "#006c9c"
+            "#f7f7f7",
+            "#2f2f2f"
         ],
         "fg_hover_color": [
-            "#cafdf5",
-            "#003768"
+            "#c3c3c3",
+            "#555555"
         ],
         "success_color": [
-            "#86e8ab",
-            "#1b806a"
+            "#dff6dd",
+            "#393d1b"
         ],
         "success_hover_color": [
-            "#d8fbde",
-            "#0a5554"
+            "#b0c3af",
+            "#5c632b"
         ]
     },
     "CTkLabel": {
         "corner_radius": 0,
         "fg_color": "transparent",
         "text_color": [
             "gray10",
@@ -282,24 +288,24 @@
     "CTkScrollableFrame": {
         "label_fg_color": [
             "gray78",
             "gray23"
         ]
     },
     "CTkScrollbar": {
-        "border_spacing": 4,
+        "border_spacing": 9,
         "button_color": [
-            "#f4f6f8",
-            "#212b36"
+            "gray55",
+            "gray41"
         ],
         "button_hover_color": [
-            "#dfe3e8",
-            "#454f5b"
+            "gray40",
+            "gray53"
         ],
-        "corner_radius": 1000,
+        "corner_radius": 0,
         "fg_color": "transparent"
     },
     "CTkSegmentedButton": {
         "border_width": 2,
         "corner_radius": 6,
         "fg_color": [
             "#979DA2",
@@ -349,49 +355,52 @@
         ],
         "progress_color": [
             "gray40",
             "#AAB0B5"
         ]
     },
     "CTkSwitch": {
-        "border_width": 0,
+        "border_width": 1,
         "button_color": [
-            "#f9fafb",
-            "#161c24"
+            "#f3f3f3",
+            "#000000"
         ],
         "button_hover_color": [
-            "#f4f6f8",
-            "#212b36"
+            "#bfbfbf",
+            "#050505"
         ],
-        "button_length": 0,
-        "corner_radius": 1000,
+        "button_length": 2,
+        "corner_radius": 8,
         "fg_color": [
-            "#c4cdd5",
-            "#637381"
+            "#ededed",
+            "#1d1d1d"
+        ],
+        "progress_color": [
+            "#0067c0",
+            "#4cc2ff"
         ],
-        "progress_color": "#00ab55",
         "text_color": [
             "gray10",
             "#DCE4EE"
         ],
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkTextbox": {
         "border_color": [
-            "#979DA2",
-            "#565B5E"
+            "#f3f3f3",
+            "#949A9F"
         ],
-        "border_width": 0,
-        "corner_radius": 6,
+        "border_width": 1,
+        "corner_radius": 0,
         "fg_color": [
-            "#dfe3e8",
-            "#454f5b"
+            "#F9F9FA",
+            "#1D1E1E"
         ],
         "scrollbar_button_color": [
             "gray55",
             "gray41"
         ],
         "scrollbar_button_hover_color": [
             "gray40",
@@ -400,16 +409,16 @@
         "text_color": [
             "gray10",
             "#DCE4EE"
         ]
     },
     "CTkToplevel": {
         "fg_color": [
-            "#f9fafb",
-            "#161c24"
+            "#ffffff",
+            "#101010"
         ]
     },
     "DropdownMenu": {
         "fg_color": [
             "gray90",
             "#1c1c1c"
         ],
```

### Comparing `customtkinterx-0.3.2/customtkinterx/Musix-Dark.png` & `customtkinterx-0.4.0/customtkinterx/Musix-Dark.png`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/Musix.png` & `customtkinterx-0.4.0/customtkinterx/Musix.png`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/customtkinterx/Office2019.json` & `customtkinterx-0.4.0/customtkinterx/Minimal.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8064146281408187%*

 * *Differences: {"'CTk'": "{'fg_color': ['#f9fafb', '#161c24']}",*

 * * "'CTkButton'": "{'corner_radius': 9, 'fg_color': ['#f9fafb', '#161c24'], 'hover_color': "*

 * *                "['#e5f3f0', '#14272a'], 'border_color': ['#82d2b8', '#0b5f48'], 'text_color': "*

 * *                "['#00a76f', '#00a76f'], 'text_color_disabled': ['#a6b0bb', '#788490']}",*

 * * "'CTkCheckbox'": "{'corner_radius': 8, 'border_width': 2, 'fg_color': ['#00a76f', '#00a76f'], "*

 * *                  "'border_color': ['#637381', '#919eab'], 'hover_color': ['#00a76f', ' […]*

```diff
@@ -1,434 +1,461 @@
 {
     "CTk": {
         "fg_color": [
-            "#ffffff",
-            "#101010"
+            "#f9fafb",
+            "#161c24"
         ]
     },
     "CTkButton": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#82d2b8",
+            "#0b5f48"
         ],
         "border_width": 1,
-        "corner_radius": 0,
+        "corner_radius": 9,
         "fg_color": [
-            "#e5e5e5",
-            "#3d3d3d"
+            "#f9fafb",
+            "#161c24"
         ],
         "hover_color": [
-            "#b2b2b2",
-            "#151515"
+            "#e5f3f0",
+            "#14272a"
         ],
         "text_color": [
-            "#000000",
-            "#ffffff"
+            "#00a76f",
+            "#00a76f"
         ],
         "text_color_disabled": [
-            "gray74",
-            "gray60"
+            "#a6b0bb",
+            "#788490"
         ]
     },
     "CTkCheckbox": {
         "border_color": [
-            "#3E454A",
-            "#949A9F"
+            "#637381",
+            "#919eab"
         ],
-        "border_width": 3,
+        "border_width": 2,
         "checkmark_color": [
-            "#DCE4EE",
-            "gray90"
+            "#f9fafb",
+            "#161c24"
         ],
-        "corner_radius": 6,
+        "corner_radius": 8,
         "fg_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "hover_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "text_color": [
-            "gray10",
-            "#DCE4EE"
+            "#212b36",
+            "#f8f8f8"
         ],
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkComboBox": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#c4cdd5",
+            "#637381"
         ],
         "border_width": 1,
         "button_color": [
-            "#f2f2f2",
-            "#565B5E"
+            "#c4cdd5",
+            "#637381"
         ],
         "button_hover_color": [
-            "#f2f2f2",
-            "#565B5E"
+            "#919eab",
+            "#919eab"
         ],
-        "corner_radius": 0,
+        "corner_radius": 10,
         "fg_color": [
-            "#ffffff",
-            "#2f2f2f"
+            "#dfe3e8",
+            "#454f5b"
         ],
         "text_color": [
             "gray10",
             "#ffffff"
         ],
         "text_color_disabled": [
             "gray50",
             "gray45"
         ]
     },
     "CTkCustom": {
+        "closebutton_border_width": 0,
         "closebutton_color": [
-            "#ffffff",
-            "#2c2c2c"
+            "#f4f6f8",
+            "#212b36"
         ],
         "closebutton_hover_color": [
             "#b40d1b",
             "#b40d1b"
         ],
         "closebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
+        "minimizebutton_border_width": 0,
         "minimizebutton_color": [
-            "#ffffff",
-            "#2c2c2c"
+            "#f4f6f8",
+            "#212b36"
         ],
         "minimizebutton_hover_color": [
-            "#cccccc",
-            "#282828"
+            "#dfe3e8",
+            "#454f5b"
         ],
         "minimizebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
         "title_color": [
-            "#ffffff",
-            "#ffffff"
+            "gray10",
+            "#DCE4EE"
         ],
         "titlebar_color": [
-            "#106ebe",
-            "#106ebe"
+            "#f4f6f8",
+            "#161c24"
         ],
         "transparent_color": "#101010"
     },
     "CTkEntry": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#eaedf0",
+            "#2f363f"
         ],
         "border_width": 1,
-        "corner_radius": 0,
+        "corner_radius": 10,
         "fg_color": [
-            "#ffffff",
-            "#2f2f2f"
+            "#f9fafb",
+            "#161c24"
         ],
         "placeholder_text_color": [
-            "gray52",
-            "gray62"
+            "#a6b0bb",
+            "#637381"
         ],
         "text_color": [
-            "#000000",
+            "#212b36",
             "#ffffff"
         ]
     },
     "CTkFont": {
         "Linux": {
             "family": "Roboto",
             "size": 13,
             "weight": "normal"
         },
         "Windows": {
-            "family": "Segoe UI",
+            "family": "Roboto",
             "size": 13,
             "weight": "normal"
         },
         "macOS": {
             "family": "SF Display",
             "size": 13,
             "weight": "normal"
         }
     },
     "CTkFrame": {
         "border_color": [
-            "#b0b2b2",
-            "#424556"
+            "#edeff1",
+            "#212b36"
         ],
         "border_width": 1,
-        "corner_radius": 0,
+        "corner_radius": 10,
         "fg_color": [
-            "#ffffff",
-            "#1c1c1c"
+            "#f9fafb",
+            "#161c24"
         ],
         "top_fg_color": [
-            "#ffffff",
-            "#2c2c2c"
+            "#f4f6f8",
+            "#212b36"
         ]
     },
     "CTkInfoBar": {
         "border_color": [
-            "#b0b2b2",
-            "#424556"
+            "#c0ebf3",
+            "#113f4d"
+        ],
+        "border_width": 1,
+        "caution_border_color": [
+            "#fae7c2",
+            "#4b3c1c"
         ],
-        "border_width": 0,
         "caution_color": [
-            "#fff4ce",
-            "#433519"
+            "#f9f3e7",
+            "#292721"
         ],
         "caution_hover_color": [
-            "#ccc3a4",
-            "#695327"
+            "#fae7c2",
+            "#4b3c1c"
+        ],
+        "caution_text_color": [
+            "#b76e00",
+            "#fed566"
         ],
         "corner_radius": 8,
+        "critical_border_color": [
+            "#fad5cd",
+            "#4b2927"
+        ],
         "critical_color": [
-            "#fde7e9",
-            "#442726"
+            "#f9edeb",
+            "#292125"
         ],
         "critical_hover_color": [
-            "#cab8ba",
-            "#6a3c3b"
+            "#fad5cd",
+            "#4b2927"
+        ],
+        "critical_text_color": [
+            "#b71d18",
+            "#ffac82"
         ],
         "fg_color": [
-            "#f7f7f7",
-            "#2f2f2f"
+            "#e5f4f8",
+            "#142832"
         ],
         "fg_hover_color": [
-            "#c3c3c3",
-            "#555555"
+            "#c0ebf3",
+            "#113f4d"
+        ],
+        "success_border_color": [
+            "#c8eed7",
+            "#194331"
         ],
         "success_color": [
-            "#dff6dd",
-            "#393d1b"
+            "#e8f5ee",
+            "#172a29"
         ],
         "success_hover_color": [
-            "#b0c3af",
-            "#5c632b"
+            "#c8eed7",
+            "#194331"
+        ],
+        "success_text_color": [
+            "#118d57",
+            "#77ed8b"
+        ],
+        "text_color": [
+            "#006c9c",
+            "#61f3f3"
         ]
     },
     "CTkLabel": {
         "corner_radius": 0,
         "fg_color": "transparent",
         "text_color": [
             "gray10",
             "#DCE4EE"
         ]
     },
     "CTkOptionMenu": {
         "button_color": [
-            "#36719F",
-            "#144870"
+            "#007867",
+            "#007867"
         ],
         "button_hover_color": [
-            "#27577D",
-            "#203A4F"
+            "#007867",
+            "#007867"
         ],
-        "corner_radius": 6,
+        "corner_radius": 8,
         "fg_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "text_color": [
-            "#DCE4EE",
-            "#DCE4EE"
+            "#ffffff",
+            "#ffffff"
         ],
         "text_color_disabled": [
             "gray74",
             "gray60"
         ]
     },
     "CTkProgressBar": {
         "border_color": [
-            "gray",
-            "gray"
+            "#00a76f",
+            "#00a76f"
         ],
         "border_width": 0,
-        "corner_radius": 1000,
+        "corner_radius": 16,
         "fg_color": [
-            "#939BA2",
-            "#4A4D50"
+            "#bde6da",
+            "#113d36"
         ],
         "progress_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ]
     },
     "CTkRadiobutton": {
         "border_color": [
-            "#3E454A",
-            "#949A9F"
+            "#637381",
+            "#919eab"
         ],
         "border_width_checked": 6,
-        "border_width_unchecked": 3,
+        "border_width_unchecked": 2,
         "corner_radius": 1000,
         "fg_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "hover_color": [
-            "#36719F",
-            "#144870"
+            "#00a76f",
+            "#00a76f"
         ],
         "text_color": [
-            "gray10",
-            "#DCE4EE"
+            "#212b36",
+            "#f8f8f8"
         ],
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkScrollableFrame": {
         "label_fg_color": [
-            "gray78",
-            "gray23"
+            "#f9fafb",
+            "#161c24"
         ]
     },
     "CTkScrollbar": {
-        "border_spacing": 9,
+        "border_spacing": 4,
         "button_color": [
-            "gray55",
-            "gray41"
+            "#a0abb7",
+            "#788490"
         ],
         "button_hover_color": [
-            "gray40",
-            "gray53"
+            "#a3aeb9",
+            "#7b8793"
         ],
-        "corner_radius": 0,
+        "corner_radius": 1000,
         "fg_color": "transparent"
     },
     "CTkSegmentedButton": {
-        "border_width": 2,
-        "corner_radius": 6,
+        "border_width": 4,
+        "corner_radius": 12,
         "fg_color": [
-            "#979DA2",
-            "gray29"
+            "#ffffff",
+            "#212b36"
         ],
         "selected_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#ffffff",
+            "#212b36"
         ],
         "selected_hover_color": [
-            "#36719F",
-            "#144870"
+            "#00744d",
+            "#00744d"
         ],
         "text_color": [
-            "#DCE4EE",
+            "#212b36",
             "#DCE4EE"
         ],
         "text_color_disabled": [
-            "gray74",
+            "#637381",
             "gray60"
         ],
         "unselected_color": [
-            "#979DA2",
-            "gray29"
+            "#ffffff",
+            "#212b36"
         ],
         "unselected_hover_color": [
-            "gray70",
-            "gray41"
+            "#00a76f",
+            "#00a76f"
         ]
     },
     "CTkSlider": {
         "border_width": 6,
         "button_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "button_corner_radius": 1000,
         "button_hover_color": [
-            "#36719F",
-            "#144870"
+            "#00a76f",
+            "#00a76f"
         ],
         "button_length": 0,
         "corner_radius": 1000,
         "fg_color": [
-            "#939BA2",
-            "#4A4D50"
+            "#bde6da",
+            "#113d36"
         ],
         "progress_color": [
-            "gray40",
-            "#AAB0B5"
+            "#00a76f",
+            "#00a76f"
         ]
     },
     "CTkSwitch": {
-        "border_width": 1,
+        "border_width": 0,
         "button_color": [
-            "#f3f3f3",
-            "#000000"
+            "#f9fafb",
+            "#ffffff"
         ],
         "button_hover_color": [
-            "#bfbfbf",
-            "#050505"
+            "#f4f6f8",
+            "#ffffff"
         ],
-        "button_length": 2,
-        "corner_radius": 8,
+        "button_length": 0,
+        "corner_radius": 1000,
         "fg_color": [
-            "#ededed",
-            "#1d1d1d"
-        ],
-        "progress_color": [
-            "#0067c0",
-            "#4cc2ff"
+            "#c7ced5",
+            "#637381"
         ],
+        "progress_color": "#00a46d",
         "text_color": [
             "gray10",
             "#DCE4EE"
         ],
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkTextbox": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#eaedf0",
+            "#2f363f"
         ],
         "border_width": 1,
-        "corner_radius": 0,
+        "corner_radius": 10,
         "fg_color": [
-            "#F9F9FA",
-            "#1D1E1E"
+            "#f9fafb",
+            "#161c24"
         ],
         "scrollbar_button_color": [
-            "gray55",
-            "gray41"
+            "#a0abb7",
+            "#788490"
         ],
         "scrollbar_button_hover_color": [
-            "gray40",
-            "gray53"
+            "#a3aeb9",
+            "#7b8793"
         ],
         "text_color": [
-            "gray10",
-            "#DCE4EE"
+            "#212b36",
+            "#ffffff"
         ]
     },
     "CTkToplevel": {
         "fg_color": [
-            "#ffffff",
-            "#101010"
+            "#f9fafb",
+            "#161c24"
         ]
     },
     "DropdownMenu": {
         "fg_color": [
-            "gray90",
-            "#1c1c1c"
+            "#feffff",
+            "#202a34"
         ],
         "hover_color": [
-            "gray75",
-            "#313131"
+            "#eaeff1",
+            "#323c47"
         ],
         "text_color": [
-            "gray10",
-            "#ffffff"
+            "#212b36",
+            "#f1f1f2"
         ]
     }
 }
```

### Comparing `customtkinterx-0.3.2/README.md` & `customtkinterx-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.3.2/PKG-INFO` & `customtkinterx-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.3.2
+Version: 0.4.0
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

