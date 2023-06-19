# Comparing `tmp/Hefesto-0.4.3.tar.gz` & `tmp/Hefesto-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hefesto-0.4.3.tar", last modified: Thu Jun  8 12:02:56 2023, max compression
+gzip compressed data, was "Hefesto-0.4.4.tar", last modified: Mon Jun 19 07:30:01 2023, max compression
```

## Comparing `Hefesto-0.4.3.tar` & `Hefesto-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-08 12:02:56.097395 Hefesto-0.4.3/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-08 12:02:56.097395 Hefesto-0.4.3/Hefesto/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.3/Hefesto/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    11315 2023-06-08 12:02:08.000000 Hefesto-0.4.3/Hefesto/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     6796 2023-06-07 10:58:15.000000 Hefesto-0.4.3/Hefesto/template.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-08 12:02:56.097395 Hefesto-0.4.3/Hefesto.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-08 12:02:55.000000 Hefesto-0.4.3/Hefesto.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-06-08 12:02:56.000000 Hefesto-0.4.3/Hefesto.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-06-08 12:02:55.000000 Hefesto-0.4.3/Hefesto.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-06-08 12:02:55.000000 Hefesto-0.4.3/Hefesto.egg-info/top_level.txt
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.3/MANIFEST.in
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-08 12:02:56.097395 Hefesto-0.4.3/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.3/README.md
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       22 2023-05-29 17:45:16.000000 Hefesto-0.4.3/requirements.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-06-08 12:02:56.097395 Hefesto-0.4.3/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-06-08 12:02:36.000000 Hefesto-0.4.3/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-19 07:30:01.926707 Hefesto-0.4.4/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-19 07:30:01.926707 Hefesto-0.4.4/Hefesto/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.4/Hefesto/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    12035 2023-06-19 07:29:08.000000 Hefesto-0.4.4/Hefesto/main.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     6781 2023-06-18 17:57:59.000000 Hefesto-0.4.4/Hefesto/template.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-19 07:30:01.926707 Hefesto-0.4.4/Hefesto.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-19 07:30:01.000000 Hefesto-0.4.4/Hefesto.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-06-19 07:30:01.000000 Hefesto-0.4.4/Hefesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-06-19 07:30:01.000000 Hefesto-0.4.4/Hefesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-06-19 07:30:01.000000 Hefesto-0.4.4/Hefesto.egg-info/top_level.txt
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.4/MANIFEST.in
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-19 07:30:01.926707 Hefesto-0.4.4/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.4/README.md
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       22 2023-05-29 17:45:16.000000 Hefesto-0.4.4/requirements.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-06-19 07:30:01.926707 Hefesto-0.4.4/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-06-19 07:29:40.000000 Hefesto-0.4.4/setup.py
```

### Comparing `Hefesto-0.4.3/Hefesto/main.py` & `Hefesto-0.4.4/Hefesto/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,42 +113,50 @@
 
                 # Relate each YAML parameter with original data input
                 for element in config[1]["columns"].items():
                     for r in row[1].index:
                         if r == element[1]:
                             dict_element = {element[0]:row[1][r]}
                             row_df[milisec_point].update(dict_element)
+                            
 
                 # Store formed element into the final table:
                 final_row_df = pd.DataFrame(row_df[milisec_point], index=[1])
                 resulting_df = pd.concat([resulting_df, final_row_df])
 
         # Reset Index:    
         resulting_df = resulting_df.reset_index(drop=True)
         # Turn any nan to None:
+
         resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+
+
         # Value edition:
         resulting_df = self.valueEdition(resulting_df)
+        resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+
+
         # Clean blanks:
         resulting_df = self.cleanBlanks(resulting_df)
-        
         # uniqid generation:
+        # print(resulting_df)
+
         resulting_df['uniqid'] = ""
         for i in resulting_df.index:
             resulting_df.at[i, "uniqid"] = milisec()
 
         
         print("Structural transformation: Done")
         new = Hefesto.__init__(self, datainput= resulting_df, reset = True)
         return new
 
     def cleanBlanks(self, resulting_df): # TODO solve the attribute_type value problem
 
         for row_final in resulting_df.iterrows():
