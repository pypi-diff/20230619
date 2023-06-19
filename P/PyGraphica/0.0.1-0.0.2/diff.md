# Comparing `tmp/PyGraphica-0.0.1.tar.gz` & `tmp/PyGraphica-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGraphica-0.0.1.tar", last modified: Sun Jun 18 09:55:16 2023, max compression
+gzip compressed data, was "PyGraphica-0.0.2.tar", last modified: Mon Jun 19 09:07:29 2023, max compression
```

## Comparing `PyGraphica-0.0.1.tar` & `PyGraphica-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 09:55:16.109763 PyGraphica-0.0.1/
--rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      287 2023-06-18 09:55:16.109763 PyGraphica-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11791 2023-06-18 07:03:21.000000 PyGraphica-0.0.1/README.md
--rw-rw-rw-   0        0        0    13331 2023-06-18 09:45:31.000000 PyGraphica-0.0.1/README.rst
--rw-rw-rw-   0        0        0      116 2023-06-18 09:55:16.111635 PyGraphica-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      447 2023-06-18 09:54:59.000000 PyGraphica-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 09:55:16.038931 PyGraphica-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 09:55:16.093040 PyGraphica-0.0.1/src/PyGraphica/
--rw-rw-rw-   0        0        0        0 2023-06-18 02:45:11.000000 PyGraphica-0.0.1/src/PyGraphica/__init__.py
--rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.1/src/PyGraphica/colours.py
--rw-rw-rw-   0        0        0    28525 2023-06-18 02:26:44.000000 PyGraphica-0.0.1/src/PyGraphica/draw.py
--rw-rw-rw-   0        0        0      994 2023-06-18 06:43:44.000000 PyGraphica-0.0.1/src/PyGraphica/fonts.py
--rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.1/src/PyGraphica/origins.py
-drwxrwxrwx   0        0        0        0 2023-06-18 09:55:16.102065 PyGraphica-0.0.1/src/PyGraphica.egg-info/
--rw-rw-rw-   0        0        0      287 2023-06-18 09:55:15.000000 PyGraphica-0.0.1/src/PyGraphica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-06-18 09:55:15.000000 PyGraphica-0.0.1/src/PyGraphica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 09:55:15.000000 PyGraphica-0.0.1/src/PyGraphica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-18 09:55:15.000000 PyGraphica-0.0.1/src/PyGraphica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 09:55:15.000000 PyGraphica-0.0.1/src/PyGraphica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:29.300967 PyGraphica-0.0.2/
+-rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      287 2023-06-19 09:07:29.300967 PyGraphica-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13331 2023-06-18 21:47:30.000000 PyGraphica-0.0.2/README.txt
+-rw-rw-rw-   0        0        0      116 2023-06-19 09:07:29.305652 PyGraphica-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      447 2023-06-18 21:45:05.000000 PyGraphica-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:29.262374 PyGraphica-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:29.278407 PyGraphica-0.0.2/src/PyGraphica/
+-rw-rw-rw-   0        0        0        0 2023-06-18 02:45:11.000000 PyGraphica-0.0.2/src/PyGraphica/__init__.py
+-rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.2/src/PyGraphica/colours.py
+-rw-rw-rw-   0        0        0    28365 2023-06-19 09:05:44.000000 PyGraphica-0.0.2/src/PyGraphica/draw.py
+-rw-rw-rw-   0        0        0      994 2023-06-18 06:43:44.000000 PyGraphica-0.0.2/src/PyGraphica/fonts.py
+-rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.2/src/PyGraphica/origins.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:29.300967 PyGraphica-0.0.2/src/PyGraphica.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 09:07:29.000000 PyGraphica-0.0.2/src/PyGraphica.egg-info/top_level.txt
```

### Comparing `PyGraphica-0.0.1/LICENSE.txt` & `PyGraphica-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.1/README.rst` & `PyGraphica-0.0.2/README.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.1/src/PyGraphica/colours.py` & `PyGraphica-0.0.2/src/PyGraphica/colours.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.1/src/PyGraphica/draw.py` & `PyGraphica-0.0.2/src/PyGraphica/draw.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,20 +122,14 @@
         self.comm_changes = list(set(new_comms)-set(self.comms))
         self.comms = new_comms
         
         #Toggle 'caps' flag
         if "CAPS" in self.comm_changes:
             self.caps = not self.caps
     
