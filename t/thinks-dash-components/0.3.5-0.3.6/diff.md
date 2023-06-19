# Comparing `tmp/thinks_dash_components-0.3.5.tar.gz` & `tmp/thinks_dash_components-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.3.5.tar", last modified: Mon Apr 17 08:01:55 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.3.6.tar", last modified: Mon Jun 19 03:44:48 2023, max compression
```

## Comparing `thinks_dash_components-0.3.5.tar` & `thinks_dash_components-0.3.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 08:01:55.109531 thinks_dash_components-0.3.5/
--rw-rw-rw-   0        0        0        0 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      453 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-04-17 08:01:55.109531 thinks_dash_components-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3706 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.5/README.md
--rw-rw-rw-   0        0        0     2309 2023-04-17 07:59:14.000000 thinks_dash_components-0.3.5/package.json
--rw-rw-rw-   0        0        0       42 2023-04-17 08:01:55.110532 thinks_dash_components-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:01:55.102530 thinks_dash_components-0.3.5/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1458 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1304 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.5/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2273 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.5/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44448 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2309 2023-04-17 08:01:35.000000 thinks_dash_components-0.3.5/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   124273 2023-04-17 08:01:34.000000 thinks_dash_components-0.3.5/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-04-17 08:01:34.000000 thinks_dash_components-0.3.5/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-04-17 08:01:55.108531 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-04-17 08:01:55.000000 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-04-17 08:01:55.000000 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 08:01:55.000000 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-17 08:01:55.000000 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 03:44:48.542964 thinks_dash_components-0.3.6/
+-rw-rw-rw-   0        0        0        0 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      453 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-06-19 03:44:48.540963 thinks_dash_components-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3706 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.6/README.md
+-rw-rw-rw-   0        0        0     2309 2023-06-19 03:43:35.000000 thinks_dash_components-0.3.6/package.json
+-rw-rw-rw-   0        0        0       42 2023-06-19 03:44:48.542964 thinks_dash_components-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:44:48.533961 thinks_dash_components-0.3.6/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1533 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1304 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.6/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2273 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.6/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44590 2023-06-19 03:44:26.000000 thinks_dash_components-0.3.6/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2309 2023-06-19 03:44:25.000000 thinks_dash_components-0.3.6/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   124286 2023-06-19 03:44:24.000000 thinks_dash_components-0.3.6/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-06-19 03:44:24.000000 thinks_dash_components-0.3.6/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-06-19 03:44:48.539963 thinks_dash_components-0.3.6/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-06-19 03:44:48.000000 thinks_dash_components-0.3.6/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-06-19 03:44:48.000000 thinks_dash_components-0.3.6/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:44:48.000000 thinks_dash_components-0.3.6/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-19 03:44:48.000000 thinks_dash_components-0.3.6/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.3.5/PKG-INFO` & `thinks_dash_components-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks_dash_components
-Version: 0.3.5
+Version: 0.3.6
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.5/README.md` & `thinks_dash_components-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/package.json` & `thinks_dash_components-0.3.6/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.3.6'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.5"
+    "version": "0.3.6"
 }
```

### Comparing `thinks_dash_components-0.3.5/setup.py` & `thinks_dash_components-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/Alert.py` & `thinks_dash_components-0.3.6/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.3.6/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.3.6/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.3.6/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.3.6/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.3.6/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.3.6/thinks_dash_components/Rotate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class MobileDropdown(Component):
-    """A MobileDropdown component.
+class Rotate(Component):
+    """A Rotate component.
 
 
 Keyword arguments:
 
 - id (string; optional)
 
-- className (string; optional)
+- delay (number; default 10)
 
-- clearable (boolean; default True)
+- message (a list of or a singular dash component, string or number; optional)
 
-- disable (boolean; optional)
+- orientation (string; optional)
 
-- notfoundMsg (string; optional)
+- reload (boolean; default True)
 
