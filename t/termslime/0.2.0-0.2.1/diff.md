# Comparing `tmp/termslime-0.2.0.tar.gz` & `tmp/termslime-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termslime-0.2.0.tar", max compression
+gzip compressed data, was "termslime-0.2.1.tar", max compression
```

## Comparing `termslime-0.2.0.tar` & `termslime-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-06-18 08:41:45.640249 termslime-0.2.0/LICENSE
--rw-r--r--   0        0        0      715 2023-06-18 10:59:12.900708 termslime-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-18 08:39:50.888877 termslime-0.2.0/README.md
--rw-r--r--   0        0        0       12 2023-06-18 09:15:03.198103 termslime-0.2.0/termslime/.gitignore
--rw-r--r--   0        0        0     5409 2023-06-18 10:57:33.410810 termslime-0.2.0/termslime/main.py
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 termslime-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-18 08:41:45.640249 termslime-0.2.1/LICENSE
+-rw-r--r--   0        0        0      721 2023-06-19 08:01:53.220073 termslime-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2318 2023-06-19 07:37:44.969079 termslime-0.2.1/README.md
+-rw-r--r--   0        0        0       12 2023-06-18 09:15:03.198103 termslime-0.2.1/termslime/.gitignore
+-rw-r--r--   0        0        0     5495 2023-06-19 07:52:23.626494 termslime-0.2.1/termslime/__main__.py
+-rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 termslime-0.2.1/PKG-INFO
```

### Comparing `termslime-0.2.0/LICENSE` & `termslime-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `termslime-0.2.0/pyproject.toml` & `termslime-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "termslime"
-version = "0.2.0"
+version = "0.2.1"
 description = "Termslime displays images in your terminal with true colors."
 license = "MIT"
 authors = ["Gary Zhang <garyzhang2002@hotmail.com>"]
 maintainers = ["Gary Zhang <garyzhang2002@hotmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/garyzbm/termslime"
 repository = "https://github.com/garyzbm/termslime"
@@ -17,8 +17,8 @@
 pillow = "^9.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-tslime = "termslime.main:main"
+tslime = "termslime.__main__:__main"
```

### Comparing `termslime-0.2.0/termslime/main.py` & `termslime-0.2.1/termslime/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import colorful as cf
-from PIL import Image
-import argparse
-import os
-import random
+import colorful as __cf
+from PIL import Image as __Image
+import argparse as __argparse
+import os as __os
+import random as __random
 
 # use true colors to display the image
-cf.use_true_colors()
+__cf.use_true_colors()
 
-def display(imgPath: str, heightLimit: int, widthLimit: int, beginPadding: int, endPadding: int, leftPadding: int) -> None:
+def __display(imgPath: str, heightLimit: int, widthLimit: int, beginPadding: int, endPadding: int, leftPadding: int) -> None:
     """
     Display an image by printing half blocks with foreground and background colors to the terminal.
 
     Args:
         imgPath - the path to the image file
         heightLimit - maximum number of lines of blocks to display the image in the terminal
         widthLimit - maximum number of blocks per line to display the image in the terminal
         beginPadding - number of empty lines before the image
         endPadding - number of empty lines after the image
         leftPadding - number of empty spaces at the beginning of each line of the image
     """
 
     # open the image and convert it to 256 colors and get its width and height
-    img = Image.open(imgPath).convert(mode="RGBA")
+    img = __Image.open(imgPath).convert(mode="RGBA")
     imgWidth, imgHeight = img.size[0], img.size[1]
 
     # calculate the resize ratio
     resizeRatio = imgHeight / (heightLimit * 2) if imgHeight > heightLimit * 2 else 1
     resizeRatio = imgWidth / widthLimit if int(imgWidth / resizeRatio) > widthLimit else resizeRatio
 
     # compress the image to fit the width and height limits and make sure the compressed height is even
-    imgResized = img.resize((int(imgWidth / resizeRatio), int(imgHeight / resizeRatio / 2) * 2), Image.Resampling.NEAREST)
+    imgResized = img.resize((int(imgWidth / resizeRatio), int(imgHeight / resizeRatio / 2) * 2), __Image.Resampling.NEAREST)
 
     # print the begin padding
     print("\n" * beginPadding, end="")
 
     # for each two row numbers x and x+1 of pixels
     for x in range(0, imgResized.size[1], 2):
 
