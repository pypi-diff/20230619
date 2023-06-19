# Comparing `tmp/thinks_dash_components-0.3.9.tar.gz` & `tmp/thinks_dash_components-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.3.9.tar", last modified: Mon Jun 19 07:35:28 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.4.0.tar", last modified: Mon Jun 19 07:51:16 2023, max compression
```

## Comparing `thinks_dash_components-0.3.9.tar` & `thinks_dash_components-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:35:28.024095 thinks_dash_components-0.3.9/
--rw-rw-rw-   0        0        0        0 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.9/LICENSE
--rw-rw-rw-   0        0        0      453 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-06-19 07:35:28.023094 thinks_dash_components-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     3706 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.9/README.md
--rw-rw-rw-   0        0        0     2309 2023-06-19 07:35:00.000000 thinks_dash_components-0.3.9/package.json
--rw-rw-rw-   0        0        0       42 2023-06-19 07:35:28.025095 thinks_dash_components-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:35:28.014092 thinks_dash_components-0.3.9/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1533 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1304 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.9/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2273 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.9/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44590 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2309 2023-06-19 07:35:19.000000 thinks_dash_components-0.3.9/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   124132 2023-06-19 07:35:18.000000 thinks_dash_components-0.3.9/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-06-19 07:35:18.000000 thinks_dash_components-0.3.9/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-06-19 07:35:28.021092 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-06-19 07:35:27.000000 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-06-19 07:35:27.000000 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:35:27.000000 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-19 07:35:27.000000 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 07:51:16.671806 thinks_dash_components-0.4.0/
+-rw-rw-rw-   0        0        0        0 2023-04-17 07:43:57.000000 thinks_dash_components-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      453 2023-04-17 07:43:57.000000 thinks_dash_components-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-06-19 07:51:16.670805 thinks_dash_components-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3706 2023-04-17 07:43:57.000000 thinks_dash_components-0.4.0/README.md
+-rw-rw-rw-   0        0        0     2309 2023-06-19 07:50:17.000000 thinks_dash_components-0.4.0/package.json
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:51:16.672804 thinks_dash_components-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-17 07:43:58.000000 thinks_dash_components-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:51:16.661801 thinks_dash_components-0.4.0/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1533 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1304 2023-04-17 07:43:58.000000 thinks_dash_components-0.4.0/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2273 2023-04-17 07:43:58.000000 thinks_dash_components-0.4.0/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44590 2023-06-19 07:51:12.000000 thinks_dash_components-0.4.0/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2309 2023-06-19 07:51:11.000000 thinks_dash_components-0.4.0/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   123724 2023-06-19 07:51:10.000000 thinks_dash_components-0.4.0/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-06-19 07:51:10.000000 thinks_dash_components-0.4.0/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-06-19 07:51:16.668802 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-06-19 07:51:16.000000 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-06-19 07:51:16.000000 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:51:16.000000 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-19 07:51:16.000000 thinks_dash_components-0.4.0/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.3.9/PKG-INFO` & `thinks_dash_components-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks_dash_components
-Version: 0.3.9
+Version: 0.4.0
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.9/README.md` & `thinks_dash_components-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/package.json` & `thinks_dash_components-0.4.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.4.0'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.9"
+    "version": "0.4.0"
 }
