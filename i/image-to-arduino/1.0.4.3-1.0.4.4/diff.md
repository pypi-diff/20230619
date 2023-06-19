# Comparing `tmp/image-to-arduino-1.0.4.3.tar.gz` & `tmp/image-to-arduino-1.0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-to-arduino-1.0.4.3.tar", last modified: Tue May  9 16:11:27 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.4.4.tar", last modified: Mon Jun 19 15:55:19 2023, max compression
```

## Comparing `image-to-arduino-1.0.4.3.tar` & `image-to-arduino-1.0.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2324 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/image_to_arduino/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/image_to_arduino/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       78 2023-05-09 16:10:50.000000 image-to-arduino-1.0.4.3/image_to_arduino/__main__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     8265 2023-05-09 15:59:47.000000 image-to-arduino-1.0.4.3/image_to_arduino/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      380 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       68 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       17 2023-05-09 16:11:27.000000 image-to-arduino-1.0.4.3/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-05-09 15:36:32.000000 image-to-arduino-1.0.4.3/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-09 16:11:27.473312 image-to-arduino-1.0.4.3/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      972 2023-05-09 16:10:00.000000 image-to-arduino-1.0.4.3/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2489 2023-06-19 15:52:12.000000 image-to-arduino-1.0.4.4/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/image_to_arduino/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/image_to_arduino/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       78 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/image_to_arduino/__main__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)    14659 2023-06-19 15:52:07.000000 image-to-arduino-1.0.4.4/image_to_arduino/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      380 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       68 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       17 2023-06-19 15:55:19.000000 image-to-arduino-1.0.4.4/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.4/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-19 15:55:19.727079 image-to-arduino-1.0.4.4/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      972 2023-06-19 15:52:47.000000 image-to-arduino-1.0.4.4/setup.py
```

### Comparing `image-to-arduino-1.0.4.3/LICENSE` & `image-to-arduino-1.0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.4.3/README.md` & `image-to-arduino-1.0.4.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 $ pip3 --version 
 $ python --version
 ```
 ### Installation
 #### Windows/Linux/Mac OS:
 ```
 $ pip3 install image-to-arduino
+```
+### Run
+#### Windows/Linux/Mac OS:
+```
 $ image-to-arduino
 ```
 ### How to upgrade version
 #### Windows/Linux/Mac OS:
 ```
 $ pip3 install --upgrade image-to-arduino
 ```
@@ -45,28 +49,30 @@
 $ git branch BRANCH-NAME 
 $ git checkout BRANCH-NAME
 ```
 4. Make changes and test<br>
 5. Submit Pull Request with comprehensive description of change
 
 ## Task list
-* <del> upgrade graphics and style </del><br>
-* <del> add more functions </del><br>
 * add more than one display size<br>
 * make icon of the app<br>
-* <del> show preview of an image </del> <br>
 * make app as .exe <br>
+* fix issue with generating dark png images with trancparency
+* resize window (width)
+* optimize gif extension option (or remove it)
+* test software
 * <del> reverse color of image </del><br>
 * <del> create function which generate full arduino code(not only arduino array) and connect it to switch button</del>
+* <del> show preview of an image </del> <br>
+* <del> upgrade graphics and style </del><br>
+* <del> add more functions </del><br>
 ## What I have learned
 *	tkinter library skills 
 *	basics of UX and GUI
 *	image processing 
 ## Used libraries
 * tkinter 
 * customtkinter
 * openCV
 * numpy
-## Version
-Version 1.0.3.2
 ## License 
 [MIT license](LICENSE)
```

### Comparing `image-to-arduino-1.0.4.3/setup.py` & `image-to-arduino-1.0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 
 setup(
    name='image-to-arduino',
-   version='1.0.4.3',
+   version='1.0.4.4',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
```

