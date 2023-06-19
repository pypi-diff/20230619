# Comparing `tmp/ycv-0.0.dev4.tar.gz` & `tmp/ycv-0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ycv-0.0.dev4.tar", last modified: Thu Feb 23 05:18:56 2023, max compression
+gzip compressed data, was "ycv-0.0.dev5.tar", last modified: Mon Jun 19 14:16:30 2023, max compression
```

## Comparing `ycv-0.0.dev4.tar` & `ycv-0.0.dev5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2023-02-23 05:18:56.565748 ycv-0.0.dev4/
--rw-rw-r--   0 arif      (1000) arif      (1000)     1071 2022-12-25 06:35:06.000000 ycv-0.0.dev4/LICENSE
--rw-rw-r--   0 arif      (1000) arif      (1000)     3204 2023-02-23 05:18:56.565748 ycv-0.0.dev4/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)     2697 2022-12-27 05:56:50.000000 ycv-0.0.dev4/README.md
--rw-rw-r--   0 arif      (1000) arif      (1000)       84 2022-12-25 07:43:20.000000 ycv-0.0.dev4/pyproject.toml
--rw-rw-r--   0 arif      (1000) arif      (1000)      697 2023-02-23 05:18:56.569748 ycv-0.0.dev4/setup.cfg
--rw-rw-r--   0 arif      (1000) arif      (1000)      420 2023-02-23 05:17:34.000000 ycv-0.0.dev4/setup.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2023-02-23 05:18:56.565748 ycv-0.0.dev4/test/
--rw-rw-r--   0 arif      (1000) arif      (1000)      204 2022-12-25 13:32:30.000000 ycv-0.0.dev4/test/test_interface.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2023-02-23 05:18:56.565748 ycv-0.0.dev4/ycv/
--rw-rw-r--   0 arif      (1000) arif      (1000)       88 2022-12-25 13:05:37.000000 ycv-0.0.dev4/ycv/__init__.py
--rw-rw-r--   0 arif      (1000) arif      (1000)     2311 2022-12-19 15:27:33.000000 ycv-0.0.dev4/ycv/publications.py
--rw-rw-r--   0 arif      (1000) arif      (1000)    25017 2023-01-02 15:05:30.000000 ycv-0.0.dev4/ycv/yamlToTex.py
--rw-rw-r--   0 arif      (1000) arif      (1000)     1503 2023-01-01 11:07:05.000000 ycv-0.0.dev4/ycv/ycv.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2023-02-23 05:18:56.565748 ycv-0.0.dev4/ycv.egg-info/
--rw-rw-r--   0 arif      (1000) arif      (1000)     3204 2023-02-23 05:18:56.000000 ycv-0.0.dev4/ycv.egg-info/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)      302 2023-02-23 05:18:56.000000 ycv-0.0.dev4/ycv.egg-info/SOURCES.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)        1 2023-02-23 05:18:56.000000 ycv-0.0.dev4/ycv.egg-info/dependency_links.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       48 2023-02-23 05:18:56.000000 ycv-0.0.dev4/ycv.egg-info/entry_points.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       20 2023-02-23 05:18:56.000000 ycv-0.0.dev4/ycv.egg-info/requires.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)        4 2023-02-23 05:18:56.000000 ycv-0.0.dev4/ycv.egg-info/top_level.txt
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 14:16:30.137742 ycv-0.0.dev5/
+-rw-r--r--   0 arif      (1000) arif      (1000)     1071 2023-06-19 13:59:34.000000 ycv-0.0.dev5/LICENSE
+-rw-r--r--   0 arif      (1000) arif      (1000)     3204 2023-06-19 14:16:30.137742 ycv-0.0.dev5/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)     2697 2023-06-19 13:59:34.000000 ycv-0.0.dev5/README.md
+-rw-r--r--   0 arif      (1000) arif      (1000)       84 2023-06-19 13:59:34.000000 ycv-0.0.dev5/pyproject.toml
+-rw-r--r--   0 arif      (1000) arif      (1000)      697 2023-06-19 14:16:30.138742 ycv-0.0.dev5/setup.cfg
+-rw-r--r--   0 arif      (1000) arif      (1000)      420 2023-06-19 14:15:58.000000 ycv-0.0.dev5/setup.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 14:16:30.133742 ycv-0.0.dev5/test/
+-rw-r--r--   0 arif      (1000) arif      (1000)      204 2023-06-19 13:59:34.000000 ycv-0.0.dev5/test/test_interface.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 14:16:30.136742 ycv-0.0.dev5/ycv/
+-rw-r--r--   0 arif      (1000) arif      (1000)       88 2023-06-19 13:59:34.000000 ycv-0.0.dev5/ycv/__init__.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2311 2023-06-19 13:59:34.000000 ycv-0.0.dev5/ycv/publications.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    25184 2023-06-19 14:04:32.000000 ycv-0.0.dev5/ycv/yamlToTex.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     1503 2023-06-19 13:59:34.000000 ycv-0.0.dev5/ycv/ycv.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 14:16:30.137742 ycv-0.0.dev5/ycv.egg-info/
+-rw-r--r--   0 arif      (1000) arif      (1000)     3204 2023-06-19 14:16:30.000000 ycv-0.0.dev5/ycv.egg-info/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)      302 2023-06-19 14:16:30.000000 ycv-0.0.dev5/ycv.egg-info/SOURCES.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)        1 2023-06-19 14:16:30.000000 ycv-0.0.dev5/ycv.egg-info/dependency_links.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       48 2023-06-19 14:16:30.000000 ycv-0.0.dev5/ycv.egg-info/entry_points.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       20 2023-06-19 14:16:30.000000 ycv-0.0.dev5/ycv.egg-info/requires.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)        4 2023-06-19 14:16:30.000000 ycv-0.0.dev5/ycv.egg-info/top_level.txt
```

### Comparing `ycv-0.0.dev4/LICENSE` & `ycv-0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev4/PKG-INFO` & `ycv-0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ycv
-Version: 0.0.dev4
+Version: 0.0.dev5
 Summary: Build CV and job application materials from yaml files
 Home-page: https://github.com/md-arif-shaikh/ycv
 Author: Md Arif Shaikh
 Author-email: arifshaikh.astro@gmail.com
 Project-URL: Bug Tracker, https://github.com/md-arif-shaikh/ycv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ycv-0.0.dev4/README.md` & `ycv-0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev4/setup.cfg` & `ycv-0.0.dev5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ycv
