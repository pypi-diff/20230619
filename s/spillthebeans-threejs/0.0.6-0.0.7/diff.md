# Comparing `tmp/spillthebeans_threejs-0.0.6.tar.gz` & `tmp/spillthebeans_threejs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spillthebeans_threejs-0.0.6.tar", last modified: Fri Jan  6 10:08:13 2023, max compression
+gzip compressed data, was "spillthebeans_threejs-0.0.7.tar", last modified: Mon Jun 19 20:41:05 2023, max compression
```

## Comparing `spillthebeans_threejs-0.0.6.tar` & `spillthebeans_threejs-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bencannell   (501) staff       (20)        0 2023-01-06 10:08:13.148446 spillthebeans_threejs-0.0.6/
--rw-r--r--   0 bencannell   (501) staff       (20)     1561 2022-10-04 14:17:19.000000 spillthebeans_threejs-0.0.6/LICENSE
--rw-r--r--   0 bencannell   (501) staff       (20)      443 2022-10-04 14:17:19.000000 spillthebeans_threejs-0.0.6/MANIFEST.in
--rw-r--r--   0 bencannell   (501) staff       (20)      287 2023-01-06 10:08:13.148319 spillthebeans_threejs-0.0.6/PKG-INFO
--rw-r--r--   0 bencannell   (501) staff       (20)     3744 2022-10-04 15:16:46.000000 spillthebeans_threejs-0.0.6/README.md
--rw-r--r--   0 bencannell   (501) staff       (20)     2263 2023-01-06 10:04:02.000000 spillthebeans_threejs-0.0.6/package.json
--rw-r--r--   0 bencannell   (501) staff       (20)       38 2023-01-06 10:08:13.148494 spillthebeans_threejs-0.0.6/setup.cfg
--rw-r--r--   0 bencannell   (501) staff       (20)      510 2022-10-04 14:17:22.000000 spillthebeans_threejs-0.0.6/setup.py
-drwxr-xr-x   0 bencannell   (501) staff       (20)        0 2023-01-06 10:08:13.147700 spillthebeans_threejs-0.0.6/spillthebeans_threejs/
--rw-r--r--   0 bencannell   (501) staff       (20)     1442 2023-01-05 12:15:41.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs/SpillthebeansThreejs.py
--rw-r--r--   0 bencannell   (501) staff       (20)     2515 2022-10-10 08:13:37.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs/__init__.py
--rw-r--r--   0 bencannell   (501) staff       (20)       96 2022-10-10 08:25:34.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs/_imports_.py
--rw-r--r--   0 bencannell   (501) staff       (20)      367 2022-10-11 18:33:58.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs/metadata.json
--rw-r--r--   0 bencannell   (501) staff       (20)     2263 2023-01-05 12:15:41.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs/package-info.json
--rw-r--r--   0 bencannell   (501) staff       (20)   935574 2023-01-06 10:06:56.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs/spillthebeans_threejs.min.js
--rw-r--r--   0 bencannell   (501) staff       (20)      105 2023-01-06 10:06:56.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs/spillthebeans_threejs.min.js.map
-drwxr-xr-x   0 bencannell   (501) staff       (20)        0 2023-01-06 10:08:13.148141 spillthebeans_threejs-0.0.6/spillthebeans_threejs.egg-info/
--rw-r--r--   0 bencannell   (501) staff       (20)      287 2023-01-06 10:08:13.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs.egg-info/PKG-INFO
--rw-r--r--   0 bencannell   (501) staff       (20)      528 2023-01-06 10:08:13.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs.egg-info/SOURCES.txt
--rw-r--r--   0 bencannell   (501) staff       (20)        1 2023-01-06 10:08:13.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs.egg-info/dependency_links.txt
--rw-r--r--   0 bencannell   (501) staff       (20)       22 2023-01-06 10:08:13.000000 spillthebeans_threejs-0.0.6/spillthebeans_threejs.egg-info/top_level.txt
+drwxr-xr-x   0 bencannell   (501) staff       (20)        0 2023-06-19 20:41:05.696825 spillthebeans_threejs-0.0.7/
+-rw-r--r--   0 bencannell   (501) staff       (20)     1561 2022-10-04 14:17:19.000000 spillthebeans_threejs-0.0.7/LICENSE
+-rw-r--r--   0 bencannell   (501) staff       (20)      443 2022-10-04 14:17:19.000000 spillthebeans_threejs-0.0.7/MANIFEST.in
+-rw-r--r--   0 bencannell   (501) staff       (20)      287 2023-06-19 20:41:05.696700 spillthebeans_threejs-0.0.7/PKG-INFO
+-rw-r--r--   0 bencannell   (501) staff       (20)     3744 2022-10-04 15:16:46.000000 spillthebeans_threejs-0.0.7/README.md
+-rw-r--r--   0 bencannell   (501) staff       (20)     2263 2023-06-19 20:22:05.000000 spillthebeans_threejs-0.0.7/package.json
+-rw-r--r--   0 bencannell   (501) staff       (20)       38 2023-06-19 20:41:05.696874 spillthebeans_threejs-0.0.7/setup.cfg
+-rw-r--r--   0 bencannell   (501) staff       (20)      510 2022-10-04 14:17:22.000000 spillthebeans_threejs-0.0.7/setup.py
+drwxr-xr-x   0 bencannell   (501) staff       (20)        0 2023-06-19 20:41:05.696040 spillthebeans_threejs-0.0.7/spillthebeans_threejs/
+-rw-r--r--   0 bencannell   (501) staff       (20)     1442 2023-06-19 20:30:59.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs/SpillthebeansThreejs.py
+-rw-r--r--   0 bencannell   (501) staff       (20)     2515 2022-10-10 08:13:37.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs/__init__.py
+-rw-r--r--   0 bencannell   (501) staff       (20)       96 2022-10-10 08:25:34.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs/_imports_.py
+-rw-r--r--   0 bencannell   (501) staff       (20)      367 2022-10-11 18:33:58.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs/metadata.json
+-rw-r--r--   0 bencannell   (501) staff       (20)     2263 2023-06-19 20:30:59.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs/package-info.json
+-rw-r--r--   0 bencannell   (501) staff       (20)   935627 2023-06-19 20:37:18.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs/spillthebeans_threejs.min.js
+-rw-r--r--   0 bencannell   (501) staff       (20)      105 2023-06-19 20:37:18.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs/spillthebeans_threejs.min.js.map
+drwxr-xr-x   0 bencannell   (501) staff       (20)        0 2023-06-19 20:41:05.696532 spillthebeans_threejs-0.0.7/spillthebeans_threejs.egg-info/
+-rw-r--r--   0 bencannell   (501) staff       (20)      287 2023-06-19 20:41:05.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs.egg-info/PKG-INFO
+-rw-r--r--   0 bencannell   (501) staff       (20)      528 2023-06-19 20:41:05.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs.egg-info/SOURCES.txt
+-rw-r--r--   0 bencannell   (501) staff       (20)        1 2023-06-19 20:41:05.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs.egg-info/dependency_links.txt
+-rw-r--r--   0 bencannell   (501) staff       (20)       22 2023-06-19 20:41:05.000000 spillthebeans_threejs-0.0.7/spillthebeans_threejs.egg-info/top_level.txt
```

### Comparing `spillthebeans_threejs-0.0.6/LICENSE` & `spillthebeans_threejs-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spillthebeans_threejs-0.0.6/README.md` & `spillthebeans_threejs-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `spillthebeans_threejs-0.0.6/package.json` & `spillthebeans_threejs-0.0.7/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.7'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends": "dash-generate-components ./src/lib/components spillthebeans_threejs -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.6"
+    "version": "0.0.7"
 }
```