@@ -53,43 +53,45 @@
             # if the two pixels are transparent, print a space
             if pixelUpper[-1] == 0 and pixelLower[-1] == 0:
                 print(" ", end="")
 
             # if only the upper pixel is transparent, print a lower half block with the lower pixel's color as the foreground color
             elif pixelUpper[-1] == 0:
                 p["fore"] = tuple(pixelLower[:-1])
-                with cf.with_palette(p) as c:
+                with __cf.with_palette(p) as c:
                     print(c.fore("▄"), end="")
 
             # if only the lower pixel is transparent, print a upper half block with the upper pixel's color as the foreground color
             elif pixelLower[-1] == 0:
                 p["fore"] = tuple(pixelUpper[:-1])
-                with cf.with_palette(p) as c:
+                with __cf.with_palette(p) as c:
                     print(c.fore("▀"), end="")
 
             # if either of the two pixels is transparent, print a lower half block with the corresponding pixel's color as the foreground and background colors
             else:
                 p["fore"] = tuple(pixelLower[:-1])
                 p["back"] = tuple(pixelUpper[:-1])
-                with cf.with_palette(p) as c:
+                with __cf.with_palette(p) as c:
                     print(c.fore_on_back("▄"), end="")
 
         # start a new row
         print()
 
     # print the end padding
     print("\n" * endPadding, end="")
 
-# the entry point of the cli
-def main():
+def __main():
+    """
+    Entry point.
+    """
 
     # set up the argument parser
-    parser = argparse.ArgumentParser(
+    parser = __argparse.ArgumentParser(
         prog="tslime",
-        description="Termslime displays images in your terminal with true colors. Project home page: https://github.com/garyzbm/termslime",
+        description="Termslime displays images in your terminal with true colors. Project home page: https://github.com/garyzbm/termslime.",
     )
 
     # add arguments
     parser.add_argument("path", type=str, help="path to an image file or a directory containing image files")
     parser.add_argument("-hl", "--heightLimit", type=int, default=500, help="maximum number of lines of blocks to display the image in the terminal")
     parser.add_argument("-wl", "--widthLimit", type=int, default=1000, help="maximum number of blocks per line to display the image in the terminal")
     parser.add_argument("-bp", "--beginPadding", type=int, default=1, help="number of empty lines before the image")
@@ -97,22 +99,22 @@
     parser.add_argument("-lp", "--leftPadding", type=int, default=1, help="number of empty spaces at the beginning of each line of the image")
 
     # parse the arguments
     args = parser.parse_args()
 
     # get path from the arguments
     imgPath = args.path
-    assert os.path.exists(imgPath), f"{imgPath} does not exist"
+    assert __os.path.exists(imgPath), f"{imgPath} does not exist"
 
     # if imgPath is a path to a directory
-    if os.path.isdir(imgPath):
+    if __os.path.isdir(imgPath):
 
         # randomly choose an image from the directory and make imgPath the path to that image
-        imgList = [file for file in os.listdir(imgPath) if file.endswith(".png") or file.endswith(".jpg") or file.endswith(".jpeg") or file.endswith("bmp")]
+        imgList = [file for file in __os.listdir(imgPath) if file.endswith(".png") or file.endswith(".jpg") or file.endswith(".jpeg") or file.endswith("bmp")]
         assert len(imgList) > 0, f"{imgPath} does not contain any image files"
-        imgPath = os.path.join(imgPath, random.choice(imgList))
+        imgPath = __os.path.join(imgPath, __random.choice(imgList))
 
     # call the display function and pass in the arguments
-    display(imgPath, args.heightLimit, args.widthLimit, args.beginPadding, args.endPadding, args.leftPadding)
+    __display(imgPath, args.heightLimit, args.widthLimit, args.beginPadding, args.endPadding, args.leftPadding)
 
 if __name__ == "__main__":
-    main()
+    __main()
```