```

### Comparing `thinks_dash_components-0.3.9/setup.py` & `thinks_dash_components-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/Alert.py` & `thinks_dash_components-0.4.0/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.4.0/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.4.0/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.4.0/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.4.0/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.4.0/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.4.0/thinks_dash_components/MobileDropdown.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/Notice.py` & `thinks_dash_components-0.4.0/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.4.0/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.4.0/thinks_dash_components/Rotate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.4.0/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.4.0/thinks_dash_components/StorageObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.4.0/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.4.0/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/_ComponentTemplate.py` & `thinks_dash_components-0.4.0/thinks_dash_components/_ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/__init__.py` & `thinks_dash_components-0.4.0/thinks_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.4.0/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/metadata.json` & `thinks_dash_components-0.4.0/thinks_dash_components/metadata.json`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/package-info.json` & `thinks_dash_components-0.4.0/thinks_dash_components/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.4.0'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.9"
+    "version": "0.4.0"
 }
```

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.4.0/thinks_dash_components/thinks_dash_components.min.js`

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
-            return a.splice(1, 0, "v0_3_9m1687160116"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_4_0m1687161068"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -123,29 +123,29 @@
         function w(e) {
             return e && "string" == typeof e.styledComponentId
         }
         var S = void 0 !== e && void 0 !== e.env && (e.env.REACT_APP_SC_ATTR || e.env.SC_ATTR) || "data-styled",
             O = "undefined" != typeof window && "HTMLElement" in window,
             E = Boolean("boolean" == typeof SC_DISABLE_SPEEDY ? SC_DISABLE_SPEEDY : void 0 !== e && void 0 !== e.env && (void 0 !== e.env.REACT_APP_SC_DISABLE_SPEEDY && "" !== e.env.REACT_APP_SC_DISABLE_SPEEDY ? "false" !== e.env.REACT_APP_SC_DISABLE_SPEEDY && e.env.REACT_APP_SC_DISABLE_SPEEDY : void 0 !== e.env.SC_DISABLE_SPEEDY && "" !== e.env.SC_DISABLE_SPEEDY && ("false" !== e.env.SC_DISABLE_SPEEDY && e.env.SC_DISABLE_SPEEDY)));
 
-        function P(e) {
+        function x(e) {
             for (var t = arguments.length, r = new Array(t > 1 ? t - 1 : 0), n = 1; n < t; n++) r[n - 1] = arguments[n];
             throw new Error("An error occurred. See https://git.io/JUIaE#" + e + " for more information." + (r.length > 0 ? " Args: " + r.join(", ") : ""))
         }
-        var x = function() {
+        var P = function() {
                 function e(e) {
                     this.groupSizes = new Uint32Array(512), this.length = 512, this.tag = e
                 }
                 var t = e.prototype;
                 return t.indexOfGroup = function(e) {
                     for (var t = 0, r = 0; r < e; r++) t += this.groupSizes[r];
                     return t
                 }, t.insertRules = function(e, t) {
                     if (e >= this.groupSizes.length) {
-                        for (var r = this.groupSizes, n = r.length, o = n; e >= o;)(o <<= 1) < 0 && P(16, "" + e);
+                        for (var r = this.groupSizes, n = r.length, o = n; e >= o;)(o <<= 1) < 0 && x(16, "" + e);
                         this.groupSizes = new Uint32Array(o), this.groupSizes.set(r), this.length = o;
                         for (var i = n; i < o; i++) this.groupSizes[i] = 0
                     }
                     for (var a = this.indexOfGroup(e + 1), s = 0, c = t.length; s < c; s++) this.tag.insertRule(a, t[s]) && (this.groupSizes[e]++, a++)
                 }, t.clearGroup = function(e) {
                     if (e < this.length) {
                         var t = this.groupSizes[e],
@@ -217,15 +217,15 @@
                     var t = this.element = M(e);
                     t.appendChild(document.createTextNode("")), this.sheet = function(e) {
                         if (e.sheet) return e.sheet;
                         for (var t = document.styleSheets, r = 0, n = t.length; r < n; r++) {
                             var o = t[r];
                             if (o.ownerNode === e) return o
                         }
-                        P(17)
+                        x(17)
                     }(t), this.length = 0
                 }
                 var t = e.prototype;
                 return t.insertRule = function(e, t) {
                     try {
                         return this.sheet.insertRule(t, e), this.length++, !0
                     } catch (e) {
@@ -271,15 +271,15 @@
                 }, e
             }(),
             F = O,
             U = {
                 isServer: !O,
                 useCSSOMInjection: !E
             },
-            G = function() {
+            X = function() {
                 function e(e, t, r) {
                     void 0 === e && (e = m), void 0 === t && (t = {}), this.options = d({}, U, {}, e), this.gs = t, this.names = new Map(r), this.server = !!e.isServer, !this.server && O && F && (F = !1, function(e) {
                         for (var t = document.querySelectorAll(R), r = 0, n = t.length; r < n; r++) {
                             var o = t[r];
                             o && "active" !== o.getAttribute(S) && (D(e, o), o.parentNode && o.parentNode.removeChild(o))
                         }
                     }(this))
@@ -289,15 +289,15 @@
                 };
                 var t = e.prototype;
                 return t.reconstructWithOptions = function(t, r) {
                     return void 0 === r && (r = !0), new e(d({}, this.options, {}, t), this.gs, r && this.names || void 0)
                 }, t.allocateGSInstance = function(e) {
                     return this.gs[e] = (this.gs[e] || 0) + 1
                 }, t.getTag = function() {
-                    return this.tag || (this.tag = (r = (t = this.options).isServer, n = t.useCSSOMInjection, o = t.target, e = r ? new z(o) : n ? new B(o) : new $(o), new x(e)));
+                    return this.tag || (this.tag = (r = (t = this.options).isServer, n = t.useCSSOMInjection, o = t.target, e = r ? new z(o) : n ? new B(o) : new $(o), new P(e)));
                     var e, t, r, n, o
                 }, t.hasNameForId = function(e, t) {
                     return this.names.has(e) && this.names.get(e).has(t)
                 }, t.registerName = function(e, t) {
                     if (_(e), this.names.has(e)) this.names.get(e).add(t);
                     else {
                         var r = new Set;
@@ -327,23 +327,23 @@
                                 }
                             }
                         }
                         return n
                     }(this)
                 }, e
             }(),
-            W = /(a)(d)/gi,
-            X = function(e) {
+            G = /(a)(d)/gi,
+            W = function(e) {
                 return String.fromCharCode(e + (e > 25 ? 39 : 97))
             };
 
         function H(e) {
             var t, r = "";
-            for (t = Math.abs(e); t > 52; t = t / 52 | 0) r = X(t % 52) + r;
-            return (X(t % 52) + r).replace(W, "$1-$2")
+            for (t = Math.abs(e); t > 52; t = t / 52 | 0) r = W(t % 52) + r;
+            return (W(t % 52) + r).replace(G, "$1-$2")
         }
         var Y = function(e, t) {
                 for (var r = t.length; r;) e = 33 * e ^ t.charCodeAt(--r);
                 return e
             },
             q = function(e) {
                 return Y(5381, e)
@@ -355,15 +355,15 @@
                 if (b(r) && !w(r)) return !1
             }
             return !0
         }
         var K = q("5.3.9"),
             J = function() {
                 function e(e, t, r) {
-                    this.rules = e, this.staticRulesId = "", this.isStatic = (void 0 === r || r.isStatic) && V(e), this.componentId = t, this.baseHash = Y(K, t), this.baseStyle = r, G.registerId(t)
+                    this.rules = e, this.staticRulesId = "", this.isStatic = (void 0 === r || r.isStatic) && V(e), this.componentId = t, this.baseHash = Y(K, t), this.baseStyle = r, X.registerId(t)
                 }
                 return e.prototype.generateAndInjectStyles = function(e, t, r) {
                     var n = this.componentId,
                         o = [];
                     if (this.baseStyle && o.push(this.baseStyle.generateAndInjectStyles(e, t, r)), this.isStatic && !r.hash)
                         if (this.staticRulesId && t.hasNameForId(n, this.staticRulesId)) o.push(this.staticRulesId);
                         else {
@@ -451,20 +451,20 @@
                 2 === e && o.length && o[0].lastIndexOf(r) > 0 && (o[0] = o[0].replace(n, h))
             }, d, function(e) {
                 if (-2 === e) {
                     var t = p;
                     return p = [], t
                 }
             }])), y.hash = l.length ? l.reduce((function(e, t) {
-                return t.name || P(15), Y(e, t.name)
+                return t.name || x(15), Y(e, t.name)
             }), 5381).toString() : "", y
         }
         var te = i.a.createContext(),
             re = (te.Consumer, i.a.createContext()),
-            ne = (re.Consumer, new G),
+            ne = (re.Consumer, new X),
             oe = ee();
 
         function ie() {
             return Object(o.useContext)(te) || ne
         }
 
         function ae() {
@@ -504,15 +504,15 @@
                 function e(e, t) {
                     var r = this;
                     this.inject = function(e, t) {
                         void 0 === t && (t = oe);
                         var n = r.name + t.hash;
                         e.hasNameForId(r.id, n) || e.insertRules(r.id, n, t(r.rules, n, "@keyframes"))
                     }, this.toString = function() {
-                        return P(12, String(r.name))
+                        return x(12, String(r.name))
                     }, this.name = e, this.id = "sc-keyframes-" + e, this.rules = t
                 }
                 return e.prototype.getName = function(e) {
                     return void 0 === e && (e = oe), this.name + e.hash
                 }, e
             }(),
             ue = /([A-Z])/,
@@ -562,32 +562,32 @@
         var Oe = function(e) {
             return H(q(e) >>> 0)
         };
 
         function Ee(e) {
             return "string" == typeof e && !0
         }
-        var Pe = function(e) {
+        var xe = function(e) {
                 return "function" == typeof e || "object" == typeof e && null !== e && !Array.isArray(e)
             },
-            xe = function(e) {
+            Pe = function(e) {
                 return "__proto__" !== e && "constructor" !== e && "prototype" !== e
             };
 
         function ke(e, t, r) {
             var n = e[r];
-            Pe(t) && Pe(n) ? je(n, t) : e[r] = t
+            xe(t) && xe(n) ? je(n, t) : e[r] = t
         }
 
         function je(e) {
             for (var t = arguments.length, r = new Array(t > 1 ? t - 1 : 0), n = 1; n < t; n++) r[n - 1] = arguments[n];
             for (var o = 0, i = r; o < i.length; o++) {
                 var a = i[o];
-                if (Pe(a))
-                    for (var s in a) xe(s) && ke(e, a[s], s)
+                if (xe(a))
+                    for (var s in a) Pe(s) && ke(e, a[s], s)
             }
             return e
         }
         var Te = i.a.createContext();
         Te.Consumer;
         var _e = {};
 
@@ -609,16 +609,16 @@
                 }(e) : h,
                 S = t.displayName && t.componentId ? Se(t.displayName) + "-" + t.componentId : t.componentId || f,
                 O = n && e.attrs ? Array.prototype.concat(e.attrs, c).filter(Boolean) : c,
                 E = t.shouldForwardProp;
             n && e.shouldForwardProp && (E = t.shouldForwardProp ? function(r, n, o) {
                 return e.shouldForwardProp(r, n, o) && t.shouldForwardProp(r, n, o)
             } : e.shouldForwardProp);
-            var P, x = new J(r, S, n ? e.componentStyle : void 0),
-                k = x.isStatic && 0 === c.length,
+            var x, P = new J(r, S, n ? e.componentStyle : void 0),
+                k = P.isStatic && 0 === c.length,
                 j = function(e, t) {
                     return function(e, t, r, n) {
                         var i = e.attrs,
                             a = e.componentStyle,
                             s = e.defaultProps,
                             c = e.foldedComponentIds,
                             u = e.shouldForwardProp,
@@ -642,58 +642,58 @@
                                     i = ae();
                                 return t ? e.generateAndInjectStyles(m, o, i) : e.generateAndInjectStyles(r, o, i)
                             }(a, n, y),
                             w = r,
                             S = v.$as || t.$as || v.as || t.as || p,
                             O = Ee(S),
                             E = v !== t ? d({}, t, {}, v) : t,
-                            P = {};
-                        for (var x in E) "$" !== x[0] && "as" !== x && ("forwardedAs" === x ? P.as = E[x] : (u ? u(x, l.a, S) : !O || Object(l.a)(x)) && (P[x] = E[x]));
-                        return t.style && v.style !== t.style && (P.style = d({}, t.style, {}, v.style)), P.className = Array.prototype.concat(c, f, g !== f ? g : null, t.className, v.className).filter(Boolean).join(" "), P.ref = w, Object(o.createElement)(S, P)
-                    }(P, e, t, k)
+                            x = {};
+                        for (var P in E) "$" !== P[0] && "as" !== P && ("forwardedAs" === P ? x.as = E[P] : (u ? u(P, l.a, S) : !O || Object(l.a)(P)) && (x[P] = E[P]));
+                        return t.style && v.style !== t.style && (x.style = d({}, t.style, {}, v.style)), x.className = Array.prototype.concat(c, f, g !== f ? g : null, t.className, v.className).filter(Boolean).join(" "), x.ref = w, Object(o.createElement)(S, x)
+                    }(x, e, t, k)
                 };
-            return j.displayName = y, (P = i.a.forwardRef(j)).attrs = O, P.componentStyle = x, P.displayName = y, P.shouldForwardProp = E, P.foldedComponentIds = n ? Array.prototype.concat(e.foldedComponentIds, e.styledComponentId) : v, P.styledComponentId = S, P.target = n ? e.target : e, P.withComponent = function(e) {
+            return j.displayName = y, (x = i.a.forwardRef(j)).attrs = O, x.componentStyle = P, x.displayName = y, x.shouldForwardProp = E, x.foldedComponentIds = n ? Array.prototype.concat(e.foldedComponentIds, e.styledComponentId) : v, x.styledComponentId = S, x.target = n ? e.target : e, x.withComponent = function(e) {
                 var n = t.componentId,
                     o = function(e, t) {
                         if (null == e) return {};
                         var r, n, o = {},
                             i = Object.keys(e);
                         for (n = 0; n < i.length; n++) r = i[n], t.indexOf(r) >= 0 || (o[r] = e[r]);
                         return o
                     }(t, ["componentId"]),
                     i = n && n + "-" + (Ee(e) ? e : Se(g(e)));
                 return Ce(e, d({}, o, {
                     attrs: O,
                     componentId: i
                 }), r)
-            }, Object.defineProperty(P, "defaultProps", {
+            }, Object.defineProperty(x, "defaultProps", {
                 get: function() {
                     return this._foldedDefaultProps
                 },
                 set: function(t) {
                     this._foldedDefaultProps = n ? je({}, e.defaultProps, t) : t
                 }
-            }), Object.defineProperty(P, "toString", {
+            }), Object.defineProperty(x, "toString", {
                 value: function() {
-                    return "." + P.styledComponentId
+                    return "." + x.styledComponentId
                 }
-            }), a && p()(P, e, {
+            }), a && p()(x, e, {
                 attrs: !0,
                 componentStyle: !0,
                 displayName: !0,
                 foldedComponentIds: !0,
                 shouldForwardProp: !0,
                 styledComponentId: !0,
                 target: !0,
                 withComponent: !0
-            }), P
+            }), x
         }
         var Ae = function(e) {
             return function e(t, r, o) {
-                if (void 0 === o && (o = m), !Object(n.isValidElementType)(r)) return P(1, String(r));
+                if (void 0 === o && (o = m), !Object(n.isValidElementType)(r)) return x(1, String(r));
                 var i = function() {
                     return t(r, o, me.apply(void 0, arguments))
                 };
                 return i.withConfig = function(n) {
                     return e(t, r, d({}, o, {}, n))
                 }, i.attrs = function(n) {
                     return e(t, r, d({}, o, {
@@ -703,25 +703,25 @@
             }(Ce, e)
         };
         ["a", "abbr", "address", "area", "article", "aside", "audio", "b", "base", "bdi", "bdo", "big", "blockquote", "body", "br", "button", "canvas", "caption", "cite", "code", "col", "colgroup", "data", "datalist", "dd", "del", "details", "dfn", "dialog", "div", "dl", "dt", "em", "embed", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hgroup", "hr", "html", "i", "iframe", "img", "input", "ins", "kbd", "keygen", "label", "legend", "li", "link", "main", "map", "mark", "marquee", "menu", "menuitem", "meta", "meter", "nav", "noscript", "object", "ol", "optgroup", "option", "output", "p", "param", "picture", "pre", "progress", "q", "rp", "rt", "ruby", "s", "samp", "script", "section", "select", "small", "source", "span", "strong", "style", "sub", "summary", "sup", "table", "tbody", "td", "textarea", "tfoot", "th", "thead", "time", "title", "tr", "track", "u", "ul", "var", "video", "wbr", "circle", "clipPath", "defs", "ellipse", "foreignObject", "g", "image", "line", "linearGradient", "marker", "mask", "path", "pattern", "polygon", "polyline", "radialGradient", "rect", "stop", "svg", "text", "textPath", "tspan"].forEach((function(e) {
             Ae[e] = Ae(e)
         }));
         ! function() {
             function e(e, t) {
-                this.rules = e, this.componentId = t, this.isStatic = V(e), G.registerId(this.componentId + 1)
+                this.rules = e, this.componentId = t, this.isStatic = V(e), X.registerId(this.componentId + 1)
             }
             var t = e.prototype;
             t.createStyles = function(e, t, r, n) {
                 var o = n(ye(this.rules, t, r, n).join(""), ""),
                     i = this.componentId + e;
                 r.insertRules(i, i, o)
             }, t.removeStyles = function(e, t) {
                 t.clearRules(this.componentId + e)
             }, t.renderStyles = function(e, t, r, n) {
-                e > 2 && G.registerId(this.componentId + e), this.removeStyles(e, r), this.createStyles(e, t, r, n)
+                e > 2 && X.registerId(this.componentId + e), this.removeStyles(e, r), this.createStyles(e, t, r, n)
             }
         }();
 
         function Re(e) {
             for (var t = arguments.length, r = new Array(t > 1 ? t - 1 : 0), n = 1; n < t; n++) r[n - 1] = arguments[n];
             var o = me.apply(void 0, [e].concat(r)).join(""),
                 i = Oe(o);
@@ -731,38 +731,38 @@
                 var e = this;
                 this._emitSheetCSS = function() {
                     var t = e.instance.toString();
                     if (!t) return "";
                     var r = N();
                     return "<style " + [r && 'nonce="' + r + '"', S + '="true"', 'data-styled-version="5.3.9"'].filter(Boolean).join(" ") + ">" + t + "</style>"
                 }, this.getStyleTags = function() {
-                    return e.sealed ? P(2) : e._emitSheetCSS()
+                    return e.sealed ? x(2) : e._emitSheetCSS()
                 }, this.getStyleElement = function() {
                     var t;
-                    if (e.sealed) return P(2);
+                    if (e.sealed) return x(2);
                     var r = ((t = {})[S] = "", t["data-styled-version"] = "5.3.9", t.dangerouslySetInnerHTML = {
                             __html: e.instance.toString()
                         }, t),
                         n = N();
                     return n && (r.nonce = n), [i.a.createElement("style", d({}, r, {
                         key: "sc-0-0"
                     }))]
                 }, this.seal = function() {
                     e.sealed = !0
-                }, this.instance = new G({
+                }, this.instance = new X({
                     isServer: !0
                 }), this.sealed = !1
             }
             var t = e.prototype;
             t.collectStyles = function(e) {
-                return this.sealed ? P(2) : i.a.createElement(se, {
+                return this.sealed ? x(2) : i.a.createElement(se, {
                     sheet: this.instance
                 }, e)
             }, t.interleaveWithNodeStream = function(e) {
-                return P(3)
+                return x(3)
             }
         }();
         t.a = Ae
     }).call(this, r(9))
 }, function(e, t, r) {
     "use strict";
     e.exports = r(10)
@@ -926,15 +926,15 @@
                 case 978:
                     return "-webkit-" + a + "-moz-" + a + a;
                 case 1019:
                 case 983:
                     return "-webkit-" + a + "-moz-" + a + "-ms-" + a + a;
                 case 883:
                     if (45 === a.charCodeAt(8)) return "-webkit-" + a + a;
-                    if (0 < a.indexOf("image-set(", 11)) return a.replace(x, "$1-webkit-$2") + a;
+                    if (0 < a.indexOf("image-set(", 11)) return a.replace(P, "$1-webkit-$2") + a;
                     break;
                 case 932:
                     if (45 === a.charCodeAt(4)) switch (a.charCodeAt(5)) {
                         case 103:
                             return "-webkit-box-" + a.replace("-grow", "") + "-webkit-" + a + "-ms-" + a.replace("grow", "positive") + a;
                         case 115:
                             return "-webkit-" + a + "-ms-" + a.replace("shrink", "negative") + a;
@@ -989,15 +989,15 @@
                     }
                     break;
                 case 973:
                 case 989:
                     if (45 !== a.charCodeAt(3) || 122 === a.charCodeAt(4)) break;
                 case 931:
                 case 953:
-                    if (!0 === P.test(e)) return 115 === (c = e.substring(e.indexOf(":") + 1)).charCodeAt(0) ? n(e.replace("stretch", "fill-available"), t, r, i).replace(":fill-available", ":stretch") : a.replace(c, "-webkit-" + c) + a.replace(c, "-moz-" + c.replace("fill-", "")) + a;
+                    if (!0 === x.test(e)) return 115 === (c = e.substring(e.indexOf(":") + 1)).charCodeAt(0) ? n(e.replace("stretch", "fill-available"), t, r, i).replace(":fill-available", ":stretch") : a.replace(c, "-webkit-" + c) + a.replace(c, "-moz-" + c.replace("fill-", "")) + a;
                     break;
                 case 962:
                     if (a = "-webkit-" + a + (102 === a.charCodeAt(5) ? "-ms-" + a : "") + a, 211 === r + i && 105 === a.charCodeAt(13) && 0 < a.indexOf("transform", 10)) return a.substring(0, a.indexOf(";", 27) + 1).replace(d, "$1-webkit-$2") + a
             }
             return a
         }
 
@@ -1032,16 +1032,16 @@
         function c(e, r) {
             var s = e;
             if (33 > s.charCodeAt(0) && (s = s.trim()), s = [s], 0 < R) {
                 var c = a(-1, r, s, s, j, k, 0, 0, 0, 0);
                 void 0 !== c && "string" == typeof c && (r = c)
             }
             var f = function e(r, s, c, f, p) {
-                for (var d, h, y, g, S, O = 0, E = 0, P = 0, x = 0, A = 0, L = 0, D = y = d = 0, N = 0, M = 0, B = 0, $ = 0, z = c.length, F = z - 1, U = "", G = "", W = "", X = ""; N < z;) {
-                    if (h = c.charCodeAt(N), N === F && 0 !== E + x + P + O && (0 !== E && (h = 47 === E ? 10 : 47), x = P = O = 0, z++, F++), 0 === E + x + P + O) {
+                for (var d, h, y, g, S, O = 0, E = 0, x = 0, P = 0, A = 0, L = 0, D = y = d = 0, N = 0, M = 0, B = 0, $ = 0, z = c.length, F = z - 1, U = "", X = "", G = "", W = ""; N < z;) {
+                    if (h = c.charCodeAt(N), N === F && 0 !== E + P + x + O && (0 !== E && (h = 47 === E ? 10 : 47), P = x = O = 0, z++, F++), 0 === E + P + x + O) {
                         if (N === F && (0 < M && (U = U.replace(l, "")), 0 < U.trim().length)) {
                             switch (h) {
                                 case 32:
                                 case 9:
                                 case 59:
                                 case 13:
                                 case 10:
@@ -1114,54 +1114,54 @@
                                             case 45:
                                                 y = U + "{" + y + "}";
                                                 break;
                                             case 107:
                                                 y = (U = U.replace(v, "$1 $2")) + "{" + y + "}", y = 1 === _ || 2 === _ && o("@" + y, 3) ? "@-webkit-" + y + "@" + y : "@" + y;
                                                 break;
                                             default:
-                                                y = U + y, 112 === f && (G += y, y = "")
+                                                y = U + y, 112 === f && (X += y, y = "")
                                         } else y = "";
                                         break;
                                     default:
                                         y = e(s, t(s, U, B), y, f, p + 1)
                                 }
-                                W += y, y = B = M = D = d = 0, U = "", h = c.charCodeAt(++N);
+                                G += y, y = B = M = D = d = 0, U = "", h = c.charCodeAt(++N);
                                 break;
                             case 125:
                             case 59:
-                                if (1 < ($ = (U = (0 < M ? U.replace(l, "") : U).trim()).length)) switch (0 === D && (d = U.charCodeAt(0), 45 === d || 96 < d && 123 > d) && ($ = (U = U.replace(" ", ":")).length), 0 < R && void 0 !== (S = a(1, U, s, r, j, k, G.length, f, p, f)) && 0 === ($ = (U = S.trim()).length) && (U = "\0\0"), d = U.charCodeAt(0), h = U.charCodeAt(1), d) {
+                                if (1 < ($ = (U = (0 < M ? U.replace(l, "") : U).trim()).length)) switch (0 === D && (d = U.charCodeAt(0), 45 === d || 96 < d && 123 > d) && ($ = (U = U.replace(" ", ":")).length), 0 < R && void 0 !== (S = a(1, U, s, r, j, k, X.length, f, p, f)) && 0 === ($ = (U = S.trim()).length) && (U = "\0\0"), d = U.charCodeAt(0), h = U.charCodeAt(1), d) {
                                     case 0:
                                         break;
                                     case 64:
                                         if (105 === h || 99 === h) {
-                                            X += U + c.charAt(N);
+                                            W += U + c.charAt(N);
                                             break
                                         }
                                     default:
-                                        58 !== U.charCodeAt($ - 1) && (G += n(U, d, h, U.charCodeAt(2)))
+                                        58 !== U.charCodeAt($ - 1) && (X += n(U, d, h, U.charCodeAt(2)))
                                 }
                                 B = M = D = d = 0, U = "", h = c.charCodeAt(++N)
                         }
                     }
                     switch (h) {
                         case 13:
                         case 10:
-                            47 === E ? E = 0 : 0 === 1 + d && 107 !== f && 0 < U.length && (M = 1, U += "\0"), 0 < R * I && a(0, U, s, r, j, k, G.length, f, p, f), k = 1, j++;
+                            47 === E ? E = 0 : 0 === 1 + d && 107 !== f && 0 < U.length && (M = 1, U += "\0"), 0 < R * I && a(0, U, s, r, j, k, X.length, f, p, f), k = 1, j++;
                             break;
                         case 59:
                         case 125:
-                            if (0 === E + x + P + O) {
+                            if (0 === E + P + x + O) {
                                 k++;
                                 break
                             }
                         default:
                             switch (k++, g = c.charAt(N), h) {
                                 case 9:
                                 case 32:
-                                    if (0 === x + O + E) switch (A) {
+                                    if (0 === P + O + E) switch (A) {
                                         case 44:
                                         case 58:
                                         case 9:
                                         case 32:
                                             g = "";
                                             break;
                                         default:
@@ -1174,91 +1174,91 @@
                                 case 12:
                                     g = "\\f";
                                     break;
                                 case 11:
                                     g = "\\v";
                                     break;
                                 case 38:
-                                    0 === x + E + O && (M = B = 1, g = "\f" + g);
+                                    0 === P + E + O && (M = B = 1, g = "\f" + g);
                                     break;
                                 case 108:
-                                    if (0 === x + E + O + T && 0 < D) switch (N - D) {
+                                    if (0 === P + E + O + T && 0 < D) switch (N - D) {
                                         case 2:
                                             112 === A && 58 === c.charCodeAt(N - 3) && (T = A);
                                         case 8:
                                             111 === L && (T = L)
                                     }
                                     break;
                                 case 58:
-                                    0 === x + E + O && (D = N);
+                                    0 === P + E + O && (D = N);
                                     break;
                                 case 44:
-                                    0 === E + P + x + O && (M = 1, g += "\r");
+                                    0 === E + x + P + O && (M = 1, g += "\r");
                                     break;
                                 case 34:
                                 case 39:
-                                    0 === E && (x = x === h ? 0 : 0 === x ? h : x);
+                                    0 === E && (P = P === h ? 0 : 0 === P ? h : P);
                                     break;
                                 case 91:
-                                    0 === x + E + P && O++;
+                                    0 === P + E + x && O++;
                                     break;
                                 case 93:
-                                    0 === x + E + P && O--;
+                                    0 === P + E + x && O--;
                                     break;
                                 case 41:
-                                    0 === x + E + O && P--;
+                                    0 === P + E + O && x--;
                                     break;
                                 case 40:
-                                    if (0 === x + E + O) {
+                                    if (0 === P + E + O) {
                                         if (0 === d) switch (2 * A + 3 * L) {
                                             case 533:
                                                 break;
                                             default:
                                                 d = 1
                                         }
-                                        P++
+                                        x++
                                     }
                                     break;
                                 case 64:
-                                    0 === E + P + x + O + D + y && (y = 1);
+                                    0 === E + x + P + O + D + y && (y = 1);
                                     break;
                                 case 42:
                                 case 47:
-                                    if (!(0 < x + O + P)) switch (E) {
+                                    if (!(0 < P + O + x)) switch (E) {
                                         case 0:
                                             switch (2 * h + 3 * c.charCodeAt(N + 1)) {
                                                 case 235:
                                                     E = 47;
                                                     break;
                                                 case 220:
                                                     $ = N, E = 42
                                             }
                                             break;
                                         case 42:
-                                            47 === h && 42 === A && $ + 2 !== N && (33 === c.charCodeAt($ + 2) && (G += c.substring($, N + 1)), g = "", E = 0)
+                                            47 === h && 42 === A && $ + 2 !== N && (33 === c.charCodeAt($ + 2) && (X += c.substring($, N + 1)), g = "", E = 0)
                                     }
                             }
                             0 === E && (U += g)
                     }
                     L = A, A = h, N++
                 }
-                if (0 < ($ = G.length)) {
-                    if (M = s, 0 < R && (void 0 !== (S = a(2, G, M, r, j, k, $, f, p, f)) && 0 === (G = S).length)) return X + G + W;
-                    if (G = M.join(",") + "{" + G + "}", 0 != _ * T) {
-                        switch (2 !== _ || o(G, 2) || (T = 0), T) {
+                if (0 < ($ = X.length)) {
+                    if (M = s, 0 < R && (void 0 !== (S = a(2, X, M, r, j, k, $, f, p, f)) && 0 === (X = S).length)) return W + X + G;
+                    if (X = M.join(",") + "{" + X + "}", 0 != _ * T) {
+                        switch (2 !== _ || o(X, 2) || (T = 0), T) {
                             case 111:
-                                G = G.replace(b, ":-moz-$1") + G;
+                                X = X.replace(b, ":-moz-$1") + X;
                                 break;
                             case 112:
-                                G = G.replace(m, "::-webkit-input-$1") + G.replace(m, "::-moz-$1") + G.replace(m, ":-ms-input-$1") + G
+                                X = X.replace(m, "::-webkit-input-$1") + X.replace(m, "::-moz-$1") + X.replace(m, ":-ms-input-$1") + X
                         }
                         T = 0
                     }
                 }
-                return X + G + W
+                return W + X + G
             }(C, s, r, 0, 0);
             return 0 < R && (void 0 !== (c = a(-2, f, s, s, j, k, f.length, 0, 0, 0)) && (f = c)), "", T = 0, k = j = 1, f
         }
         var u = /^\0+/g,
             l = /[\0\r\f]/g,
             f = /: */g,
             p = /zoo|gra/,
@@ -1269,16 +1269,16 @@
             m = /::(place)/g,
             b = /:(read-only)/g,
             g = /[svh]\w+-[tblr]{2}/,
             w = /\(\s*(.*)\s*\)/g,
             S = /([\s\S]*?);/g,
             O = /-self|flex-/g,
             E = /[^]*?(:[rp][el]a[\w-]+)[^]*/,
-            P = /stretch|:\s*\w+\-(?:conte|avail)/,
-            x = /([^-])(image-set\()/,
+            x = /stretch|:\s*\w+\-(?:conte|avail)/,
+            P = /([^-])(image-set\()/,
             k = 1,
             j = 1,
             T = 0,
             _ = 1,
             C = [],
             A = [],
             R = 0,
@@ -1736,38 +1736,38 @@
 
     function E(e) {
         return (E = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
 
-    function P(e, t) {
+    function x(e, t) {
         return t || (t = e.slice(0)), Object.freeze(Object.defineProperties(e, {
             raw: {
                 value: Object.freeze(t)
             }
         }))
     }
-    var x = Object(y.b)(n || (n = P(["\n  from{\n    opacity: 0;\n  }\n  to {\n    opacity: 1;\n  }\n"]))),
-        k = Object(y.b)(o || (o = P(["\n  from{\n    opacity: 1;\n  }\n  to {\n    opacity: 0;\n  }\n"]))),
+    var P = Object(y.b)(n || (n = x(["\n  from{\n    opacity: 0;\n  }\n  to {\n    opacity: 1;\n  }\n"]))),
+        k = Object(y.b)(o || (o = x(["\n  from{\n    opacity: 1;\n  }\n  to {\n    opacity: 0;\n  }\n"]))),
         j = y.a.div.attrs((function(e) {
             return {
                 duration: e.duration,
                 isFadeout: e.isFadeout
             }
-        }))(i || (i = P(["\n    position: fixed;\n    top: 0;\n    left: 0;\n    display: flex;\n    align-items: center;\n    justify-content: center;\n    width: 100%;\n    height: 100%;\n    background-color: ", ";\n    padding: 50px;\n    box-sizing: border-box;\n    animation: ", " ease-in-out\n        ", "ms forwards;\n"])), "#00000099", (function(e) {
-            return e.isFadeout ? k : x
+        }))(i || (i = x(["\n    position: fixed;\n    top: 0;\n    left: 0;\n    display: flex;\n    align-items: center;\n    justify-content: center;\n    width: 100%;\n    height: 100%;\n    background-color: ", ";\n    padding: 50px;\n    box-sizing: border-box;\n    animation: ", " ease-in-out\n        ", "ms forwards;\n"])), "#00000099", (function(e) {
+            return e.isFadeout ? k : P
         }), (function(e) {
             return e.duration
         })),
-        T = y.a.div(a || (a = P(["\n    padding: 15px 0 20px;\n    background-color: white;\n    border-radius: 10px;\n    display: flex;\n    flex-direction: column;\n    width: 100%;\n"]))),
-        _ = y.a.div(s || (s = P(["\n    border-bottom: solid thin black;\n    padding: 5px 30px;\n"]))),
-        C = y.a.div(c || (c = P(["\n    padding: 10px 30px;\n"]))),
-        A = y.a.div(u || (u = P(["\n    display: flex;\n    justify-content: flex-end;\n    gap: 10px;\n    padding: 0 30px;\n    box-sizing: content-box;\n"]))),
-        R = y.a.button(l || (l = P(["\n    flex: 1;\n    padding: 3px 0;\n    background-color: ", ";\n    border-radius: 9999px;\n    border: solid thin ", ";\n    color: white;\n"])), "#00000099", "#00000099"),
+        T = y.a.div(a || (a = x(["\n    padding: 15px 0 20px;\n    background-color: white;\n    border-radius: 10px;\n    display: flex;\n    flex-direction: column;\n    width: 100%;\n"]))),
+        _ = y.a.div(s || (s = x(["\n    border-bottom: solid thin black;\n    padding: 5px 30px;\n"]))),
+        C = y.a.div(c || (c = x(["\n    padding: 10px 30px;\n"]))),
+        A = y.a.div(u || (u = x(["\n    display: flex;\n    justify-content: flex-end;\n    gap: 10px;\n    padding: 0 30px;\n    box-sizing: content-box;\n"]))),
+        R = y.a.button(l || (l = x(["\n    flex: 1;\n    padding: 3px 0;\n    background-color: ", ";\n    border-radius: 9999px;\n    border: solid thin ", ";\n    color: white;\n"])), "#00000099", "#00000099"),
         L = function(e) {
             ! function(e, t) {
                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                 e.prototype = Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
@@ -2131,32 +2131,32 @@
                 }, c)
             }
         }]) && M(t.prototype, r), n && M(t, n), Object.defineProperty(t, "prototype", {
             writable: !1
         }), i
     }(d.Component);
 
-    function G(e) {
-        return (G = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function X(e) {
+        return (X = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function W(e, t) {
+    function G(e, t) {
         var r = "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
         if (!r) {
             if (Array.isArray(e) || (r = function(e, t) {
                     if (!e) return;
-                    if ("string" == typeof e) return X(e, t);
+                    if ("string" == typeof e) return W(e, t);
                     var r = Object.prototype.toString.call(e).slice(8, -1);
                     "Object" === r && e.constructor && (r = e.constructor.name);
                     if ("Map" === r || "Set" === r) return Array.from(e);
-                    if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return X(e, t)
+                    if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return W(e, t)
                 }(e)) || t && e && "number" == typeof e.length) {
                 r && (e = r);
                 var n = 0,
                     o = function() {};
                 return {
                     s: o,
                     n: function() {
@@ -2194,15 +2194,15 @@
                 } finally {
                     if (s) throw i
                 }
             }
         }
     }
 
-    function X(e, t) {
+    function W(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var r = 0, n = new Array(t); r < t; r++) n[r] = e[r];
         return n
     }
 
     function H() {
         H = function() {
@@ -2234,15 +2234,15 @@
                 return e[t] = r
             }
         }
 
         function u(e, t, r, o) {
             var i = t && t.prototype instanceof p ? t : p,
                 a = Object.create(i.prototype),
-                s = new x(o || []);
+                s = new P(o || []);
             return n(a, "_invoke", {
                 value: S(e, r, s)
             }), a
         }
 
         function l(e, t, r) {
             try {
@@ -2289,15 +2289,15 @@
                     function a() {
                         return new t((function(o, a) {
                             ! function n(o, i, a, s) {
                                 var c = l(e[o], e, i);
                                 if ("throw" !== c.type) {
                                     var u = c.arg,
                                         f = u.value;
-                                    return f && "object" == G(f) && r.call(f, "__await") ? t.resolve(f.__await).then((function(e) {
+                                    return f && "object" == X(f) && r.call(f, "__await") ? t.resolve(f.__await).then((function(e) {
                                         n("next", e, a, s)
                                     }), (function(e) {
                                         n("throw", e, a, s)
                                     })) : t.resolve(f).then((function(e) {
                                         u.value = e, a(u)
                                     }), (function(e) {
                                         return n("throw", e, a, s)
@@ -2361,20 +2361,20 @@
         function E(e) {
             var t = {
                 tryLoc: e[0]
             };
             1 in e && (t.catchLoc = e[1]), 2 in e && (t.finallyLoc = e[2], t.afterLoc = e[3]), this.tryEntries.push(t)
         }
 
-        function P(e) {
+        function x(e) {
             var t = e.completion || {};
             t.type = "normal", delete t.arg, e.completion = t
         }
 
-        function x(e) {
+        function P(e) {
             this.tryEntries = [{
                 tryLoc: "root"
             }], e.forEach(E, this), this.reset(!0)
         }
 
         function k(e) {
             if (e) {
@@ -2437,18 +2437,18 @@
                 function e() {
                     for (; r.length;) {
                         var n = r.pop();
                         if (n in t) return e.value = n, e.done = !1, e
                     }
                     return e.done = !0, e
                 }
-        }, e.values = k, x.prototype = {
-            constructor: x,
+        }, e.values = k, P.prototype = {
+            constructor: P,
             reset: function(e) {
-                if (this.prev = 0, this.next = 0, this.sent = this._sent = void 0, this.done = !1, this.delegate = null, this.method = "next", this.arg = void 0, this.tryEntries.forEach(P), !e)
+                if (this.prev = 0, this.next = 0, this.sent = this._sent = void 0, this.done = !1, this.delegate = null, this.method = "next", this.arg = void 0, this.tryEntries.forEach(x), !e)
                     for (var t in this) "t" === t.charAt(0) && r.call(this, t) && !isNaN(+t.slice(1)) && (this[t] = void 0)
             },
             stop: function() {
                 this.done = !0;
                 var e = this.tryEntries[0].completion;
                 if ("throw" === e.type) throw e.arg;
                 return this.rval
@@ -2494,25 +2494,25 @@
             complete: function(e, t) {
                 if ("throw" === e.type) throw e.arg;
                 return "break" === e.type || "continue" === e.type ? this.next = e.arg : "return" === e.type ? (this.rval = this.arg = e.arg, this.method = "return", this.next = "end") : "normal" === e.type && t && (this.next = t), f
             },
             finish: function(e) {
                 for (var t = this.tryEntries.length - 1; t >= 0; --t) {
                     var r = this.tryEntries[t];
-                    if (r.finallyLoc === e) return this.complete(r.completion, r.afterLoc), P(r), f
+                    if (r.finallyLoc === e) return this.complete(r.completion, r.afterLoc), x(r), f
                 }
             },
             catch: function(e) {
                 for (var t = this.tryEntries.length - 1; t >= 0; --t) {
                     var r = this.tryEntries[t];
                     if (r.tryLoc === e) {
                         var n = r.completion;
                         if ("throw" === n.type) {
                             var o = n.arg;
-                            P(r)
+                            x(r)
                         }
                         return o
                     }
                 }
                 throw new Error("illegal catch attempt")
             },
             delegateYield: function(e, t, r) {
@@ -2585,15 +2585,15 @@
                 r = Reflect.construct(n, arguments, o)
             } else r = n.apply(this, arguments);
             return Z(this, r)
         }
     }
 
     function Z(e, t) {
-        if (t && ("object" === G(t) || "function" == typeof t)) return t;
+        if (t && ("object" === X(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return Q(e)
     }
 
     function Q(e) {
         if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return e
@@ -2612,24 +2612,24 @@
             configurable: !0,
             writable: !0
         }) : e[t] = r, e
     }
 
     function re(e) {
         var t = function(e, t) {
-            if ("object" !== G(e) || null === e) return e;
+            if ("object" !== X(e) || null === e) return e;
             var r = e[Symbol.toPrimitive];
             if (void 0 !== r) {
                 var n = r.call(e, t || "default");
-                if ("object" !== G(n)) return n;
+                if ("object" !== X(n)) return n;
                 throw new TypeError("@@toPrimitive must return a primitive value.")
             }
             return ("string" === t ? String : Number)(e)
         }(e, "string");
-        return "symbol" === G(t) ? t : String(t)
+        return "symbol" === X(t) ? t : String(t)
     }
     U.defaultProps = {
         readonly: !1,
         n_clicks: 0
     }, U.propTypes = {
         id: p.a.string,
         options: p.a.array.isRequired,
@@ -2895,15 +2895,15 @@
                     n = e.source.keyPath;
                 e.onerror = function(e) {
                     var o = e.target.error;
                     if (t && o.code === r.ErrorCode.ABORT_ERROR) {
                         var i;
                         if (Array.isArray(n)) {
                             var a, s = [],
-                                c = W(n);
+                                c = G(n);
                             try {
                                 for (c.s(); !(a = c.n()).done;) {
                                     var u = a.value;
                                     s.push("".concat(u, ": ").concat(t[u]))
                                 }
                             } catch (o) {
                                 c.e(o)
@@ -2983,27 +2983,27 @@
                     }))
                 })).then((function(t) {
                     var r = t.isChange,
                         n = t.createStores,
                         o = t.deleteStores;
                     r && e.open(null, (function(t) {
                         console.log("-- INDEXED DB CREATE STORES", n);
-                        var r, i = W(n);
+                        var r, i = G(n);
                         try {
                             for (i.s(); !(r = i.n()).done;) {
                                 var a = r.value;
                                 t.createObjectStore(a.name, a.option)
                             }
                         } catch (e) {
                             i.e(e)
                         } finally {
                             i.f()
                         }
                         console.log("-- INDEXED DB DELETE STORES", o);
-                        var s, c = W(o);
+                        var s, c = G(o);
                         try {
                             for (c.s(); !(s = c.n()).done;) {
                                 var u = s.value;
                                 t.deleteObjectStore(u)
                             }
                         } catch (e) {
                             c.e(e)
@@ -3295,17 +3295,17 @@
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }();
         return function() {
-            var r, n = Pe(e);
+            var r, n = xe(e);
             if (t) {
-                var o = Pe(this).constructor;
+                var o = xe(this).constructor;
                 r = Reflect.construct(n, arguments, o)
             } else r = n.apply(this, arguments);
             return Ee(this, r)
         }
     }
 
     function Ee(e, t) {
@@ -3313,25 +3313,25 @@
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
-    function Pe(e) {
-        return (Pe = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+    function xe(e) {
+        return (xe = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
     ve.defaultProps = {}, ve.propTypes = {
         id: p.a.string,
         children: p.a.node,
         setProps: p.a.func
     };
-    var xe = function(e) {
+    var Pe = function(e) {
         ! function(e, t) {
             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             e.prototype = Object.create(t && t.prototype, {
                 constructor: {
                     value: e,
                     writable: !0,
                     configurable: !0
@@ -3356,15 +3356,15 @@
                 var e = this;
                 this.mo = new MutationObserver((function(t) {
                     var r, n = be(t);
                     try {
                         for (n.s(); !(r = n.n()).done;) {
                             r.value;
                             var o = e.isLoading();
-                            if (console.log("-- LOADING WRAPPER", "{this.props.id} is loading {isLoading}"), null !== o) {
+                            if (null !== o) {
                                 e.setLoading(o);
                                 break
                             }
                         }
                     } catch (e) {
                         n.e(e)
                     } finally {
@@ -3385,27 +3385,26 @@
         }, {
             key: "isTarget",
             value: function(e) {
                 var t, r = be(e);
                 try {
                     for (r.s(); !(t = r.n()).done;) {
                         var n = t.value;
-                        if (n.tagName && n.className && -1 !== n.className.split(" ").indexOf(this.props.targetClassName)) return console.log("-- LOADING WRAPPER TARGET", this.props.id, n), !0
+                        if (n.tagName && n.className && -1 !== n.className.split(" ").indexOf(this.props.targetClassName)) return !0
                     }
                 } catch (e) {
                     r.e(e)
                 } finally {
                     r.f()
                 }
                 return !1
             }
         }, {
             key: "isLoading",
             value: function() {
-                console.log("-- LOADING WRAPPER IS LOADING", this.props.id, this.ref.current, this.ref);
                 var e = this.ref.current.querySelector(".loading");
                 if (this.props.ignores) {
                     var t, r = be(this.props.ignores);
                     try {
                         for (r.s(); !(t = r.n()).done;) {
                             var n = t.value,
                                 o = this.ref.current.querySelector("[data-loading_ignore=" + n + "] .loading");
@@ -3420,21 +3419,21 @@
                 return e.style.length > 0
             }
         }, {
             key: "setLoading",
             value: function(e) {
                 var t = this,
                     r = this;
-                !this.props.is_stop && e && (console.log("-- LOADING WRAPPER", this.props.id, "loading start"), this.props.setProps({
+                !this.props.is_stop && e && (this.props.setProps({
                     is_loading: !0
                 }), this.setState({
                     isLoading: !0
                 }), this.interval || (this.interval = setInterval((function() {
-                    t.isLoading() || (console.log("-- LOADING WRAPPER", t.props.id, "loading end"), clearInterval(t.interval), t.interval = null, setTimeout((function() {
-                        console.log("-- LOADING WRAPPER", t.props.id, "loading end confirm"), r.props.setProps({
+                    t.isLoading() || (clearInterval(t.interval), t.interval = null, setTimeout((function() {
+                        r.props.setProps({
                             is_loading: !1
                         }), r.setState({
                             isLoading: !1
                         })
                     }), r.props.delay))
                 }), this.props.interval)))
             }
@@ -3481,19 +3480,19 @@
                     ref: this.ref
                 }, n)
             }
         }]) && we(t.prototype, r), n && we(t, n), Object.defineProperty(t, "prototype", {
             writable: !1
         }), i
     }(d.Component);
-    xe.defaultProps = {
+    Pe.defaultProps = {
         delay: 500,
         interval: 1e3,
         is_stop: !1
-    }, xe.propTypes = {
+    }, Pe.propTypes = {
         children: p.a.node,
         id: p.a.string,
         className: p.a.string,
         targetClassName: p.a.string.isRequired,
         delay: p.a.number,
         interval: p.a.number,
         ignores: p.a.arrayOf(p.a.string),
@@ -3649,15 +3648,15 @@
 
     function Ue(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var r = 0, n = new Array(t); r < t; r++) n[r] = e[r];
         return n
     }
 
-    function Ge(e, t) {
+    function Xe(e, t) {
         for (var r = 0; r < t.length; r++) {
             var n = t[r];
             n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, (o = n.key, i = void 0, i = function(e, t) {
                 if ("object" !== ze(e) || null === e) return e;
                 var r = e[Symbol.toPrimitive];
                 if (void 0 !== r) {
                     var n = r.call(e, t || "default");
@@ -3666,21 +3665,21 @@
                 }
                 return ("string" === t ? String : Number)(e)
             }(o, "string"), "symbol" === ze(i) ? i : String(i)), n)
         }
         var o, i
     }
 
-    function We(e, t) {
-        return (We = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+    function Ge(e, t) {
+        return (Ge = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
-    function Xe(e) {
+    function We(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
@@ -3735,17 +3734,17 @@
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }), Object.defineProperty(e, "prototype", {
                     writable: !1
-                }), t && We(e, t)
+                }), t && Ge(e, t)
             }(i, e);
-            var t, r, n, o = Xe(i);
+            var t, r, n, o = We(i);
 
             function i(e) {
                 var t;
                 return function(e, t) {
                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                 }(this, i), (t = o.call(this, e)).state = {
                     open: !1,
@@ -3936,15 +3935,15 @@
                         onTouchStart: this.touchStart,
                         onTouchEnd: this.touchEnd
                     }, h.a.createElement(it, {
                         id: this.id + "-list",
                         ref: this.listRef
                     }, c)))
                 }
-            }]) && Ge(t.prototype, r), n && Ge(t, n), Object.defineProperty(t, "prototype", {
+            }]) && Xe(t.prototype, r), n && Xe(t, n), Object.defineProperty(t, "prototype", {
                 writable: !1
             }), i
         }(d.Component);
 
     function pt(e) {
         return Me({
             tag: "svg",
@@ -4107,22 +4106,22 @@
         notfoundMsg: p.a.string,
         clearable: p.a.bool,
         setProps: p.a.func,
         disable: p.a.bool,
         label: p.a.string
     };
     var Et = y.a.div(Ke || (Ke = Ot(["\n    position: fixed;\n    top: 0;\n    left: 0;\n    width: 100%;\n    height: 100%;\n"]))),
-        Pt = y.a.div.attrs((function(e) {
+        xt = y.a.div.attrs((function(e) {
             return {
                 iconColor: e.iconColor
             }
         }))(Je || (Je = Ot(["\n    width: 30px;\n    height: 30px;\n    position: relative;\n\n    svg {\n        width: 100%;\n        height: 100%;\n        color: ", ";\n    }\n"])), (function(e) {
             return e.iconColor
         })),
-        xt = y.a.span.attrs((function(e) {
+        Pt = y.a.span.attrs((function(e) {
             return {
                 color: e.color,
                 badgeColor: e.badgeColor,
                 borderColor: e.borderColor
             }
         }))(Ze || (Ze = Ot(["\n    width: 1.2em;\n    height: 1.2em;\n    align-items: center;\n    justify-content: center;\n    position: absolute;\n    top: 0;\n    right: -0.3em;\n    background-color: ", ";\n    border-radius: 50%;\n    border: solid 2px ", ";\n    color: ", ";\n    font-size: 0.7em;\n    line-height: 1;\n    box-sizing: content-box;\n"])), (function(e) {
             return e.badgeColor
@@ -4352,24 +4351,24 @@
                         f.e(e)
                     } finally {
                         f.f()
                     }
                     return h.a.createElement("div", {
                         id: r,
                         className: "dash-notice"
-                    }, h.a.createElement(Pt, {
+                    }, h.a.createElement(xt, {
                         iconColor: o,
                         className: "dn-icon",
                         onClick: this.open
                     }, h.a.createElement(Et, {
                         className: "dn-bg",
                         style: {
                             display: this.state.isOpen ? "block" : "none"
                         }
-                    }), h.a.createElement(pt, null), h.a.createElement(xt, {
+                    }), h.a.createElement(pt, null), h.a.createElement(Pt, {
                         color: o,
                         badgeColor: a,
                         borderColor: i,
                         style: {
                             display: n.length > 0 ? "flex" : "none"
                         }
                     }, n.length), h.a.createElement(kt, {
@@ -4564,21 +4563,21 @@
                 }
                 return ("string" === t ? String : Number)(e)
             }(o, "string"), "symbol" === Ft(i) ? i : String(i)), n)
         }
         var o, i
     }
 
-    function Gt(e, t) {
-        return (Gt = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+    function Xt(e, t) {
+        return (Xt = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
-    function Wt(e) {
+    function Gt(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
@@ -4587,19 +4586,19 @@
         }();
         return function() {
             var r, n = Ht(e);
             if (t) {
                 var o = Ht(this).constructor;
                 r = Reflect.construct(n, arguments, o)
             } else r = n.apply(this, arguments);
-            return Xt(this, r)
+            return Wt(this, r)
         }
     }
 
-    function Xt(e, t) {
+    function Wt(e, t) {
         if (t && ("object" === Ft(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
@@ -4631,17 +4630,17 @@
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }), Object.defineProperty(e, "prototype", {
                     writable: !1
-                }), t && Gt(e, t)
+                }), t && Xt(e, t)
             }(i, e);
-            var t, r, n, o = Wt(i);
+            var t, r, n, o = Gt(i);
 
             function i(e) {
                 var t;
                 return function(e, t) {
                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                 }(this, i), (t = o.call(this, e)).state = {
                     orientation: t.getOrientation()
@@ -5331,25 +5330,25 @@
         }();
         return function() {
             var r, n = kr(e);
             if (t) {
                 var o = kr(this).constructor;
                 r = Reflect.construct(n, arguments, o)
             } else r = n.apply(this, arguments);
-            return Pr(this, r)
+            return xr(this, r)
         }
     }
 
-    function Pr(e, t) {
+    function xr(e, t) {
         if (t && ("object" === wr(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-        return xr(e)
+        return Pr(e)
     }
 
-    function xr(e) {
+    function Pr(e) {
         if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return e
     }
 
     function kr(e) {
         return (kr = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
@@ -5375,15 +5374,15 @@
         }(i, e);
         var t, r, n, o = Er(i);
 
         function i(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-            }(this, i), (t = o.call(this, e)).change = t.change.bind(xr(t)), t
+            }(this, i), (t = o.call(this, e)).change = t.change.bind(Pr(t)), t
         }
         return t = i, (r = [{
             key: "change",
             value: function(e) {
                 var t = e.target.value;
                 t = (t = t.replace(/[０-９]/g, (function(e) {
                     return String.fromCharCode(e.charCodeAt(0) - 65248)
@@ -5428,15 +5427,15 @@
     })), r.d(t, "IndexedDB", (function() {
         return ie
     })), r.d(t, "InputNumber", (function() {
         return jr
     })), r.d(t, "IosScrollWrapper", (function() {
         return ve
     })), r.d(t, "LoadingWrapper", (function() {
-        return xe
+        return Pe
     })), r.d(t, "MobileDropdown", (function() {
         return ft
     })), r.d(t, "Notice", (function() {
         return At
     })), r.d(t, "Rotate", (function() {
         return Kt
     })), r.d(t, "SelectableBox", (function() {
```

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.4.0/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks-dash-components
-Version: 0.3.9
+Version: 0.4.0
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.9/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.4.0/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

