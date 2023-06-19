# Comparing `tmp/ocp_vscode-1.0.0.tar.gz` & `tmp/ocp_vscode-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-1.0.0.tar", last modified: Sun May  7 16:14:31 2023, max compression
+gzip compressed data, was "ocp_vscode-1.1.0.tar", last modified: Mon Jun 19 20:23:35 2023, max compression
```

## Comparing `ocp_vscode-1.0.0.tar` & `ocp_vscode-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 16:14:31.684552 ocp_vscode-1.0.0/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-1.0.0/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-05-07 16:14:31.684606 ocp_vscode-1.0.0/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)     2228 2023-05-07 15:55:57.000000 ocp_vscode-1.0.0/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 16:14:31.683832 ocp_vscode-1.0.0/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      948 2023-04-27 17:11:08.000000 ocp_vscode-1.0.0/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4750 2023-04-21 15:55:51.000000 ocp_vscode-1.0.0/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    16915 2023-04-29 09:55:32.000000 ocp_vscode-1.0.0/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10045 2023-05-07 13:07:57.000000 ocp_vscode-1.0.0/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)    21269 2023-05-07 13:29:25.000000 ocp_vscode-1.0.0/ocp_vscode/show.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 16:14:31.684462 ocp_vscode-1.0.0/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      346 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       38 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-05-07 16:14:31.684875 ocp_vscode-1.0.0/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1136 2023-05-07 11:26:55.000000 ocp_vscode-1.0.0/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-19 20:23:35.768740 ocp_vscode-1.1.0/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-1.1.0/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-19 20:23:35.768790 ocp_vscode-1.1.0/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)     4132 2023-06-19 20:04:27.000000 ocp_vscode-1.1.0/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-19 20:23:35.767942 ocp_vscode-1.1.0/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-17 10:13:52.000000 ocp_vscode-1.1.0/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-17 10:13:52.000000 ocp_vscode-1.1.0/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 07:30:58.000000 ocp_vscode-1.1.0/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-17 10:13:52.000000 ocp_vscode-1.1.0/ocp_vscode/comms.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     9869 2023-06-17 10:13:52.000000 ocp_vscode-1.1.0/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-17 10:13:52.000000 ocp_vscode-1.1.0/ocp_vscode/finder.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    24578 2023-06-19 06:30:51.000000 ocp_vscode-1.1.0/ocp_vscode/show.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-19 20:23:35.768631 ocp_vscode-1.1.0/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-19 20:23:35.000000 ocp_vscode-1.1.0/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-06-19 20:23:35.000000 ocp_vscode-1.1.0/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-19 20:23:35.000000 ocp_vscode-1.1.0/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-19 20:23:35.000000 ocp_vscode-1.1.0/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       61 2023-06-19 20:23:35.000000 ocp_vscode-1.1.0/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-06-19 20:23:35.000000 ocp_vscode-1.1.0/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-06-19 20:23:35.769050 ocp_vscode-1.1.0/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1202 2023-06-17 10:13:52.000000 ocp_vscode-1.1.0/setup.py
```

### Comparing `ocp_vscode-1.0.0/LICENSE` & `ocp_vscode-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.0.0/PKG-INFO` & `ocp_vscode-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 1.0.0
+Version: 1.1.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.0.0/ocp_vscode/animation.py` & `ocp_vscode-1.1.0/ocp_vscode/animation.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import json
 
 from ocp_tessellate.utils import numpy_to_json
-from .config import send
+from .comms import send_data
 
 
 def collect_paths(assembly, path=""):
     result = []
     new_path = f"{path}/{assembly.label}"
     result.append(new_path)
     for child in assembly.children:
@@ -114,8 +114,8 @@
             # if path not in self.paths:
             #     raise ValueError(f"Path '{path}' does not exist in assembly")
 
         self.tracks.append((path, action, times, values))
 
     def animate(self, speed):
         data = {"data": self.tracks, "type": "animation", "config": {"speed": speed}}
-        send(json.loads(numpy_to_json(data)))
+        send_data(json.loads(numpy_to_json(data)))
```

### Comparing `ocp_vscode-1.0.0/ocp_vscode/colors.py` & `ocp_vscode-1.1.0/ocp_vscode/colors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 from colorsys import hsv_to_rgb, rgb_to_hsv
 from random import randrange, seed, random
 from webcolors import name_to_rgb
 
