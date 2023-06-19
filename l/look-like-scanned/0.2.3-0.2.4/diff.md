# Comparing `tmp/look_like_scanned-0.2.3.tar.gz` & `tmp/look_like_scanned-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "look_like_scanned-0.2.3.tar", max compression
+gzip compressed data, was "look_like_scanned-0.2.4.tar", max compression
```

## Comparing `look_like_scanned-0.2.3.tar` & `look_like_scanned-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/LICENSE
--rw-r--r--   0        0        0    10207 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/README.md
--rw-r--r--   0        0        0     1778 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/scanner/__init__.py
--rw-r--r--   0        0        0    13210 2023-05-29 03:38:37.382989 look_like_scanned-0.2.3/scanner/scanner.py
--rw-r--r--   0        0        0    11725 1970-01-01 00:00:00.000000 look_like_scanned-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/LICENSE
+-rw-r--r--   0        0        0    10326 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/README.md
+-rw-r--r--   0        0        0     1778 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/scanner/__init__.py
+-rw-r--r--   0        0        0    13653 2023-06-19 06:11:55.870797 look_like_scanned-0.2.4/scanner/scanner.py
+-rw-r--r--   0        0        0    11844 1970-01-01 00:00:00.000000 look_like_scanned-0.2.4/PKG-INFO
```

### Comparing `look_like_scanned-0.2.3/LICENSE` & `look_like_scanned-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `look_like_scanned-0.2.3/README.md` & `look_like_scanned-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # look-like-scanned
 
 [![Pylint](https://github.com/navchandar/look-like-scanned/actions/workflows/pylint.yml/badge.svg)](https://github.com/navchandar/look-like-scanned/actions/workflows/pylint.yml)  [![PyTest](https://github.com/navchandar/look-like-scanned/actions/workflows/tests.yml/badge.svg)](https://github.com/navchandar/look-like-scanned/actions/workflows/tests.yml)
 ![license](https://img.shields.io/badge/license-MIT-blue.svg)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/navchandar/look-like-scanned/issues)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) 
 
- - Python script to make documents look like they were scanned. 
+ - Python script to make documents look like they were scanned.
 
- - It converts every page of a given PDF file into an image-based page and applies random askew and brightness (very mild) effects to simulate the appearance of scanned documents.
+ - Local, Private, Secure, Open-Source and Transparent!
+
+ - Converts every page of a given PDF file into an image-based page and applies random askew and brightness (very mild) effects to simulate the appearance of scanned documents.
  
  - The resulting pages are then combined back into an Output PDF file.
 
  - There are options to combine / convert image files into PDF as well.
 
- - Output PDF files are saved in the same input folder with a suffix _"filename_output.pdf"_
+ - Output PDF files are saved in the same folder with a suffix _"File_Name_output.pdf"_
 
 
 ## Installation
 
 Install from the [Python Package Index (PyPI)](https://pypi.org/project/look-like-scanned/)
 ```shell
 pip install look-like-scanned
@@ -97,14 +99,16 @@
 
 - The supported file types are: ".jpg", ".png", ".jpeg", ".webp", ".pdf".
 
 - The output PDF file size **will be bigger** than the input file because the pages are stored in image format.
 
 - Bookmarks / Links / Metadata will be removed when saving the output file.
 
+- Transparency will be removed from png files when converting to pdf.
+
 - Password protected PDF files are not yet supported.
 
 
 ## License
  
  [MIT license](LICENSE)
