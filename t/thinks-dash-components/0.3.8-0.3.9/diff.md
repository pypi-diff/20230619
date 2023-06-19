# Comparing `tmp/thinks_dash_components-0.3.8.tar.gz` & `tmp/thinks_dash_components-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.3.8.tar", last modified: Mon Jun 19 07:23:15 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.3.9.tar", last modified: Mon Jun 19 07:35:28 2023, max compression
```

## Comparing `thinks_dash_components-0.3.8.tar` & `thinks_dash_components-0.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:23:15.658413 thinks_dash_components-0.3.8/
--rw-rw-rw-   0        0        0        0 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.8/LICENSE
--rw-rw-rw-   0        0        0      453 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-06-19 07:23:15.657412 thinks_dash_components-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3706 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.8/README.md
--rw-rw-rw-   0        0        0     2309 2023-06-19 07:22:48.000000 thinks_dash_components-0.3.8/package.json
--rw-rw-rw-   0        0        0       42 2023-06-19 07:23:15.658413 thinks_dash_components-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:23:15.650412 thinks_dash_components-0.3.8/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1533 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1304 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.8/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2273 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.8/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44590 2023-06-19 07:23:06.000000 thinks_dash_components-0.3.8/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2309 2023-06-19 07:23:05.000000 thinks_dash_components-0.3.8/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   124286 2023-06-19 07:23:03.000000 thinks_dash_components-0.3.8/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-06-19 07:23:03.000000 thinks_dash_components-0.3.8/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-06-19 07:23:15.656412 thinks_dash_components-0.3.8/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-06-19 07:23:15.000000 thinks_dash_components-0.3.8/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-06-19 07:23:15.000000 thinks_dash_components-0.3.8/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:23:15.000000 thinks_dash_components-0.3.8/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-19 07:23:15.000000 thinks_dash_components-0.3.8/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 07:35:28.024095 thinks_dash_components-0.3.9/
+-rw-rw-rw-   0        0        0        0 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0      453 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-06-19 07:35:28.023094 thinks_dash_components-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3706 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.9/README.md
+-rw-rw-rw-   0        0        0     2309 2023-06-19 07:35:00.000000 thinks_dash_components-0.3.9/package.json
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:35:28.025095 thinks_dash_components-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:35:28.014092 thinks_dash_components-0.3.9/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1533 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1304 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.9/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2273 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.9/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44590 2023-06-19 07:35:20.000000 thinks_dash_components-0.3.9/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2309 2023-06-19 07:35:19.000000 thinks_dash_components-0.3.9/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   124132 2023-06-19 07:35:18.000000 thinks_dash_components-0.3.9/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-06-19 07:35:18.000000 thinks_dash_components-0.3.9/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-06-19 07:35:28.021092 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-06-19 07:35:27.000000 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-06-19 07:35:27.000000 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:35:27.000000 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-19 07:35:27.000000 thinks_dash_components-0.3.9/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.3.8/PKG-INFO` & `thinks_dash_components-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks_dash_components
-Version: 0.3.8
+Version: 0.3.9
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.8/README.md` & `thinks_dash_components-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/package.json` & `thinks_dash_components-0.3.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.3.9'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.8"
+    "version": "0.3.9"
 }