+__all__ = [
+    "BaseColorMap",
+    "ColorMap",
+    "get_colormap",
+    "set_colormap",
+    "unset_colormap",
+    "web_to_rgb",
+]
+
 try:
     import matplotlib as mpl
     import numpy as np
 
     HAS_MATPLOTLIB = True
 
 except:
@@ -238,27 +247,27 @@
 
 
 def web_to_rgb(name):
     rgb = name_to_rgb(name)
     return (rgb.red / 255, rgb.green / 255, rgb.blue / 255)
 
 
-class ColorMap:
+class BaseColorMap:
     def __init__(self):
         self.index = 0
         self.alpha = 1.0
 
     def __iter__(self):
         return self
 
     def reset(self):
         self.index = 0
 
 
-class ListedColorMap(ColorMap):
+class ListedColorMap(BaseColorMap):
     def __init__(self, colors, alpha=1.0, reverse=False):
         super().__init__()
 
         self.colors = []
         for i in range(len(colors)):
             if isinstance(colors[i], str):
                 self.colors.append(web_to_rgb(colors[i]))
@@ -274,15 +283,15 @@
         if self.index >= self.n:
             self.index = 0
         elem = self.colors[self.index]
         self.index += 1
         return (*elem, self.alpha)
 
 
-class SegmentedColorMap(ColorMap):
+class SegmentedColorMap(BaseColorMap):
     def __init__(self, length, mapper, alpha=1.0, reverse=False, **params):
         super().__init__()
 
         self.mapper = mapper
         self.length = length
         self.params = params
         self.alpha = alpha
@@ -295,15 +304,15 @@
         if self.reverse:
             t = 1 - t
         color = self.mapper(t, **self.params)
         self.index += 1
         return (*color, self.alpha)
 
 
-class GoldenRatioColormap(ColorMap):
+class GoldenRatioColormap(BaseColorMap):
     def __init__(self, mapper, alpha=1.0, reverse=False, **params):
         super().__init__()
 
         self.mapper = mapper
         self.params = params
         self.alpha = alpha
         self.reverse = reverse
@@ -315,15 +324,15 @@
             t = 1 - t
         color = self.mapper(t, **self.params)
 
         self.index += 1
         return (*color, self.alpha)
 
 
-class SeededColormap(ColorMap):
+class SeededColormap(BaseColorMap):
     def __init__(self, seed_value, mapper, alpha=1.0, no_param=False, **params):
         super().__init__()
 
         self.mapper = mapper
         self.params = params
         self.seed_value = seed_value
         self.alpha = alpha
@@ -339,15 +348,15 @@
             color = self.mapper(t, **self.params)
         return (*color, self.alpha)
 
     def reset(self):
         seed(self.seed_value)
 
 
-class CM:
+class ColorMap:
     @staticmethod
     def accent(alpha=1.0, reverse=False):
         return ListedColorMap(colormaps["Accent"], alpha=alpha, reverse=reverse)
 
     @staticmethod
     def dark2(alpha=1.0, reverse=False):
         return ListedColorMap(colormaps["Dark2"], alpha=alpha, reverse=reverse)
@@ -416,10 +425,37 @@
 
     @staticmethod
     def segmented(length=10, colormap="hsv", alpha=1.0, reverse=False):
         if colormap == "hsv":
             return SegmentedColorMap(length, hsv_mapper, alpha=alpha, reverse=reverse)
         elif colormap.startswith("mpl"):
             _, name = colormap.split(":")
+            if not isinstance(mpl.colormaps[name], mpl.colors.LinearSegmentedColormap):
+                raise ValueError(
+                    f"{name} is not a segemented matplotlib colormap, use ColorMap.listed({length}, {colormap}))"
+                )
+                name = default
             return SegmentedColorMap(
                 length, matplotlib_mapper, alpha=alpha, name=name, reverse=reverse
             )