### Comparing `spillthebeans_threejs-0.0.6/spillthebeans_threejs/SpillthebeansThreejs.py` & `spillthebeans_threejs-0.0.7/spillthebeans_threejs/SpillthebeansThreejs.py`

 * *Files identical despite different names*

### Comparing `spillthebeans_threejs-0.0.6/spillthebeans_threejs/__init__.py` & `spillthebeans_threejs-0.0.7/spillthebeans_threejs/__init__.py`

 * *Files identical despite different names*

### Comparing `spillthebeans_threejs-0.0.6/spillthebeans_threejs/package-info.json` & `spillthebeans_threejs-0.0.7/spillthebeans_threejs/package-info.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.7'"}*

```diff
@@ -56,9 +56,9 @@
         "build:backends": "dash-generate-components ./src/lib/components spillthebeans_threejs -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.5"
+    "version": "0.0.7"
 }
```

### Comparing `spillthebeans_threejs-0.0.6/spillthebeans_threejs/spillthebeans_threejs.min.js` & `spillthebeans_threejs-0.0.7/spillthebeans_threejs/spillthebeans_threejs.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
         ! function(e, t) {
             if (!_[e] || !x[e]) return;
             for (var n in x[e] = !1, t) Object.prototype.hasOwnProperty.call(t, n) && (f[n] = t[n]);
             0 == --g && 0 === v && w()
         }(e, n), t && t(e, n)
     };
     var n, r = !0,