```

### Comparing `thinks_dash_components-0.3.8/setup.py` & `thinks_dash_components-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/Alert.py` & `thinks_dash_components-0.3.9/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.3.9/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.3.9/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.3.9/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.3.9/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.3.9/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.3.9/thinks_dash_components/MobileDropdown.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/Notice.py` & `thinks_dash_components-0.3.9/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.3.9/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.3.9/thinks_dash_components/Rotate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.3.9/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.3.9/thinks_dash_components/StorageObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.3.9/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.3.9/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/_ComponentTemplate.py` & `thinks_dash_components-0.3.9/thinks_dash_components/_ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/__init__.py` & `thinks_dash_components-0.3.9/thinks_dash_components/__init__.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.3.9/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/metadata.json` & `thinks_dash_components-0.3.9/thinks_dash_components/metadata.json`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/package-info.json` & `thinks_dash_components-0.3.9/thinks_dash_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.3.9'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.8"
+    "version": "0.3.9"
 }
```

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.3.9/thinks_dash_components/thinks_dash_components.min.js`

 * *Files 1% similar despite different names*

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
-            return a.splice(1, 0, "v0_3_8m1687159381"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_3_9m1687160116"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -173,27 +173,27 @@
             C = function(e) {
                 return j.get(e)
             },
             A = function(e, t) {
                 t >= T && (T = t + 1), k.set(e, t), j.set(t, e)
             },
             R = "style[" + S + '][data-styled-version="5.3.9"]',
-            I = new RegExp("^" + S + '\\.g(\\d+)\\[id="([\\w\\d-]+)"\\].*?"([^"]*)'),
-            L = function(e, t, r) {
+            L = new RegExp("^" + S + '\\.g(\\d+)\\[id="([\\w\\d-]+)"\\].*?"([^"]*)'),
+            I = function(e, t, r) {
                 for (var n, o = r.split(","), i = 0, a = o.length; i < a; i++)(n = o[i]) && e.registerName(t, n)
             },
             D = function(e, t) {
                 for (var r = (t.textContent || "").split("/*!sc*/\n"), n = [], o = 0, i = r.length; o < i; o++) {
                     var a = r[o].trim();
                     if (a) {
-                        var s = a.match(I);
+                        var s = a.match(L);
                         if (s) {
                             var c = 0 | parseInt(s[1], 10),
                                 u = s[2];
-                            0 !== c && (A(u, c), L(e, u, s[3]), e.getTag().insertRules(c, n)), n.length = 0
+                            0 !== c && (A(u, c), I(e, u, s[3]), e.getTag().insertRules(c, n)), n.length = 0
                         } else n.push(a)
                     }
                 }
             },
             N = function() {
                 return r.nc
             },
@@ -352,18 +352,18 @@
         function V(e) {
             for (var t = 0; t < e.length; t += 1) {
                 var r = e[t];
                 if (b(r) && !w(r)) return !1
             }
             return !0
         }
-        var J = q("5.3.9"),
-            K = function() {
+        var K = q("5.3.9"),
+            J = function() {
                 function e(e, t, r) {
-                    this.rules = e, this.staticRulesId = "", this.isStatic = (void 0 === r || r.isStatic) && V(e), this.componentId = t, this.baseHash = Y(J, t), this.baseStyle = r, G.registerId(t)
+                    this.rules = e, this.staticRulesId = "", this.isStatic = (void 0 === r || r.isStatic) && V(e), this.componentId = t, this.baseHash = Y(K, t), this.baseStyle = r, G.registerId(t)
                 }
                 return e.prototype.generateAndInjectStyles = function(e, t, r) {
                     var n = this.componentId,
                         o = [];
                     if (this.baseStyle && o.push(this.baseStyle.generateAndInjectStyles(e, t, r)), this.isStatic && !r.hash)
                         if (this.staticRulesId && t.hasNameForId(n, this.staticRulesId)) o.push(this.staticRulesId);
                         else {
@@ -609,15 +609,15 @@
                 }(e) : h,
                 S = t.displayName && t.componentId ? Se(t.displayName) + "-" + t.componentId : t.componentId || f,
                 O = n && e.attrs ? Array.prototype.concat(e.attrs, c).filter(Boolean) : c,
                 E = t.shouldForwardProp;
             n && e.shouldForwardProp && (E = t.shouldForwardProp ? function(r, n, o) {
                 return e.shouldForwardProp(r, n, o) && t.shouldForwardProp(r, n, o)
             } : e.shouldForwardProp);
-            var P, x = new K(r, S, n ? e.componentStyle : void 0),
+            var P, x = new J(r, S, n ? e.componentStyle : void 0),
                 k = x.isStatic && 0 === c.length,
                 j = function(e, t) {
                     return function(e, t, r, n) {
                         var i = e.attrs,
                             a = e.componentStyle,
                             s = e.defaultProps,
                             c = e.foldedComponentIds,
@@ -1000,15 +1000,15 @@
             }
             return a
         }
 
         function o(e, t) {
             var r = e.indexOf(1 === t ? ":" : "{"),
                 n = e.substring(0, 3 !== t ? r : 10);
-            return r = e.substring(r + 1, e.length - 1), I(2 !== t ? n : n.replace(E, "$1"), r, t)
+            return r = e.substring(r + 1, e.length - 1), L(2 !== t ? n : n.replace(E, "$1"), r, t)
         }
 
         function i(e, t) {
             var r = n(t, t.charCodeAt(0), t.charCodeAt(1), t.charCodeAt(2));
             return r !== t + ";" ? r.replace(S, " or ($1)").substring(4) : "(" + t + ")"
         }
 
@@ -1022,25 +1022,25 @@
                 default:
                     d = f
             }
             if (d !== t) return d
         }
 
         function s(e) {
-            return void 0 !== (e = e.prefix) && (I = null, e ? "function" != typeof e ? _ = 1 : (_ = 2, I = e) : _ = 0), s
+            return void 0 !== (e = e.prefix) && (L = null, e ? "function" != typeof e ? _ = 1 : (_ = 2, L = e) : _ = 0), s
         }
 
         function c(e, r) {
             var s = e;
             if (33 > s.charCodeAt(0) && (s = s.trim()), s = [s], 0 < R) {
                 var c = a(-1, r, s, s, j, k, 0, 0, 0, 0);
                 void 0 !== c && "string" == typeof c && (r = c)
             }
             var f = function e(r, s, c, f, p) {
-                for (var d, h, y, g, S, O = 0, E = 0, P = 0, x = 0, A = 0, I = 0, D = y = d = 0, N = 0, M = 0, B = 0, $ = 0, z = c.length, F = z - 1, U = "", G = "", W = "", X = ""; N < z;) {
+                for (var d, h, y, g, S, O = 0, E = 0, P = 0, x = 0, A = 0, L = 0, D = y = d = 0, N = 0, M = 0, B = 0, $ = 0, z = c.length, F = z - 1, U = "", G = "", W = "", X = ""; N < z;) {
                     if (h = c.charCodeAt(N), N === F && 0 !== E + x + P + O && (0 !== E && (h = 47 === E ? 10 : 47), x = P = O = 0, z++, F++), 0 === E + x + P + O) {
                         if (N === F && (0 < M && (U = U.replace(l, "")), 0 < U.trim().length)) {
                             switch (h) {
                                 case 32:
                                 case 9:
                                 case 59:
                                 case 13:
@@ -1141,15 +1141,15 @@
                                 }
                                 B = M = D = d = 0, U = "", h = c.charCodeAt(++N)
                         }
                     }
                     switch (h) {
                         case 13:
                         case 10:
-                            47 === E ? E = 0 : 0 === 1 + d && 107 !== f && 0 < U.length && (M = 1, U += "\0"), 0 < R * L && a(0, U, s, r, j, k, G.length, f, p, f), k = 1, j++;
+                            47 === E ? E = 0 : 0 === 1 + d && 107 !== f && 0 < U.length && (M = 1, U += "\0"), 0 < R * I && a(0, U, s, r, j, k, G.length, f, p, f), k = 1, j++;
                             break;
                         case 59:
                         case 125:
                             if (0 === E + x + P + O) {
                                 k++;
                                 break
                             }
@@ -1181,15 +1181,15 @@
                                     0 === x + E + O && (M = B = 1, g = "\f" + g);
                                     break;
                                 case 108:
                                     if (0 === x + E + O + T && 0 < D) switch (N - D) {
                                         case 2:
                                             112 === A && 58 === c.charCodeAt(N - 3) && (T = A);
                                         case 8:
-                                            111 === I && (T = I)
+                                            111 === L && (T = L)
                                     }
                                     break;
                                 case 58:
                                     0 === x + E + O && (D = N);
                                     break;
                                 case 44:
                                     0 === E + P + x + O && (M = 1, g += "\r");
@@ -1205,15 +1205,15 @@
                                     0 === x + E + P && O--;
                                     break;
                                 case 41:
                                     0 === x + E + O && P--;
                                     break;
                                 case 40:
                                     if (0 === x + E + O) {
-                                        if (0 === d) switch (2 * A + 3 * I) {
+                                        if (0 === d) switch (2 * A + 3 * L) {
                                             case 533:
                                                 break;
                                             default:
                                                 d = 1
                                         }
                                         P++
                                     }
@@ -1235,15 +1235,15 @@
                                             break;
                                         case 42:
                                             47 === h && 42 === A && $ + 2 !== N && (33 === c.charCodeAt($ + 2) && (G += c.substring($, N + 1)), g = "", E = 0)
                                     }
                             }
                             0 === E && (U += g)
                     }
-                    I = A, A = h, N++
+                    L = A, A = h, N++
                 }
                 if (0 < ($ = G.length)) {
                     if (M = s, 0 < R && (void 0 !== (S = a(2, G, M, r, j, k, $, f, p, f)) && 0 === (G = S).length)) return X + G + W;
                     if (G = M.join(",") + "{" + G + "}", 0 != _ * T) {
                         switch (2 !== _ || o(G, 2) || (T = 0), T) {
                             case 111:
                                 G = G.replace(b, ":-moz-$1") + G;
@@ -1278,27 +1278,27 @@
             k = 1,
             j = 1,
             T = 0,
             _ = 1,
             C = [],
             A = [],
             R = 0,
-            I = null,
-            L = 0;
+            L = null,
+            I = 0;
         return c.use = function e(t) {
             switch (t) {
                 case void 0:
                 case null:
                     R = A.length = 0;
                     break;
                 default:
                     if ("function" == typeof t) A[R++] = t;
                     else if ("object" == typeof t)
                         for (var r = 0, n = t.length; r < n; ++r) e(t[r]);
-                    else L = 0 | !!t
+                    else I = 0 | !!t
             }
             return e
         }, c.set = s, void 0 !== e && s(e), c
     }
 }, function(e, t, r) {
     "use strict";
     t.a = {
@@ -1760,15 +1760,15 @@
             return e.duration
         })),
         T = y.a.div(a || (a = P(["\n    padding: 15px 0 20px;\n    background-color: white;\n    border-radius: 10px;\n    display: flex;\n    flex-direction: column;\n    width: 100%;\n"]))),
         _ = y.a.div(s || (s = P(["\n    border-bottom: solid thin black;\n    padding: 5px 30px;\n"]))),
         C = y.a.div(c || (c = P(["\n    padding: 10px 30px;\n"]))),
         A = y.a.div(u || (u = P(["\n    display: flex;\n    justify-content: flex-end;\n    gap: 10px;\n    padding: 0 30px;\n    box-sizing: content-box;\n"]))),
         R = y.a.button(l || (l = P(["\n    flex: 1;\n    padding: 3px 0;\n    background-color: ", ";\n    border-radius: 9999px;\n    border: solid thin ", ";\n    color: white;\n"])), "#00000099", "#00000099"),
-        I = function(e) {
+        L = function(e) {
             ! function(e, t) {
                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                 e.prototype = Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
@@ -1885,16 +1885,16 @@
                     }, c)))
                 }
             }]) && g(t.prototype, r), n && g(t, n), Object.defineProperty(t, "prototype", {
                 writable: !1
             }), i
         }(d.Component);
 
-    function L(e) {
-        return (L = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function I(e) {
+        return (I = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function D(e, t) {
@@ -1958,23 +1958,23 @@
         return n
     }
 
     function M(e, t) {
         for (var r = 0; r < t.length; r++) {
             var n = t[r];
             n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, (o = n.key, i = void 0, i = function(e, t) {
-                if ("object" !== L(e) || null === e) return e;
+                if ("object" !== I(e) || null === e) return e;
                 var r = e[Symbol.toPrimitive];
                 if (void 0 !== r) {
                     var n = r.call(e, t || "default");
-                    if ("object" !== L(n)) return n;
+                    if ("object" !== I(n)) return n;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
-            }(o, "string"), "symbol" === L(i) ? i : String(i)), n)
+            }(o, "string"), "symbol" === I(i) ? i : String(i)), n)
         }
         var o, i
     }
 
     function B(e, t) {
         return (B = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
             return e.__proto__ = t, e
@@ -1999,31 +1999,31 @@
                 r = Reflect.construct(n, arguments, o)
             } else r = n.apply(this, arguments);
             return z(this, r)
         }
     }
 
     function z(e, t) {
-        if (t && ("object" === L(t) || "function" == typeof t)) return t;
+        if (t && ("object" === I(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
     function F(e) {
         return (F = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
-    I.defaultProps = {
+    L.defaultProps = {
         is_open: !1,
         duration: 150
-    }, I.propTypes = {
+    }, L.propTypes = {
         id: p.a.string,
         message: p.a.node.isRequired,
         title: p.a.node,
         buttons: p.a.arrayOf(p.a.object).isRequired,
         value: p.a.oneOfType([p.a.string, p.a.number]),
         is_open: p.a.bool,
         duration: p.a.number,
@@ -2557,21 +2557,21 @@
     function V(e, t) {
         for (var r = 0; r < t.length; r++) {
             var n = t[r];
             n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, re(n.key), n)
         }
     }
 
-    function J(e, t) {
-        return (J = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+    function K(e, t) {
+        return (K = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
-    function K(e) {
+    function J(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
@@ -2648,17 +2648,17 @@
                 constructor: {
                     value: e,
                     writable: !0,
                     configurable: !0
                 }
             }), Object.defineProperty(e, "prototype", {
                 writable: !1
-            }), t && J(e, t)
+            }), t && K(e, t)
         }(a, e);
-        var t, r, n, o, i = K(a);
+        var t, r, n, o, i = J(a);
 
         function a(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
             }(this, a), te(Q(t = i.call(this, e)), "Action", {
                 INSERT: "exe_insert",
@@ -3497,22 +3497,22 @@
         delay: p.a.number,
         interval: p.a.number,
         ignores: p.a.arrayOf(p.a.string),
         is_loading: p.a.bool,
         is_stop: p.a.bool,
         setProps: p.a.func
     };
-    var ke, je, Te, _e, Ce, Ae, Re, Ie = {
+    var ke, je, Te, _e, Ce, Ae, Re, Le = {
             color: void 0,
             size: void 0,
             className: void 0,
             style: void 0,
             attr: void 0
         },
-        Le = h.a.createContext && h.a.createContext(Ie),
+        Ie = h.a.createContext && h.a.createContext(Le),
         De = function() {
             return (De = Object.assign || function(e) {
                 for (var t, r = 1, n = arguments.length; r < n; r++)
                     for (var o in t = arguments[r]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
             }).apply(this, arguments)
         },
@@ -3557,17 +3557,17 @@
                     color: e.color || t.color
                 }, t.style), e.style),
                 height: s,
                 width: s,
                 xmlns: "http://www.w3.org/2000/svg"
             }), i && h.a.createElement("title", null, i), e.children)
         };
-        return void 0 !== Le ? h.a.createElement(Le.Consumer, null, (function(e) {
+        return void 0 !== Ie ? h.a.createElement(Ie.Consumer, null, (function(e) {
             return t(e)
-        })) : t(Ie)
+        })) : t(Le)
     }
 
     function $e(e) {
         return Me({
             tag: "svg",
             attr: {
                 viewBox: "0 0 16 16",
@@ -3717,15 +3717,15 @@
     function Ve(e, t) {
         return t || (t = e.slice(0)), Object.freeze(Object.defineProperties(e, {
             raw: {
                 value: Object.freeze(t)
             }
         }))
     }
-    var Je, Ke, Ze, Qe, et, tt, rt, nt, ot = y.a.div(ke || (ke = Ve(["\n    box-sizing: border-box;\n    width: 100%;\n    padding: 0;\n    margin: 0;\n    border: solid thin black;\n    border-top: none;\n    overflow: auto;\n    position: fixed;\n    z-index: 150;\n    /* height: 100px; */\n"]))),
+    var Ke, Je, Ze, Qe, et, tt, rt, nt, ot = y.a.div(ke || (ke = Ve(["\n    box-sizing: border-box;\n    width: 100%;\n    padding: 0;\n    margin: 0;\n    border: solid thin black;\n    border-top: none;\n    overflow: auto;\n    position: fixed;\n    z-index: 150;\n    /* height: 100px; */\n"]))),
         it = y.a.ul(je || (je = Ve(["\n    width: 100%;\n    list-style: none;\n    padding: 0;\n    margin: 0;\n    height: max-content;\n"]))),
         at = y.a.li(Te || (Te = Ve(["\n    box-sizing: border-box;\n    width: 100%;\n    margin: 0;\n    padding: 2px 5px;\n    display: flex;\n    justify-content: flex-start;\n    align-items: center;\n"]))),
         st = y.a.div(_e || (_e = Ve(["\n    box-sizing: border-box;\n    width: 100%;\n    min-height: 2rem;\n    padding: 2px 5px;\n    margin: 0;\n    border: solid thin black;\n    position: relative;\n    display: flex;\n    justify-content: flex-start;\n    align-items: center;\n    z-index: 50;\n"]))),
         ct = y.a.span(Ce || (Ce = Ve(["\n    box-sizing: border-box;\n    width: 100%;\n    padding: 0;\n    margin: 0;\n"]))),
         ut = y.a.span(Ae || (Ae = Ve(["\n    position: absolute;\n    height: 100%;\n    width: 30px;\n    top: 0;\n    right: 0;\n    display: flex;\n    justify-content: center;\n    align-items: center;\n"]))),
         lt = y.a.div(Re || (Re = Ve(["\n    position: fixed;\n    width: 100%;\n    height: 100%;\n    top: 0;\n    left: 0;\n    z-index: 100;\n"]))),
         ft = function(e) {
@@ -3820,15 +3820,15 @@
                         var t = e.getBoundingClientRect().height;
                         e.scrollTop + t > e.scrollHeight - 1 && (e.scrollTop = e.scrollHeight - t - 1)
                     }
                 }
             }, {
                 key: "componentDidUpdate",
                 value: function() {
-                    if (console.log("-- MOBILE DROPDOWN OPTIONS", JSON.stringify(this.options), JSON.stringify(this.props.options), JSON.stringify(this.options) !== JSON.stringify(this.props.options)), JSON.stringify(this.options) !== JSON.stringify(this.props.options)) {
+                    if (JSON.stringify(this.options) !== JSON.stringify(this.props.options)) {
                         var e = this.getOption();
                         this.options = this.props.options, this.props.setProps({
                             value: e.value
                         })
                     }
                     this.pos && (this.wrapRef.current.scrollTop = this.pos)
                 }
@@ -3892,15 +3892,15 @@
                             for (l.s(); !(u = l.n()).done;) {
                                 var f = u.value;
                                 c.push(h.a.createElement(at, {
                                     key: f.value,
                                     "data-value": f.value,
                                     "data-label": f.label,
                                     onClick: this.select
-                                }, h.a.createElement("span", null, f.label))), String(f.value) === String(a) && console.log("-- MOBILE DROPDOWN", a, s)
+                                }, h.a.createElement("span", null, f.label))), String(f.value) === String(a) && console.log("-- MOBILE DROPDOWN", "value:" + a, "label:" + s)
                             }
                         } catch (e) {
                             l.e(e)
                         } finally {
                             l.f()
                         }
                     } else c.push(h.a.createElement(at, {
@@ -4106,20 +4106,20 @@
         value: p.a.oneOfType([p.a.string, p.a.number]),
         notfoundMsg: p.a.string,
         clearable: p.a.bool,
         setProps: p.a.func,
         disable: p.a.bool,
         label: p.a.string
     };
-    var Et = y.a.div(Je || (Je = Ot(["\n    position: fixed;\n    top: 0;\n    left: 0;\n    width: 100%;\n    height: 100%;\n"]))),
+    var Et = y.a.div(Ke || (Ke = Ot(["\n    position: fixed;\n    top: 0;\n    left: 0;\n    width: 100%;\n    height: 100%;\n"]))),
         Pt = y.a.div.attrs((function(e) {
             return {
                 iconColor: e.iconColor
             }
-        }))(Ke || (Ke = Ot(["\n    width: 30px;\n    height: 30px;\n    position: relative;\n\n    svg {\n        width: 100%;\n        height: 100%;\n        color: ", ";\n    }\n"])), (function(e) {
+        }))(Je || (Je = Ot(["\n    width: 30px;\n    height: 30px;\n    position: relative;\n\n    svg {\n        width: 100%;\n        height: 100%;\n        color: ", ";\n    }\n"])), (function(e) {
             return e.iconColor
         })),
         xt = y.a.span.attrs((function(e) {
             return {
                 color: e.color,
                 badgeColor: e.badgeColor,
                 borderColor: e.borderColor
@@ -4392,15 +4392,15 @@
         return (Rt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function It(e, t) {
+    function Lt(e, t) {
         for (var r = 0; r < t.length; r++) {
             var n = t[r];
             n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, (o = n.key, i = void 0, i = function(e, t) {
                 if ("object" !== Rt(e) || null === e) return e;
                 var r = e[Symbol.toPrimitive];
                 if (void 0 !== r) {
                     var n = r.call(e, t || "default");
@@ -4409,16 +4409,16 @@
                 }
                 return ("string" === t ? String : Number)(e)
             }(o, "string"), "symbol" === Rt(i) ? i : String(i)), n)
         }
         var o, i
     }
 
-    function Lt(e, t) {
-        return (Lt = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+    function It(e, t) {
+        return (It = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
     function Dt(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
@@ -4491,15 +4491,15 @@
                 constructor: {
                     value: e,
                     writable: !0,
                     configurable: !0
                 }
             }), Object.defineProperty(e, "prototype", {
                 writable: !1
-            }), t && Lt(e, t)
+            }), t && It(e, t)
         }(i, e);
         var t, r, n, o = Dt(i);
 
         function i(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
@@ -4534,15 +4534,15 @@
             key: "render",
             value: function() {
                 var e = this.props.id;
                 return h.a.createElement("div", {
                     id: e
                 })
             }
-        }]) && It(t.prototype, r), n && It(t, n), Object.defineProperty(t, "prototype", {
+        }]) && Lt(t.prototype, r), n && Lt(t, n), Object.defineProperty(t, "prototype", {
             writable: !1
         }), i
     }(d.Component);
 
     function Ft(e) {
         return (Ft = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
@@ -4620,15 +4620,15 @@
         setProps: p.a.func
     };
     var Yt, qt, Vt = y.a.div($t || (Yt = ["\n    position: fixed;\n    top: 0;\n    height: 0;\n    width: 100%;\n    height: 100%;\n"], qt || (qt = Yt.slice(0)), $t = Object.freeze(Object.defineProperties(Yt, {
             raw: {
                 value: Object.freeze(qt)
             }
         })))),
-        Jt = function(e) {
+        Kt = function(e) {
             ! function(e, t) {
                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                 e.prototype = Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
@@ -4690,35 +4690,35 @@
                     }, e)
                 }
             }]) && Ut(t.prototype, r), n && Ut(t, n), Object.defineProperty(t, "prototype", {
                 writable: !1
             }), i
         }(d.Component);
 
-    function Kt(e) {
-        return (Kt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Jt(e) {
+        return (Jt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function Zt(e, t) {
         for (var r = 0; r < t.length; r++) {
             var n = t[r];
             n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, (o = n.key, i = void 0, i = function(e, t) {
-                if ("object" !== Kt(e) || null === e) return e;
+                if ("object" !== Jt(e) || null === e) return e;
                 var r = e[Symbol.toPrimitive];
                 if (void 0 !== r) {
                     var n = r.call(e, t || "default");
-                    if ("object" !== Kt(n)) return n;
+                    if ("object" !== Jt(n)) return n;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
-            }(o, "string"), "symbol" === Kt(i) ? i : String(i)), n)
+            }(o, "string"), "symbol" === Jt(i) ? i : String(i)), n)
         }
         var o, i
     }
 
     function Qt(e, t) {
         return (Qt = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
             return e.__proto__ = t, e
@@ -4743,32 +4743,32 @@
                 r = Reflect.construct(n, arguments, o)
             } else r = n.apply(this, arguments);
             return tr(this, r)
         }
     }
 
     function tr(e, t) {
-        if (t && ("object" === Kt(t) || "function" == typeof t)) return t;
+        if (t && ("object" === Jt(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
     function rr(e) {
         return (rr = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
-    Jt.defaultProps = {
+    Kt.defaultProps = {
         reload: !0,
         timing: "all",
         delay: 10
-    }, Jt.propTypes = {
+    }, Kt.propTypes = {
         id: p.a.string,
         orientation: p.a.string,
         message: p.a.node,
         reload: p.a.bool,
         timing: p.a.string,
         delay: p.a.number,
         setProps: p.a.func
@@ -5418,15 +5418,15 @@
         value: 0
     }, jr.propTypes = {
         id: p.a.string,
         value: p.a.oneOfType([p.a.number, p.a.string]),
         className: p.a.string,
         setProps: p.a.func
     }, r.d(t, "Alert", (function() {
-        return I
+        return L
     })), r.d(t, "DesignableRadioItems", (function() {
         return U
     })), r.d(t, "IndexedDB", (function() {
         return ie
     })), r.d(t, "InputNumber", (function() {
         return jr
     })), r.d(t, "IosScrollWrapper", (function() {
@@ -5434,15 +5434,15 @@
     })), r.d(t, "LoadingWrapper", (function() {
         return xe
     })), r.d(t, "MobileDropdown", (function() {
         return ft
     })), r.d(t, "Notice", (function() {
         return At
     })), r.d(t, "Rotate", (function() {
-        return Jt
+        return Kt
     })), r.d(t, "SelectableBox", (function() {
         return nr
     })), r.d(t, "OperationObserver", (function() {
         return zt
     })), r.d(t, "TouchableComponent", (function() {
         return pr
     })), r.d(t, "UrlObserver", (function() {
```

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.3.9/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks-dash-components
-Version: 0.3.8
+Version: 0.3.9
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.8/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.3.9/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