+
+    @staticmethod
+    def listed(length=10, colormap="mpl:plasma", colors=None, alpha=1.0, reverse=False):
+        if colors is not None:
+            return ListedColorMap(
+                colors,
+                alpha=alpha,
+                reverse=reverse,
+            )
+        else:
+            _, name = colormap.split(":")
+            colormap = mpl.colormaps[name]
+            if not isinstance(colormap, mpl.colors.ListedColormap):
+                f"{name} is not a listed matplotlib colormap, use ColorMap.segmented({length}, {colormap}))"
+
+            interval = len(colormap.colors) // (length - 1)
+
+            return ListedColorMap(
+                [colormap.colors[i] for i in range(0, len(colormap.colors), interval)],
+                alpha=alpha,
+                reverse=reverse,
+            )
```

### Comparing `ocp_vscode-1.0.0/ocp_vscode/config.py` & `ocp_vscode-1.1.0/ocp_vscode/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import requests
-import orjson as json
-from ocp_tessellate.utils import Timer
+from .comms import send_command, send_data, get_port
 
+__all__ = [
+    "workspace_config",
+    "combined_config",
+    "set_viewer_config",
+    "set_defaults",
+    "reset_defaults",
+    "get_default",
+    "get_defaults",
+    "status",
+]
 
 CONFIG_UI_KEYS = [
     "axes",
     "axes0",
     "black_edges",
     "grid",
     "ortho",
@@ -55,15 +63,15 @@
     "deviation",
     "direct_intensity",
 ]
 
 CONFIG_CONTROL_KEYS = [
     "edge_accuracy",
     "debug",
-    "mate_scale",
+    "helper_scale",
     "render_edges",
     "render_mates",
     "render_joints",
     "render_normals",
     "reset_camera",
     "timeit",
 ]
@@ -97,51 +105,20 @@
 ]
 
 DEFAULTS = {
     "render_edges": True,
     "render_normals": False,
     "render_mates": False,
     "render_joints": False,
-    "mate_scale": 1.0,
+    "helper_scale": 1.0,
     "timeit": False,
     "reset_camera": True,
     "debug": False,
 }
 
-CMD_URL = "http://127.0.0.1"
-CMD_PORT = 3939
-REQUEST_TIMEOUT = 2000
-
-
-def set_port(port):
-    global CMD_PORT
-    CMD_PORT = port
-
-
-def send(data, port=None, timeit=False):
-    if data.get("config") is not None and data["config"].get("collapse") is not None:
-        data["config"]["collapse"] = str(data["config"]["collapse"])
-
-    if port is None:
-        port = CMD_PORT
-    try:
-        with Timer(timeit, "", "json dumps", 1):
-            j = json.dumps(data)
-
-        with Timer(timeit, "", "http send", 1):
-            r = requests.post(f"{CMD_URL}:{port}", data=j)
-
-    except Exception as ex:
-        print("Cannot connect to viewer, is it running and the right port provided?")
-        print(ex)
-        return
-
-    if r.status_code != 201:
-        print("Error", r.text)
-
 
 def set_viewer_config(
     axes=None,
     axes0=None,
     grid=None,
     ortho=None,
     transparent=None,
@@ -159,21 +136,22 @@
     pan_speed=None,
     rotate_speed=None,
     glass=None,
     tools=None,
     tree_width=None,
     collapse=None,
     reset_camera=None,
+    states=None,
 ):
     config = {k: v for k, v in locals().items() if v is not None}
     data = {
         "type": "ui",
         "config": config,
     }
-    send(data)
+    send_data(data)
 
 
 def get_default(key):
     return DEFAULTS.get(key)
 
 
 def get_defaults():
@@ -208,15 +186,16 @@
     default_edgecolor=None,
     ambient_intensity=None,
     direct_intensity=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