-            if row_final[1]["value"] == None and row_final[1]["valueIRI"] == None and row_final[1]["comments"] == None and row_final[1]["agent_id"] == None:
+            if row_final[1]["value"] == None and row_final[1]["valueIRI"] == None and row_final[1]["comments"] == None and row_final[1]["agent_id"] == None and row_final[1]["target_type"] == None:
                 resulting_df = resulting_df.drop(row_final[0])
         del resulting_df["value"]
         del resulting_df["valueIRI"]
 
         return resulting_df
 
     def valueEdition(self, resulting_df):
@@ -166,41 +174,50 @@
         # Datatype:
         datatypeRelation = {
             "xsd:string":"value_string",
             "xsd:date" : "value_date",
             "xsd:float": "value_float",
             "xsd:integer":"value_integer"
         }
+        modelList = ["Deathdate","First_Visit","Symptoms_onset"]
         
         # Value edition:
         for index, row in resulting_df.iterrows():
             for k,v in datatypeRelation.items():
                 
                 # value ---> value_DATATYPE:
                 if row["value_datatype"] == k:
                     resulting_df.at[index, v] = resulting_df["value"][index]
                     resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
-                # enddate correction:
-                if row["startdate"] != None and row["enddate"] == None:
-                    resulting_df.at[index,"enddate"] = resulting_df["startdate"][index]
-                    resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
-
             for k,v in valueRelation.items():
                 # valueIRI ---> attribute_id/value:
                 if row["model"] == k:
                     resulting_df.at[index, v] = resulting_df["valueIRI"][index]
                     resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
             # attribute_id_value
             if row["model"] == "Genetic":
                 resulting_df.at[index, "attribute_id_value"] = resulting_df["value"][index]
                 resulting_df.at[index, "value_string"] = None # Deleting the value_string in case it moves from value to value_string
                 resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
+            if row["value"] != None and row["value_datatype"] == "xsd:date":
+                resulting_df.at[index, "date"] = resulting_df["value"][index]
+                resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+
+            if row["value"] != None and row["value_datatype"] == "xsd:float" and row["model"] in modelList:
+                resulting_df.at[index, "age"] = resulting_df["value"][index]
+                resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+
+            # enddate correction:
+            if row["startdate"] != None and row["enddate"] == None:
+                resulting_df.at[index,"enddate"] = resulting_df["startdate"][index]
+                resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+
         return resulting_df
 
     def get_uri(self, col, ont):
 
         
         if not col in list(self.df_data.columns):
             sys.exit("ERROR: selected column doesnt exist")
@@ -272,15 +289,15 @@
         print("Replacement from " + key + "to "+ value + " at column " + col +": Done")
         new = Hefesto.__init__(self, datainput= self.df_data, reset = True)
         return new
         
 
 # # Test 1:
 
-# test = Hefesto(datainput = "../data/INPUT_DATA_test.csv")
+# test = Hefesto(datainput = "../data/INPUT_DATA.csv")
 # transform = test.transformFiab()
 # transform.to_csv ("../data/OUTPUT_DATA.csv", index = False, header=True)
 
 # # # Test 2
 # with open("../data/CDEconfig.yaml") as file:
 #     configuration = yaml.load(file, Loader=yaml.FullLoader)