-- options (list; optional)
-
-- value (string | number; optional)"""
-    _children_props = []
-    _base_nodes = ['children']
+- timing (string; default 'all')"""
+    _children_props = ['message']
+    _base_nodes = ['message', 'children']
     _namespace = 'thinks_dash_components'
-    _type = 'MobileDropdown'
+    _type = 'Rotate'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, options=Component.UNDEFINED, value=Component.UNDEFINED, notfoundMsg=Component.UNDEFINED, clearable=Component.UNDEFINED, disable=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'className', 'clearable', 'disable', 'notfoundMsg', 'options', 'value']
+    def __init__(self, id=Component.UNDEFINED, orientation=Component.UNDEFINED, message=Component.UNDEFINED, reload=Component.UNDEFINED, timing=Component.UNDEFINED, delay=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'delay', 'message', 'orientation', 'reload', 'timing']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'className', 'clearable', 'disable', 'notfoundMsg', 'options', 'value']
+        self.available_properties = ['id', 'delay', 'message', 'orientation', 'reload', 'timing']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
-        super(MobileDropdown, self).__init__(**args)
+        super(Rotate, self).__init__(**args)
```

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/Notice.py` & `thinks_dash_components-0.3.6/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.3.6/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.3.6/thinks_dash_components/_ComponentTemplate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
-class Rotate(Component):
-    """A Rotate component.
-
+class _ComponentTemplate(Component):
+    """A _ComponentTemplate component.
+ExampleComponent is an example component.
+It takes a property, `label`, and
+displays it.
+It renders an input with the property `value`
+which is editable by the user.
 
 Keyword arguments:
 
-- id (string; optional)
-
-- delay (number; default 10)
-
-- message (a list of or a singular dash component, string or number; optional)
+- id (string; optional):
+    The ID used to identify this component in Dash callbacks.
 
-- orientation (string; optional)
+- label (string; required):
+    A label that will be printed when this component is rendered.
 
-- reload (boolean; default True)
-
-- timing (string; default 'all')"""
-    _children_props = ['message']
-    _base_nodes = ['message', 'children']
+- value (string; optional):
+    The value displayed in the input."""
+    _children_props = []
+    _base_nodes = ['children']
     _namespace = 'thinks_dash_components'
-    _type = 'Rotate'
+    _type = '_ComponentTemplate'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, orientation=Component.UNDEFINED, message=Component.UNDEFINED, reload=Component.UNDEFINED, timing=Component.UNDEFINED, delay=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'delay', 'message', 'orientation', 'reload', 'timing']
+    def __init__(self, id=Component.UNDEFINED, label=Component.REQUIRED, value=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'label', 'value']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'delay', 'message', 'orientation', 'reload', 'timing']
+        self.available_properties = ['id', 'label', 'value']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
-        super(Rotate, self).__init__(**args)
+        for k in ['label']:
+            if k not in args:
+                raise TypeError(
+                    'Required argument `' + k + '` was not specified.')
+
+        super(_ComponentTemplate, self).__init__(**args)
```

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.3.6/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.3.6/thinks_dash_components/StorageObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.3.6/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.3.6/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/__init__.py` & `thinks_dash_components-0.3.6/thinks_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.3.6/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/metadata.json` & `thinks_dash_components-0.3.6/thinks_dash_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995039682539683%*

 * *Differences: {"'src/lib/components/MobileDropdown.react.js'": "{'props': {'label': OrderedDict([('type', "*

 * *                                                 "OrderedDict([('name', 'string')])), ('required', "*

 * *                                                 "False), ('description', '')])}}"}*

```diff
@@ -1006,14 +1006,21 @@
             "id": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
+            "label": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
             "notfoundMsg": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
```

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/package-info.json` & `thinks_dash_components-0.3.6/thinks_dash_components/package-info.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.3.6'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.5"
+    "version": "0.3.6"
 }
