# Comparing `tmp/atila_vue-0.3.0-py3-none-any.whl.zip` & `tmp/atila_vue-0.3.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 355875 bytes, number of entries: 43
--rw-r--r--  2.0 unx     8312 b- defN 23-Jun-19 04:42 atila_vue/__init__.py
+Zip file size: 355891 bytes, number of entries: 43
+-rw-r--r--  2.0 unx     8288 b- defN 23-Jun-19 06:43 atila_vue/__init__.py
 -rw-rw-r--  2.0 unx   110548 b- defN 21-Nov-28 08:59 atila_vue/static/favicon.ico
 -rw-r--r--  2.0 unx      773 b- defN 23-Jun-18 15:45 atila_vue/static/manifest.json
 -rw-rw-r--  2.0 unx       81 b- defN 21-Nov-28 08:59 atila_vue/static/robots.txt
 -rw-rw-r--  2.0 unx     5924 b- defN 21-Nov-28 08:59 atila_vue/static/sw.js
 -rw-r--r--  2.0 unx     1740 b- defN 23-Jun-19 00:16 atila_vue/static/atila-vue/components/dev/vuex-state.vue
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-18 15:45 atila_vue/static/atila-vue/css/custom.css
 -rw-r--r--  2.0 unx     1026 b- defN 23-Jun-18 15:45 atila_vue/static/atila-vue/etc/offline.html
@@ -33,13 +33,13 @@
 -rw-rw-r--  2.0 unx    12568 b- defN 21-Nov-28 08:59 atila_vue/static/vue/helpers.js
 -rw-rw-r--  2.0 unx      814 b- defN 21-Nov-28 08:59 atila_vue/templates/__framework/bs5.j2
 -rw-r--r--  2.0 unx     1986 b- defN 22-Sep-29 07:59 atila_vue/templates/__framework/html.j2
 -rw-r--r--  2.0 unx    10390 b- defN 22-Sep-29 07:59 atila_vue/templates/__framework/vue.j2
 -rw-r--r--  2.0 unx      812 b- defN 23-Jun-18 15:45 atila_vue/templates/atila-vue/bs5.j2
 -rw-r--r--  2.0 unx     2079 b- defN 23-Jun-18 15:45 atila_vue/templates/atila-vue/html.j2
 -rw-r--r--  2.0 unx    12772 b- defN 23-Jun-19 02:38 atila_vue/templates/atila-vue/vue.j2
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-19 05:55 atila_vue-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    14928 b- defN 23-Jun-19 05:55 atila_vue-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 05:55 atila_vue-0.3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-19 05:55 atila_vue-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4091 b- defN 23-Jun-19 05:55 atila_vue-0.3.0.dist-info/RECORD
-43 files, 534366 bytes uncompressed, 349185 bytes compressed:  34.7%
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-19 06:43 atila_vue-0.3.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14930 b- defN 23-Jun-19 06:43 atila_vue-0.3.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 06:43 atila_vue-0.3.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-19 06:43 atila_vue-0.3.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4101 b- defN 23-Jun-19 06:43 atila_vue-0.3.0.1.dist-info/RECORD
+43 files, 534354 bytes uncompressed, 349181 bytes compressed:  34.7%
```

## zipnote {}

```diff
@@ -108,23 +108,23 @@
 
 Filename: atila_vue/templates/atila-vue/html.j2
 Comment: 
 
 Filename: atila_vue/templates/atila-vue/vue.j2
 Comment: 
 
-Filename: atila_vue-0.3.0.dist-info/LICENSE
+Filename: atila_vue-0.3.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: atila_vue-0.3.0.dist-info/METADATA
+Filename: atila_vue-0.3.0.1.dist-info/METADATA
 Comment: 
 
-Filename: atila_vue-0.3.0.dist-info/WHEEL
+Filename: atila_vue-0.3.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: atila_vue-0.3.0.dist-info/top_level.txt
+Filename: atila_vue-0.3.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: atila_vue-0.3.0.dist-info/RECORD
+Filename: atila_vue-0.3.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atila_vue/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.0"
+__version__ = "0.3.0.1"
 
 import os
 import json
 import atila
 import skitai
 from skitai.wastuff.api import ISODateTimeWithOffsetEncoder
 import re
@@ -138,15 +138,14 @@
                     context.push (vue_path) # server push
                 else:
                     pathes.append (vue_path) # prefetch
             routes_list = ",\n ".join (routes)
             return routes_list, pathes, bases
 
         def validate_routes (bases):
-            print (bases)
             match = False
             current_uri = context.request.split_uri () [0]
             if current_uri == '/':
                 match = True
             elif bases == {'/'}:
                 match = True
             else:
```

## Comparing `atila_vue-0.3.0.dist-info/LICENSE` & `atila_vue-0.3.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `atila_vue-0.3.0.dist-info/METADATA` & `atila_vue-0.3.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atila-vue
-Version: 0.3.0
+Version: 0.3.0.1
 Summary: Atila Extension For VueJS 2 SFC and SSR
 Home-page: https://gitlab.com/atila-ext/atila-vue
 Author: Hans Roh
 Author-email: hansroh@gmail.com
 License: MIT
 Download-URL: https://pypi.python.org/pypi/atila-vue
 Platform: posix
```

## Comparing `atila_vue-0.3.0.dist-info/RECORD` & `atila_vue-0.3.0.1.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-atila_vue/__init__.py,sha256=hP2dRTCJwKEjt2LFyyFPfVWs2bZKXKolsNs8W_L1xoE,8312
+atila_vue/__init__.py,sha256=mW36Q4dVJws4phJNPG5Bf7ibWEfAoSfKwgWIU7uKH0g,8288
 atila_vue/static/favicon.ico,sha256=Y81o7R-VsIsKR1-F1O6LZIP8B-X9GncO9BngbEvrwcw,110548
 atila_vue/static/manifest.json,sha256=GOfB4apelzs8PQItmvkYy1f47ZcsrZ8b5BvctI9DxWw,773
 atila_vue/static/robots.txt,sha256=I4VYY4dr1_Xswh2N9qv392fczzep-zSs8V2DMoKvRyM,81
 atila_vue/static/sw.js,sha256=90ts70g0XSyoPG-V7XpyJVYKJb8lO-BivqvzeoicwgE,5924
 atila_vue/static/atila-vue/components/dev/vuex-state.vue,sha256=AqvqCbe-lDYzgy0iW-ZnFuFQjnK9lu8fkErsLgSgk0A,1740
 atila_vue/static/atila-vue/css/custom.css,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atila_vue/static/atila-vue/etc/offline.html,sha256=-BFXmTWjrbH7ECBeEvxbsVFNFUs0sBRnMP4__v0AZV8,1026
@@ -32,12 +32,12 @@
 atila_vue/static/vue/helpers.js,sha256=1czmQ-8F1vDCrPlvDufq8aqp62Z4ws-AZNPLPZJ_lO0,12568
 atila_vue/templates/__framework/bs5.j2,sha256=ET-On4rK-A98N2T86wFV0n43WucnmdAzBSej4c5rvo0,814
 atila_vue/templates/__framework/html.j2,sha256=XMPR3Jx0WcsMMm1fZxwVOBqWwEOoGqzZiFCVS9lmulY,1986
 atila_vue/templates/__framework/vue.j2,sha256=VepM740z4y_eSVQ71cx7_ENpybAPlC-jyp0nuBPKAjA,10390
 atila_vue/templates/atila-vue/bs5.j2,sha256=kXe28z-jYQYuJR28SlMoqRDH4QByscrhzlQFR5ukcgw,812
 atila_vue/templates/atila-vue/html.j2,sha256=1fNoZz7PRM8pLGVAm3MSkpA8ukQX3Wvy5l30AZk6gs8,2079
 atila_vue/templates/atila-vue/vue.j2,sha256=WFVLU8OsA9L12VVRdNFW0gO5yg55rMpHJofMESI1W3M,12772
-atila_vue-0.3.0.dist-info/LICENSE,sha256=iuQpb5TfQxJBqC5J_NcWavJzOw8bJCUpUjGg2CdjvPc,1083
-atila_vue-0.3.0.dist-info/METADATA,sha256=LC8wLKlZoaK5KUm_x4CH6JmottAR2awZgL1vOYdYMyo,14928
-atila_vue-0.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-atila_vue-0.3.0.dist-info/top_level.txt,sha256=z_R5CB27SfinABw2rSw7XAz1sGrDfbUQ9EEVwiAqb9k,10
-atila_vue-0.3.0.dist-info/RECORD,,
+atila_vue-0.3.0.1.dist-info/LICENSE,sha256=iuQpb5TfQxJBqC5J_NcWavJzOw8bJCUpUjGg2CdjvPc,1083
+atila_vue-0.3.0.1.dist-info/METADATA,sha256=ZjlLvAz3PdIIjf2bEl3TVvdrj5iF4O1Pm7dZV3Rsj0I,14930
+atila_vue-0.3.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+atila_vue-0.3.0.1.dist-info/top_level.txt,sha256=z_R5CB27SfinABw2rSw7XAz1sGrDfbUQ9EEVwiAqb9k,10
+atila_vue-0.3.0.1.dist-info/RECORD,,
```

