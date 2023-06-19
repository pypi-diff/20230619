# Comparing `tmp/image-to-arduino-1.0.4.4.tar.gz` & `tmp/image-to-arduino-1.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-to-arduino-1.0.4.4.tar", last modified: Mon Jun 19 15:55:19 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.4.5.tar", last modified: Mon Jun 19 15:58:12 2023, max compression
```

## Comparing `image-to-arduino-1.0.4.4.tar` & `image-to-arduino-1.0.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2489 2023-06-19 15:52:12.000000 image-to-arduino-1.0.4.4/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/image_to_arduino/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/image_to_arduino/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       78 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/image_to_arduino/__main__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)    14659 2023-06-19 15:52:07.000000 image-to-arduino-1.0.4.4/image_to_arduino/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      380 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       68 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       17 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      972 2023-06-19 15:52:47.000000 image-to-arduino-1.0.4.4/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2489 2023-06-19 15:52:12.000000 image-to-arduino-1.0.4.5/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/image_to_arduino/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/image_to_arduino/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       78 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/image_to_arduino/__main__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)    14653 2023-06-19 15:57:42.000000 image-to-arduino-1.0.4.5/image_to_arduino/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      380 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       68 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       17 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      972 2023-06-19 15:57:18.000000 image-to-arduino-1.0.4.5/setup.py
```

### Comparing `image-to-arduino-1.0.4.4/LICENSE` & `image-to-arduino-1.0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.4.4/README.md` & `image-to-arduino-1.0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.4.4/image_to_arduino/main.py` & `image-to-arduino-1.0.4.5/image_to_arduino/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,8 +352,7 @@
     clear_all_button = customtkinter.CTkButton(root, text="Clear All", command=clear_all)
     clear_all_button.grid(row=5, column=0, pady=5, padx=10, columnspan=1, sticky="nsew")  
 
     # Configure the window to not be resizable
     root.resizable(False, False)
 
     root.mainloop()
-main()
```

### Comparing `image-to-arduino-1.0.4.4/setup.py` & `image-to-arduino-1.0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 
 setup(
    name='image-to-arduino',
-   version='1.0.4.4',
+   version='1.0.4.5',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
```

