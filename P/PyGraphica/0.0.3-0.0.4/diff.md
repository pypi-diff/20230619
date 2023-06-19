# Comparing `tmp/PyGraphica-0.0.3.tar.gz` & `tmp/PyGraphica-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGraphica-0.0.3.tar", last modified: Mon Jun 19 09:22:54 2023, max compression
+gzip compressed data, was "PyGraphica-0.0.4.tar", last modified: Mon Jun 19 09:44:28 2023, max compression
```

## Comparing `PyGraphica-0.0.3.tar` & `PyGraphica-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:22:54.490856 PyGraphica-0.0.3/
--rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      287 2023-06-19 09:22:54.490856 PyGraphica-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    13331 2023-06-18 21:47:30.000000 PyGraphica-0.0.3/README.txt
--rw-rw-rw-   0        0        0      116 2023-06-19 09:22:54.496148 PyGraphica-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      445 2023-06-19 09:22:09.000000 PyGraphica-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:22:54.451927 PyGraphica-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 09:22:54.467845 PyGraphica-0.0.3/src/PyGraphica/
--rw-rw-rw-   0        0        0        0 2023-06-18 02:45:11.000000 PyGraphica-0.0.3/src/PyGraphica/__init__.py
--rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.3/src/PyGraphica/colours.py
--rw-rw-rw-   0        0        0    28374 2023-06-19 09:21:36.000000 PyGraphica-0.0.3/src/PyGraphica/draw.py
--rw-rw-rw-   0        0        0      873 2023-06-19 09:19:35.000000 PyGraphica-0.0.3/src/PyGraphica/fonts.py
--rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.3/src/PyGraphica/origins.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:22:54.490856 PyGraphica-0.0.3/src/PyGraphica.egg-info/
--rw-rw-rw-   0        0        0      287 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 09:22:54.000000 PyGraphica-0.0.3/src/PyGraphica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:44:28.022899 PyGraphica-0.0.4/
+-rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      287 2023-06-19 09:44:28.022899 PyGraphica-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    13331 2023-06-18 21:47:30.000000 PyGraphica-0.0.4/README.txt
+-rw-rw-rw-   0        0        0      116 2023-06-19 09:44:28.022899 PyGraphica-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      445 2023-06-19 09:42:20.000000 PyGraphica-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:44:27.974277 PyGraphica-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 09:44:27.994686 PyGraphica-0.0.4/src/PyGraphica/
+-rw-rw-rw-   0        0        0        0 2023-06-18 02:45:11.000000 PyGraphica-0.0.4/src/PyGraphica/__init__.py
+-rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.4/src/PyGraphica/colours.py
+-rw-rw-rw-   0        0        0    28435 2023-06-19 09:42:08.000000 PyGraphica-0.0.4/src/PyGraphica/draw.py
+-rw-rw-rw-   0        0        0      873 2023-06-19 09:19:35.000000 PyGraphica-0.0.4/src/PyGraphica/fonts.py
+-rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.4/src/PyGraphica/origins.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:44:28.022899 PyGraphica-0.0.4/src/PyGraphica.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/top_level.txt
```

### Comparing `PyGraphica-0.0.3/LICENSE.txt` & `PyGraphica-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.3/README.txt` & `PyGraphica-0.0.4/README.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.3/src/PyGraphica/colours.py` & `PyGraphica-0.0.4/src/PyGraphica/colours.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.3/src/PyGraphica/draw.py` & `PyGraphica-0.0.4/src/PyGraphica/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
         self.width = width
         self.content = ""
         self.visible = True
         #Text that will be displayed as a prompt when the textbox is empty
         self.default_text = default_text
 
         #Text object component of textbox
-        self.__text = text(self.__window,self.x1,self.y1,self.size,(0,0,0),"Type here...","OpenSans")
+        self.__text = text(self.__window,self.x1,self.y1,self.size,(0,0,0),"Type here...","PyGraphica/fonts/calibri.ttf")
         #The textbox will have its own display function, so the text component must be removed from the list of objects to display
         all_shapes.remove(self.__text)
 
         #create function to calculate the width of the textbox to the start of the text
         if self.__window.origin in [1,3]:
             self.__add_width = lambda obj:obj.__text.x1-obj.width
         else:
@@ -468,14 +468,15 @@
             else:
                 self.width = width
         else:
             resize = False
         
         #If necessary, rewrite image (copy) into new size, then load resized image
         if resize:
+            img = Image.open(self.path)
             img = img.resize((width,height))
             path = self.path.split(".")
             path = path[0] + "_PyGraphica_cropped." + path[1]
             img.save(path)
             self.__img = sdl2.ext.image.load_image(path)
 
             self.__hard_width = width
```

### Comparing `PyGraphica-0.0.3/src/PyGraphica/fonts.py` & `PyGraphica-0.0.4/src/PyGraphica/fonts.py`

 * *Files identical despite different names*