-        i = "ebd65cd0db3486c61c12",
+        i = "f76f3dc2a4e2d855c10c",
         s = {},
         a = [],
         o = [];
 
     function l(e) {
         var t = C[e];
         if (!t) return E;
@@ -114,15 +114,15 @@
 
     function M(e) {
         if ("idle" !== h) throw new Error("check() is only allowed in idle status");
         return r = e, d("check"), (t = 1e4, t = t || 1e4, new Promise((function(e, n) {
             if ("undefined" == typeof XMLHttpRequest) return n(new Error("No browser support"));
             try {
                 var r = new XMLHttpRequest,
-                    i = E.p + "13075d2-wps-hmr.json";
+                    i = E.p + "725575e-wps-hmr.json";
                 r.open("GET", i, !0), r.timeout = t, r.send(null)
             } catch (e) {
                 return n(e)
             }
             r.onreadystatechange = function() {
                 if (4 === r.readyState)
                     if (0 === r.status) n(new Error("Manifest request to " + i + " timed out."));
@@ -151,15 +151,15 @@
         }));
         var t
     }
 
     function A(e) {
         _[e] ? (x[e] = !0, g++, function(e) {
             var t = document.createElement("script");
-            t.charset = "utf-8", t.src = E.p + "13075d2-" + e + "-wps-hmr.js", document.head.appendChild(t)
+            t.charset = "utf-8", t.src = E.p + "725575e-" + e + "-wps-hmr.js", document.head.appendChild(t)
         }(e)) : y[e] = !0
     }
 
     function w() {
         d("ready");
         var e = p;
         if (p = null, e)
@@ -411,15 +411,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(B()),
                 n = R(e);
             if (!t) return n;
             var r = n.split("/"),
                 i = r.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_0_6m1672999614"), r.splice(-1, 1, i.join(".")), r.join("/")
+            return i.splice(1, 0, "v0_0_7m1687207035"), r.splice(-1, 1, i.join(".")), r.join("/")
         }
     }
     return E.h = function() {
         return i
     }, l(61)(E.s = 61)
 }([function(e, t, n) {
     "use strict";
@@ -26964,36 +26964,41 @@
             clearcoat: 1,
             clearcoatRoughness: 0,
             metalness: 1,
             side: p.DoubleSide
         }),
         We = function(e) {
             var t = Object(l.useRef)(),
-                n = Ne("/assets/open_can.glb"),
-                r = n.nodes,
-                i = (n.materials, He(Object(l.useState)(e.rotation), 2)),
-                s = (i[0], i[1], He(Object(l.useState)(e.axis), 2)),
-                a = (s[0], s[1], He(Object(l.useState)(0), 2)),
-                o = (a[0], a[1], He(Object(l.useState)(e.canAngle), 2)),
-                u = o[0],
-                h = (o[1], r.Can001.geometry),
-                d = r.Can002.geometry;
+                n = Ne("/assets/single-can.glb").nodes,
+                r = He(Object(l.useState)(e.canAngle), 2),
+                i = r[0],
+                s = (r[1], n["can-base"].children[0].geometry),
+                a = n["can-middle"].children[0].geometry,
+                o = n["can-top"].children[0].geometry,
+                u = [s, a, a.clone(), o],
+                h = n["can-lid"].geometry,
+                d = [je, je, je, je];
             return Object(l.useEffect)((function() {
-                h.scale(15, 15, 15), h.rotateZ(u), h.translate(0, 1.5, 0), d.scale(15, 15, 15), d.rotateZ(u), d.translate(0, 1.5, 0)
+                u.forEach((function(e) {
+                    e.scale(15, 15, 15), e.rotateZ(i), e.translate(0, 1.5, 0)
+                })), h.scale(15, 15, 15), h.rotateZ(i), h.translate(0, 1.5, 0)
             }), []), c.a.createElement("group", {
                 ref: t,
                 dispose: null
-            }, c.a.createElement("mesh", {
+            }, u.map((function(e, t) {
+                return c.a.createElement("mesh", {
+                    key: t,
+                    geometry: e,
+                    material: d[t],
+                    castShadow: !0
+                })
+            })), c.a.createElement("mesh", {
                 geometry: h,
                 material: je,
                 castShadow: !0
-            }), c.a.createElement("mesh", {
-                geometry: d,
-                material: je,
-                castShadow: !0
             }), c.a.createElement(ke, {
                 scale: 10,
                 blur: 5,
                 far: 10,
                 frames: 1
             }))
         },
@@ -30188,15 +30193,15 @@
             }
         }, c.a.createElement("perspectiveCamera", {
             makeDefault: !0,
             position: [-500, 500, 1500]
         }), c.a.createElement(ii, null), c.a.createElement(g, null), c.a.createElement(l.Suspense, {
             fallback: null
         }, c.a.createElement(oi, e), c.a.createElement(_, {
-            preset: "warehouse"
+            files: "/assets/background.hdr"
         }))), c.a.createElement(T, null))
     }
     li.defaultProps = {
         axis: new p.Vector3(1, 0, 0),
         rotation: .01,
         scale: .5
     }, li.propTypes = {
```

### Comparing `spillthebeans_threejs-0.0.6/spillthebeans_threejs.egg-info/SOURCES.txt` & `spillthebeans_threejs-0.0.7/spillthebeans_threejs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