-    mate_scale=None,
+    helper_scale=None,
+    mate_scale=None,  # DEPRECATED
     debug=None,
     timeit=None,
 ):
     """Set viewer defaults
     Keywords to configure the viewer:
     - UI
         glass:             Use glass mode where tree is an overlay over the cad object (default=False)
@@ -228,15 +207,16 @@
         axes0:             Show axes at (0,0,0) (default=False)
         grid:              Show grid (default=False)
         ortho:             Use orthographic projections (default=True)
         transparent:       Show objects transparent (default=False)
         default_opacity:   Opacity value for transparent objects (default=0.5)
         black_edges:       Show edges in black color (default=False)
         orbit_control:     Mouse control use "orbit" control instead of "trackball" control (default=False)
-        collapse:          1: collapse all leaf nodes, C: collapse all nodes, E: expand all nodes (default=1)
+        collapse:          1: collapse all single leaf nodes, R: expand root only,
+                           C: collapse all nodes, E: expand all nodes (default=1)
         ticks:             Hint for the number of ticks in both directions (default=10)
         up:                Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
         explode:           Turn on explode mode (default=False)
 
         zoom:              Zoom factor of view (default=1.0)
         position:          Camera position
         quaternion:        Camera orientation as quaternion
@@ -256,24 +236,29 @@
         default_edgecolor: Default mesh color (default=(128, 128, 128))
         ambient_intensity  Intensity of ambient ligth (default=1.0)
         direct_intensity   Intensity of direct lights (default=0.12)
 
         render_edges:      Render edges  (default=True)
         render_normals:    Render normals (default=False)
         render_mates:      Render mates for MAssemblies (default=False)
-        render_joints:      Render mates for MAssemblies (default=False)
-        mate_scale:        Scale of rendered mates for MAssemblies (default=1)
+        render_joints:     Render mates for MAssemblies (default=False)
+        helper_scale:      Scale of rendered helpers (locations, axis, mates for MAssemblies) (default=1)
 
     - Debug
         debug:             Show debug statements to the VS Code browser console (default=False)
         timeit:            Show timing information from level 0-3 (default=False)
     """
 
     kwargs = {k: v for k, v in locals().items() if v is not None}
 
+    if kwargs.get("mate_scale") is not None:
+        print("\nmate_scale is deprecated, use helper_scale instead\n")
+        kwargs["helper_scale"] = kwargs["mate_scale"]
+        del kwargs["mate_scale"]
+
     global DEFAULTS
     for key, value in kwargs.items():
         if key in CONFIG_KEYS:
             DEFAULTS[key] = value
         else:
             print(f"'{key}' is an unkown config, ignored!")
 
@@ -284,42 +269,45 @@
     return get_default(key) if value is None else value
 
 
 def ui_filter(conf):
     return {k: v for k, v in conf.items() if k in CONFIG_UI_KEYS}
 
 
-def status(port=None):
+def status(port=None, debug=False):
     if port is None:
-        port = CMD_PORT
+        port = get_port()
     try:
-        conf = requests.get(f"{CMD_URL}:{port}/status").json()["text"]
-        return conf
+        response = send_command("status", port=port)
+        if debug:
+            return response.get("_debugStarted", False)
+        else:
+            return response.get("text", {})
 
     except Exception as ex:
         raise RuntimeError(
             "Cannot access viewer status. Is the viewer running?\n" + str(ex.args)
         )
 
 
 def workspace_config(port=None):
     if port is None:
-        port = CMD_PORT
+        port = get_port()
     try:
-        return requests.get(f"{CMD_URL}:{port}/config").json()
+        return send_command("config", port=port)
 
     except Exception as ex:
         raise RuntimeError(
             "Cannot access viewer config. Is the viewer running?\n" + str(ex.args)
         )
 
 
 def combined_config(port=None, use_status=True):
     if port is None:
-        port = CMD_PORT
+        port = get_port()
 
     try:
         wspace_config = workspace_config(port)
         wspace_status = status(port)
 
     except Exception as ex:
         raise RuntimeError(
@@ -364,12 +352,12 @@
         set_viewer_config(transparent=config["transparent"])
 
     DEFAULTS = {
         "render_edges": True,
         "render_normals": False,
         "render_mates": False,
         "render_joints": False,
-        "mate_scale": 1.0,
+        "helper_scale": 1.0,
         "timeit": False,
         "reset_camera": True,
         "debug": False,
     }
```

### Comparing `ocp_vscode-1.0.0/ocp_vscode/show.py` & `ocp_vscode-1.1.0/ocp_vscode/show.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,38 +9,63 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
+import sys
 from ocp_tessellate import PartGroup
 from ocp_tessellate.convert import (
     tessellate_group,
     get_normal_len,
     combined_bb,
     to_assembly,
     mp_get_results,
+    is_topods_shape,
+    is_vector,
 )
 from ocp_tessellate.utils import numpy_to_buffer_json, Timer, Color
+from ocp_tessellate.ocp_utils import (
+    is_vector,
+    is_topods_shape,
+    is_topods_compound,
+    is_cadquery,
+    is_cadquery_assembly,
+    is_cadquery_sketch,
+    is_build123d,
+    is_build123d_assembly,
+    is_toploc_location,
+)
+
 from ocp_tessellate.mp_tessellator import init_pool, keymap, close_pool
-from ocp_tessellate.cad_objects import OCP_PartGroup
+from ocp_tessellate.cad_objects import (
+    OCP_PartGroup,
+    OCP_Edges,
+    OCP_Faces,
+    OCP_Part,
+    OCP_Vertices,
+)
+from ocp_tessellate.convert import to_assembly, conv
 import ocp_tessellate.convert as oc
 
 from .config import (
     preset,
     get_changed_config,
     workspace_config,
     combined_config,
     get_default,
-    send,
+    status,
+    set_viewer_config,
 )
+from .comms import send_data, MessageType
 from .colors import *
 
+__all__ = ["show", "show_object", "reset_show", "show_all", "show_clear"]
+
 OBJECTS = {"objs": [], "names": [], "colors": [], "alphas": []}
 
 
 def _tessellate(
     *cad_objs, names=None, colors=None, alphas=None, progress=None, **kwargs
 ):
     if workspace_config().get("_splash"):
@@ -80,15 +105,15 @@
             names=names,
             colors=colors,
             alphas=alphas,
             render_mates=kwargs.get("render_mates", get_changed_config("render_mates")),
             render_joints=kwargs.get(
                 "render_joints", get_changed_config("render_joints")
             ),
-            mate_scale=kwargs.get("mate_scale", get_changed_config("mate_scale")),
+            helper_scale=kwargs.get("helper_scale", get_changed_config("helper_scale")),
             default_color=kwargs.get(
                 "default_color", get_changed_config("default_color")
             ),
             show_parent=kwargs.get("show_parent", get_changed_config("show_parent")),
             progress=progress,
         )
 
@@ -182,15 +207,15 @@
         **kwargs,
     )
     if config.get("dark") is not None:
         config["theme"] = "dark"
     elif config.get("orbit_control") is not None:
         config["control"] = "orbit" if config["control"] else "trackball"
     elif config.get("collapse") is not None:
-        mapping = {"1": 1, "E": 0, "C": 2}
+        mapping = {"1": 1, "E": 0, "C": 2, "R": 3}
         config["collapse"] = mapping.get(config["collapse"], 1)
 
     if config.get("debug") is not None and config["debug"]:
         print("\nconfig:\n", config)
 
     if kwargs.get("explode") is not None:
         config["explode"] = kwargs["explode"]
@@ -275,17 +300,19 @@
     direct_intensity=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
     show_parent=None,
     parallel=None,
-    mate_scale=None,
+    helper_scale=None,
+    mate_scale=None,  # DEPRECATED
     debug=None,
     timeit=None,
+    _force_in_debug=False,
 ):
     """Show CAD objects in Visual Studio Code
     Parameters
         cad_objs:                All cad objects that should be shown as positional parameters
 
     Keywords for show:
         names:                   List of names for the cad_objs. Needs to have the same length as cad_objs
@@ -306,15 +333,16 @@
         axes0:                   Show axes at (0,0,0) (default=False)
         grid:                    Show grid (default=False)
         ortho:                   Use orthographic projections (default=True)
         transparent:             Show objects transparent (default=False)
         default_opacity:         Opacity value for transparent objects (default=0.5)
         black_edges:             Show edges in black color (default=False)
         orbit_control:           Mouse control use "orbit" control instead of "trackball" control (default=False)
-        collapse:                1: collapse all leaf nodes, C: collapse all nodes, E: expand all nodes (default=1)
+        collapse:                1: collapse all single leaf nodes, R: expand root only,
+                                 C: collapse all nodes, E: expand all nodes (default=1)
         ticks:                   Hint for the number of ticks in both directions (default=10)
         up:                      Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
         explode:                 Turn on explode mode (default=False)
 
         zoom:                    Zoom factor of view (default=1.0)
         position:                Camera position
         quaternion:              Camera orientation as quaternion
@@ -340,28 +368,51 @@
 
         render_edges:            Render edges  (default=True)
         render_normals:          Render normals (default=False)
         render_mates:            Render mates for MAssemblies (default=False)
         render_joints:           Render build123d joints (default=False)
         parallel:                Tessellate objects in parallel (default=False)
         show_parent:             Render parent of faces, edges or vertices as wireframe
-        mate_scale:              Scale of rendered mates for MAssemblies (default=1)
+        helper_scale:              Scale of rendered helpers (locations, axis, mates for MAssemblies) (default=1)
 
     - Debug
         debug:                   Show debug statements to the VS Code browser console (default=False)
         timeit:                  Show timing information from level 0-3 (default=False)
     """