-    #When the window is closed (and the window deleted) clean up any images in the 'images' folder
-    def __del__(self):
-        for file in os.listdir("PyGraphica/images"):
-            os.remove("PyGraphica/images/"+file)
-        all_shapes = []
-    
 class line:
     def __init__(self,window,x1,y1,x2,y2,colour):
         self.__window = window
         #start coordinates = (x1,y1); end coordinates = (x2,y2)
         self.x1 = x1
         self.y1 = y1
         self.x2 =  x2
@@ -408,16 +402,18 @@
                 self.height = height
 
         self.__hard_width = width
         self.__hard_height = height
         
         #resize the image and save it to the 'images' folder, then reload the saved image
         img = img.resize((width,height))
-        img.save("PyGraphica/images/"+self.path.split("/")[-1])
-        self.__img = sdl2.ext.load_image("PyGraphica/images/"+self.path.split("/")[-1])
+        path = self.path.split(".")
+        path = path[0] + "_PyGraphica_cropped." + path[1]
+        img.save(path)
+        self.__img = sdl2.ext.image.load_image(path)
 
         all_shapes.append(self)
 
         start_x = int(self.x1)
         start_y = int(self.y1)
         width = int(self.width)
         height = int(self.height)
@@ -438,54 +434,57 @@
             self.x2 = str(end_x)
             self.y2 = str(end_y)
         else:
             self.x2 = end_x
             self.y2 = end_y
     
     def display(self):
+        path = self.path.split(".")
+        path = path[0] + "_PyGraphica_cropped." + path[1]
+        img = Image.open(path)
+
         width = make_width(self.__window,self.width)
         self.__hard_width = width
         height = make_height(self.__window,self.height)
         self.__hard_height = height
 
         start = make_pos(self.__window,(self.x1,self.y1))
         end = make_pos(self.__window,(self.x2,self.y2))
 
         resize = True
 
         #Check if any sizing has changed
-        if self.__hard_width != self.__img.w and self.__hard_height != self.__img.h:
+        if self.__hard_width != img.width and self.__hard_height != img.height:
             pass
-        elif self.__hard_width != self.__img.w:
+        elif self.__hard_width != img.width:
             height = int(width * (1/self.aspect_ratio))
             if type(self.width) == str:
                 self.height = rela_height(self.__window,height)
             else:
                 self.height = height
-        elif self.__hard_height != self.__img.h:
+        elif self.__hard_height != img.height:
             width = int(height * self.aspect_ratio)
             if type(self.height) == str:
                 self.width = rela_width(self.__window,width)
             else:
                 self.width = width
         else:
             resize = False
         
         #If necessary, rewrite image (copy) into new size, then load resized image
         if resize:
-            img = Image.open(self.path)
             img = img.resize((width,height))
+            path = self.path.split(".")
+            path = path[0] + "_PyGraphica_cropped." + path[1]
+            img.save(path)
+            self.__img = sdl2.ext.image.load_image(path)
 
             self.__hard_width = width
             self.__hard_height = height
 
-            img.save("PyGraphica/images/"+self.path.split("/")[-1])
-
-            self.__img = sdl2.ext.load_image("PyGraphica/images/"+self.path.split("/")[-1])
-
             start_x = int(self.x1)
             start_y = int(self.y1)
             width = int(self.width)
             height = int(self.height)
 
             if self.__window.origin in [0,2,4]:
                 end_x = start_x + width
@@ -498,15 +497,14 @@
                 end_y = start_y - height
 
             if type(self.width) == str:
                 self.end = (str(end_x),str(end_y))
             else:
                 self.end = (end_x,end_y)
         
-        #Display image
         sdl2.SDL_BlitSurface(self.__img,None,self.__window.surface,sdl2.SDL_Rect(start[0],start[1],end[0],end[1]))
 
 #Check for overlap between two objects
 def collision(object1, object2):
     overlap = True
     X1 = sorted([object1.x1,object1.x2])
     Y1 = sorted([object1.y1,object1.y2])
```

### Comparing `PyGraphica-0.0.1/src/PyGraphica/fonts.py` & `PyGraphica-0.0.2/src/PyGraphica/fonts.py`

 * *Files identical despite different names*

