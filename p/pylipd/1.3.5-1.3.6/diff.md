# Comparing `tmp/pylipd-1.3.5.tar.gz` & `tmp/pylipd-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylipd-1.3.5.tar", last modified: Fri May 19 17:48:29 2023, max compression
+gzip compressed data, was "pylipd-1.3.6.tar", last modified: Mon Jun 19 18:45:49 2023, max compression
```

## Comparing `pylipd-1.3.5.tar` & `pylipd-1.3.6.tar`

### file list

```diff
@@ -1,38 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 17:48:22.000000 pylipd-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 17:48:29.209162 pylipd-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-19 17:48:22.000000 pylipd-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd/globals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/globals/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    29677 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/lipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/lipd_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/series/regexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/usage_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16043 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/legacy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    43683 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/lipd_to_rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/multi_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/rdf_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/rdf_to_lipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-19 17:48:22.000000 pylipd-1.3.5/pylipd/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:48:29.209162 pylipd-1.3.5/pylipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 17:48:29.000000 pylipd-1.3.5/pylipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 17:48:22.000000 pylipd-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-19 17:48:29.209162 pylipd-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-19 17:48:22.000000 pylipd-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:49.737635 pylipd-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 18:45:43.000000 pylipd-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-19 18:45:49.737635 pylipd-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-19 18:45:43.000000 pylipd-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:49.729635 pylipd-1.3.6/pylipd/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:49.729635 pylipd-1.3.6/pylipd/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  3654866 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/ODP846.Lawrence.2006.lpd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:49.737635 pylipd-1.3.6/pylipd/data/Pages2k/
+-rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Ant-WAIS-Divide.Severinghaus.2012.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Arc-Kongressvatnet.D'Andrea.2012.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Asi-SourthAndMiddleUrals.Demezhko.2007.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Eur-CoastofPortugal.Abrantes.2011.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Eur-FinnishLakelands.Helama.2014.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Eur-LakeSilvaplana.Trachsel.2010.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Eur-NorthernScandinavia.Esper.2012.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Eur-NorthernSpain.Martin-Chivelet.2011.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Eur-SpanishPyrenees.Dorado-Linan.2012.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Eur-SpannagelCave.Mangini.2005.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Eur-Stockholm.Leijonhufvud.2009.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Ocn-AlboranSea436B.Nieto-Moreno.2013.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Ocn-FeniDrift.Richter.2009.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Ocn-PedradeLume-CapeVerdeIslands.Moses.2006.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Ocn-RedSea.Felis.2000.lpd
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/data/Pages2k/Ocn-SinaiPeninsula,RedSea.Moustafa.2000.lpd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:49.737635 pylipd-1.3.6/pylipd/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/globals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/globals/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/globals/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/globals/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/globals/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37224 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/lipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/lipd_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:49.737635 pylipd-1.3.6/pylipd/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/series/regexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/usage_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:49.737635 pylipd-1.3.6/pylipd/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16043 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/utils/legacy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43683 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/utils/lipd_to_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/utils/multi_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/utils/rdf_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/utils/rdf_to_lipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-19 18:45:43.000000 pylipd-1.3.6/pylipd/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:45:49.737635 pylipd-1.3.6/pylipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-19 18:45:49.000000 pylipd-1.3.6/pylipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-19 18:45:49.000000 pylipd-1.3.6/pylipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:45:49.000000 pylipd-1.3.6/pylipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:45:49.000000 pylipd-1.3.6/pylipd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 18:45:49.000000 pylipd-1.3.6/pylipd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 18:45:49.000000 pylipd-1.3.6/pylipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-19 18:45:43.000000 pylipd-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-19 18:45:49.737635 pylipd-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-19 18:45:43.000000 pylipd-1.3.6/setup.py
```

### Comparing `pylipd-1.3.5/LICENSE` & `pylipd-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/PKG-INFO` & `pylipd-1.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Author: Varun Ratnakar
+Author: Varun Ratnakar, Deborah Khider
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.5
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.6
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.0
```

### Comparing `pylipd-1.3.5/README.md` & `pylipd-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd/globals/queries.py` & `pylipd-1.3.6/pylipd/globals/queries.py`

 * *Files 16% similar despite different names*

```diff
@@ -105,21 +105,33 @@
         OPTIONAL{?pub le:institution ?institution .}
         OPTIONAL{?pub le:hasLink ?url .}
         OPTIONAL{?pub le:url ?url2 .}
     }
     GROUP BY ?pub ?dsname ?title ?doi ?year ?pubyear ?journal ?volume ?issue ?pages ?type ?publisher ?report ?citeKey ?edition ?institution ?url ?url2
 """
 
+QUERY_DISTINCT_VARIABLE="""
+    PREFIX le: <http://linked.earth/ontology#>
+    
+    SELECT distinct ?variableName 
+    WHERE {
+        ?uri le:name ?variableName .
+        ?uri le:hasVariableID ?TSID
+    }
+    
+
+"""
+
 QUERY_VARIABLE = """
     PREFIX le: <http://linked.earth/ontology#>
 
