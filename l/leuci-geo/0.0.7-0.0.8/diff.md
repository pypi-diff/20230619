# Comparing `tmp/leuci-geo-0.0.7.tar.gz` & `tmp/leuci-geo-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leuci-geo-0.0.7.tar", last modified: Sat Jun 17 19:25:52 2023, max compression
+gzip compressed data, was "leuci-geo-0.0.8.tar", last modified: Mon Jun 19 19:29:36 2023, max compression
```

## Comparing `leuci-geo-0.0.7.tar` & `leuci-geo-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 19:25:52.615055 leuci-geo-0.0.7/
--rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.7/LICENSE
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-17 19:25:52.615055 leuci-geo-0.0.7/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.7/README.md
--rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.7/pyproject.toml
--rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-06-17 19:25:52.615055 leuci-geo-0.0.7/setup.cfg
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 19:25:52.605055 leuci-geo-0.0.7/src/
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 19:25:52.605055 leuci-geo-0.0.7/src/leuci_geo/
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.7/src/leuci_geo/__init__.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     2963 2023-05-29 13:51:47.000000 leuci-geo-0.0.7/src/leuci_geo/geocalculator.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)    27123 2023-06-04 18:16:10.000000 leuci-geo-0.0.7/src/leuci_geo/pdbgeometry.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     2844 2023-05-29 13:40:46.000000 leuci-geo-0.0.7/src/leuci_geo/pdbloader.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     9405 2023-06-04 13:05:42.000000 leuci-geo-0.0.7/src/leuci_geo/pdbobject.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-05-29 10:54:24.000000 leuci-geo-0.0.7/src/leuci_geo/pdbspace.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)    22543 2023-06-17 19:12:49.000000 leuci-geo-0.0.7/src/leuci_geo/reportmaker.py
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 19:25:52.615055 leuci-geo-0.0.7/src/leuci_geo.egg-info/
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-17 19:25:52.000000 leuci-geo-0.0.7/src/leuci_geo.egg-info/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)      385 2023-06-17 19:25:52.000000 leuci-geo-0.0.7/src/leuci_geo.egg-info/SOURCES.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-06-17 19:25:52.000000 leuci-geo-0.0.7/src/leuci_geo.egg-info/dependency_links.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-06-17 19:25:52.000000 leuci-geo-0.0.7/src/leuci_geo.egg-info/top_level.txt
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-19 19:29:36.027644 leuci-geo-0.0.8/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.8/LICENSE
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-19 19:29:36.027644 leuci-geo-0.0.8/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.8/README.md
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.8/pyproject.toml
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-06-19 19:29:36.027644 leuci-geo-0.0.8/setup.cfg
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-19 19:29:36.017644 leuci-geo-0.0.8/src/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-19 19:29:36.017644 leuci-geo-0.0.8/src/leuci_geo/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.8/src/leuci_geo/__init__.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2963 2023-05-29 13:51:47.000000 leuci-geo-0.0.8/src/leuci_geo/geocalculator.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    27123 2023-06-04 18:16:10.000000 leuci-geo-0.0.8/src/leuci_geo/pdbgeometry.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2844 2023-05-29 13:40:46.000000 leuci-geo-0.0.8/src/leuci_geo/pdbloader.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     9405 2023-06-04 13:05:42.000000 leuci-geo-0.0.8/src/leuci_geo/pdbobject.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-05-29 10:54:24.000000 leuci-geo-0.0.8/src/leuci_geo/pdbspace.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    22826 2023-06-19 19:28:31.000000 leuci-geo-0.0.8/src/leuci_geo/reportmaker.py
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-19 19:29:36.027644 leuci-geo-0.0.8/src/leuci_geo.egg-info/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-19 19:29:35.000000 leuci-geo-0.0.8/src/leuci_geo.egg-info/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      385 2023-06-19 19:29:36.000000 leuci-geo-0.0.8/src/leuci_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-06-19 19:29:35.000000 leuci-geo-0.0.8/src/leuci_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-06-19 19:29:35.000000 leuci-geo-0.0.8/src/leuci_geo.egg-info/top_level.txt
```

### Comparing `leuci-geo-0.0.7/LICENSE` & `leuci-geo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.7/PKG-INFO` & `leuci-geo-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.7
+Version: 0.0.8
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leuci-geo-0.0.7/setup.cfg` & `leuci-geo-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = leuci-geo
-version = 0.0.7
+version = 0.0.8
 author = Rachel Alcraft
 author_email = rachelalcraft@gmail.com
 description = geometric paramaters and searches of protein structures
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `leuci-geo-0.0.7/src/leuci_geo/geocalculator.py` & `leuci-geo-0.0.8/src/leuci_geo/geocalculator.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.7/src/leuci_geo/pdbgeometry.py` & `leuci-geo-0.0.8/src/leuci_geo/pdbgeometry.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.7/src/leuci_geo/pdbloader.py` & `leuci-geo-0.0.8/src/leuci_geo/pdbloader.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.7/src/leuci_geo/pdbobject.py` & `leuci-geo-0.0.8/src/leuci_geo/pdbobject.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.7/src/leuci_geo/reportmaker.py` & `leuci-geo-0.0.8/src/leuci_geo/reportmaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,20 +247,26 @@
         # Having plotted we now need to get the image data from the plt
         if not overlay:
             encoded = self.getPlotImage(self.fig, self.ax)
             htmlstring = '<img src="data:image/png;base64, {}">'.format(encoded.decode('utf-8')) + '\n'
             self.HTMLIncrement()
             self.html_string += '<td width=' + str(int(100 / self.cols)) + '%>' + htmlstring + '</td>\n'
 
-    def addPlotPi(self, data,geo_x,hue,title='',colors=[],overlay=False,alpha=1):
+    def addPlotPi(self, data,geo_x,hue,title='',colors=[],overlay=False,alpha=1,percent=False):
         self.incrementOverlay(overlay)
         if colors == []:
-            plt.pie(data[geo_x],labels=data[hue])
+            if percent:
+                plt.pie(data[geo_x],labels=data[hue], autopct='%1.1f%%')
+            else:
+                plt.pie(data[geo_x],labels=data[hue])
         else:
-            plt.pie(data[geo_x], labels=data[hue],colors=colors,alpha=alpha)
+            if percent:
+                plt.pie(data[geo_x], labels=data[hue],colors=colors,alpha=alpha, autopct='%1.1f%%')
+            else:
+                plt.pie(data[geo_x], labels=data[hue],colors=colors,alpha=alpha)
         plt.title(title)
         # Having plotted we now need to get the image data from the plt
         if not overlay:
             encoded = self.getPlotImage(self.fig, self.ax)
             htmlstring = '<img src="data:image/png;base64, {}">'.format(encoded.decode('utf-8')) + '\n'
             self.HTMLIncrement()
             self.html_string += '<td width=' + str(int(100 / self.cols)) + '%>' + htmlstring + '</td>\n'
@@ -512,28 +518,28 @@
         # html += '<style> body {background-color:SeaShell;} table {table-layout:fixed;display:table;margin:0 auto;}td {border:1px solid RosyBrown;background-color:SeaShell;}</style>'
         # html += '<style> body {background-color:HoneyDew;} table {background-color:HoneyDew;} .innertable td {border:1px solid MistyRose;background-color:MintCream;}</style>'
         html += '<style> body {text-align:center;background-color:' + self.clr_background + ' ;} img {width:95% }'
         html += 'table {font-size:0.8vw;width:95%;table-layout:fixed;display:table;margin:0 auto;background-color:lightgrey ;}'
         html += ' td {border:1px solid ' + self.clr_behindplot + ';background-color:' + self.clr_behindplot + ';}</style>'
         html += '</head>\n'
         html += '<body>'
-        if not remove_strip:
-            html += '<hr/>'
-            html += '<div style="background-color:' + self.clr_header + ';padding:10px"> LeucipPy: Protein Geometry Correlations </div>'
+        # if not remove_strip:
+        #    html += '<hr/>'
+        #    html += '<div style="background-color:' + self.clr_header + ';padding:10px"> LeucipPy: Protein Geometry Correlations </div>'
         html += '<hr/>'
         html += '<div style="background-color:lightgrey;padding:5px">'
         html += '<h1>' + title + '</h1>\n'
         html += '</div>'
         html += '<hr/>\n'
 
         return html
 
     def getFooterString(self):
         html = '<hr/><div style = "background-color:' + self.clr_header +';padding:10px" >'
-        html += '<a href = "https://rachelalcraft.github.io/leucippy.html" title = "LeucipPy" target = "_self">LeucipPy</a>'
+        html += '<a href = "https://rachelalcraft.github.io/leucipPy.html" title = "LeucipPy" target = "_self">LeucipPy</a>'
         html += ' by <a href = "mailto:rachelalcraft@gmail.com">Rachel Alcraft</a>'
         html += ' ~ supervisor <a href = "http://people.cryst.bbk.ac.uk/~ubcg66a/">Mark A Williams</a>'
         html += ' ~ Birkbeck, University of London (2021)'
         html += ' ~ Follow <a href = "https://rachelalcraft.github.io/citing.html"> citation guidance </a> </br></div><hr/>'
         return html
```

### Comparing `leuci-geo-0.0.7/src/leuci_geo.egg-info/PKG-INFO` & `leuci-geo-0.0.8/src/leuci_geo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.7
+Version: 0.0.8
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