```

### Comparing `look_like_scanned-0.2.3/pyproject.toml` & `look_like_scanned-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "look-like-scanned"
-version = "0.2.3"
+version = "0.2.4"
 description = "Python script to make documents look like they were scanned."
 authors = ["navchandar <12165092+navchandar@users.noreply.github.com>"]
 repository    = "https://github.com/navchandar/look-like-scanned"
 homepage = "https://github.com/navchandar/look-like-scanned"
 readme = "README.md"
 keywords = ["pdf", "scan", "scanner", "image-to-pdf", "pdf-to-scan"]
 packages = [
```

### Comparing `look_like_scanned-0.2.3/scanner/scanner.py` & `look_like_scanned-0.2.4/scanner/scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 
 import os
 import io
 import random
 import argparse
 import colorama
 from colorama import Fore, Style
-from pprint import pprint
 import pypdfium2 as pdfium
 from PIL import Image, ImageEnhance
+from pathlib import Path
+from pprint import pprint as pretty_print
 
-SUPPORTED_IMAGES = [".jpg", ".png", ".jpeg", ".webp"]
-SUPPORTED_DOCS = [".pdf", ".PDF"]
+SUPPORTED_IMAGES = ["jpg", "png", "jpeg", "webp"]
+SUPPORTED_DOCS = ["pdf", "PDF"]
 CHOICES = ["y", "yes", "n", "no", "true", "false"]
 
 
-def print_color_text(text, color):
+def print_color(text, color):
     """
     Print the specified text in the given color.
     Available colors: 'black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white'.
     """
     color_map = {
         "black": Fore.BLACK,
         "red": Fore.RED,
@@ -48,23 +49,25 @@
         type=str,
         help="The input folder to read files from and convert (default: current directory)",
     )
     parser.add_argument(
         "-f",
         "--file_type_or_name",
         type=str,
-        help="The file types to process or file name to process. Valid value - image, pdf, file names (default: pdf)",
+        help="The file types to process or file name to process.\
+    Valid value - image, pdf, file names (default: pdf)",
     )
     parser.add_argument(
         "-q",
         "--file_quality",
         type=int,
         choices=range(50, 101, 5),
         default=95,
-        help="The quality of the converted output files. Valid range - 50 to 100 increment in steps of 5 (default: 95)",
+        help="The quality of the converted output files.\
+    Valid range - 50 to 100 increment in steps of 5 (default: 95)",
     )
     parser.add_argument(
         "-a",
         "--askew",
         type=str.lower,
         choices=CHOICES,
         default="yes",
@@ -94,22 +97,25 @@
         print(f"Processing files from {input_folder=}")
     else:
         print(f"Error: Input folder path not found: {input_folder}")
     return input_folder
 
 
 def get_quality(args):
+    """Return the output file quality from command-line argument"""
     return args.file_quality
 
 
 def get_askew(args):
+    """Return if output file should have skewed pages"""
     return args.askew.lower().startswith(("y", "t"))
 
 
 def get_recurse(args):
+    """Return if input files should be searched within sub folders"""
     return args.recurse.lower().startswith(("y", "t"))
 
 
 def get_file_type(args):
     """Get file type and supported documents based on input arguments"""
     if args.file_type_or_name:
         file_type = args.file_type_or_name.lower()
@@ -142,17 +148,16 @@
     return human_size(os.stat(file_path).st_size)
 
 
 def files_exists(file_path):
     """Check if given file path exists in the file system"""
     if os.path.exists(file_path):
         return True
-    else:
-        print_color_text(f"File doesn't exist or incorrect path: {file_path}", "Red")
-        return False
+    print_color(f"File doesn't exist or incorrect path: {file_path}", "Red")
+    return False
 
 
 def reduce_image_quality(image, quality=100, compression="JPEG"):
     """Reduce quality of a given image object"""
     img_byte_array = io.BytesIO()
     # Save the image to the in-memory file object
     image.save(img_byte_array, quality=quality, format=compression)
@@ -189,18 +194,18 @@
     """
     images_list = []
     doc = pdfium.PdfDocument(pdf_path)
     for page in doc:
         # increase render resolution for better scanned image quality
         bitmap = page.render(scale=2)
         image = bitmap.to_pil()
+        image = image.convert("RGB")
 
         # Reduce image quality a little bit
         image = reduce_image_quality(image, image_quality)
-        image = image.convert("RGB")
 
         # increase brightness a little bit
         enhancer = ImageEnhance.Brightness(image)
         image = enhancer.enhance(random.uniform(1.01, 1.02))
 
         # Rotate every image by a small random angle
         if askew:
@@ -282,42 +287,44 @@
         energy_saved = f"{energy_saved:.2f} kilo Watt hours"
     else:
         energy_saved = energy_saved / 1000000
         energy_saved = f"{energy_saved:.2f} Mega Watt hours"
 
     if pages_scanned > 0:
         savings = f"\nYou just saved {energy_saved} energy by avoiding printing {pages_scanned} pages of paper!\n"
-        print_color_text(savings, "Green")
+        print_color(savings, "Green")
 
 
 def convert_images_to_pdf(input_image_list, image_quality, askew):
     """Converts all image files in a folder to PDF"""
     images_list = []
+    output_pdf_path = None
+    if input_image_list:
+        # Output pdf name will be the fetched from first Image's name
+        output_pdf_path = os.path.splitext(input_image_list[0])[0] + "_output.pdf"
+        for image_path in input_image_list:
+            if files_exists(image_path):
+                try:
+                    image = Image.open(image_path)
+                    image = image.convert("RGB")
+
+                    # reduce image quality a little bit
+                    image = reduce_image_quality(image, image_quality)
+
+                    # Rotate every image by a small random angle
+                    if askew:
+                        image = rotate_image(image, random.uniform(-0.75, 0.75))
+
+                    image = _change_image_to_byte_buffer(image)
+                    images_list.append(image)
+                except Exception as err:
+                    print_color(f"Error converting file {image_path} :- {err}", "Red")
 
-    # Output pdf name will be the fetched from first Image's name
-    output_pdf_path = os.path.splitext(input_image_list[0])[0] + "_output.pdf"
-    for image_path in input_image_list:
-        if files_exists(image_path):
-            try:
-                image = Image.open(image_path)
-                # reduce image quality a little bit
-                image = reduce_image_quality(image, image_quality)
-                image = image.convert("RGB")
-
-                # Rotate every image by a small random angle
-                if askew:
-                    image = rotate_image(image, random.uniform(-0.75, 0.75))
-
-                image = _change_image_to_byte_buffer(image)
-                images_list.append(image)
-            except Exception as e:
-                print_color_text(f"Error converting file {image_path} :- {e}", "Red")
-
-    pages_scanned = _save_image_obj_to_pdf(images_list, output_pdf_path, pdf_version=17)
-    _calc_energy_savings(pages_scanned)
+        pages_scanned = _save_image_obj_to_pdf(images_list, output_pdf_path)
+        _calc_energy_savings(pages_scanned)
     return output_pdf_path
 
 
 def convert_pdf_to_scanned(pdf_list, image_quality, askew):
     """
     Converts PDF files into scanned PDF files
     """
@@ -326,38 +333,40 @@
     for pdf_path in pdf_list:
         if files_exists(pdf_path):
             try:
                 output_path = _add_suffix(pdf_path)
                 images = _convert_pdf_pages_to_jpg_list(pdf_path, image_quality, askew)
                 pages_scanned += _save_image_obj_to_pdf(images, output_path)
                 output_file_list.append(output_path)
-            except Exception as e:
-                print_color_text(f"Error converting file {pdf_path} :- {e}", "Red")
+            except Exception as err:
+                print_color(f"Error converting file {pdf_path} :- {err}", "Red")
 
     _calc_energy_savings(pages_scanned)
     return output_file_list
 
 
 def find_matching_files(input_folder, file_type_list, recurse=False):
     """
-    Find files in given input folder and filter only matching file types.
-    If recurse is True, this method will identify all matching files in all sub directories.
+    Find files in the given input folder and filter only matching file types.
+    If recurse is True, this method will identify all matching files in all subdirectories.
     """
     files_list = []
     try:
-        for file in os.listdir(input_folder):
-            path = os.path.join(input_folder, file)
-            if os.path.isfile(path) and any(
-                file.endswith(ext) for ext in file_type_list
-            ):
-                files_list.append(path)
-            if recurse and os.path.isdir(path):
-                files_list.extend(find_matching_files(path, file_type_list, recurse))
-    except Exception as e:
-        print_color_text(f"Error when searching for files :- {e}", "Red")
+        path = Path(input_folder)
+        for file in path.iterdir():
+            if file.is_file() and file.suffix.lower().lstrip(".") in file_type_list:
+                files_list.append(str(file.absolute()))
+            elif recurse and file.is_dir():
+                files_list.extend(find_matching_files(file, file_type_list, recurse))
+    except FileNotFoundError as err:
+        print_color(f"Input folder not found: {input_folder}", "red")
+    except PermissionError as err:
+        print_color(f"Permission denied: {input_folder}", "red")
+    except Exception as err:
+        print_color(f"Error when searching for files: {err}", "red")
     return files_list
 
 
 def sort_by_top_level_directory(path):
     """Method to help sort file paths based on level"""
     directories = path.split(os.path.sep)
     return len(directories)
@@ -370,39 +379,35 @@
     # Gather input arguments from command-line
     input_folder = get_input_folder(args)
     quality = get_quality(args)
     askew = get_askew(args)
     recurse = get_recurse(args)
     doc_type, file_type_list = get_file_type(args)
 
-    print_color_text(
-        f"{quality=} {recurse=} {askew=} {doc_type=} {file_type_list=}", "Cyan"
-    )
+    print_color(f"{quality=} {recurse=} {askew=} {doc_type=} {file_type_list=}", "Cyan")
 
     # Gather the input files based on the arguments
     files_list = find_matching_files(input_folder, file_type_list, recurse)
     # Sort file paths so output gets saved in top level directory
     files_list = sorted(files_list, key=sort_by_top_level_directory)
 
-    print_color_text(f"\nMatching Files Found: {len(files_list)}", "Blue")
-    pprint(files_list)
+    print_color(f"\nMatching Files Found: {len(files_list)}", "Blue")
+    pretty_print(files_list)
 
     # Convert the files found into output files
     pdf_path = None
     if doc_type == "image":
         pdf_path = convert_images_to_pdf(files_list, quality, askew)
     elif doc_type == "pdf":
         pdf_path = convert_pdf_to_scanned(files_list, quality, askew)
     else:
-        print("Error: Unsupported file format!")
+        print_color("Error: Unsupported file format!", "Red")
 
     if pdf_path:
-        print(f"The Output PDF files saved at:")
-        pprint(pdf_path)
+        print("The Output PDF files saved at:")
+        pretty_print(pdf_path)
     else:
-        print_color_text(
-            "No matching files found. No output documents generated!", "Red"
-        )
+        print_color("No matching files found. No output documents generated!\n", "Red")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `look_like_scanned-0.2.3/PKG-INFO` & `look_like_scanned-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: look-like-scanned
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python script to make documents look like they were scanned.
 Home-page: https://github.com/navchandar/look-like-scanned
 Keywords: pdf,scan,scanner,image-to-pdf,pdf-to-scan
 Author: navchandar
 Author-email: 12165092+navchandar@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -34,23 +34,25 @@
 # look-like-scanned
 
 [![Pylint](https://github.com/navchandar/look-like-scanned/actions/workflows/pylint.yml/badge.svg)](https://github.com/navchandar/look-like-scanned/actions/workflows/pylint.yml)  [![PyTest](https://github.com/navchandar/look-like-scanned/actions/workflows/tests.yml/badge.svg)](https://github.com/navchandar/look-like-scanned/actions/workflows/tests.yml)
 ![license](https://img.shields.io/badge/license-MIT-blue.svg)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/navchandar/look-like-scanned/issues)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) 
 
- - Python script to make documents look like they were scanned. 
+ - Python script to make documents look like they were scanned.
 
- - It converts every page of a given PDF file into an image-based page and applies random askew and brightness (very mild) effects to simulate the appearance of scanned documents.
+ - Local, Private, Secure, Open-Source and Transparent!
+
+ - Converts every page of a given PDF file into an image-based page and applies random askew and brightness (very mild) effects to simulate the appearance of scanned documents.
  
  - The resulting pages are then combined back into an Output PDF file.
 
  - There are options to combine / convert image files into PDF as well.
 
- - Output PDF files are saved in the same input folder with a suffix _"filename_output.pdf"_
+ - Output PDF files are saved in the same folder with a suffix _"File_Name_output.pdf"_
 
 
 ## Installation
 
 Install from the [Python Package Index (PyPI)](https://pypi.org/project/look-like-scanned/)
 ```shell
 pip install look-like-scanned
@@ -130,14 +132,16 @@
 
 - The supported file types are: ".jpg", ".png", ".jpeg", ".webp", ".pdf".
 
 - The output PDF file size **will be bigger** than the input file because the pages are stored in image format.
 
 - Bookmarks / Links / Metadata will be removed when saving the output file.
 
+- Transparency will be removed from png files when converting to pdf.
+
 - Password protected PDF files are not yet supported.
 
 
 ## License
  
  [MIT license](LICENSE)
```

