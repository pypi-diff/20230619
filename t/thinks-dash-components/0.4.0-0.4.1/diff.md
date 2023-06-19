# Comparing `tmp/thinks_dash_components-0.4.0.tar.gz` & `tmp/thinks_dash_components-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.4.0.tar", last modified: Mon Jun 19 07:51:16 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.4.1.tar", last modified: Mon Jun 19 08:38:17 2023, max compression
```

## Comparing `thinks_dash_components-0.4.0.tar` & `thinks_dash_components-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:51:16.671806 thinks_dash_components-0.4.0/
--rw-rw-rw-   0        0        0        0 2023-04-17 07:43:57.000000 thinks_dash_components-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      453 2023-04-17 07:43:57.000000 thinks_dash_components-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-06-19 07:51:16.670805 thinks_dash_components-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3706 2023-04-17 07:43:57.000000 thinks_dash_components-0.4.0/README.md
--rw-rw-rw-   0        0        0     2309 2023-06-19 07:50:17.000000 thinks_dash_components-0.4.0/package.json
--rw-rw-rw-   0        0        0       42 2023-06-19 07:51:16.672804 thinks_dash_components-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-04-17 07:43:58.000000 thinks_dash_components-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:51:16.661801 thinks_dash_components-0.4.0/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1533 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1304 2023-04-17 07:43:58.000000 thinks_dash_components-0.4.0/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2273 2023-04-17 07:43:58.000000 thinks_dash_components-0.4.0/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44590 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2309 2023-06-19 07:51:11.000000 thinks_dash_components-0.4.0/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   123724 2023-06-19 07:51:10.000000 thinks_dash_components-0.4.0/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-06-19 07:51:10.000000 thinks_dash_components-0.4.0/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-06-19 07:51:16.668802 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-06-19 07:51:16.000000 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-06-19 07:51:16.000000 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:51:16.000000 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-19 07:51:16.000000 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 08:38:17.115049 thinks_dash_components-0.4.1/
+-rw-rw-rw-   0        0        0        0 2023-04-17 07:43:57.000000 thinks_dash_components-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      453 2023-04-17 07:43:57.000000 thinks_dash_components-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-06-19 08:38:17.114049 thinks_dash_components-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3706 2023-04-17 07:43:57.000000 thinks_dash_components-0.4.1/README.md
+-rw-rw-rw-   0        0        0     2309 2023-06-19 08:37:55.000000 thinks_dash_components-0.4.1/package.json
+-rw-rw-rw-   0        0        0       42 2023-06-19 08:38:17.116052 thinks_dash_components-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-17 07:43:58.000000 thinks_dash_components-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:38:17.107047 thinks_dash_components-0.4.1/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1533 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1304 2023-04-17 07:43:58.000000 thinks_dash_components-0.4.1/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2273 2023-04-17 07:43:58.000000 thinks_dash_components-0.4.1/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44590 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2309 2023-06-19 08:38:08.000000 thinks_dash_components-0.4.1/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   123763 2023-06-19 08:38:06.000000 thinks_dash_components-0.4.1/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-06-19 08:38:06.000000 thinks_dash_components-0.4.1/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-06-19 08:38:17.113050 thinks_dash_components-0.4.1/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-06-19 08:38:16.000000 thinks_dash_components-0.4.1/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-06-19 08:38:17.000000 thinks_dash_components-0.4.1/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:38:16.000000 thinks_dash_components-0.4.1/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-19 08:38:16.000000 thinks_dash_components-0.4.1/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.4.0/PKG-INFO` & `thinks_dash_components-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks_dash_components
-Version: 0.4.0
+Version: 0.4.1
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.4.0/README.md` & `thinks_dash_components-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/package.json` & `thinks_dash_components-0.4.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.4.1'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `thinks_dash_components-0.4.0/setup.py` & `thinks_dash_components-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/Alert.py` & `thinks_dash_components-0.4.1/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.4.1/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.4.1/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.4.1/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.4.1/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.4.1/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.4.1/thinks_dash_components/MobileDropdown.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/Notice.py` & `thinks_dash_components-0.4.1/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.4.1/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.4.1/thinks_dash_components/Rotate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.4.1/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.4.1/thinks_dash_components/StorageObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.4.1/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.4.1/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/_ComponentTemplate.py` & `thinks_dash_components-0.4.1/thinks_dash_components/_ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/__init__.py` & `thinks_dash_components-0.4.1/thinks_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.4.1/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/metadata.json` & `thinks_dash_components-0.4.1/thinks_dash_components/metadata.json`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/package-info.json` & `thinks_dash_components-0.4.1/thinks_dash_components/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.4.1'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.4.1/thinks_dash_components/thinks_dash_components.min.js`

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
-            return a.splice(1, 0, "v0_4_0m1687161068"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_4_1m1687163884"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -3769,22 +3769,24 @@
                 key: "select",
                 value: function(e) {
                     var t = e.currentTarget.dataset;
                     console.log("-- MOBILE DROPDOWN SELECT", JSON.stringify(t)), this.setState({
                         open: !1,
                         listStyle: this.closeStyle
                     }), this.props.setProps({
-                        value: t.value
+                        value: t.value,
+                        label: t.label
                     })
                 }
             }, {
                 key: "clear",
                 value: function(e) {
                     this.props.setProps({
-                        value: null
+                        value: null,
+                        label: null
                     }), e && e.stopPropagation()
                 }
             }, {
                 key: "close",
                 value: function() {
                     this.setState({
                         open: !1,
@@ -3822,15 +3824,16 @@
                 }
             }, {
                 key: "componentDidUpdate",
                 value: function() {
                     if (JSON.stringify(this.options) !== JSON.stringify(this.props.options)) {
                         var e = this.getOption();
                         this.options = this.props.options, this.props.setProps({
-                            value: e.value
+                            value: e.value,
+                            label: e.label
                         })
                     }
                     this.pos && (this.wrapRef.current.scrollTop = this.pos)
                 }
             }, {
                 key: "componentDidMount",
                 value: function() {
```

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.4.1/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks-dash-components
-Version: 0.4.0
+Version: 0.4.1
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.4.0/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.4.1/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