+    if sys.gettrace() is not None and not _force_in_debug:
+        print("\nshow and show_object are ignored in debugging sessions\n")
+        return
+
+    kwargs = {
+        k: v
+        for k, v in locals().items()
+        if v is not None
+        and k
+        not in [
+            "cad_objs",
+            "names",
+            "colors",
+            "alphas",
+            "port",
+            "progress",
+        ]
+    }
+
+    if kwargs.get("mate_scale") is not None:
+        print("\nmate_scale is deprecated, use helper_scale instead\n")
+        kwargs["helper_scale"] = kwargs["mate_scale"]
+        del kwargs["mate_scale"]
 
     timeit = preset("timeit", timeit)
 
     names = align_attrs(names, len(cad_objs), None, "names", explode=False)
 
     # Handle colormaps
 
-    if isinstance(colors, ColorMap):
+    if isinstance(colors, BaseColorMap):
         colors = [next(colors) for _ in range(len(cad_objs))]
         alphas = [None] * len(cad_objs)  # alpha is encoded in colors
     else:
         colors = align_attrs(colors, len(cad_objs), None, "colors")
         alphas = align_attrs(alphas, len(cad_objs), None, "alphas")
 
     map_colors = None
@@ -380,47 +431,28 @@
             if alphas[i] is None and len(colors[i]) == 4:
                 alphas[i] = colors[i][3]
             colors[i] = colors[i][:3]
 
     if default_edgecolor is not None:
         default_edgecolor = Color(default_edgecolor).web_color
 
-    kwargs = {
-        k: v
-        for k, v in locals().items()
-        if v is not None
-        and k
-        not in [
-            "cad_objs",
-            "names",
-            "colormap",
-            "colors",
-            "alphas",
-            "port",
-            "progress",
-        ]
-    }
-
-    if explode is not None:
-        kwargs["explode"] = explode
-
     progress = Progress([] if progress is None else [c for c in progress])
 
     with Timer(timeit, "", "overall"):
         data = _convert(
             *cad_objs,
             names=names,
             colors=colors,
             alphas=alphas,
             progress=progress,
             **kwargs,
         )
 
     with Timer(timeit, "", "send"):
-        return send(data, port=port, timeit=timeit)
+        return send_data(data, port=port, timeit=timeit)
 
 
 def reset_show():
     global OBJECTS
 
     OBJECTS = {"objs": [], "names": [], "colors": [], "alphas": []}
 
@@ -467,15 +499,16 @@
     direct_intensity=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
     parallel=None,
     show_parent=None,
