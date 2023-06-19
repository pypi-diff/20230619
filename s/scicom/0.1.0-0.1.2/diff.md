# Comparing `tmp/scicom-0.1.0.tar.gz` & `tmp/scicom-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicom-0.1.0.tar", last modified: Wed May 17 13:12:39 2023, max compression
+gzip compressed data, was "scicom-0.1.2.tar", last modified: Mon Jun 19 13:52:16 2023, max compression
```

## Comparing `scicom-0.1.0.tar` & `scicom-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      232 2023-05-04 13:08:18.000000 scicom-0.1.0/AUTHORS.rst
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1086 2022-01-06 13:40:40.000000 scicom-0.1.0/LICENSE.md
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)       28 2023-05-08 08:24:28.000000 scicom-0.1.0/MANIFEST.in
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2448 2023-05-17 13:12:39.769400 scicom-0.1.0/PKG-INFO
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1670 2023-01-16 10:15:23.000000 scicom-0.1.0/README.md
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      104 2021-09-30 09:13:37.000000 scicom-0.1.0/pyproject.toml
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1011 2023-05-17 13:12:39.769400 scicom-0.1.0/setup.cfg
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.765400 scicom-0.1.0/src/
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.765400 scicom-0.1.0/src/scicom/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 09:13:37.000000 scicom-0.1.0/src/scicom/__init__.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/src/scicom/data/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)    22954 2023-05-17 13:09:30.000000 scicom-0.1.0/src/scicom/data/agentsCoordinates.geojson
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)   327135 2023-05-08 08:24:28.000000 scicom-0.1.0/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     7225 2023-05-08 08:24:28.000000 scicom-0.1.0/src/scicom/data/relPop_plosOne.csv
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)    73605 2023-05-08 08:24:28.000000 scicom-0.1.0/src/scicom/data/relativePopulation_1650.csv
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/src/scicom/historicalletters/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2023-05-04 12:33:04.000000 scicom-0.1.0/src/scicom/historicalletters/__init__.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     7915 2023-05-17 09:50:10.000000 scicom-0.1.0/src/scicom/historicalletters/agents.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     4148 2023-05-15 09:22:32.000000 scicom-0.1.0/src/scicom/historicalletters/model.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2293 2023-05-15 09:25:08.000000 scicom-0.1.0/src/scicom/historicalletters/server.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2661 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/historicalletters/space.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1257 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/historicalletters/util.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/src/scicom/randomletters/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1206 2023-05-04 12:39:24.000000 scicom-0.1.0/src/scicom/randomletters/SimpleContinuousModule.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 09:13:37.000000 scicom-0.1.0/src/scicom/randomletters/__init__.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     4837 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/randomletters/agents.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2723 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/randomletters/model.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     3197 2023-05-15 09:09:27.000000 scicom-0.1.0/src/scicom/randomletters/server.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      610 2023-05-04 12:51:27.000000 scicom-0.1.0/src/scicom/run.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-05-17 13:12:39.769400 scicom-0.1.0/src/scicom.egg-info/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2448 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/PKG-INFO
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      871 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/SOURCES.txt
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        1 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/dependency_links.txt
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      111 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/requires.txt
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        7 2023-05-17 13:12:39.000000 scicom-0.1.0/src/scicom.egg-info/top_level.txt
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-06-19 13:52:16.965670 scicom-0.1.2/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      232 2023-05-04 13:08:18.000000 scicom-0.1.2/AUTHORS.rst
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1086 2022-01-06 13:40:40.000000 scicom-0.1.2/LICENSE.md
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)       28 2023-05-08 08:24:28.000000 scicom-0.1.2/MANIFEST.in
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2448 2023-06-19 13:52:16.965670 scicom-0.1.2/PKG-INFO
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1670 2023-01-16 10:15:23.000000 scicom-0.1.2/README.md
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      104 2021-09-30 09:13:37.000000 scicom-0.1.2/pyproject.toml
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1011 2023-06-19 13:52:16.965670 scicom-0.1.2/setup.cfg
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-06-19 13:52:16.961670 scicom-0.1.2/src/
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-06-19 13:52:16.961670 scicom-0.1.2/src/scicom/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 09:13:37.000000 scicom-0.1.2/src/scicom/__init__.py
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-06-19 13:52:16.965670 scicom-0.1.2/src/scicom/data/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)    22934 2023-06-19 13:49:27.000000 scicom-0.1.2/src/scicom/data/agentsCoordinates.geojson
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)   327135 2023-05-08 08:24:28.000000 scicom-0.1.2/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     7225 2023-05-08 08:24:28.000000 scicom-0.1.2/src/scicom/data/relPop_plosOne.csv
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)    73605 2023-05-08 08:24:28.000000 scicom-0.1.2/src/scicom/data/relativePopulation_1650.csv
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-06-19 13:52:16.965670 scicom-0.1.2/src/scicom/historicalletters/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2023-05-04 12:33:04.000000 scicom-0.1.2/src/scicom/historicalletters/__init__.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     8540 2023-06-19 13:30:25.000000 scicom-0.1.2/src/scicom/historicalletters/agents.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     6586 2023-06-19 13:28:27.000000 scicom-0.1.2/src/scicom/historicalletters/model.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2539 2023-06-19 13:46:44.000000 scicom-0.1.2/src/scicom/historicalletters/server.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2661 2023-05-15 09:09:27.000000 scicom-0.1.2/src/scicom/historicalletters/space.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1257 2023-05-15 09:09:27.000000 scicom-0.1.2/src/scicom/historicalletters/util.py
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-06-19 13:52:16.965670 scicom-0.1.2/src/scicom/randomletters/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1206 2023-05-04 12:39:24.000000 scicom-0.1.2/src/scicom/randomletters/SimpleContinuousModule.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 09:13:37.000000 scicom-0.1.2/src/scicom/randomletters/__init__.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     4837 2023-05-15 09:09:27.000000 scicom-0.1.2/src/scicom/randomletters/agents.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2723 2023-05-15 09:09:27.000000 scicom-0.1.2/src/scicom/randomletters/model.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     3197 2023-05-15 09:09:27.000000 scicom-0.1.2/src/scicom/randomletters/server.py
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      610 2023-05-04 12:51:27.000000 scicom-0.1.2/src/scicom/run.py
+drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2023-06-19 13:52:16.961670 scicom-0.1.2/src/scicom.egg-info/
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2448 2023-06-19 13:52:16.000000 scicom-0.1.2/src/scicom.egg-info/PKG-INFO
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      871 2023-06-19 13:52:16.000000 scicom-0.1.2/src/scicom.egg-info/SOURCES.txt
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        1 2023-06-19 13:52:16.000000 scicom-0.1.2/src/scicom.egg-info/dependency_links.txt
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      111 2023-06-19 13:52:16.000000 scicom-0.1.2/src/scicom.egg-info/requires.txt
+-rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        7 2023-06-19 13:52:16.000000 scicom-0.1.2/src/scicom.egg-info/top_level.txt
```

### Comparing `scicom-0.1.0/LICENSE.md` & `scicom-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/PKG-INFO` & `scicom-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scicom
-Version: 0.1.0
+Version: 0.1.2
 Summary: Simulating various aspects of scientific communication via Agent-based models.
 Home-page: https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels
 Author: Bernardo S. Buarque, Malte Vogl
 Author-email: bsbuarque@mpiwg-berlin.mpg.de, mvogl@mpiwg-berlin.mpg.de
 Project-URL: Project Home, https://modelsen.mpiwg-berlin.mpg.de
 Project-URL: Bug Tracker, https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scicom-0.1.0/README.md` & `scicom-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/setup.cfg` & `scicom-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scicom