```

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.3.6/thinks_dash_components/thinks_dash_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(o()),
                 r = i(e);
             if (!t) return r;
             var n = r.split("/"),
                 a = n.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_3_5m1681718492"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_3_6m1687146261"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -3873,62 +3873,63 @@
                         label: null,
                         value: null
                     }
                 }
             }, {
                 key: "render",
                 value: function() {
-                    var e, t = this.props,
-                        r = t.id,
-                        n = t.className,
-                        o = t.options,
-                        i = t.notfoundMsg,
-                        a = t.clearable,
-                        s = t.value,
+                    var e = this.props,
+                        t = e.id,
+                        r = e.className,
+                        n = e.options,
+                        o = e.notfoundMsg,
+                        i = e.clearable,
+                        a = e.value,
+                        s = e.label,
                         c = [];
-                    if (o && o.length > 0) {
-                        var u, l = Fe(o);
+                    if (n && n.length > 0) {
+                        var u, l = Fe(n);
                         try {
                             for (l.s(); !(u = l.n()).done;) {
                                 var f = u.value;
                                 c.push(h.a.createElement(at, {
                                     key: f.value,
                                     "data-value": f.value,
                                     "data-label": f.label,
                                     onClick: this.select
-                                }, h.a.createElement("span", null, f.label))), String(f.value) === String(s) && (e = f.label, console.log("-- MOBILE DROPDOWN", s, e))
+                                }, h.a.createElement("span", null, f.label))), String(f.value) === String(a) && console.log("-- MOBILE DROPDOWN", a, s)
                             }
                         } catch (e) {
                             l.e(e)
                         } finally {
                             l.f()
                         }
                     } else c.push(h.a.createElement(at, {
                         key: "not_found",
                         onClick: this.select
-                    }, h.a.createElement("span", null, i || "No results found")));
+                    }, h.a.createElement("span", null, o || "No results found")));
                     return h.a.createElement("div", {
-                        id: r,
+                        id: t,
                         style: {
                             width: "100%",
                             position: "relative"
                         },
-                        className: "mobile-dropdown " + n + (this.state.open ? " open" : "")
+                        className: "mobile-dropdown " + r + (this.state.open ? " open" : "")
                     }, h.a.createElement(lt, {
                         className: "mobile-dropdown-bg",
                         style: {
                             display: this.state.open ? "block" : "none"
                         },
                         onTouchEnd: this.close
                     }), h.a.createElement(st, {
                         id: this.id + "-value",
                         className: "mobile-dropdown-value",
                         onTouchEnd: this.toggle,
                         ref: this.valueRef
-                    }, h.a.createElement(ct, null, e), a ? h.a.createElement(ut, {
+                    }, h.a.createElement(ct, null, s), i ? h.a.createElement(ut, {
                         onTouchEnd: this.clear,
                         className: "mobile-dropdown-clear"
                     }, h.a.createElement($e, null)) : null), h.a.createElement(ot, {
                         className: "mobile-dropdown-list",
                         style: this.state.listStyle,
                         ref: this.wrapRef,
                         onScroll: this.scroll,
@@ -4102,15 +4103,16 @@
         id: p.a.string,
         className: p.a.string,
         options: p.a.array,
         value: p.a.oneOfType([p.a.string, p.a.number]),
         notfoundMsg: p.a.string,
         clearable: p.a.bool,
         setProps: p.a.func,
-        disable: p.a.bool
+        disable: p.a.bool,
+        label: p.a.string
     };
     var Et = y.a.div(Je || (Je = Ot(["\n    position: fixed;\n    top: 0;\n    left: 0;\n    width: 100%;\n    height: 100%;\n"]))),
         Pt = y.a.div.attrs((function(e) {
             return {
                 iconColor: e.iconColor
             }
         }))(Ke || (Ke = Ot(["\n    width: 30px;\n    height: 30px;\n    position: relative;\n\n    svg {\n        width: 100%;\n        height: 100%;\n        color: ", ";\n    }\n"])), (function(e) {
```

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.3.6/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks-dash-components
-Version: 0.3.5
+Version: 0.3.6
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.5/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.3.6/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

