# Comparing `tmp/st_line_plotter-0.0.8.tar.gz` & `tmp/st_line_plotter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_line_plotter-0.0.8.tar", last modified: Mon Jun 19 06:34:37 2023, max compression
+gzip compressed data, was "st_line_plotter-0.0.9.tar", last modified: Mon Jun 19 07:21:05 2023, max compression
```

## Comparing `st_line_plotter-0.0.8.tar` & `st_line_plotter-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:34:37.314294 st_line_plotter-0.0.8/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-06-08 13:50:21.000000 st_line_plotter-0.0.8/LICENSE
--rw-r--r--   0 elliotglas   (501) staff       (20)       51 2023-06-14 07:33:03.000000 st_line_plotter-0.0.8/MANIFEST.in
--rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-19 06:34:37.314119 st_line_plotter-0.0.8/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-06-19 06:34:37.314350 st_line_plotter-0.0.8/setup.cfg
--rw-r--r--   0 elliotglas   (501) staff       (20)      671 2023-06-19 06:34:28.000000 st_line_plotter-0.0.8/setup.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:34:37.309291 st_line_plotter-0.0.8/st_line_plotter/
--rw-r--r--   0 elliotglas   (501) staff       (20)     2144 2023-06-19 06:31:15.000000 st_line_plotter-0.0.8/st_line_plotter/__init__.py
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:34:37.308140 st_line_plotter-0.0.8/st_line_plotter/frontend/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:34:37.311315 st_line_plotter-0.0.8/st_line_plotter/frontend/build/
--rw-r--r--   0 elliotglas   (501) staff       (20)      859 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/asset-manifest.json
--rw-r--r--   0 elliotglas   (501) staff       (20)     2119 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/index.html
--rw-r--r--   0 elliotglas   (501) staff       (20)      564 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/precache-manifest.dca2b6b2012232a6d569502759b645c6.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     1183 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/service-worker.js
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:34:37.308294 st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:34:37.313861 st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/
--rw-r--r--   0 elliotglas   (501) staff       (20)   459951 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     1909 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.LICENSE.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)  1700559 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     9963 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/main.e5ec0f99.chunk.js
--rw-r--r--   0 elliotglas   (501) staff       (20)    35841 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/main.e5ec0f99.chunk.js.map
--rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 elliotglas   (501) staff       (20)     8317 2023-06-19 06:34:30.000000 st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 06:34:37.310318 st_line_plotter-0.0.8/st_line_plotter.egg-info/
--rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-19 06:34:37.000000 st_line_plotter-0.0.8/st_line_plotter.egg-info/PKG-INFO
--rw-r--r--   0 elliotglas   (501) staff       (20)      944 2023-06-19 06:34:37.000000 st_line_plotter-0.0.8/st_line_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-06-19 06:34:37.000000 st_line_plotter-0.0.8/st_line_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-19 06:34:37.000000 st_line_plotter-0.0.8/st_line_plotter.egg-info/requires.txt
--rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-19 06:34:37.000000 st_line_plotter-0.0.8/st_line_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 07:21:05.879028 st_line_plotter-0.0.9/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2340 2023-06-08 13:50:21.000000 st_line_plotter-0.0.9/LICENSE
+-rw-r--r--   0 elliotglas   (501) staff       (20)       51 2023-06-14 07:33:03.000000 st_line_plotter-0.0.9/MANIFEST.in
+-rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-19 07:21:05.878846 st_line_plotter-0.0.9/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)       38 2023-06-19 07:21:05.879088 st_line_plotter-0.0.9/setup.cfg
+-rw-r--r--   0 elliotglas   (501) staff       (20)      671 2023-06-19 07:20:52.000000 st_line_plotter-0.0.9/setup.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 07:21:05.874061 st_line_plotter-0.0.9/st_line_plotter/
+-rw-r--r--   0 elliotglas   (501) staff       (20)     7211 2023-06-19 07:19:31.000000 st_line_plotter-0.0.9/st_line_plotter/__init__.py
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 07:21:05.873227 st_line_plotter-0.0.9/st_line_plotter/frontend/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 07:21:05.876131 st_line_plotter-0.0.9/st_line_plotter/frontend/build/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      859 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/asset-manifest.json
+-rw-r--r--   0 elliotglas   (501) staff       (20)     2119 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/index.html
+-rw-r--r--   0 elliotglas   (501) staff       (20)      564 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/precache-manifest.6279477322d7616ea3eaabbcb4ce811d.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1183 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/service-worker.js
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 07:21:05.873382 st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 07:21:05.878595 st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/
+-rw-r--r--   0 elliotglas   (501) staff       (20)   459951 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1909 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.LICENSE.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)  1700559 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     9954 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/main.a9c05652.chunk.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)    35862 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/main.a9c05652.chunk.js.map
+-rw-r--r--   0 elliotglas   (501) staff       (20)     1598 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 elliotglas   (501) staff       (20)     8317 2023-06-19 07:20:18.000000 st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 elliotglas   (501) staff       (20)        0 2023-06-19 07:21:05.875170 st_line_plotter-0.0.9/st_line_plotter.egg-info/
+-rw-r--r--   0 elliotglas   (501) staff       (20)      298 2023-06-19 07:21:05.000000 st_line_plotter-0.0.9/st_line_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 elliotglas   (501) staff       (20)      944 2023-06-19 07:21:05.000000 st_line_plotter-0.0.9/st_line_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)        1 2023-06-19 07:21:05.000000 st_line_plotter-0.0.9/st_line_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-19 07:21:05.000000 st_line_plotter-0.0.9/st_line_plotter.egg-info/requires.txt
+-rw-r--r--   0 elliotglas   (501) staff       (20)       16 2023-06-19 07:21:05.000000 st_line_plotter-0.0.9/st_line_plotter.egg-info/top_level.txt
```

### Comparing `st_line_plotter-0.0.8/LICENSE` & `st_line_plotter-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.8/setup.py` & `st_line_plotter-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_line_plotter",
-    version="0.0.8",
+    version="0.0.9",
     author="Elliot Glas",
     author_email="elliot.glas@hotmail.se",
     description="A tool to place lines on an image and get back the coordinates for those lines",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/asset-manifest.json` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/asset-manifest.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068181818181819%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.a9c05652.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.a9c05652.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.a9c05652.chunk.js.map', "*

 * *            "'precache-manifest.6279477322d7616ea3eaabbcb4ce811d.js': "*

 * *            "'./precache-manifest.6279477322d7616ea3eaabbcb4ce811d.js', delete: "*

 * *            "['precache-manifest.dca2b6b2012232a6d569502759b645c6.js']}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/js/runtime-main.11ec9aca.js",
         "static/js/2.eb731a1a.chunk.js",
-        "static/js/main.e5ec0f99.chunk.js"
+        "static/js/main.a9c05652.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.e5ec0f99.chunk.js",
-        "main.js.map": "./static/js/main.e5ec0f99.chunk.js.map",
-        "precache-manifest.dca2b6b2012232a6d569502759b645c6.js": "./precache-manifest.dca2b6b2012232a6d569502759b645c6.js",
+        "main.js": "./static/js/main.a9c05652.chunk.js",
+        "main.js.map": "./static/js/main.a9c05652.chunk.js.map",
+        "precache-manifest.6279477322d7616ea3eaabbcb4ce811d.js": "./precache-manifest.6279477322d7616ea3eaabbcb4ce811d.js",
         "runtime-main.js": "./static/js/runtime-main.11ec9aca.js",
         "runtime-main.js.map": "./static/js/runtime-main.11ec9aca.js.map",
         "service-worker.js": "./service-worker.js",
         "static/js/2.eb731a1a.chunk.js": "./static/js/2.eb731a1a.chunk.js",
         "static/js/2.eb731a1a.chunk.js.LICENSE.txt": "./static/js/2.eb731a1a.chunk.js.LICENSE.txt",
         "static/js/2.eb731a1a.chunk.js.map": "./static/js/2.eb731a1a.chunk.js.map"
     }
```

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/index.html` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.eb731a1a.chunk.js"></script><script src="./static/js/main.e5ec0f99.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><style>body,html{height:100%;width:100%;margin:0;padding:0}</style></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.eb731a1a.chunk.js"></script><script src="./static/js/main.a9c05652.chunk.js"></script></body></html>
```

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/service-worker.js` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/service-worker.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.dca2b6b2012232a6d569502759b645c6.js"
+    "./precache-manifest.6279477322d7616ea3eaabbcb4ce811d.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.LICENSE.txt` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.map` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/main.e5ec0f99.chunk.js` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/main.a9c05652.chunk.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -171,73 +171,73 @@
                         f = e.setIndex,
                         p = Math.sqrt(Math.pow(a - n, 2) + Math.pow(i - r, 2)),
                         h = [(a - n) / p, (i - r) / p],
                         v = [-h[1], h[0]],
                         m = "".concat(n + 7 * h[0], ",").concat(r + 7 * h[1]),
                         b = "".concat(a, ",").concat(i),
                         y = (n + a) / 2,