-version = 0.1.0
+version = 0.1.2
 author = Bernardo S. Buarque, Malte Vogl
 author_email = bsbuarque@mpiwg-berlin.mpg.de, mvogl@mpiwg-berlin.mpg.de
 description = Simulating various aspects of scientific communication via Agent-based models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels
 project_urls =
```

### Comparing `scicom-0.1.0/src/scicom/data/agentsCoordinates.geojson` & `scicom-0.1.2/src/scicom/data/agentsCoordinates.geojson`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9932638888888888%*

 * *Differences: {"'features'": "{0: {'geometry': {'coordinates': [11.8767611, 45.4064349]}}, 1: {'geometry': "*

 * *               "{'coordinates': [-2.58791, 51.454513]}}, 2: {'geometry': {'coordinates': [4.4667, "*

 * *               "51.0167]}}, 3: {'geometry': {'coordinates': [11.3426163, 44.494887]}}, 4: "*

 * *               "{'geometry': {'coordinates': [3.057256, 50.62925]}}, 5: {'geometry': "*

 * *               "{'coordinates': [11.3426163, 44.494887]}}, 6: {'geometry': {'coordinates': "*

 * *               "[2.575986, 44.349389]}}, 7: { […]*

```diff
@@ -1,690 +1,690 @@
 {
     "features": [
         {
             "geometry": {
                 "coordinates": [
-                    2.0807123,
-                    49.4295387
+                    11.8767611,
+                    45.4064349
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P0"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.89779,
-                    48.3705449
+                    -2.58791,
+                    51.454513
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P1"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    7.6261347,
-                    51.9606649
+                    4.4667,
+                    51.0167
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P2"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.946256,
-                    44.4056499
+                    11.3426163,
+                    44.494887
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P3"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.0226511,
-                    45.133249
+                    3.057256,
+                    50.62925
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P4"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    2.8779388,
-                    50.8492265
+                    11.3426163,
+                    44.494887
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P5"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.0471788,
-                    52.2799112
+                    2.575986,
+                    44.349389
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P6"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    3.3879338,
-                    50.6056475
+                    9.6929845,
+                    45.0526206
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P7"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    3.7174243,
-                    51.0543422
+                    2.3522219,
+                    48.856614
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P8"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    2.8779388,
-                    50.8492265
+                    11.8796336,
+                    43.4632839
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P9"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.0226511,
-                    45.133249
+                    10.9200867,
+                    44.6488366
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P10"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    11.4516022,
-                    53.8979416
+                    3.057256,
+                    50.62925
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P11"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    11.3426163,
-                    44.494887
+                    10.0226511,
+                    45.133249
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P12"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.9916215,
-                    45.4383842
+                    10.0226511,
+                    45.133249
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P13"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.946256,
-                    44.4056499
+                    11.8767611,
+                    45.4064349
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P14"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    9.1859243,
-                    45.4654219
+                    -0.57918,
+                    44.837789
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P15"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.89779,
-                    48.3705449
+                    10.3279036,
+                    44.801485
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P16"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    3.003078,
-                    43.184277
+                    11.3307574,
+                    43.318809
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P17"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -1.0872979,
-                    53.9599651
+                    9.2744485,
+                    45.5845001
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P18"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    6.0240539,
-                    47.237829
+                    3.215795,
+                    43.344233
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P19"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -1.519693,
-                    52.406822
+                    4.805528,
+                    43.949317
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P20"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    1.909251,
-                    47.902964
+                    -1.61778,
+                    54.978252
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P21"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -2.715974,
-                    52.056398
+                    3.28268,
+                    48.20065
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P22"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    12.3155151,
-                    45.4408474
+                    9.1859243,
+                    45.4654219
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P23"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    2.398782,
-                    47.081012
+                    2.3522219,
+                    48.856614
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P24"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.2118019,
-                    45.5415526
+                    -0.57918,
+                    44.837789
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P25"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.3279036,
-                    44.801485
+                    8.5226185,
+                    47.3908524
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P26"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.946256,
-                    44.4056499
+                    11.3426163,
+                    44.494887
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P27"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    6.9602786,
-                    50.937531
+                    11.2558136,
+                    43.7695604
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P28"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    9.1859243,
-                    45.4654219
+                    12.3155151,
+                    45.4408474
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P29"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    12.3155151,
-                    45.4408474
+                    -0.0947961,
+                    51.5038411
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P30"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -3.533899,
-                    50.718412
+                    10.3279036,
+                    44.801485
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P31"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    11.8767611,
-                    45.4064349
+                    12.0407312,
+                    44.2227398
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P32"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    5.724524,
-                    45.188529
+                    4.8719854,
+                    50.4673883
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P33"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    11.3426163,
-                    44.494887
+                    12.3155151,
+                    45.4408474
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P34"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -0.3367413,
-                    53.7456709
+                    6.1757156,
+                    49.1193089
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P35"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    3.7174243,
-                    51.0543422
+                    1.099971,
+                    49.443232
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P36"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    3.876716,
-                    43.610769
+                    -0.0947961,
+                    51.5038411
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P37"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.5226185,
-                    47.3908524
+                    2.3522219,
+                    48.856614
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P38"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.0471788,
-                    52.2799112
+                    9.7320104,
+                    52.3758916
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P39"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -0.612747,
-                    44.881793
+                    2.1486413,
+                    43.9250853
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P40"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -1.1581086,
-                    52.9547832
+                    10.0226511,
+                    45.133249
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P41"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -0.399752,
-                    54.283113
+                    6.0838868,
+                    50.7753455
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P42"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.4016888,
-                    43.7228386
+                    2.8779388,
+                    50.8492265
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P43"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    12.1016236,
-                    49.0134297
+                    -0.0947961,
+                    51.5038411
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P44"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    2.3522219,
-                    48.856614
+                    4.4667,
+                    51.0167
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P45"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    11.2558136,
-                    43.7695604
+                    -1.519693,
+                    52.406822
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P46"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    6.9602786,
-                    50.937531
+                    2.3522219,
+                    48.856614
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P47"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    2.8779388,
-                    50.8492265
+                    -0.0947961,
+                    51.5038411
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P48"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    2.3522219,
-                    48.856614
+                    -0.026577,
+                    52.97894
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P49"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    12.5695158,
-                    44.0678288
+                    11.8767611,
+                    45.4064349
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P50"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    1.444209,
-                    43.604652
+                    4.805528,
+                    43.949317
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P51"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    3.3879338,
-                    50.6056475
+                    11.8796336,
+                    43.4632839
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P52"
             },
             "type": "Feature"
@@ -701,250 +701,250 @@
                 "unique_id": "P53"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    12.3155151,
-                    45.4408474
+                    3.003078,
+                    43.184277
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P54"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    9.2744485,
-                    45.5845001
+                    12.0407312,
+                    44.2227398
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P55"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -0.612747,
-                    44.881793
+                    12.3155151,
+                    45.4408474
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P56"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    11.2558136,
-                    43.7695604
+                    12.2035294,
+                    44.4183598
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P57"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    11.3307574,
-                    43.318809
+                    8.105754,
+                    51.5711476
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P58"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    12.3155151,
-                    45.4408474
+                    11.2558136,
+                    43.7695604
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P59"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.50272,
-                    43.843078
+                    11.02988,
+                    50.984768
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P60"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -0.0947961,
-                    51.5038411
+                    10.9200867,
+                    44.6488366
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P61"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    11.4516022,
-                    53.8979416
+                    12.3155151,
+                    45.4408474
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P62"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    1.0789089,
-                    51.280233
+                    9.1859243,
+                    45.4654219
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P63"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    9.6929845,
-                    45.0526206
+                    4.835659,
+                    45.764043
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P64"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    9.1859243,
-                    45.4654219
+                    6.6371433,
+                    49.749992
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P65"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.9200867,
-                    44.6488366
+                    6.1757156,
+                    49.1193089
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P66"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -0.399752,
-                    54.283113
+                    1.858686,
+                    50.95129
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P67"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    3.003078,
-                    43.184277
+                    10.9916215,
+                    45.4383842
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P68"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -1.1397592,
-                    52.6368778
+                    13.0770347,
+                    54.3090654
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P69"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    0.68484,
-                    47.394144
+                    3.003078,
+                    43.184277
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P70"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -0.540579,
-                    53.230688
+                    11.3307574,
+                    43.318809
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P71"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.6296859,
-                    44.6989932
+                    9.1859243,
+                    45.4654219
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P72"
             },
             "type": "Feature"
@@ -961,81 +961,81 @@
                 "unique_id": "P73"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.8016937,
-                    53.0792962
+                    5.36978,
+                    43.296482
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P74"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.2472526,
-                    49.9928617
+                    12.3155151,
+                    45.4408474
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P75"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    6.0838868,
-                    50.7753455
+                    8.946256,
+                    44.4056499
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P76"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    2.353663,
-                    43.212161
+                    9.1732384,
+                    47.6779496
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P77"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    3.876716,
-                    43.610769
+                    12.3155151,
+                    45.4408474
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P78"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.4571001,
-                    51.2098649
+                    10.5267696,
+                    52.2688736
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P79"
             },
             "type": "Feature"
@@ -1052,250 +1052,250 @@
                 "unique_id": "P80"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.4115179,
-                    53.2464214
+                    2.3522219,
+                    48.856614
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P81"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    0.68484,
-                    47.394144
+                    10.9916215,
+                    45.4383842
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P82"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.4115179,
-                    53.2464214
+                    5.5796662,
+                    50.6325574
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P83"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    2.0807123,
-                    49.4295387
+                    8.946256,
+                    44.4056499
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P84"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    0.1562369,
-                    45.648377
+                    -4.1426565,
+                    50.3754565
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P85"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    3.7174243,
-                    51.0543422
+                    2.252208,
+                    50.750115
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P86"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    1.909251,
-                    47.902964
+                    2.398782,
+                    47.081012
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P87"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    11.3426163,
-                    44.494887
+                    10.0226511,
+                    45.133249
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P88"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.2118019,
-                    45.5415526
+                    3.057256,
+                    50.62925
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P89"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    1.261105,
-                    45.833619
+                    10.4115179,
+                    53.2464214
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P90"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -2.715974,
-                    52.056398
+                    2.3522219,
+                    48.856614
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P91"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    2.295753,
-                    49.894067
+                    11.5354214,
+                    45.5454787
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P92"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.946256,
-                    44.4056499
+                    8.3507182,
+                    49.6341372
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P93"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    12.3155151,
-                    45.4408474
+                    4.89236,
+                    44.933393
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P94"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -0.612747,
-                    44.881793
+                    8.946256,
+                    44.4056499
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P95"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    10.2118019,
-                    45.5415526
+                    6.9602786,
+                    50.937531
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P96"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    -2.238156,
-                    51.8642449
+                    11.3307574,
+                    43.318809
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P97"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    8.946256,
-                    44.4056499
+                    10.7913751,
+                    45.1564168
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P98"
             },
             "type": "Feature"
         },
         {
             "geometry": {
                 "coordinates": [
-                    12.3155151,
-                    45.4408474
+                    10.6865593,
+                    53.8654673
                 ],
                 "type": "Point"
             },
             "properties": {
                 "unique_id": "P99"
             },
             "type": "Feature"
```

### Comparing `scicom-0.1.0/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson` & `scicom-0.1.2/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom/data/relPop_plosOne.csv` & `scicom-0.1.2/src/scicom/data/relPop_plosOne.csv`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom/data/relativePopulation_1650.csv` & `scicom-0.1.2/src/scicom/data/relativePopulation_1650.csv`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom/historicalletters/agents.py` & `scicom-0.1.2/src/scicom/historicalletters/agents.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 import mesa
 import mesa_geo as mg
 
 
 class SenderAgent(mg.GeoAgent):
 
     def __init__(
-        self, unique_id, model, geometry, crs, updateTopic, threshold, moveRange, letterRange
+        self, unique_id, model, geometry, crs, updateTopic, similarityThreshold, moveRange, letterRange
     ):
         super().__init__(unique_id, model, geometry, crs)
         self.region_id = 'FR62'
+        self.activationWeight = 1
         self.updateTopic = updateTopic
-        self.threshold = threshold
+        self.similarityThreshold = similarityThreshold
         self.moveRange = moveRange
         self.letterRange = letterRange
         self.topicLedger = []
-        self.lettersReceived = []
+        # self.lettersReceived = []
         self.numLettersReceived = 0
-        self.lettersSend = []
+        # self.lettersSend = []
         self.numLettersSend = 0
 
     def move(self, neighbors):
         """The agent can randomly move to neighboring positions."""
         if neighbors:
             # Random decision to move or not, weights are 10% moving, 90% staying.
             move = random.choices([0, 1], weights=[0.9, 0.1], k=1)
@@ -34,39 +35,39 @@
                 possible_steps = []
                 # Weighted random choice to target of moving.
                 # Strong receivers are more likely targets.
                 for n in neighbors:
                     if n != self:
                         possible_steps.append(n.geometry)
                         weights.append(n.numLettersReceived)
-                if sum(weights) > 0:
-                    lineEndPoint = random.choices(possible_steps, weights, k=1)
-                else:
-                    lineEndPoint = random.choices(possible_steps, k=1)
-                lineSegment = LineString([self.geometry, lineEndPoint[0]])
-                next_position = lineSegment.interpolate(random.random(), normalized=True)
-                self.model.space.move_sender(self, next_position)
+                # Capture cases where no possible steps exist.
+                if possible_steps:
+                    if sum(weights) > 0:
+                        lineEndPoint = random.choices(possible_steps, weights, k=1)
+                    else:
+                        lineEndPoint = random.choices(possible_steps, k=1)
+                    lineSegment = LineString([self.geometry, lineEndPoint[0]])
+                    next_position = lineSegment.interpolate(random.random(), normalized=True)
+                    self.model.space.move_sender(self, next_position)
 
     @property
     def has_topic(self):
         """Current topic of the agent."""
         return self.topicVec
 
     def has_letter_contacts(self, neighbors=False):
         """List of already established and potential contacts.
 
         Implements the ego-reinforcing by allowing mutliple entries
         of the same agent. In neighbourhods agents are added proportional
         to the number of letters they received, thus increasing the reinforcement.
         """
         contacts = []
-        senders = self.lettersReceived
-        receivers = self.lettersSend
-        contacts.extend(senders)
-        contacts.extend(receivers)
+        socialNetwork = [x for x in self.model.G.neighbors(self.unique_id)]
+        contacts.extend(socialNetwork)
         if neighbors:
             neighborRec = []
             for n in neighbors:
                 if n != self:
                     # TODO: We could here exclude already listed receivers/senders?!
                     if n.numLettersReceived > 0:
                         nMult = [n] * n.numLettersReceived
@@ -97,61 +98,69 @@
             receiver = random.choice(contacts)
             if isinstance(receiver, SenderAgent):
                 initTopic = self.chooses_topic(receiver)
                 # Calculate distance between own chosen topic 
                 # and current topic of receiver.
                 # TODO: Rethink this step!
                 distance = np.linalg.norm(np.array(receiver.topicVec) - np.array(initTopic))
-                # If the calculated distance falls below a threshold,
+                # If the calculated distance falls below a similarityThreshold,
                 # send the letter.
-                if distance < self.threshold:
+                if distance < self.similarityThreshold:
                     receiver.numLettersReceived += 1
-                    receiver.lettersReceived.append(self.unique_id)
+                    # receiver.lettersReceived.append(self.unique_id)
                     self.numLettersSend += 1
-                    self.lettersSend.append(receiver.unique_id)
+                    # self.lettersSend.append(receiver.unique_id)
                     # Update model social network
                     self.model.G.add_edge(self.unique_id, receiver.unique_id)
                     self.model.G.nodes()[self.unique_id]['numLettersSend'] = self.numLettersSend
                     self.model.G.nodes()[receiver.unique_id][
                         'numLettersReceived'
                     ] = receiver.numLettersReceived
                     # Update agents topic vector as a weighted sum
                     # of the original sender topic and a scaled 
                     # random projection of the sender topic towards 
                     # the receiver topic.
+                    # TODO: Consider dropping the origial topic vector, since this 
+                    # corresponds to a strong bias of the old topic.
                     updateTopicVec = self.topicVec + self.updateTopic * np.random.uniform(0, 1) * (np.array(receiver.topicVec) - np.array(self.topicVec))
                     self.model.letterLedger.append(
                         (
                             self.unique_id, receiver.unique_id, self.geometry, receiver.geometry,
                             updateTopicVec, self.model.schedule.steps
                         )
                     )
                     self.topicLedger.append(
                         self.topicVec
                     )
                     self.topicVec = updateTopicVec
                     self.model.updatedTopic += 1
 
     def step(self):
-        neighborsMove = [
-            x for x in self.model.space.get_neighbors_within_distance(
-                self,
-                distance=self.moveRange * self.model.meandistance,
-                center=False
-            ) if isinstance(x, SenderAgent)
-        ]
-        neighborsSend = [
-            x for x in self.model.space.get_neighbors_within_distance(
-                self,
-                distance=self.letterRange * self.model.meandistance,
-                center=False
-            ) if isinstance(x, SenderAgent)
-        ]
-        self.sendLetter(neighborsSend)
-        self.move(neighborsMove)
+        currentActivation = random.choices(
+            population=[0, 1],
+            weights=[1 - self.activationWeight, self.activationWeight],
+            k=1  
+        )
+        if currentActivation[0] == 1:
+            neighborsMove = [
+                x for x in self.model.space.get_neighbors_within_distance(
+                    self,
+                    distance=self.moveRange * self.model.meandistance,
+                    center=False
+                ) if isinstance(x, SenderAgent)
+            ]
+            neighborsSend = [
+                x for x in self.model.space.get_neighbors_within_distance(
+                    self,
+                    distance=self.letterRange * self.model.meandistance,
+                    center=False
+                ) if isinstance(x, SenderAgent)
+            ]
+            self.sendLetter(neighborsSend)
+            self.move(neighborsMove)
 
 
 class RegionAgent(mg.GeoAgent):
     init_num_people: int
     persons_in_region: list
 
     def __init__(self, unique_id, model, geometry, crs, init_num_people=0):
@@ -191,9 +200,9 @@
         unique_id,
         model,
         topicVec
     ):
         """Create letter with position, topic vector and parameters."""
         super().__init__(unique_id, model)
         self.topicVec = topicVec
