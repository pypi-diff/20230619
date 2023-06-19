# Comparing `tmp/st_line_plotter-0.0.3.tar.gz` & `tmp/st_line_plotter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_line_plotter-0.0.3.tar", last modified: Mon Jun 19 05:52:20 2023, max compression
+gzip compressed data, was "st_line_plotter-0.0.4.tar", last modified: Mon Jun 19 06:00:06 2023, max compression
```

## Comparing `st_line_plotter-0.0.3.tar` & `st_line_plotter-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 05:52:20.024894 st_line_plotter-0.0.3/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-06-08 13:50:21.000000 st_line_plotter-0.0.3/LICENSE
--rw-r--r--   0 elliotglas   (501) staff       (20)       51 2023-06-14 07:33:03.000000 st_line_plotter-0.0.3/MANIFEST.in
--rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-19 05:52:20.024709 st_line_plotter-0.0.3/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-06-19 05:52:20.024974 st_line_plotter-0.0.3/setup.cfg
--rw-r--r--   0 elliotglas   (501) staff       (20)      671 2023-06-19 05:50:24.000000 st_line_plotter-0.0.3/setup.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 05:52:20.018313 st_line_plotter-0.0.3/st_line_plotter/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2495 2023-06-19 05:48:41.000000 st_line_plotter-0.0.3/st_line_plotter/__init__.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 05:52:20.017149 st_line_plotter-0.0.3/st_line_plotter/frontend/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 05:52:20.020684 st_line_plotter-0.0.3/st_line_plotter/frontend/build/
--rw-r--r--   0 elliotglas   (501) staff       (20)      928 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/asset-manifest.json
--rw-r--r--   0 elliotglas   (501) staff       (20)     2119 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/index.html
--rw-r--r--   0 elliotglas   (501) staff       (20)      673 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/precache-manifest.2789ed6399de93230535e104691ce67f.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     1183 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/service-worker.js
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 05:52:20.017393 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 05:52:20.024009 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/
--rw-r--r--   0 elliotglas   (501) staff       (20)   459440 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     1909 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.LICENSE.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)  1700606 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     7864 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)    26390 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     8317 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 05:52:20.024230 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/media/
--rw-r--r--   0 elliotglas   (501) staff       (20)   149674 2023-06-13 13:38:23.000000 st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/media/ground.0d5856bc.png
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 05:52:20.019492 st_line_plotter-0.0.3/st_line_plotter.egg-info/
--rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-19 05:52:19.000000 st_line_plotter-0.0.3/st_line_plotter.egg-info/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)     1008 2023-06-19 05:52:19.000000 st_line_plotter-0.0.3/st_line_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-06-19 05:52:19.000000 st_line_plotter-0.0.3/st_line_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-19 05:52:19.000000 st_line_plotter-0.0.3/st_line_plotter.egg-info/requires.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-19 05:52:19.000000 st_line_plotter-0.0.3/st_line_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:00:06.464777 st_line_plotter-0.0.4/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-06-08 13:50:21.000000 st_line_plotter-0.0.4/LICENSE
+-rw-r--r--   0 elliotglas   (501) staff       (20)       51 2023-06-14 07:33:03.000000 st_line_plotter-0.0.4/MANIFEST.in
+-rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-19 06:00:06.464577 st_line_plotter-0.0.4/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-06-19 06:00:06.464846 st_line_plotter-0.0.4/setup.cfg
+-rw-r--r--   0 elliotglas   (501) staff       (20)      671 2023-06-19 05:59:45.000000 st_line_plotter-0.0.4/setup.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:00:06.456521 st_line_plotter-0.0.4/st_line_plotter/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2213 2023-06-19 05:59:27.000000 st_line_plotter-0.0.4/st_line_plotter/__init__.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:00:06.455336 st_line_plotter-0.0.4/st_line_plotter/frontend/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:00:06.458808 st_line_plotter-0.0.4/st_line_plotter/frontend/build/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      928 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/asset-manifest.json
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2119 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/index.html
+-rw-r--r--   0 elliotglas   (501) staff       (20)      673 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/precache-manifest.2789ed6399de93230535e104691ce67f.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1183 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/service-worker.js
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:00:06.455573 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:00:06.463770 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/
+-rw-r--r--   0 elliotglas   (501) staff       (20)   459440 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1909 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.LICENSE.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)  1700606 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     7864 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)    26390 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     8317 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:00:06.464028 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/media/
+-rw-r--r--   0 elliotglas   (501) staff       (20)   149674 2023-06-13 13:38:23.000000 st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/media/ground.0d5856bc.png
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:00:06.457633 st_line_plotter-0.0.4/st_line_plotter.egg-info/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-19 06:00:06.000000 st_line_plotter-0.0.4/st_line_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1008 2023-06-19 06:00:06.000000 st_line_plotter-0.0.4/st_line_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-06-19 06:00:06.000000 st_line_plotter-0.0.4/st_line_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-19 06:00:06.000000 st_line_plotter-0.0.4/st_line_plotter.egg-info/requires.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-19 06:00:06.000000 st_line_plotter-0.0.4/st_line_plotter.egg-info/top_level.txt
```

### Comparing `st_line_plotter-0.0.3/LICENSE` & `st_line_plotter-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/setup.py` & `st_line_plotter-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_line_plotter",
-    version="0.0.3",
+    version="0.0.4",
     author="Elliot Glas",
     author_email="elliot.glas@hotmail.se",
     description="A tool to place lines on an image and get back the coordinates for those lines",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_line_plotter-0.0.3/st_line_plotter/__init__.py` & `st_line_plotter-0.0.4/st_line_plotter/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,27 +25,29 @@
     size = fig.get_size_inches()*fig.dpi
 
     buffer = BytesIO()
     fig.savefig(buffer, format='PNG')
     base64_image = base64.b64encode(buffer.getvalue()).decode('utf-8')
     data_url = f"data:image/png;base64,{base64_image}"
 