-    SELECT ?uri ?varid ?varname 
+    SELECT ?uri ?TSID ?variableName 
     WHERE {
-        ?uri le:name ?varname .
-        ?uri le:hasVariableID ?varid
+        ?uri le:name ?variableName .
+        ?uri le:hasVariableID ?TSID
     }
 """
 
 QUERY_VARIABLE_GRAPH = """
     PREFIX le: <http://linked.earth/ontology#>
 
     CONSTRUCT {
@@ -154,22 +166,24 @@
             ?var ?pv1 ?v1 .
             ?var ?p1 ?o1 .        
             ?o1 ?pv2 ?v2 .
             ?o1 ?p2 ?o2 .
             ?o2 ?pv3 ?v3 .
             ?var le:foundInTable ?table .
             ?var le:foundInDataset ?ds .
+            ?var le:foundInDatasetName ?dsname
         }
     }
     WHERE {
         ?table le:includesVariable ?var .
         {
             {
                 # level 1
                 ?var le:foundInDataset ?ds .
+                ?ds le:name ?dsname .
                 ?var ?pv1 ?v1  # get primitives
                     FILTER (isLiteral(?v1)) .
             }
             UNION
             {
                 # level 2
                 {
@@ -215,19 +229,20 @@
         ?ds le:name ?dsname .
         ?ds le:proxyArchiveType ?archiveType .
         FILTER regex(?archiveType, "[archiveType].*", "i")
     }
 """
 
 QUERY_FILTER_VARIABLE_NAME = """
-    SELECT ?uri ?dsuri ?tableuri ?id ?name WHERE {
+    SELECT ?uri ?dsuri ?dsname ?tableuri ?id ?name WHERE {
         ?uri le:hasVariableID ?id .
         ?uri le:name ?name .
         FILTER regex(?name, "[name].*", "i") .
         ?uri le:foundInDataset ?dsuri .
+        ?uri le:foundInDatasetName ?dataSetName .
         ?uri le:foundInTable ?tableuri .
     }
 """
 
 QUERY_TIMESERIES_ESSENTIALS_PALEO ="""
     PREFIX wgs84: <http://www.w3.org/2003/01/geo/wgs84_pos#>
     SELECT ?dataSetName ?archiveType ?geo_meanLat ?geo_meanLon ?geo_meanElev 
@@ -236,38 +251,43 @@
     ?time_units ?depth_variableName ?depth_values ?depth_units WHERE {
         ?ds a le:Dataset .
         ?ds le:name ?dataSetName .
             FILTER regex(?dataSetName, "[dsname].*", "i").
         OPTIONAL{?ds le:proxyArchiveType ?archiveType .}
         
         ?ds le:collectedFrom ?loc .
-        ?loc wgs84:lat ?geo_meanLat .
-        ?loc wgs84:long ?geo_meanLon .
+        OPTIONAL{?loc wgs84:lat ?geo_meanLat .}
+        OPTIONAL{?loc wgs84:long ?geo_meanLon .}
         OPTIONAL {?loc wgs84:alt ?geo_meanElev .}
         
         ?ds le:includesPaleoData ?data .
         ?data le:foundInMeasurementTable ?table .
         ?table le:includesVariable ?var .
+        
         ?var le:name ?paleoData_variableName .
+        FILTER (!regex(?paleoData_variableName, "year.*") && !regex(?paleoData_variableName, "age.*") && !regex(?paleoData_variableName, "depth.*")) .
+   		
         ?var le:hasValues ?paleoData_values .
         OPTIONAL{?var le:hasUnits ?paleoData_units .}
         OPTIONAL{?var le:proxy ?paleoData_proxy .}
         OPTIONAL{?var le:proxyGeneral ?paleoData_proxyGeneral .}
         
-        ?table le:includesVariable ?timevar .
+        
+        OPTIONAL{?table le:includesVariable ?timevar .
         ?timevar le:name ?time_variableName .
             FILTER (regex(?time_variableName, "year.*") || regex(?time_variableName, "age.*")) .
         ?timevar le:hasValues ?time_values .
-            OPTIONAL{?timevar le:hasUnits ?time_units .}
+            OPTIONAL{?timevar le:hasUnits ?time_units .}}
         
-        ?table le:includesVariable ?depthvar .
+        OPTIONAL{?table le:includesVariable ?depthvar .
         ?depthvar le:name ?depth_variableName .
             FILTER (regex(?depth_variableName, "depth.*")) .
         ?depthvar le:hasValues ?depth_values .
-            OPTIONAL{?depthvar le:hasUnits ?depth_units .}
+            OPTIONAL{?depthvar le:hasUnits ?depth_units .}}
+        
     }
 """
 
 QUERY_TIMESERIES_ESSENTIALS_CHRON ="""
     PREFIX wgs84: <http://www.w3.org/2003/01/geo/wgs84_pos#>
     SELECT ?dataSetName ?archiveType ?geo_meanLat ?geo_meanLon ?geo_meanElev 
     ?chronData_variableName ?chronData_values ?chronData_units 
@@ -275,32 +295,114 @@
     ?time_units ?depth_variableName ?depth_values ?depth_units WHERE {
         ?ds a le:Dataset .
         ?ds le:name ?dataSetName .
             FILTER regex(?dataSetName, "[dsname].*", "i").
         OPTIONAL{?ds le:proxyArchiveType ?archiveType .}
         
         ?ds le:collectedFrom ?loc .
-        ?loc wgs84:lat ?geo_meanLat .
-        ?loc wgs84:long ?geo_meanLon .
+        OPTIONAL{?loc wgs84:lat ?geo_meanLat .}
+        OPTIONAL{?loc wgs84:long ?geo_meanLon .}
         OPTIONAL {?loc wgs84:alt ?geo_meanElev .}
         
         ?ds le:includesChronData ?data .
         ?data le:foundInMeasurementTable ?table .
         ?table le:includesVariable ?var .
         ?var le:name ?chronData_variableName .
+        FILTER (!regex(?chron_variableName, "year.*") && !regex(?chron_variableName, "age.*") && !regex(?chron_variableName, "depth.*")) .
+   		
         ?var le:hasValues ?chronData_values .
         OPTIONAL{?var le:hasUnits ?chronData_units .}
         
-        ?table le:includesVariable ?timevar .
+        OPTIONAL{?table le:includesVariable ?timevar .
         ?timevar le:name ?time_variableName .
             FILTER (regex(?time_variableName, "year.*") || regex(?time_variableName, "age.*")) .
         ?timevar le:hasValues ?time_values .
-            OPTIONAL{?timevar le:hasUnits ?time_units .}
+            OPTIONAL{?timevar le:hasUnits ?time_units .}}
         
-        ?table le:includesVariable ?depthvar .
+        OPTIONAL{?table le:includesVariable ?depthvar .
         ?depthvar le:name ?depth_variableName .
             FILTER (regex(?depth_variableName, "depth.*")) .
         ?depthvar le:hasValues ?depth_values .
-            OPTIONAL{?depthvar le:hasUnits ?depth_units .}
+            OPTIONAL{?depthvar le:hasUnits ?depth_units .}}
+    }
+"""
+
+QUERY_VARIABLE_PROPERTIES="""
+    PREFIX le: <http://linked.earth/ontology#>
+    SELECT  DISTINCT ?property where {
+    
+    ?ds a le:Dataset .
+    
+    {?ds le:includesPaleoData ?data .
+    ?data le:foundInMeasurementTable ?table .
+    ?table le:includesVariable ?var .
+    ?var ?property ?value .}
+    
+    UNION
+    
+    {OPTIONAL{?ds le:includesChronData ?data1 .
+    ?data1 le:foundInMeasurementTable ?table1 .
+    ?table1 le:includesVariable ?var1 .
+    ?var1 ?property ?value1 .}}
+    
+    }
+"""
+
+
+QUERY_DATASET_PROPERTIES="""
+    PREFIX le: <http://linked.earth/ontology#>
+    SELECT DISTINCT ?property where {
+    ?ds a le:Dataset .
+    ?ds ?property ?value .
     }
 """
 
+QUERY_MODEL_PROPERTIES="""
+    PREFIX le: <http://linked.earth/ontology#>
+    SELECT  DISTINCT ?property where {
+    
+    ?ds a le:Dataset .
+    
+    {OPTIONAL{?ds le:includesPaleoData ?data .
+              ?data le:paleoModeledBy ?paleomodel .
+              ?paleomodel ?property ?value .}}
+    
+    UNION
+    
+    {OPTIONAL{?ds le:includesChronData ?chron .
+              ?chron le:paleoModeledBy ?chronmodel .
+              ?chronmodel ?property ?value .}}
+    
+    }
+"""
+
+QUERY_VARIABLE_ESSENTIALS="""
+    PREFIX le: <http://linked.earth/ontology#>
+    SELECT ?dataSetName ?archiveType ?name ?TSID ?values ?units ?proxy where {
+        ?var le:name ?name .
+        ?var le:foundInDatasetName ?dataSetName .
+            #FILTER regex(?dataSetName, "[dsname].*", "i").
+            
+        OPTIONAL{?var le:hasVariableID ?TSID .}
+        ?var le:hasValues ?values .
+        OPTIONAL{?var le:hasUnits ?units .}
+        OPTIONAL{?var le:archiveType ?archiveType .}
+        OPTIONAL{?var le:proxy ?proxy .}
+        
+        
+        
+        }
+"""
+
+QUERY_LOCATION ="""
+    PREFIX wgs84: <http://www.w3.org/2003/01/geo/wgs84_pos#>
+    SELECT ?dataSetName ?geo_meanLat ?geo_meanLon ?geo_meanElev WHERE {
+        ?ds a le:Dataset .
+        ?ds le:name ?dataSetName .
+            FILTER regex(?dataSetName, "[dsname].*", "i").
+        
+        ?ds le:collectedFrom ?loc .
+        OPTIONAL{?loc wgs84:lat ?geo_meanLat .}
+        OPTIONAL{?loc wgs84:long ?geo_meanLon .}
+        OPTIONAL{?loc wgs84:alt ?geo_meanElev .}
+        }
+"""
```

### Comparing `pylipd-1.3.5/pylipd/globals/schema.py` & `pylipd-1.3.6/pylipd/globals/schema.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd/lipd.py` & `pylipd-1.3.6/pylipd/lipd.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 import re
 import os.path
 import tempfile
 import pandas as pd
 import random
 import string
 import io
+import numpy as np
+import ast
 
 from rdflib import ConjunctiveGraph, URIRef
 from tqdm import tqdm
-from .globals.queries import QUERY_ALL_VARIABLES_GRAPH, QUERY_BIBLIO, QUERY_DSID, QUERY_DSNAME, QUERY_ENSEMBLE_TABLE, QUERY_ENSEMBLE_TABLE_SHORT, QUERY_FILTER_ARCHIVE_TYPE, QUERY_FILTER_GEO, QUERY_VARIABLE, QUERY_VARIABLE_GRAPH, QUERY_UNIQUE_ARCHIVE_TYPE
+from .globals.queries import QUERY_ALL_VARIABLES_GRAPH, QUERY_BIBLIO, QUERY_DSID, QUERY_DSNAME, QUERY_ENSEMBLE_TABLE, QUERY_ENSEMBLE_TABLE_SHORT, QUERY_FILTER_ARCHIVE_TYPE, QUERY_FILTER_GEO, QUERY_VARIABLE, QUERY_VARIABLE_GRAPH, QUERY_UNIQUE_ARCHIVE_TYPE, QUERY_TIMESERIES_ESSENTIALS_CHRON, QUERY_TIMESERIES_ESSENTIALS_PALEO, QUERY_DISTINCT_VARIABLE, QUERY_DATASET_PROPERTIES, QUERY_VARIABLE_PROPERTIES, QUERY_MODEL_PROPERTIES, QUERY_LOCATION
 from .lipd_series import LiPDSeries
 from .utils.multi_processing import multi_convert_to_rdf, multi_load_lipd
 from .utils.rdf_graph import RDFGraph
 
 from .utils.rdf_to_lipd import RDFToLiPD
 from .utils.legacy_utils import LiPD_Legacy
 from .utils.utils import sanitizeId
@@ -134,14 +136,17 @@
         if type(lipdfiles) is not list:
             lipdfiles = [lipdfiles]
             
         numfiles = len(lipdfiles)
         print(f"Loading {numfiles} LiPD files")
         self.graph = multi_load_lipd(self.graph, lipdfiles, parallel)
         print("Loaded..")
+    
+    #def load_from_lipdverse(self, datasetID, version=None):
+        
 
 
     def convert_lipd_dir_to_rdf(self, lipd_dir, rdf_file, parallel=False):
         '''Convert a directory containing LiPD files into a single RDF file (to be used for uploading to Knowledge Bases like GraphDB)
 
         Parameters
         ----------
@@ -411,14 +416,18 @@
             lipd_remote.set_endpoint("https://linkedearth.graphdb.mint.isi.edu/repositories/LiPDVerse2")
             ts_list = lipd_remote.get_timeseries(["Ocn-MadangLagoonPapuaNewGuinea.Kuhnert.2001", "MD98_2181.Stott.2007", "Ant-WAIS-Divide.Severinghaus.2012"])
             for dsname, tsos in ts_list.items():
                 for tso in tsos:
                     if 'paleoData_variableName' in tso:
                         print(dsname+': '+tso['paleoData_variableName']+': '+tso['archiveType'])
         '''
+        
+        if type(dsnames)==str:
+            dsnames=[dsnames]
+        
         ts = self._get_timeseries(dsnames)
         if to_dataframe == False:
             return ts
         elif to_dataframe == True:
             dict_list =[]
 
             for item in ts.keys():
@@ -436,14 +445,86 @@
             d = converter.convert_to_json(dsname)
             print("Extracting timeseries from dataset: " + dsname + " ...")
             if len(d.items()):
                 tss = LiPD_Legacy().extract(d)
                 timeseries[dsname] = tss
         return timeseries
     
+    def get_timeseries_essentials(self, dsname = None, mode='paleo'):
+        ''' Returns specific properties for timeseries: 'dataSetName', 'archiveType', 'geo_meanLat', 'geo_meanLon',
+               'geo_meanElev', 'paleoData_variableName', 'paleoData_values',
+               'paleoData_units', 'paleoData_proxy' (paleo only), 'paleoData_proxyGeneral' (paleo only),
+               'time_variableName', 'time_values', 'time_units', 'depth_variableName',
+               'depth_values', 'depth_units'
+        
+
+        Parameters
+        ----------
+        dsname : str, optional
+            The name of the dataset for which to return the timeseries information. The default is None.
+        mode : paleo, chron
+            Whether to retrun the information stored in the PaleoMeasurementTable or the ChronMeasurementTable. The default is 'paleo'.
+
+        Raises
+        ------
+        ValueError
+            Need to select either 'chron' or 'paleo'
+
+        Returns
+        -------
+        qres_df : pandas.DataFrame
+            A pandas dataframe returning the properties in columns for each series stored in a row of the dataframe
+
+        Example
+        --------
+        
+        .. jupyter-execute::
+            
+            from pylipd.utils.dataset import load_datasets
+            lipd = load_datasets('ODP846.Lawrence.2006.lpd')
+            df_paleo = lipd.get_timeseries_essentials(mode='paleo')
+            print(df_paleo)
+        
+        To return the information stored in the ChronTable:
+        
+        .. jupyter-execute::
+            
+            from pylipd.utils.dataset import load_datasets
+            lipd = load_datasets('ODP846.Lawrence.2006.lpd')  
+            df_chron = lipd.get_timeseries_essentials(mode='chron')
+            print(df_chron)
+    
+        '''
+        
+        if dsname is None:
+            dsname= ''
+        
+        if mode == 'paleo':
+            query = QUERY_TIMESERIES_ESSENTIALS_PALEO
+            query = query.replace("[dsname]", dsname)
+        elif mode == 'chron':
+            query = QUERY_TIMESERIES_ESSENTIALS_CHRON
+            query = query.replace("[dsname]", dsname)
+        else:
+            raise ValueError("The mode should be either 'paleo' or 'chron'")
+    
+        qres, qres_df = self.query(query)
+        
+        try:
+            qres_df['paleoData_values']=qres_df['paleoData_values'].apply(lambda row : np.fromstring(row.strip("[]"), sep=','))
+        except:
+            qres_df['chronData_values']=qres_df['chronData_values'].apply(lambda row : np.fromstring(row.strip("[]"), sep=','))
+        
+        
+        qres_df['time_values']=qres_df['time_values'].apply(lambda x : np.fromstring(x.strip("[]"), sep=',') if x is not None else None)
+        qres_df['depth_values']=qres_df['depth_values'].apply(lambda x : np.fromstring(x.strip("[]"), sep=',') if x is not None else None)
+        
+        
+        return qres_df
+            
 
     def get_lipd(self, dsname):
         '''Get LiPD json for a dataset
 
         Parameters
         ----------
 
@@ -703,15 +784,47 @@
             print(lipd.get_all_archiveTypes())
 
         '''
         
         qres, qres_df = self.query(QUERY_UNIQUE_ARCHIVE_TYPE)
         return [str(row.archiveType) for row in qres]
         
+    def get_all_locations(self, dsname = None):
+        '''Return geographical coordinates for all the datasets.       
+
+        Parameters
+        ----------
+        dsname : str, optional
+            The name of the dataset for which to return the timeseries information. The default is None.
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            A pandas dataframe returning the latitude, longitude and elevation for each dataset
+        
+        Examples
+        --------
         
+        .. jupyter-execute::
+            
+            from pylipd.utils.dataset import load_dir
+            lipd = load_dir('Pages2k')
+            df = lipd.get_all_locations()
+            print(df)
+
+        '''
+        
+        if dsname is None:
+            dsname= ''
+        
+        query = QUERY_LOCATION
+        query = query.replace("[dsname]", dsname)
+            
+                
+        return self.query(query)[1]
 
     def get_ensemble_tables(self, dsname = None, ensembleVarName = None, ensembleDepthVarName = 'depth'):
         '''Gets ensemble tables from the LiPD graph
 
         Parameters
         ----------
 
@@ -764,14 +877,19 @@
        
             query = QUERY_ENSEMBLE_TABLE
             query = query.replace("[dsname]", dsname)
             query = query.replace("[ensembleVarName]", ensembleVarName)
             query = query.replace("[ensembleDepthVarName]", ensembleDepthVarName)
 
         qres, qres_df = self.query(query)
+        
+        qres_df['ensembleDepthValues']=qres_df['ensembleDepthValues'].apply(lambda row : np.fromstring(row.strip("[]"), sep=','))
+        qres_df['ensembleVariableValues']=qres_df['ensembleVariableValues'].apply(lambda row : np.array(ast.literal_eval(row)))
+        
+        
         return qres_df
 
 
     def get_all_variables(self):
         '''
         Returns a list of all variables in the graph
         
@@ -795,14 +913,118 @@
             
             df = lipd.get_all_variables()
             print(df)
 
         '''
         return self.query(QUERY_VARIABLE)[1]
 
+    def get_all_variable_names(self):
+        """
+        Get a list of all possible distinct variableNames. Useful for filtering and qeurying. 
+
+        Returns
+        -------
+        list
+            A list of unique variableName 
+        
+        Examples
+        --------
+        
+        .. jupyter-execute::
+            
+            from pylipd.utils.dataset import load_dir
+            lipd = load_dir('Pages2k')
+            varName = lipd.get_all_variable_names()
+            print(varName)
+        
+
+        """
+        
+        return self.query(QUERY_DISTINCT_VARIABLE)[1].iloc[:,0].values.tolist()
+    
+    def get_dataset_properties(self):
+        """Get a list of unique properties attached to a dataset. 
+        
+        Note: Some properties will return another object (e.g., 'publishedIn' will give you a Publication object with its own properties)
+        Note: Not all datasets will have the same available properties (i.e., not filled in by a user)
+        
+
+        Returns
+        -------
+        clean_list : list
+            A list of avialable properties that can queried
+
+        Examples
+        --------
+        
+        .. jupyter-execute::
+            
+            from pylipd.utils.dataset import load_dir
+            lipd = load_dir(name='Pages2k')
+            dataset_properties = lipd.get_dataset_properties()
+            print(dataset_properties)
+        """
+        
+        query_list = self.query(QUERY_DATASET_PROPERTIES)[1].iloc[:,0].values.tolist()
+        clean_list = [item.split("#")[-1] for item in query_list]
+        
+        return clean_list
+    
+    def get_variable_properties(self):
+        '''Get a list of variable properties that can be used for querying
+        
+
+        Returns
+        -------
+        list
+            A list of unique variable properties
+        
+        Examples
+        --------
+        
+        .. jupyter-execute::
+            
+            from pylipd.utils.dataset import load_dir
+            lipd = load_dir(name='Pages2k')
+            variable_properties = lipd.get_variable_properties()
+            print(variable_properties)
+
+        '''
+        
+        query_list = self.query(QUERY_VARIABLE_PROPERTIES)[1].iloc[:,0].values.tolist()
+        clean_list = [item.split("#")[-1] for item in query_list]
+        
+        return clean_list
+    
+    def get_model_properties(self):
+        '''Get all the properties associated with a model
+        
+
+        Returns
+        -------
+        List
+            A list of unique properties attached to models
+        
+        Examples
+        --------
+        
+        .. jupyter-execute::
+            
+            from pylipd.utils.dataset import load_datasets
+            lipd = load_datasets(names='ODP846')
+            model_properties = lipd.get_model_properties()
+            print(model_properties)
+
+
+        '''
+        
+        query_list = self.query(QUERY_MODEL_PROPERTIES)[1].iloc[:,0].values.tolist()
+        clean_list = [item.split("#")[-1] for item in query_list]
+        
+        return clean_list
 
     def to_lipd_series(self, parallel=False):
         '''
         Converts the LiPD object to a LiPDSeries object
 
         Parameters
         ----------
@@ -859,15 +1081,15 @@
 
         pylipd.lipd.LiPD
             A new LiPD object that only contains datasets that fall within the bounding box
         
         Examples
         --------
         
-        pyLipd ships with existing datasets that can be loaded directly through the package. Let's load the Euro2k sample datasets using this method.
+        pyLipd ships with existing datasets that can be loaded directly through the package. Let's load the Pages2k sample datasets using this method.
         
         .. jupyter-execute::
             
             from pylipd.utils.dataset import load_dir
 
             lipd = load_dir()
             Lfiltered = lipd.filter_by_geo_bbox(0,25,50,50)
@@ -899,21 +1121,21 @@
         
         pylipd.lipd.LiPD
             A new LiPD object that only contains datasets that have the specified archive type (regex)
         
         Examples
         --------
         
-        pyLipd ships with existing datasets that can be loaded directly through the package. Let's load the Euro2k sample datasets using this method.
+        pyLipd ships with existing datasets that can be loaded directly through the package. Let's load the Pages2k sample datasets using this method.
         
         .. jupyter-execute::
             
             from pylipd.utils.dataset import load_dir
 
-            lipd = load_dir()
+            lipd = load_dir('Pages2k')
             Lfiltered = lipd.filter_by_archive_type('marine')
             Lfiltered.get_all_dataset_names()
         
         '''
         query = QUERY_FILTER_ARCHIVE_TYPE
         query = query.replace("[archiveType]", archiveType)
         qres, qres_df = self.query(query)
```

### Comparing `pylipd-1.3.5/pylipd/lipd_series.py` & `pylipd-1.3.6/pylipd/lipd_series.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from rdflib import ConjunctiveGraph, Namespace, URIRef
 from tqdm import tqdm
-from .globals.queries import QUERY_FILTER_VARIABLE_NAME, QUERY_VARIABLE
+from .globals.queries import QUERY_FILTER_VARIABLE_NAME, QUERY_VARIABLE, QUERY_DISTINCT_VARIABLE, QUERY_VARIABLE_ESSENTIALS
 
 from pylipd.globals.urls import ONTONS
 from .utils.multi_processing import multi_load_lipd_series
 from .utils.rdf_graph import RDFGraph
 from .utils.utils import sanitizeId
 
+import numpy as np
+
 
 class LiPDSeries(RDFGraph):
     '''The LiPD Series class describes a collection of `LiPD (Linked Paleo Data) <https://cp.copernicus.org/articles/12/1093/2016/cp-12-1093-2016.html>`_ 
     variables. It contains an `RDF <https://www.w3.org/RDF/>`_ Graph which is serialization of  LiPD variables into an RDF graph containing terms from 
     the `LiPD Ontology <http://linked.earth/Ontology/release/core/1.2.0/index-en.html>`. Each LiPD Variable is also associated with the LiPD itself
     so it can be deserialized into the original LiPD format.
     How to browse and query the LiPD variables is described in a short example below.
@@ -88,15 +90,74 @@
             df = S.get_all_variables()
             
             print(df)
         
         
         '''        
         return self.query(QUERY_VARIABLE)[1]
+    
+    def get_all_variable_names(self):
+        
+        """
+        Get a list of all possible distinct variableNames. Useful for filtering and qeurying. 
+
+        Returns
+        -------
+        list
+            A list of unique variableName 
+        
+        Examples
+        --------
+        
+        .. jupyter-execute::
+            
+            from pylipd.utils.dataset import load_dir
+            lipd = load_dir('Pages2k')
+            S = lipd.to_lipd_series()
+            varName = S.get_all_variable_names()
+            print(varName)
+        """
+
+        return self.query(QUERY_DISTINCT_VARIABLE)[1].iloc[:,0].values.tolist()
+
+    def get_timeseries_essentials(self):
+        '''This function returns information about each variable: `dataSetName`, `archiveType`, `name`, `values`, `units`, `TSID`, `proxy`.
+
+        Returns
+        -------
+        qres_df : pandas.DataFrame
+            A dataframe containing the information in each column
+        
+        Examples
+        --------
+        
+        .. jupyter-execute::
+
+            from pylipd.utils.dataset import load_dir
 
+            lipd = load_dir()
+            S = lipd.to_lipd_series()
+            df = S.get_timeseries_essentials()
+            
+            print(df)
+
+        '''
+        
+    
+        query = QUERY_VARIABLE_ESSENTIALS
+        qres, qres_df = self.query(query)
+        
+        #fix the dataframe
+        for _,row in qres_df.iterrows():
+            string = row['dataSetName'].split('/')[-1]
+            row['dataSetName'] = string
+        
+        qres_df['values']=qres_df['values'].apply(lambda row : np.fromstring(row.strip("[]"), sep=','))
+        
+        return qres_df
 
     def filter_by_name(self, name):
         '''
         Filters series to return a new LiPDSeries that only keeps variables that have the specified name (regex)
 
         Parameters
         ----------
```

### Comparing `pylipd-1.3.5/pylipd/series/regexes.py` & `pylipd-1.3.6/pylipd/series/regexes.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd/usage.py` & `pylipd-1.3.6/pylipd/usage.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd/usage_parallel.py` & `pylipd-1.3.6/pylipd/usage_parallel.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,43 +2,49 @@
     from pylipd.lipd import LiPD
 
     local_lipd_dir = "/Users/varun/git/LiPD/PyLiPD/data/lpd.latest"
 
     L = LiPD()
 
     L.load_from_dir("examples/data/Euro2k", parallel=True, cutoff=1000)
-    Lfiltered = L.filter_by_archive_type("marine")
-    print(len(Lfiltered.get_all_dataset_names()))
-    print(Lfiltered.get_all_archiveTypes())
+    # Lfiltered = L.filter_by_geo_bbox(0,25,50,50)
+    # print(Lfiltered.get_all_dataset_names())
+
+    # Lfiltered = L.filter_by_archive_type("marine")
+    # print(len(Lfiltered.get_all_dataset_names()))
+    # print(Lfiltered.get_all_archiveTypes())
+    # print(Lfiltered.get_all_dataset_names())
 
     # Convert LiPD files to RDF    
     # L.convert_lipd_dir_to_rdf(
     #     local_lipd_dir,
     #     local_lipd_dir+".nq", 
     #     parallel=True)
     
-    '''
-    L.load_from_dir(local_lipd_dir, parallel=True, cutoff=1000)
+
+    #L.load_from_dir(local_lipd_dir, parallel=True, cutoff=100)
     
     print(f"Total number of datasets: {len(L.get_all_dataset_names())}")
 
     print("Filtering by archive type and bounding box")
     
-    Lfiltered = L.filter_by_archive_type("marine").filter_by_geo_bbox(-50, -50, 50, 50)
+    #Lfiltered = L.filter_by_archive_type("marine").filter_by_geo_bbox(-50, -50, 50, 50)
     
-    print(f"Total number of filtered datasets: {len(Lfiltered.get_all_dataset_names())}")
+    #print(f"Total number of filtered datasets: {len(Lfiltered.get_all_dataset_names())}")
 
     # Free up memory by deleting the original LiPD object
-    del L
+    #del L
 
     # Convert to LiPD Series
     print("Creating LiPD Series...")
-    S = Lfiltered.to_lipd_series(parallel=True)
+    S = L.to_lipd_series(parallel=True)
+
+    df = S.get_timeseries_essentials()
+    print(df)
 
-    print("Filtering LiPD Series with variable name starting with 'd18O'")
-    S = S.filter_by_name("d18O")
+    #print("Filtering LiPD Series with variable name starting with 'd18O'")
+    #S = S.filter_by_name("d18O")
     
     print("Printing all valid variables")
-    print(S.get_all_variables()['varname'])
-    '''
+    print(S.get_all_variables())
 
     exit()
```

### Comparing `pylipd-1.3.5/pylipd/utils/dataset.py` & `pylipd-1.3.6/pylipd/utils/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 """
 
 from pathlib import Path
 import glob
 from pylipd.lipd import LiPD
 
 DATA_DIR = Path(__file__).parents[1].joinpath("data").resolve()
-FOLDER_DIR = DATA_DIR.joinpath('Euro2k/')
+FOLDER_DIR = DATA_DIR.joinpath('Pages2k/')
+#print(DATA_DIR)
 
 def available_dataset_names():
     '''Helper function to easily see what datasets are available to load
 
     Returns
     -------
     names : list
@@ -59,12 +60,16 @@
            pass
     
     L = LiPD()
     L.load(full_paths)
    
     return L
 
-def load_dir():
+def load_dir(name = 'Pages2k'):
+    
+    if name!= 'Pages2k':
+        raise ValueError("Option for folder is 'Pages2k")
+    
     L = LiPD()
     L.load_from_dir(str(FOLDER_DIR))
     
-    return L
+    return L
```

### Comparing `pylipd-1.3.5/pylipd/utils/legacy_utils.py` & `pylipd-1.3.6/pylipd/utils/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd/utils/lipd_to_rdf.py` & `pylipd-1.3.6/pylipd/utils/lipd_to_rdf.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd/utils/multi_processing.py` & `pylipd-1.3.6/pylipd/utils/multi_processing.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd/utils/rdf_graph.py` & `pylipd-1.3.6/pylipd/utils/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd/utils/rdf_to_lipd.py` & `pylipd-1.3.6/pylipd/utils/rdf_to_lipd.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd/utils/utils.py` & `pylipd-1.3.6/pylipd/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pylipd-1.3.5/pylipd.egg-info/PKG-INFO` & `pylipd-1.3.6/pylipd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pylipd
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python utilities for handling LiPD data
 Home-page: https://github.com/linkedearth/pylipd
-Author: Varun Ratnakar
+Author: Varun Ratnakar, Deborah Khider
 Author-email: varunratnakar@gmail.com
 License: Apache 2-0 License
-Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.5
+Download-URL: https://github.com/linkedearth/pylipd/tarball/1.3.6
 Project-URL: Bug Tracker, https://github.com/linkedearth/pylipd/issues
 Keywords: Paleoclimate, Data Analysis, LiPD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.0
```

### Comparing `pylipd-1.3.5/setup.cfg` & `pylipd-1.3.6/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = pylipd
-version = 1.3.5
-author = Varun Ratnakar
+version = 1.3.6
+author = Varun Ratnakar, Deborah Khider
 author_email = varunratnakar@gmail.com
 description = Python utilities for handling LiPD data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/linkedearth/pylipd
 project_urls = 
 	Bug Tracker = https://github.com/linkedearth/pylipd/issues
@@ -22,14 +22,15 @@
 install_requires = 
 	rdflib
 	pandas
 	doi2bib
 	pybtex
 	tqdm
 	bagit
+	numpy
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pylipd-1.3.5/setup.py` & `pylipd-1.3.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import os
 from setuptools import setup, find_packages
 
-version = '1.3.5'
+version = '1.3.6'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pylipd',
     packages=find_packages(),
     include_package_data=True,
+    package_data={'': ['data/*.lpd', 'data/Pages2k/*.lpd']},
     zip_safe=False,
     version=version,
     license='Apache 2-0 License',
     description='Python utilities for handling LiPD data',
     long_description=read("README.md"),
     long_description_content_type = 'text/markdown',
-    author='Varun Ratnakar',
+    author='Varun Ratnakar, Deborah Khider',
     author_email='varunratnakar@gmail.com',
     url='https://github.com/linkedearth/pylipd',
     download_url='https://github.com/linkedearth/pylipd/tarball/'+version,
     keywords=['Paleoclimate, Data Analysis, LiPD'],
     package_dir = {'':'.'},
     classifiers=[],
     install_requires=[
         "rdflib",
         "pandas",
         "doi2bib",
         "pybtex",
         "tqdm",
-        "bagit"
+        "bagit",
+        "numpy"
     ],
     python_requires=">=3.9.0"
 )
```