-        self.lettersReceived = 0
-        self.lettersSend = 0
+        self.numLettersReceived = 0
+        self.numLettersSend = 0
```

### Comparing `scicom-0.1.0/src/scicom/historicalletters/server.py` & `scicom-0.1.2/src/scicom/historicalletters/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,28 @@
 model_params = {
     "population": 100,
     # "population": mesa.visualization.Slider(
     #     "Number of persons",
     #     100, 10, 200, 10,
     #     description="Choose how many persons to include in the model.",
     # ),
+    "useSocialNetwork": mesa.visualization.Checkbox(
+        "Create initial social network of agents",
+        False
+    ),
+    "useActivation": mesa.visualization.Checkbox(
+        "Use heterogenous activations",
+        False
+    ),
     "updateTopic": mesa.visualization.Slider(
         "Strength of adoption",
         0.05, 0.01, 0.3, 0.05,
         description="Choose how strongly letter sending changes ones topics.",
     ),
-    "threshold": mesa.visualization.Slider(
+    "similarityThreshold": mesa.visualization.Slider(
         "Similarity threshold",
         0.5, 0.0, 1.0, 0.5,
         description="Choose how similar two persons topics have to be, to send a letter.",
     ),
     "moveRange": mesa.visualization.Slider(
         "Range for moving position</br>(% of mean agent distances)",
         0.5, 0, 1, 0.1,
```

### Comparing `scicom-0.1.0/src/scicom/historicalletters/space.py` & `scicom-0.1.2/src/scicom/historicalletters/space.py`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom/historicalletters/util.py` & `scicom-0.1.2/src/scicom/historicalletters/util.py`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom/randomletters/SimpleContinuousModule.py` & `scicom-0.1.2/src/scicom/randomletters/SimpleContinuousModule.py`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom/randomletters/agents.py` & `scicom-0.1.2/src/scicom/randomletters/agents.py`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom/randomletters/model.py` & `scicom-0.1.2/src/scicom/randomletters/model.py`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom/randomletters/server.py` & `scicom-0.1.2/src/scicom/randomletters/server.py`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom/run.py` & `scicom-0.1.2/src/scicom/run.py`

 * *Files identical despite different names*

### Comparing `scicom-0.1.0/src/scicom.egg-info/PKG-INFO` & `scicom-0.1.2/src/scicom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scicom
-Version: 0.1.0
+Version: 0.1.2
 Summary: Simulating various aspects of scientific communication via Agent-based models.
 Home-page: https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels
 Author: Bernardo S. Buarque, Malte Vogl
 Author-email: bsbuarque@mpiwg-berlin.mpg.de, mvogl@mpiwg-berlin.mpg.de
 Project-URL: Project Home, https://modelsen.mpiwg-berlin.mpg.de
 Project-URL: Bug Tracker, https://gitlab.gwdg.de/modelsen/sciencecommunicationmodels/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scicom-0.1.0/src/scicom.egg-info/SOURCES.txt` & `scicom-0.1.2/src/scicom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