-    width = width if width == None else size[0]
-    height = height if height == None else size[1]
+    width = width if width != None else size[0]
+    height = height if height != None else size[1]
 
     component_value = _component_func(lines=lines, image=data_url, changed=changed, width=width, height=height, key=key, default=0)
     return component_value
 
 
 # Test code
 if not _RELEASE:
     import streamlit as st
     st.set_page_config(layout="wide")
 
     fig = plt.figure()
+    print("Fig1",fig)
+
     plt.plot(range(10)) 
     size = fig.get_size_inches()*fig.dpi
 
     buffer = BytesIO()
     fig.savefig(buffer, format='PNG')
     base64_image = base64.b64encode(buffer.getvalue()).decode('utf-8')
     data_url = f"data:image/png;base64,{base64_image}"
@@ -60,15 +62,11 @@
     #    st.session_state.changed = 0
     #if st.button("Edit 1"):
     #    st.session_state.changed = 1
     #if st.button("Edit 2"):
     #    st.session_state.changed = 2
 
     #print(st.session_state.changed)
-    lines1 = st_line_plotter(lines=st.session_state["lines"], changed=1, image=v_camera, width=2048 / scale, height=1536 / scale, key=1)
+    lines1 = st_line_plotter(lines=st.session_state["lines"], changed=1, fig=fig, key=1)
     if lines1 != 0 and lines1 != st.session_state["lines"]:
         st.session_state["lines"] = lines1
         st.session_state.changed = 1
-    lines2 = st_line_plotter(lines=st.session_state["lines"],changed=2, image=v_ground, width=800, height=360, key=2)
-    if lines2 != 0 and lines2 != st.session_state["lines"]:
-        st.session_state["lines"] = lines2
-    print(st.session_state["lines"])
```

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/asset-manifest.json` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/index.html` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/precache-manifest.2789ed6399de93230535e104691ce67f.js` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/precache-manifest.2789ed6399de93230535e104691ce67f.js`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/service-worker.js` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.LICENSE.txt` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.map` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/2.51f30e44.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js.map` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/main.e8acecfa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter/frontend/build/static/media/ground.0d5856bc.png` & `st_line_plotter-0.0.4/st_line_plotter/frontend/build/static/media/ground.0d5856bc.png`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.3/st_line_plotter.egg-info/SOURCES.txt` & `st_line_plotter-0.0.4/st_line_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

