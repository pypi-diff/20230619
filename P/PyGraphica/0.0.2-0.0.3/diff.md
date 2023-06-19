# Comparing `tmp/PyGraphica-0.0.2.tar.gz` & `tmp/PyGraphica-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGraphica-0.0.2.tar", last modified: Mon Jun 19 09:07:29 2023, max compression
+gzip compressed data, was "PyGraphica-0.0.3.tar", last modified: Mon Jun 19 09:22:54 2023, max compression
```

## Comparing `PyGraphica-0.0.2.tar` & `PyGraphica-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:29.300967 PyGraphica-0.0.2/
--rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      287 2023-06-19 09:07:29.300967 PyGraphica-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13331 2023-06-18 21:47:30.000000 PyGraphica-0.0.2/README.txt
--rw-rw-rw-   0        0        0      116 2023-06-19 09:07:29.305652 PyGraphica-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      447 2023-06-18 21:45:05.000000 PyGraphica-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:29.262374 PyGraphica-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:29.278407 PyGraphica-0.0.2/src/PyGraphica/
--rw-rw-rw-   0        0        0        0 2023-06-18 02:45:11.000000 PyGraphica-0.0.2/src/PyGraphica/__init__.py
--rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.2/src/PyGraphica/colours.py
--rw-rw-rw-   0        0        0    28365 2023-06-19 09:05:44.000000 PyGraphica-0.0.2/src/PyGraphica/draw.py
--rw-rw-rw-   0        0        0      994 2023-06-18 06:43:44.000000 PyGraphica-0.0.2/src/PyGraphica/fonts.py
--rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.2/src/PyGraphica/origins.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:29.300967 PyGraphica-0.0.2/src/PyGraphica.egg-info/
--rw-rw-rw-   0        0        0      287 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:22:54.490856 PyGraphica-0.0.3/
+-rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      287 2023-06-19 09:22:54.490856 PyGraphica-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13331 2023-06-18 21:47:30.000000 PyGraphica-0.0.3/README.txt
+-rw-rw-rw-   0        0        0      116 2023-06-19 09:22:54.496148 PyGraphica-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      445 2023-06-19 09:22:09.000000 PyGraphica-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:22:54.451927 PyGraphica-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 09:22:54.467845 PyGraphica-0.0.3/src/PyGraphica/
+-rw-rw-rw-   0        0        0        0 2023-06-18 02:45:11.000000 PyGraphica-0.0.3/src/PyGraphica/__init__.py
+-rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.3/src/PyGraphica/colours.py
+-rw-rw-rw-   0        0        0    28374 2023-06-19 09:21:36.000000 PyGraphica-0.0.3/src/PyGraphica/draw.py
+-rw-rw-rw-   0        0        0      873 2023-06-19 09:19:35.000000 PyGraphica-0.0.3/src/PyGraphica/fonts.py
+-rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.3/src/PyGraphica/origins.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:22:54.490856 PyGraphica-0.0.3/src/PyGraphica.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/top_level.txt
```

### Comparing `PyGraphica-0.0.2/LICENSE.txt` & `PyGraphica-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.2/README.txt` & `PyGraphica-0.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.2/src/PyGraphica/colours.py` & `PyGraphica-0.0.3/src/PyGraphica/colours.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.2/src/PyGraphica/draw.py` & `PyGraphica-0.0.3/src/PyGraphica/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,27 +204,27 @@
         if not self.__window.mouse_held and self.__window.mouse_down:
             if self.hover and not self.clicked:
                 self.clicked = True
             else:
                 self.clicked = False
 
 class text:
-    def __init__(self, window, x1, y1, size, colour, content, font = "PyGraphica/my_fonts/calibri.ttf"):
+    def __init__(self, window, x1, y1, size, colour, content, font = "my_fonts/calibri.ttf"):
         self.__window = window
         self.x1 = x1
         self.y1 = y1
         self.size = size
         self.colour = colour
-        self.font = font
         self.content = content
         self.visible = True
         self.height = 0
         self.width = 0
         self.hover = False
         self.clicked = False
+        self.font = os.getcwd() + "/" + font
         all_shapes.append(self)
 
         start = make_pos(self.__window,(self.x1,self.y1))
         size = make_height(self.__window,self.size)
 
         #Create font object
         font = sdl2.ext.ttf.FontTTF(self.font,str(str(size)+"px"),self.colour)
```