```

### Comparing `Hefesto-0.4.3/Hefesto/template.py` & `Hefesto-0.4.4/Hefesto/template.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,222 +6,216 @@
     Birthyear = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type = "http://purl.obolibrary.org/obo/NCIT_C83164",
       value_datatype = "xsd:integer",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Birthdate = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type = "http://purl.obolibrary.org/obo/NCIT_C68615",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Deathdate = dict( 
       process_type= "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type = "http://purl.obolibrary.org/obo/NCIT_C70810",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     First_visit = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type = "http://purl.obolibrary.org/obo/NCIT_C164021",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Sex = dict( 
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C28421",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
 
     Status = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C166244",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Diagnosis = dict(
       process_type= "http://purl.obolibrary.org/obo/NCIT_C15220",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type2= "http://purl.obolibrary.org/obo/NCIT_C2991",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Symptoms = dict(
       process_type= "http://purl.obolibrary.org/obo/NCIT_C15220",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type2= "http://purl.obolibrary.org/obo/NCIT_C100104",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
+    ),
+
+    Symptoms_onset = dict(
+      process_type= "http://purl.obolibrary.org/obo/NCIT_C15220",
+      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
+      attribute_type2= "http://purl.obolibrary.org/obo/NCIT_C100104",
+      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C124353",
+      value_datatype = "xsd:date",
+      startdate = None,
+      enddate = None,
+      pid = None
     ),
 
     Genetic = dict(
       process_type= "http://purl.obolibrary.org/obo/NCIT_C15709",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type= "http://purl.obolibrary.org/obo/NCIT_C103223",
       attribute_id_type = "http://purl.obolibrary.org/obo/NCIT_C45766",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Consent_contacted = dict(
       process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
       output_type = "http://purl.obolibrary.org/obo/OBIB_0000488",
       attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Consent_used = dict(
       process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
       output_type = "http://purl.obolibrary.org/obo/DUO_0000001",
       attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Biobank = dict(
       process_type= "http://purl.obolibrary.org/obo/OMIABIS_0000061",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C115570",
       attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25429",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Disability = dict(
       process_type = None,
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type = "http://purl.obolibrary.org/obo/NCIT_C21007",
       value_datatype = "xsd:float",
       startdate = None,
       enddate = None,
-      pid = None,
-      context_id = None
+      pid = None
     ),
 
     Body_measurement = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470" ,
       output_type=  "http://purl.obolibrary.org/obo/NCIT_C70856" ,
       value_datatype= "xsd:float" ,
       startdate= None ,
       enddate= None ,
       comments= None ,
-      pid= None ,
-      context_id= None 
+      pid= None  
     ),
 
 
     Lab_measurement = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C25294" ,
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856" ,
       value_datatype= "xsd:float" ,
       startdate= None ,
       enddate= None ,
       comments= None ,
-      pid= None ,
-      context_id= None 
+      pid= None 
     ),
 
 
     Imaging = dict(
       process_type = None ,
       output_type =  "http://purl.obolibrary.org/obo/NCIT_C70856" ,
       attribute_type = "http://purl.obolibrary.org/obo/NCIT_C176708",
       attribute_id_type = "http://purl.obolibrary.org/obo/NCIT_C81289",
       value_datatype = "xsd:string" ,
       startdate= None ,
       enddate= None ,
       comments= None ,
-      pid = None ,
-      context_id= None 
+      pid = None 
     ),
 
 
     Intervention = dict(
       value_datatype = "xsd:string" ,
+      process_type = None ,
+      target_type = None ,
       startdate= None ,
       enddate= None ,
       comments= None ,
-      pid= None ,
-      context_id= None 
+      pid= None 
     ),
 
 
     Clinical_trial = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C71104" ,
       output_type=  "http://purl.obolibrary.org/obo/NCIT_C115575" ,
       attribute_type2 = "http://purl.obolibrary.org/obo/NCIT_C2991" ,
       agent_type = "http://purl.obolibrary.org/obo/NCIT_C16696" ,
       value_datatype= "xsd:string",
       startdate= None ,
       enddate= None ,
       comments= None ,
-      pid= None ,
-      context_id= None
+      pid= None 
     ),
 
 
     Medications = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C25409",
       output_type =  "http://purl.obolibrary.org/obo/NCIT_C459" ,
       agent_type = "http://purl.obolibrary.org/obo/NCIT_C177929",
       value_datatype= "xsd:float",
       startdate= None ,
       enddate = None ,
       comments = None ,
-      pid = None ,
-      context_id = None 
+      pid = None 
     )
 
 
   )
```

### Comparing `Hefesto-0.4.3/README.md` & `Hefesto-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `Hefesto-0.4.3/setup.py` & `Hefesto-0.4.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     readme = readme_file.read()
 
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name="Hefesto",
-    version="0.4.3",
+    version="0.4.4",
     packages=["Hefesto"],
     author="Pablo Alarcón Moreno",
     author_email="pabloalarconmoreno@gmail.com",
     url="https://github.com/pabloalarconm/hefesto",
     description="Preprocessing datatable toolkit",
     license="MIT",
     keywords=["EJP","CDE"]
```