-    mate_scale=None,
+    helper_scale=None,
+    mate_scale=None,  # DEPRECATED
     debug=None,
     timeit=None,
 ):
     """Incrementally show CAD objects in Visual Studio Code
 
     Parameters:
         obj:                     The CAD object to be shown
@@ -502,15 +535,16 @@
         axes0:                   Show axes at (0,0,0) (default=False)
         grid:                    Show grid (default=False)
         ortho:                   Use orthographic projections (default=True)
         transparent:             Show objects transparent (default=False)
         default_opacity:         Opacity value for transparent objects (default=0.5)
         black_edges:             Show edges in black color (default=False)
         orbit_control:           Mouse control use "orbit" control instead of "trackball" control (default=False)
-        collapse:                1: collapse all leaf nodes, C: collapse all nodes, E: expand all nodes (default=1)
+        collapse:                1: collapse all single leaf nodes, R: expand root only,
+                                 C: collapse all nodes, E: expand all nodes (default=1)
         ticks:                   Hint for the number of ticks in both directions (default=10)
         up:                      Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
 
         zoom:                    Zoom factor of view (default=1.0)
         position:                Camera position
         quaternion:              Camera orientation as quaternion
         target:                  Camera look at target
@@ -535,15 +569,15 @@
 
         render_edges:            Render edges  (default=True)
         render_normals:          Render normals (default=False)
         render_mates:            Render mates for MAssemblies (default=False)
         render_joints:           Render build123d joints (default=False)
         parallel:                Tessellate objects in parallel (default=False)
         show_parent:             Render parent of faces, edges or vertices as wireframe
-        mate_scale:              Scale of rendered mates for MAssemblies (default=1)
+        helper_scale:            Scale of rendered helpers (locations, axis, mates for MAssemblies) (default=1)
 
     - Debug
         debug:                   Show debug statements to the VS Code browser console (default=False)
         imeit:                   Show timing information from level 0-3 (default=False)
     """
 
     kwargs = {
@@ -585,7 +619,89 @@
         names=OBJECTS["names"],
         colors=OBJECTS["colors"],
         alphas=OBJECTS["alphas"],
         port=port,
         progress=progress,
         **kwargs,
     )
+
+
+first_call = True
+
+
+def show_clear():
+    data = {
+        "type": "clear",
+    }
+    send_data(data)
+
+
+def show_all(variables=None, exclude=None, **kwargs):
+    import inspect
+
+    global first_call
+
+    if variables is None:
+        cf = inspect.currentframe()
+        variables = cf.f_back.f_locals
+
+    if exclude is None:
+        exclude = []
+
+    objects = []
+    names = []
+    for name, obj in variables.items():
+        if isinstance(obj, type):
+            continue  # ignore classes
+
+        if name not in exclude:
+            if hasattr(obj, "_obj") and obj._obj is None:
+                continue
+
+            if hasattr(obj, "locations") and hasattr(obj, "local_locations"):
+                obj = obj.locations
+
+            if hasattr(obj, "to_location"):
+                obj = obj.to_location()
+
+            if (
+                (
+                    hasattr(obj, "wrapped")
+                    and (
+                        is_topods_shape(obj.wrapped)
+                        or is_topods_compound(obj.wrapped)
+                        or is_toploc_location(obj.wrapped)
+                    )
+                )
+                or is_vector(obj)  # Vector
+                or is_cadquery(obj)
+                or is_build123d(obj)
+                or is_cadquery_assembly(obj)
+                or (
+                    isinstance(obj, (list, tuple))
+                    and len(obj) > 0
+                    and hasattr(obj[0], "wrapped")
+                )
+            ):
+                objects.append(obj)
+                names.append(name)
+
+            elif isinstance(
+                obj, (OCP_PartGroup, OCP_Edges, OCP_Faces, OCP_Part, OCP_Vertices)
+            ):
+                objects.append(obj)
+                obj.name = name
+                names.append(name)
+
+            elif is_cadquery_sketch(obj):
+                pg = to_assembly([obj], names=[name])
+                pg.name = name
+                objects.append(pg)
+                names.append(name)
+
+    kwargs["reset_camera"] = first_call
+
+    if len(objects) > 0:
+        show(*objects, names=names, collapse="R", _force_in_debug=True, **kwargs)
+        first_call = False
+    else:
+        show_clear()
```

### Comparing `ocp_vscode-1.0.0/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-1.1.0/ocp_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-vscode
-Version: 1.0.0
+Version: 1.1.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.0.0/setup.cfg` & `ocp_vscode-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.0
+current_version = 1.1.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-1.0.0/setup.py` & `ocp_vscode-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "1.0.0",
+    "version": "1.1.0",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via pythreejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
-    "install_requires": ["ocp-tessellate>=1.0.2", "requests", "orjson"],
+    "install_requires": [
+        "ocp-tessellate>=1.1.0",
+        "requests",
+        "orjson",
+        "websockets>=11.0, <11.1",
+    ],
     "packages": find_packages(),
     "zip_safe": False,
     "author": "Bernhard Walter",
     "author_email": "b_walter@arcor.de",
     "url": "https://github.com/bernhard-42/vscode-ocp-cad-viewer",
     "keywords": ["vscode", "widgets", "CAD", "cadquery"],
     "classifiers": [
```