-version = 0.0.dev4
+version = 0.0.dev5
 author = Md Arif Shaikh
 author_email = arifshaikh.astro@gmail.com
 description = Build CV and job application materials from yaml files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/md-arif-shaikh/ycv
 project_urls =
```

### Comparing `ycv-0.0.dev4/ycv/publications.py` & `ycv-0.0.dev5/ycv/publications.py`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev4/ycv/yamlToTex.py` & `ycv-0.0.dev5/ycv/yamlToTex.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 class yamlToTeX:
     """Module for building materials for job applications."""
 
     def __init__(self, authinfo_file="authinfo.yaml", style_file="style.yaml",
                  job=None):
         """Init with yaml files for author info and styles.
 
-        parameters:
-        -----------
+        Parameters
+        ----------
         authinfo_file:
             yaml file containg author information.
         style_file:
             yaml file containg styles to apply in TeX.
         job_name:
             Job name to create all files in a directory with job name.
         """
@@ -108,45 +108,45 @@
         fl = open(yaml_file, "r")
         data = yaml.load(fl, Loader=yaml.CLoader)
         fl.close()
         return data
 
     def create_tex_preamble(self):
         preamble = "\\documentclass[10pt]{article}\n"
-        preamble +="\\usepackage[margin=0.8in]{geometry}\n"
-        preamble +="\\usepackage[dvipsnames, usenames]{xcolor}\n"
-        preamble +="\\definecolor{linkcolor}{rgb}{0.0,0.3,0.5}\n"
+        preamble += "\\usepackage[margin=0.8in]{geometry}\n"
+        preamble += "\\usepackage[dvipsnames, usenames]{xcolor}\n"
+        preamble += "\\definecolor{linkcolor}{rgb}{0.0,0.3,0.5}\n"
         hyperref_colors = {}
         for c in ["linkcolor", "citecolor", "filecolor", "urlcolor"]:
             if self.style["tex"][c] is not None:
                 hyperref_colors[c] = self.style["tex"][c]
             else:
                 hyperref_colors[c] = "linkcolor"
-        preamble +=(f"\\usepackage[colorlinks=true, linkcolor={hyperref_colors['linkcolor']},"
-                    f"citecolor={hyperref_colors['citecolor']},"
-                    f"filecolor={hyperref_colors['filecolor']},"
-                    f"urlcolor={hyperref_colors['filecolor']},pdfusetitle]{{hyperref}}\n")
+        preamble += (f"\\usepackage[colorlinks=true, linkcolor={hyperref_colors['linkcolor']},"
+                     f"citecolor={hyperref_colors['citecolor']},"
+                     f"filecolor={hyperref_colors['filecolor']},"
+                     f"urlcolor={hyperref_colors['filecolor']},pdfusetitle]{{hyperref}}\n")
         preamble += "\\usepackage{titlesec}\n"
         preamble += ("\\titleformat{\\section}\n"
                      "{\\normalfont\\Large\\bfseries}{\\thesection}{1em}{}[{\\titlerule[0.5pt]}]")
         if "preamble" in self.style["tex"] and self.style["tex"]["preamble"] is not None:
             preamble += self.style["tex"]["preamble"]
         return preamble
         
     def create_header(self, doc_type="cv"):
         """Create header for TeX.
 
-        parameters:
-        -----------
+        Parameters
+        ----------
         doc_type:
             Type of documents the header is intended for.
             Default is "cv"
 
-        returns:
-        --------
+        Returns
+        -------
             header string suitable to be used in TeX documents.
         """
         align_dict = {"left": "{flushleft}",
                       "right": "{flushright}",
                       "center": "{center}"}
         align = align_dict[self.header_style["align"]]
         title = self.style[doc_type]["title"]
@@ -230,21 +230,21 @@
         os.system(f"pdflatex -interaction=nonstopmode -halt-on-error {tex_file}")
         if self.job is not None:
             os.chdir(current_dir)
 
     def create_cv_body(self, cv_file):
         """Create CV body based on cv_file.
 
-        parameters:
-        -----------
+        Parameters
+        ----------
         cv_file:
             yaml file containing data to build cv.
 
-        returns:
-        --------
+        Returns
+        -------
             Text to be used in TeX file for CV.
         """
         self.cv_file = cv_file
         self.cv = self.get_data_from_yaml_file(self.cv_file)
         self.cv_section_number = "" if self.style["cv"]["numbered-section"] == "y" else "*"
         self.cv_section = self.style["cv"]["section"]
         cv_body = ""
@@ -320,14 +320,20 @@
             if sec == "directory":
                 continue
             bib_dict = pubsections[sec]
             pub_text += self.create_list_of_publications_body(bib_dict)
         return pub_text
 
     def create_list_of_publications(self, publication_file):
+        """
+        Parameters
+        ----------
+        publication_file:
+            Path to publication file.
+        """
         # Write a TeX file
         self.pub = self.get_data_from_yaml_file(publication_file)
         extra_name = ("_" + self.job) if self.job is not None else ""
         tex_file = "list_of_publications" + extra_name + ".tex"
         if self.job is not None:
             if not os.path.exists(self.job):
                 os.mkdir(self.job)
@@ -439,15 +445,16 @@
                     "from-month": month,
                     "to-month": month,
                     "to-year": year,
                     "from-year": year})
             date = self.get_duration_from_dict(t)
             tex += r"\item "
             if "title" in t:
-                tex += f"``{t['title']}\", "
+                tit = t['title'].replace("_", "\\_")
+                tex += f"``{tit}\""
             if "conference" in t:
                 tex += self.create_link(t['conference-url'], t['conference'])
             if "institute" in t:
                 tex += self.create_link(t['institute-url'], t['institute'])
             tex += f"{t['city']}, {t['country']}, " + "\n"
             tex += date
         tex += "\\end{enumerate}\n"
```

### Comparing `ycv-0.0.dev4/ycv/ycv.py` & `ycv-0.0.dev5/ycv/ycv.py`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev4/ycv.egg-info/PKG-INFO` & `ycv-0.0.dev5/ycv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ycv
-Version: 0.0.dev4
+Version: 0.0.dev5
 Summary: Build CV and job application materials from yaml files
 Home-page: https://github.com/md-arif-shaikh/ycv
 Author: Md Arif Shaikh
 Author-email: arifshaikh.astro@gmail.com
 Project-URL: Bug Tracker, https://github.com/md-arif-shaikh/ycv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