-                        g = (r + i) / 2,
-                        x = function() {
+                        x = (r + i) / 2,
+                        g = function() {
                             f(s)
                         };
                     return o.a.createElement("svg", null, o.a.createElement("circle", {
                         key: "".concat(n).concat(r),
                         cx: n,
                         cy: r,
                         r: "".concat(7),
                         stroke: d,
                         strokeWidth: "3",
                         fill: "none",
-                        onClick: x
+                        onClick: g
                     }), o.a.createElement("circle", {
                         key: "".concat(n).concat(r, "'"),
                         cx: n,
                         cy: r,
                         r: "".concat(7),
                         stroke: "transparent",
                         strokeWidth: "6",
                         fill: "transparent",
-                        onClick: x
+                        onClick: g
                     }), o.a.createElement("polyline", {
                         key: "".concat(a).concat(i),
                         points: "".concat(m, " ").concat(b),
                         stroke: d,
                         strokeWidth: "3",
                         fill: "none",
-                        onClick: x
+                        onClick: g
                     }), o.a.createElement("polyline", {
                         key: "".concat(a).concat(i, "'"),
                         points: "".concat(m, " ").concat(b),
                         stroke: "transparent",
                         strokeWidth: "6",
                         fill: "transparent",
-                        onClick: x
+                        onClick: g
                     }), o.a.createElement("text", {
                         x: n - 2 * c.length,
                         y: r - 14,
                         fontSize: 10,
                         fontFamily: "sans-serif",
                         fill: "white",
-                        onClick: x
+                        onClick: g
                     }, c), o.a.createElement("text", {
                         x: y + 7 * v[0] * 2,
-                        y: g + 7 * v[1] * 2,
+                        y: x + 7 * v[1] * 2,
                         textAnchor: "middle",
                         fontSize: 8,
                         fontFamily: "sans-serif",
                         fill: "white",
-                        onClick: x
+                        onClick: g
                     }, l), o.a.createElement("text", {
                         x: y - 7 * v[0] * 2,
-                        y: g - 7 * v[1] * 2,
+                        y: x - 7 * v[1] * 2,
                         textAnchor: "middle",
                         fontSize: 8,
                         fontFamily: "sans-serif",
                         fill: "white",
-                        onClick: x
+                        onClick: g
                     }, u))
                 },
                 p = function(e) {
                     var t = e.placeholder,
                         n = e.value,
                         a = e.whichProp,
                         i = e.onClick,
@@ -362,25 +362,25 @@
                     a = n[0],
                     i = n[1],
                     p = Object(r.useState)([]),
                     v = Object(s.a)(p, 2),
                     m = v[0],
                     b = v[1],
                     y = Object(r.useState)(),
-                    g = Object(s.a)(y, 2),
-                    x = g[0],
-                    E = g[1],
+                    x = Object(s.a)(y, 2),
+                    g = x[0],
+                    E = x[1],
                     j = ["red", "green", "blue", "yellow", "pink"],
                     _ = e.args.image,
                     O = e.args.width,
                     k = e.args.height,
                     S = Object(r.useState)(e.args.key),
-                    C = Object(s.a)(S, 2),
-                    w = C[0],
-                    P = (C[1], e.args.changed),
+                    w = Object(s.a)(S, 2),
+                    C = w[0],
+                    P = (w[1], e.args.changed),
                     D = 0,
                     R = Object(r.useState)(!1),
                     M = Object(s.a)(R, 2),
                     N = M[0],
                     z = M[1];
                 var F = null;
                 Object(r.useEffect)((function() {
@@ -390,15 +390,15 @@
                             return d.Streamlit.setComponentValue(t), t
                         })), z(!0)), "Enter" === e.key && E(void 0)
                     }))
                 }), []), Object(r.useEffect)((function() {
                     ! function() {
                         var t = e.args.lines;
                         console.log(t), i((function(e) {
-                            return n = e, r = t, (w === P ? n : r).map((function(e) {
+                            return n = e, r = t, (C === P ? n : r).map((function(e) {
                                 return Object(u.a)(Object(u.a)({}, e), {}, {
                                     id: (t = e, "".concat(t.x1).concat(t.y1).concat(t.x2).concat(t.y2).concat(t.name).concat(t.dir1).concat(t.dir2))
                                 });
                                 var t
                             }));
                             var n, r
                         }))
@@ -424,21 +424,21 @@
                         flexDirection: "column"
                     }
                 }, o.a.createElement("div", {
                     style: {
                         width: O,
                         height: k,
                         backgroundImage: "url(".concat(_, ")"),
-                        backgroundPosition: "center",
-                        backgroundSize: "100%",
+                        backgroundSize: "cover",
+                        overflow: "hidden",
                         position: "relative",
                         display: "inline-block"
                     },
                     onClick: function(e) {
-                        void 0 === x && function(e) {
+                        void 0 === g && function(e) {
                             var t = function(e) {
                                     var t = e.target.getBoundingClientRect();
                                     return [e.clientX - t.left, e.clientY - t.top]
                                 }(e),
                                 n = Object(s.a)(t, 2),
                                 r = n[0],
                                 o = n[1];
@@ -454,26 +454,26 @@
                                         x2: r,
                                         y2: o,
                                         name: "Vertex ".concat(m.length),
                                         dir1: "Up",
                                         dir2: "Down",
                                         id: "".concat(u).concat(d).concat(r).concat(o, "Vertex ".concat(m.length), "Up", "Down")
                                     };
-                                w === P && i((function(e) {
+                                C === P && i((function(e) {
                                     return [].concat(Object(l.a)(e), [f])
                                 })), z(!0), D = (D + 1) % j.length, F = null
                             }
                         }(e)
                     }
                 }, o.a.createElement("svg", {
                     width: O,
                     height: k
-                }, m)), o.a.createElement("div", null, w === P ? void 0 !== x ? o.a.createElement(h, {
-                    coords: a[x],
-                    index: x,
+                }, m)), o.a.createElement("div", null, C === P ? void 0 !== g ? o.a.createElement(h, {
+                    coords: a[g],
+                    index: g,
                     setCoordinates: i,
                     setCoordinatesChanged: z,
                     setIndex: E
                 }) : o.a.createElement("div", {
                     style: {
                         display: "flex",
                         maxWidth: O,
@@ -535,8 +535,8 @@
             })
         }
     },
     [
         [15, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.e5ec0f99.chunk.js.map
+//# sourceMappingURL=main.a9c05652.chunk.js.map
```

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/main.e5ec0f99.chunk.js.map` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/main.a9c05652.chunk.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8422643746295199%*

 * *Differences: {"'file'": "'static/js/main.a9c05652.chunk.js'",*

 * * "'mappings'": "'6IACAA,OAAOC,eAAeC,EAAS,aAAc,CAAEC,OAAO,IACtDD,EAAQE,2BAAwB,EAChC,IAAIC,EAAUC,EAAQ,GAClBC,EAA4BD,EAAQ,GAsBxCJ,EAAQE,sBAlBoB,WACxB,IAAII,GAAK,EAAIH,EAAQI,YAAaC,EAAaF,EAAG,GAAIG,EAAgBH,EAAG,GAezE,OAdA,EAAIH,EAAQO,YAAW,WACnB,IAAIC,EAAgB,SAAUC,GAE1BH,EADkBG,EACQC,SAI9BR,EAA0BS,UAAUC,OAAOC,iBAAiBX,EAA0BS,UAAUG,aAAcN,GAC9GN,EAA0BS,UAAUI,oBAIpC,OAHc,WACVb,EAA0BS,UAAUC,OAAOI,oBAAoBd,EAA0BS,UAAUG,aAAcN,MAGtH,IACIH,I,oECvBX,IAAIY,EAAYC,MAAQA,KAAKD,UAAa […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.e5ec0f99.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.a9c05652.chunk.js",
+    "mappings": "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",
     "names": [
         "Object",
         "defineProperty",
         "exports",
         "value",
         "useNullableRenderData",
         "react_1",
@@ -212,16 +212,16 @@
         "verticesArray",
         "push",
         "updateVertices",
         "display",
         "flexDirection",
         "height",
         "backgroundImage",
-        "backgroundPosition",
         "backgroundSize",
+        "overflow",
         "position",
         "_getClickCoords",
         "dim",
         "getBoundingClientRect",
         "clientX",
         "left",
         "clientY",
@@ -258,13 +258,13 @@
     "sourcesContent": [
         "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.useNullableRenderData = void 0;\nvar react_1 = require(\"react\");\nvar streamlit_component_lib_1 = require(\"streamlit-component-lib\");\n/**\n * Returns `RenderData` received from Streamlit after the first render event received.\n */\nvar useNullableRenderData = function () {\n    var _a = (0, react_1.useState)(), renderData = _a[0], setRenderData = _a[1];\n    (0, react_1.useEffect)(function () {\n        var onRenderEvent = function (event) {\n            var renderEvent = event;\n            setRenderData(renderEvent.detail);\n        };\n        // Set up event listeners, and signal to Streamlit that we're ready.\n        // We won't render the component until we receive the first RENDER_EVENT.\n        streamlit_component_lib_1.Streamlit.events.addEventListener(streamlit_component_lib_1.Streamlit.RENDER_EVENT, onRenderEvent);\n        streamlit_component_lib_1.Streamlit.setComponentReady();\n        var cleanup = function () {\n            streamlit_component_lib_1.Streamlit.events.removeEventListener(streamlit_component_lib_1.Streamlit.RENDER_EVENT, onRenderEvent);\n        };\n        return cleanup;\n    }, []);\n    return renderData;\n};\nexports.useNullableRenderData = useNullableRenderData;\n",
         "\"use strict\";\nvar __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nvar __createBinding = (this && this.__createBinding) || (Object.create ? (function(o, m, k, k2) {\n    if (k2 === undefined) k2 = k;\n    Object.defineProperty(o, k2, { enumerable: true, get: function() { return m[k]; } });\n}) : (function(o, m, k, k2) {\n    if (k2 === undefined) k2 = k;\n    o[k2] = m[k];\n}));\nvar __setModuleDefault = (this && this.__setModuleDefault) || (Object.create ? (function(o, v) {\n    Object.defineProperty(o, \"default\", { enumerable: true, value: v });\n}) : function(o, v) {\n    o[\"default\"] = v;\n});\nvar __importStar = (this && this.__importStar) || function (mod) {\n    if (mod && mod.__esModule) return mod;\n    var result = {};\n    if (mod != null) for (var k in mod) if (k !== \"default\" && Object.prototype.hasOwnProperty.call(mod, k)) __createBinding(result, mod, k);\n    __setModuleDefault(result, mod);\n    return result;\n};\nvar __importDefault = (this && this.__importDefault) || function (mod) {\n    return (mod && mod.__esModule) ? mod : { \"default\": mod };\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.useRenderData = void 0;\nvar jsx_runtime_1 = require(\"react/jsx-runtime\");\nvar react_1 = __importStar(require(\"react\"));\nvar streamlit_component_lib_1 = require(\"streamlit-component-lib\");\nvar useNullableRenderData_1 = require(\"./useNullableRenderData\");\nvar ErrorBoundary_1 = __importDefault(require(\"./ErrorBoundary\"));\nvar renderDataContext = react_1.default.createContext(undefined);\n/**\n * Returns `RenderData` received from Streamlit.\n */\nvar useRenderData = function () {\n    var contextValue = (0, react_1.useContext)(renderDataContext);\n    if (contextValue == null) {\n        throw new Error(\"useRenderData() must be used inside <StreamlitProvider />\");\n    }\n    return contextValue;\n};\nexports.useRenderData = useRenderData;\nvar StreamlitProvider = function (props) {\n    var renderData = (0, useNullableRenderData_1.useNullableRenderData)();\n    (0, react_1.useEffect)(function () {\n        streamlit_component_lib_1.Streamlit.setFrameHeight();\n    });\n    // Don't render until we've gotten our first data from Streamlit.\n    if (renderData == null) {\n        return null;\n    }\n    return ((0, jsx_runtime_1.jsx)(ErrorBoundary_1.default, { children: (0, jsx_runtime_1.jsx)(renderDataContext.Provider, __assign({ value: renderData }, { children: props.children }), void 0) }, void 0));\n};\nexports.default = StreamlitProvider;\n",
         "\"use strict\";\nvar __extends = (this && this.__extends) || (function () {\n    var extendStatics = function (d, b) {\n        extendStatics = Object.setPrototypeOf ||\n            ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\n            function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\n        return extendStatics(d, b);\n    };\n    return function (d, b) {\n        if (typeof b !== \"function\" && b !== null)\n            throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\n        extendStatics(d, b);\n        function __() { this.constructor = d; }\n        d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\n    };\n})();\nvar __importDefault = (this && this.__importDefault) || function (mod) {\n    return (mod && mod.__esModule) ? mod : { \"default\": mod };\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\nvar jsx_runtime_1 = require(\"react/jsx-runtime\");\nvar react_1 = __importDefault(require(\"react\"));\n/**\n * Shows errors thrown from child components.\n */\nvar ErrorBoundary = /** @class */ (function (_super) {\n    __extends(ErrorBoundary, _super);\n    function ErrorBoundary(props) {\n        var _this = _super.call(this, props) || this;\n        _this.state = { error: undefined };\n        return _this;\n    }\n    ErrorBoundary.getDerivedStateFromError = function (error) {\n        // Update state so the next render will show the fallback UI.\n        return { error: error };\n    };\n    ErrorBoundary.prototype.render = function () {\n        if (this.state.error != null) {\n            return ((0, jsx_runtime_1.jsxs)(\"div\", { children: [(0, jsx_runtime_1.jsx)(\"h1\", { children: \"Component Error\" }, void 0), (0, jsx_runtime_1.jsx)(\"span\", { children: this.state.error.message }, void 0)] }, void 0));\n        }\n        return this.props.children;\n    };\n    return ErrorBoundary;\n}(react_1.default.PureComponent));\nexports.default = ErrorBoundary;\n",
         "import React from \"react\"\nimport { VertexData } from \"./LinePlacementPlot\"\n\ninterface VertexProps {\n  data: VertexData\n  index: number\n  color: string\n  setIndex: React.Dispatch<React.SetStateAction<number | undefined>>\n}\n\nconst RADIUS = 7\n\nconst Vertex: React.FC<VertexProps> = ({\n  data: { x1, y1, x2, y2, name, dir1, dir2 },\n  index,\n  color,\n  setIndex,\n}) => {\n  let length = Math.sqrt(Math.pow(x2 - x1, 2) + Math.pow(y2 - y1, 2))\n  let dir: [number, number] = [(x2 - x1) / length, (y2 - y1) / length]\n  let perpendicularDir: [number, number] = [-dir[1], dir[0]]\n  let from = `${x1 + dir[0] * RADIUS},${y1 + dir[1] * RADIUS}`\n  let to = `${x2},${y2}`\n\n  let midX = (x1 + x2) / 2\n  let midY = (y1 + y2) / 2\n\n  const onClick = () => {\n    setIndex(index)\n  }\n  return (\n    <svg>\n      <circle\n        key={`${x1}${y1}`}\n        cx={x1}\n        cy={y1}\n        r={`${RADIUS}`}\n        stroke={color}\n        strokeWidth=\"3\"\n        fill=\"none\"\n        onClick={onClick}\n      />\n      <circle\n        key={`${x1}${y1}'`}\n        cx={x1}\n        cy={y1}\n        r={`${RADIUS}`}\n        stroke=\"transparent\"\n        strokeWidth=\"6\"\n        fill=\"transparent\"\n        onClick={onClick}\n      />\n      <polyline\n        key={`${x2}${y2}`}\n        points={`${from} ${to}`}\n        stroke={color}\n        strokeWidth=\"3\"\n        fill=\"none\"\n        onClick={onClick}\n      />\n      <polyline\n        key={`${x2}${y2}'`}\n        points={`${from} ${to}`}\n        stroke=\"transparent\"\n        strokeWidth=\"6\"\n        fill=\"transparent\"\n        onClick={onClick}\n      />\n      <text\n        x={x1 - name.length * 2}\n        y={y1 - RADIUS * 2}\n        fontSize={10}\n        fontFamily=\"sans-serif\"\n        fill=\"white\"\n        onClick={onClick}\n      >\n        {name}\n      </text>\n      <text\n        x={midX + perpendicularDir[0] * RADIUS * 2}\n        y={midY + perpendicularDir[1] * RADIUS * 2}\n        textAnchor=\"middle\"\n        fontSize={8}\n        fontFamily=\"sans-serif\"\n        fill=\"white\"\n        onClick={onClick}\n      >\n        {dir1}\n      </text>\n      <text\n        x={midX - perpendicularDir[0] * RADIUS * 2}\n        y={midY - perpendicularDir[1] * RADIUS * 2}\n        textAnchor=\"middle\"\n        fontSize={8}\n        fontFamily=\"sans-serif\"\n        fill=\"white\"\n        onClick={onClick}\n      >\n        {dir2}\n      </text>\n    </svg>\n  )\n}\n\nexport default Vertex\n",
         "import React from \"react\"\nimport { useState } from \"react\"\nimport { VertexData } from \"./LinePlacementPlot\"\n\ninterface InputProps {\n  placeholder: string\n  value: string\n  whichProp: keyof VertexData\n  onClick: (arg: string, whichProp: keyof VertexData) => void\n}\n\n/*export const CoordinateInput: React.FC<InputProps> = ({\n  placeholder,\n  value,\n  index,\n  whichProp,\n  setCoordinates,\n  onClick\n}) => {\n  const [focus, setFocus] = useState<boolean>(false)\n  const [val, setVal] = useState<string>(value)\n  return (\n    <input\n      type=\"text\"\n      placeholder={placeholder}\n      value={val}\n      style={{\n        backgroundColor: \"#282434\",\n        outline: focus ? \"2px solid #ff3030\" : \"none\",\n        padding: \"10px\",\n        color: \"#ffffff\",\n        borderRadius: \"5px\",\n        border: \"none\",\n        fontSize: \"12px\",\n        margin: \"4px\",\n        boxSizing: \"border-box\",\n        width: \"9.9%\",\n      }}\n      onChange={(e) => {\n        setVal(e.target.value)\n        \n      }}\n      onFocus={() => setFocus(true)}\n      onBlur={() => setFocus(false)}\n    />\n  )\n}*/\n\nexport const TextInput: React.FC<InputProps> = ({\n  placeholder,\n  value,\n  whichProp,\n  onClick,\n}) => {\n  const [focus, setFocus] = useState<boolean>(false)\n  const [val, setVal] = useState<string>(value)\n  return (\n    <input\n      type=\"text\"\n      placeholder={placeholder}\n      value={val}\n      style={{\n        backgroundColor: \"#282434\",\n        outline: focus ? \"2px solid #ff3030\" : \"none\",\n        padding: \"10px\",\n        color: \"#ffffff\",\n        borderRadius: \"5px\",\n        border: \"none\",\n        fontSize: \"12px\",\n        margin: \"4px\",\n        boxSizing: \"border-box\",\n        width: \"9.9%\",\n      }}\n      onChange={(e) => {\n        e.persist()\n        setVal(e.target.value)\n        onClick(e.target.value, whichProp)\n      }}\n      onFocus={() => setFocus(true)}\n      onBlur={() => setFocus(false)}\n    />\n  )\n}\n",
         "import React from \"react\"\nimport { TextInput } from \"./Input\"\nimport { VertexData } from \"./LinePlacementPlot\"\n\ninterface TextFieldProps {\n  coords: VertexData\n  index: number\n  setCoordinates: React.Dispatch<React.SetStateAction<VertexData[]>>\n  setCoordinatesChanged: React.Dispatch<React.SetStateAction<boolean>>\n  setIndex: React.Dispatch<React.SetStateAction<number | undefined>>\n}\n\nexport const TextField: React.FC<TextFieldProps> = ({\n  coords,\n  index,\n  setCoordinates,\n  setCoordinatesChanged,\n  setIndex,\n}) => {\n  const handleClick = () => {\n    setIndex(undefined)\n    setCoordinates((coords) => {\n      const updatedCoords = [...coords]\n      updatedCoords.splice(index, 1)\n      setCoordinatesChanged(true)\n      return updatedCoords\n    })\n  }\n\n  const coordinateClick = (arg: string, whichProp: keyof VertexData): void => {\n    if (!isNaN(+arg)) {\n      const newCoord = +arg\n      setCoordinates((coords) => {\n        let coordRef: any = coords[index]\n        coordRef[whichProp] = newCoord\n        coords[index] = coordRef\n        setCoordinatesChanged(true)\n        return [...coords]\n      })\n    }\n  }\n\n  const textClick = (arg: string, whichProp: keyof VertexData): void => {\n    setCoordinates((coords) => {\n      const newVal = arg\n      console.log(newVal)\n      let coordRef: any = coords[index]\n      coordRef[whichProp] = newVal\n      coords[index] = coordRef\n      setCoordinatesChanged(true)\n      return [...coords]\n    })\n  }\n  return (\n    <div>\n      <TextInput\n        placeholder=\"Name\"\n        value={coords.name}\n        whichProp={\"name\"}\n        onClick={textClick}\n      />\n      <TextInput\n        placeholder=\"Direction 1\"\n        value={coords.dir1}\n        whichProp={\"dir1\"}\n        onClick={textClick}\n      />\n\n      <TextInput\n        placeholder=\"Direction 2\"\n        value={coords.dir2}\n        whichProp={\"dir2\"}\n        onClick={textClick}\n      />\n      <TextInput\n        placeholder=\"First X-coordinate\"\n        value={String(coords.x1)}\n        whichProp={\"x1\"}\n        onClick={coordinateClick}\n      />\n      <TextInput\n        placeholder=\"First Y-coordinate\"\n        value={String(coords.y1)}\n        whichProp={\"y1\"}\n        onClick={coordinateClick}\n      />\n      <TextInput\n        placeholder=\"Second X-coordinate\"\n        value={String(coords.x2)}\n        whichProp={\"x2\"}\n        onClick={coordinateClick}\n      />\n      <TextInput\n        placeholder=\"Second Y-coordinate\"\n        value={String(coords.y2)}\n        whichProp={\"y2\"}\n        onClick={coordinateClick}\n      />\n      <button\n        onClick={handleClick}\n        style={{\n          backgroundColor: \"#282434\",\n          outline: \"none\",\n          padding: \"10px\",\n          color: \"#ffffff\",\n          borderRadius: \"5px\",\n          border: \"none\",\n          fontSize: \"12px\",\n          margin: \"4px\",\n          boxSizing: \"border-box\",\n          width: \"5%\",\n        }}\n      >\n        X\n      </button>\n    </div>\n  )\n}\n",
-        "import { Streamlit } from \"streamlit-component-lib\"\nimport { useRenderData } from \"streamlit-component-lib-react-hooks\"\nimport React, { useState, useEffect } from \"react\"\nimport Vertex from \"./Vertex\"\nimport { TextField } from \"./TextField\"\n\nexport interface VertexData {\n  id: string\n  name: string\n  dir1: string\n  dir2: string\n  x1: number\n  y1: number\n  x2: number\n  y2: number\n}\n\nfunction equal(vertex1: VertexData, vertex2: VertexData): boolean {\n  return (\n    vertex1.id === vertex2.id &&\n    vertex1.name === vertex2.name &&\n    vertex1.dir1 === vertex2.dir1 &&\n    vertex1.dir2 === vertex2.dir2 &&\n    vertex1.x1 === vertex2.x1 &&\n    vertex1.y1 === vertex2.y1 &&\n    vertex1.x2 === vertex2.x2 &&\n    vertex1.y2 === vertex2.y2\n  )\n}\n\nfunction contains(data: VertexData, arr: VertexData[]): boolean {\n  return arr.some((otherData) => equal(data, otherData))\n}\n\nexport function calcVertexId(vertex: VertexData): string {\n  return `${vertex.x1}${vertex.y1}${vertex.x2}${vertex.y2}${vertex.name}${vertex.dir1}${vertex.dir2}`\n}\n\nconst LinePlacementPlot: React.VFC = () => {\n  // \"useRenderData\" returns the renderData passed from Python.\n  const renderData = useRenderData()\n  const [coordinates, setCoordinates] = useState<VertexData[]>([])\n  const [vertices, setVertices] = useState<JSX.Element[]>([])\n  const [selectedIndex, setSelectedIndex] = useState<number | undefined>()\n  const colors = [\"red\", \"green\", \"blue\", \"yellow\", \"pink\"]\n  const img = renderData.args[\"image\"]\n  const WIDTH = renderData.args[\"width\"]\n  const HEIGHT = renderData.args[\"height\"]\n  const [key, setKey] = useState<number>(renderData.args[\"key\"])\n  const changed = renderData.args[\"changed\"]\n  let colorIndex = 0\n  const [coordinatesChanged, setCoordinatesChanged] = useState(false)\n\n  function reduceVertexArrays(arr1: VertexData[], arr2: VertexData[]) {\n    const resArray: VertexData[] = key === changed ? arr1 : arr2\n    return resArray.map((data) => {\n      return { ...data, id: calcVertexId(data) }\n    })\n  }\n\n  let firstClick: [number, number] | null = null\n\n  useEffect(() => {\n    const handleKeyDown = (event: KeyboardEvent) => {\n      if ((event.ctrlKey || event.metaKey) && event.key === \"z\") {\n        setSelectedIndex(undefined)\n        setCoordinates((coords) => {\n          const arr = coords.slice(0, -1)\n          Streamlit.setComponentValue(arr)\n          return arr\n        })\n        setCoordinatesChanged(true)\n      }\n      if (event.key === \"Enter\") {\n        setSelectedIndex(undefined)\n      }\n    }\n\n    window.addEventListener(\"keydown\", handleKeyDown)\n  }, [])\n\n  useEffect(() => {\n    const renderArgs = () => {\n      const args: VertexData[] = renderData.args[\"lines\"]\n      console.log(args)\n      setCoordinates((coords) => reduceVertexArrays(coords, args))\n    }\n    renderArgs()\n  }, [renderData.args])\n\n  useEffect(() => {\n    const updateVertices = () => {\n      const verticesArray: JSX.Element[] = []\n      for (let i = 0; i < coordinates.length; i++) {\n        const data = coordinates[i]\n        verticesArray.push(\n          <Vertex\n            data={data}\n            index={i}\n            setIndex={setSelectedIndex}\n            color={colors[colorIndex]}\n            key={`vertex_${data.id}}`}\n          />\n        )\n        colorIndex = (colorIndex + 1) % colors.length\n      }\n      setVertices(verticesArray)\n      if (coordinatesChanged) {\n        Streamlit.setComponentValue(coordinates)\n        setCoordinatesChanged(false)\n      }\n    }\n    updateVertices()\n  }, [coordinates])\n\n  const getClickCoords = (event: {\n    target: any\n    clientX: number\n    clientY: number\n  }) => {\n    var e = event.target\n    var dim = e.getBoundingClientRect()\n    var x = event.clientX - dim.left\n    var y = event.clientY - dim.top\n    return [x, y]\n  }\n\n  const click = (event: any) => {\n    const [x, y] = getClickCoords(event)\n    if (firstClick === null) {\n      firstClick = [x, y]\n    } else {\n      const [x1, y1] = firstClick\n      const nextCoord: VertexData = {\n        x1: x1,\n        y1: y1,\n        x2: x,\n        y2: y,\n        name: `Vertex ${vertices.length}`,\n        dir1: \"Up\",\n        dir2: \"Down\",\n        id: `${x1}${y1}${x}${y}${`Vertex ${vertices.length}`}${\"Up\"}${\"Down\"}`,\n      }\n      if (key === changed) setCoordinates((coords) => [...coords, nextCoord])\n      setCoordinatesChanged(true)\n      colorIndex = (colorIndex + 1) % colors.length\n      firstClick = null\n    }\n  }\n\n  return (\n    <div\n      style={{\n        display: \"flex\",\n        flexDirection: \"column\",\n      }}\n    >\n      <div\n        style={{\n          width: WIDTH,\n          height: HEIGHT,\n          backgroundImage: `url(${img})`,\n          backgroundPosition: \"center\",\n          backgroundSize: \"100%\",\n          position: \"relative\",\n          display: \"inline-block\",\n        }}\n        onClick={(event) => {\n          if (selectedIndex === undefined) click(event)\n        }}\n      >\n        <svg width={WIDTH} height={HEIGHT}>\n          {vertices}\n        </svg>\n      </div>\n      <div>\n        {key === changed ? (\n          selectedIndex !== undefined ? (\n            <TextField\n              coords={coordinates[selectedIndex]}\n              index={selectedIndex}\n              setCoordinates={setCoordinates}\n              setCoordinatesChanged={setCoordinatesChanged}\n              setIndex={setSelectedIndex}\n            ></TextField>\n          ) : (\n            <div style={{ display: \"flex\", maxWidth: WIDTH, flexWrap: \"wrap\" }}>\n              {coordinates.map((data, index) => (\n                <h4\n                  style={{\n                    backgroundColor: \"#282434\",\n                    outline: \"none\",\n                    padding: \"10px\",\n                    color: \"#ffffff\",\n                    borderRadius: \"5px\",\n                    border: \"none\",\n                    fontSize: \"12px\",\n                    margin: \"4px\",\n                    boxSizing: \"border-box\",\n                    width: WIDTH / 8,\n                    fontFamily: \"sans-serif\",\n                    fontWeight: 10,\n                  }}\n                  onClick={() => setSelectedIndex(index)}\n                  key={`name_${data.id}`}\n                >\n                  {data.name}\n                </h4>\n              ))}\n            </div>\n          )\n        ) : (\n          <></>\n        )}\n      </div>\n    </div>\n  )\n}\n\nexport default LinePlacementPlot\n",
+        "import { Streamlit } from \"streamlit-component-lib\"\nimport { useRenderData } from \"streamlit-component-lib-react-hooks\"\nimport React, { useState, useEffect } from \"react\"\nimport Vertex from \"./Vertex\"\nimport { TextField } from \"./TextField\"\nimport image from \"./assets/ground.png\"\n\nexport interface VertexData {\n  id: string\n  name: string\n  dir1: string\n  dir2: string\n  x1: number\n  y1: number\n  x2: number\n  y2: number\n}\n\nfunction equal(vertex1: VertexData, vertex2: VertexData): boolean {\n  return (\n    vertex1.id === vertex2.id &&\n    vertex1.name === vertex2.name &&\n    vertex1.dir1 === vertex2.dir1 &&\n    vertex1.dir2 === vertex2.dir2 &&\n    vertex1.x1 === vertex2.x1 &&\n    vertex1.y1 === vertex2.y1 &&\n    vertex1.x2 === vertex2.x2 &&\n    vertex1.y2 === vertex2.y2\n  )\n}\n\nfunction contains(data: VertexData, arr: VertexData[]): boolean {\n  return arr.some((otherData) => equal(data, otherData))\n}\n\nexport function calcVertexId(vertex: VertexData): string {\n  return `${vertex.x1}${vertex.y1}${vertex.x2}${vertex.y2}${vertex.name}${vertex.dir1}${vertex.dir2}`\n}\n\nconst LinePlacementPlot: React.VFC = () => {\n  // \"useRenderData\" returns the renderData passed from Python.\n  const renderData = useRenderData()\n  const [coordinates, setCoordinates] = useState<VertexData[]>([])\n  const [vertices, setVertices] = useState<JSX.Element[]>([])\n  const [selectedIndex, setSelectedIndex] = useState<number | undefined>()\n  const colors = [\"red\", \"green\", \"blue\", \"yellow\", \"pink\"]\n  const img = renderData.args[\"image\"]\n  const WIDTH = renderData.args[\"width\"]\n  const HEIGHT = renderData.args[\"height\"]\n  const [key, setKey] = useState<number>(renderData.args[\"key\"])\n  const changed = renderData.args[\"changed\"]\n  let colorIndex = 0\n  const [coordinatesChanged, setCoordinatesChanged] = useState(false)\n\n  function reduceVertexArrays(arr1: VertexData[], arr2: VertexData[]) {\n    const resArray: VertexData[] = key === changed ? arr1 : arr2\n    return resArray.map((data) => {\n      return { ...data, id: calcVertexId(data) }\n    })\n  }\n\n  let firstClick: [number, number] | null = null\n\n  useEffect(() => {\n    const handleKeyDown = (event: KeyboardEvent) => {\n      if ((event.ctrlKey || event.metaKey) && event.key === \"z\") {\n        setSelectedIndex(undefined)\n        setCoordinates((coords) => {\n          const arr = coords.slice(0, -1)\n          Streamlit.setComponentValue(arr)\n          return arr\n        })\n        setCoordinatesChanged(true)\n      }\n      if (event.key === \"Enter\") {\n        setSelectedIndex(undefined)\n      }\n    }\n\n    window.addEventListener(\"keydown\", handleKeyDown)\n  }, [])\n\n  useEffect(() => {\n    const renderArgs = () => {\n      const args: VertexData[] = renderData.args[\"lines\"]\n      console.log(args)\n      setCoordinates((coords) => reduceVertexArrays(coords, args))\n    }\n    renderArgs()\n  }, [renderData.args])\n\n  useEffect(() => {\n    const updateVertices = () => {\n      const verticesArray: JSX.Element[] = []\n      for (let i = 0; i < coordinates.length; i++) {\n        const data = coordinates[i]\n        verticesArray.push(\n          <Vertex\n            data={data}\n            index={i}\n            setIndex={setSelectedIndex}\n            color={colors[colorIndex]}\n            key={`vertex_${data.id}}`}\n          />\n        )\n        colorIndex = (colorIndex + 1) % colors.length\n      }\n      setVertices(verticesArray)\n      if (coordinatesChanged) {\n        Streamlit.setComponentValue(coordinates)\n        setCoordinatesChanged(false)\n      }\n    }\n    updateVertices()\n  }, [coordinates])\n\n  const getClickCoords = (event: {\n    target: any\n    clientX: number\n    clientY: number\n  }) => {\n    var e = event.target\n    var dim = e.getBoundingClientRect()\n    var x = event.clientX - dim.left\n    var y = event.clientY - dim.top\n    return [x, y]\n  }\n\n  const click = (event: any) => {\n    const [x, y] = getClickCoords(event)\n    if (firstClick === null) {\n      firstClick = [x, y]\n    } else {\n      const [x1, y1] = firstClick\n      const nextCoord: VertexData = {\n        x1: x1,\n        y1: y1,\n        x2: x,\n        y2: y,\n        name: `Vertex ${vertices.length}`,\n        dir1: \"Up\",\n        dir2: \"Down\",\n        id: `${x1}${y1}${x}${y}${`Vertex ${vertices.length}`}${\"Up\"}${\"Down\"}`,\n      }\n      if (key === changed) setCoordinates((coords) => [...coords, nextCoord])\n      setCoordinatesChanged(true)\n      colorIndex = (colorIndex + 1) % colors.length\n      firstClick = null\n    }\n  }\n\n  return (\n    <div\n      style={{\n        display: \"flex\",\n        flexDirection: \"column\",\n      }}\n    >\n      <div\n        style={{\n          width: WIDTH,\n          height: HEIGHT,\n          backgroundImage: `url(${img})`,\n          backgroundSize: \"cover\",\n          overflow: \"hidden\",\n          position: \"relative\",\n          display: \"inline-block\",\n        }}\n        onClick={(event) => {\n          if (selectedIndex === undefined) click(event)\n        }}\n      >\n        <svg width={WIDTH} height={HEIGHT}>\n          {vertices}\n        </svg>\n      </div>\n      <div>\n        {key === changed ? (\n          selectedIndex !== undefined ? (\n            <TextField\n              coords={coordinates[selectedIndex]}\n              index={selectedIndex}\n              setCoordinates={setCoordinates}\n              setCoordinatesChanged={setCoordinatesChanged}\n              setIndex={setSelectedIndex}\n            ></TextField>\n          ) : (\n            <div style={{ display: \"flex\", maxWidth: WIDTH, flexWrap: \"wrap\" }}>\n              {coordinates.map((data, index) => (\n                <h4\n                  style={{\n                    backgroundColor: \"#282434\",\n                    outline: \"none\",\n                    padding: \"10px\",\n                    color: \"#ffffff\",\n                    borderRadius: \"5px\",\n                    border: \"none\",\n                    fontSize: \"12px\",\n                    margin: \"4px\",\n                    boxSizing: \"border-box\",\n                    width: WIDTH / 8,\n                    fontFamily: \"sans-serif\",\n                    fontWeight: 10,\n                  }}\n                  onClick={() => setSelectedIndex(index)}\n                  key={`name_${data.id}`}\n                >\n                  {data.name}\n                </h4>\n              ))}\n            </div>\n          )\n        ) : (\n          <></>\n        )}\n      </div>\n    </div>\n  )\n}\n\nexport default LinePlacementPlot\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport { StreamlitProvider } from \"streamlit-component-lib-react-hooks\"\nimport LinePlacementPlot from \"./LinePlacementPlot\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <StreamlitProvider>\n      <LinePlacementPlot />\n    </StreamlitProvider>\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n",
         "\"use strict\";\nvar __importDefault = (this && this.__importDefault) || function (mod) {\n    return (mod && mod.__esModule) ? mod : { \"default\": mod };\n};\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.useNullableRenderData = exports.StreamlitProvider = exports.useRenderData = void 0;\nvar StreamlitProvider_1 = require(\"./StreamlitProvider\");\nObject.defineProperty(exports, \"useRenderData\", { enumerable: true, get: function () { return StreamlitProvider_1.useRenderData; } });\nObject.defineProperty(exports, \"StreamlitProvider\", { enumerable: true, get: function () { return __importDefault(StreamlitProvider_1).default; } });\nvar useNullableRenderData_1 = require(\"./useNullableRenderData\");\nObject.defineProperty(exports, \"useNullableRenderData\", { enumerable: true, get: function () { return useNullableRenderData_1.useNullableRenderData; } });\n"
     ],
     "version": 3
 }
```

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.8/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `st_line_plotter-0.0.9/st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `st_line_plotter-0.0.8/st_line_plotter.egg-info/SOURCES.txt` & `st_line_plotter-0.0.9/st_line_plotter.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 st_line_plotter.egg-info/PKG-INFO
 st_line_plotter.egg-info/SOURCES.txt
 st_line_plotter.egg-info/dependency_links.txt
 st_line_plotter.egg-info/requires.txt
 st_line_plotter.egg-info/top_level.txt
 st_line_plotter/frontend/build/asset-manifest.json
 st_line_plotter/frontend/build/index.html
-st_line_plotter/frontend/build/precache-manifest.dca2b6b2012232a6d569502759b645c6.js
+st_line_plotter/frontend/build/precache-manifest.6279477322d7616ea3eaabbcb4ce811d.js
 st_line_plotter/frontend/build/service-worker.js
 st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js
 st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.LICENSE.txt
 st_line_plotter/frontend/build/static/js/2.eb731a1a.chunk.js.map
-st_line_plotter/frontend/build/static/js/main.e5ec0f99.chunk.js
-st_line_plotter/frontend/build/static/js/main.e5ec0f99.chunk.js.map
+st_line_plotter/frontend/build/static/js/main.a9c05652.chunk.js
+st_line_plotter/frontend/build/static/js/main.a9c05652.chunk.js.map
 st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js
 st_line_plotter/frontend/build/static/js/runtime-main.11ec9aca.js.map
```

