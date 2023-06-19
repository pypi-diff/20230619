# Comparing `tmp/apidb-0.1.5.tar.gz` & `tmp/apidb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidb-0.1.5.tar", last modified: Wed Feb  1 03:08:43 2023, max compression
+gzip compressed data, was "apidb-0.2.0.tar", last modified: Mon Jun 19 02:43:24 2023, max compression
```

## Comparing `apidb-0.1.5.tar` & `apidb-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 03:08:43.805966 apidb-0.1.5/
--rw-rw-rw-   0        0        0     1090 2023-01-26 02:06:17.000000 apidb-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1968 2023-02-01 03:08:43.804969 apidb-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1464 2023-01-26 03:56:45.000000 apidb-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-02-01 03:08:43.786020 apidb-0.1.5/apidb/
--rw-rw-rw-   0        0        0        0 2023-01-26 02:04:32.000000 apidb-0.1.5/apidb/__init__.py
--rw-rw-rw-   0        0        0    13427 2023-02-01 02:48:05.000000 apidb-0.1.5/apidb/apidb_core.py
-drwxrwxrwx   0        0        0        0 2023-02-01 03:08:43.803972 apidb-0.1.5/apidb.egg-info/
--rw-rw-rw-   0        0        0     1968 2023-02-01 03:08:43.000000 apidb-0.1.5/apidb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-02-01 03:08:43.000000 apidb-0.1.5/apidb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 03:08:43.000000 apidb-0.1.5/apidb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-02-01 03:08:43.000000 apidb-0.1.5/apidb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-01 03:08:43.000000 apidb-0.1.5/apidb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-01 03:08:43.805966 apidb-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      771 2023-02-01 03:08:40.000000 apidb-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:43:24.560490 apidb-0.2.0/
+-rw-rw-rw-   0        0        0     1090 2023-01-26 02:06:17.000000 apidb-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1968 2023-06-19 02:43:24.560490 apidb-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1464 2023-01-26 03:56:45.000000 apidb-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 02:43:24.540544 apidb-0.2.0/apidb/
+-rw-rw-rw-   0        0        0        0 2023-01-26 02:04:32.000000 apidb-0.2.0/apidb/__init__.py
+-rw-rw-rw-   0        0        0    13794 2023-06-19 02:42:22.000000 apidb-0.2.0/apidb/apidb_core.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:43:24.559493 apidb-0.2.0/apidb.egg-info/
+-rw-rw-rw-   0        0        0     1968 2023-06-19 02:43:23.000000 apidb-0.2.0/apidb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-06-19 02:43:24.000000 apidb-0.2.0/apidb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 02:43:24.000000 apidb-0.2.0/apidb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-19 02:43:24.000000 apidb-0.2.0/apidb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 02:43:24.000000 apidb-0.2.0/apidb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 02:43:24.560490 apidb-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-06-19 02:43:21.000000 apidb-0.2.0/setup.py
```

### Comparing `apidb-0.1.5/LICENSE` & `apidb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apidb-0.1.5/PKG-INFO` & `apidb-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidb
-Version: 0.1.5
+Version: 0.2.0
 Summary: Autogenerate API based on DB structure directly from Python using ORM
 Home-page: https://github.com/DovaX/apidb
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apidb-0.1.5/README.md` & `apidb-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `apidb-0.1.5/apidb/apidb_core.py` & `apidb-0.2.0/apidb/apidb_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from flask import jsonify, request
 
 
-
-
-
 from fastapi import FastAPI
 
 
 
 # description = """
 # This is your API
 # """
@@ -38,96 +35,100 @@
         f.__name__ = add_function_parameter
         return f
     return decorator
 
 
 
 class CustomEndpoint:
-    def __init__(self,app,name,operation,function,api_url="/api/",id_variable="id",show_method_tags=True,show_endpoint_tags=True):
+    def __init__(self,app,name,operation,function,body_template,api_url="/api/",id_variable="id",show_method_tags=True,show_endpoint_tags=True):
         self.app=app
         self.name=name #should be in plural
         self.operation=operation
         self.function=function
+        self.body_template = body_template
         self.api_url=api_url
         self.id_variable=id_variable
         self.show_method_tags=show_method_tags
         self.show_endpoint_tags=show_endpoint_tags
         self.operation_method_tag_dict={"read_all":"get","read":"get","create":"post","delete":"delete","delete_all":"delete","update":"put"}
       
          
     def initialize_custom_endpoint(self):
         tags=[]
+        body_template = self.body_template
         if self.show_endpoint_tags:
             tags+=[self.name.capitalize()+" Methods"]
         if self.show_method_tags:
             tags+=[self.operation_method_tag_dict[self.operation].capitalize()+" Methods"]
     
         if 'read_all'==self.operation:
             @self.app.get(self.api_url+self.name,tags=tags)
             @rename_function('read_all_'+self.name)
             def read_all_items():
-                result=self.function() 
+                result=self.function()
                 return {"result":result}
         
         if 'read'==self.operation:
             item=self.name[:-1]
-            @self.app.get(self.api_url+self.name[:-1]+"/{"+self.id_variable+"}",tags=tags)
+            @self.app.get(self.api_url+item+"/{"+self.id_variable+"}",tags=tags)
             @rename_function('read_'+item)
             def read_item(uid): #TODO: generalize uid for any variable name
                 result=self.function(uid) 
                 return {"result":result}
     
     
         if 'create'==self.operation:
-            item=self.name
-            @self.app.post(self.api_url+self.name,tags=tags)
+            item=self.name[:-1]
+            @self.app.post(self.api_url+item,tags=tags)
             @rename_function('create_'+item)
-            def add_item(**kwargs):
-                result=self.function(kwargs)
+            def add_item(body_template:body_template):
+                params = [getattr(body_template, field) for field in body_template.dict().keys()]
+                result = self.function(params)
                 return {"result":result}
+                # return {}
             
         if 'update'==self.operation:
             item=self.name[:-1]
-            @self.app.put(self.api_url+self.name[:-1]+"/{"+self.id_variable+"}",tags=tags)
+            @self.app.put(self.api_url+item+"/{"+self.id_variable+"}",tags=tags)
             @rename_function('update_'+item)
-            def update_item(uid):
-                result=self.function()
+            def update_item(uid, body_template:body_template):
+                params = [uid] + [getattr(body_template, field) for field in body_template.dict().keys()]
+                result=self.function(params)
                 return {"result":result}
         
             
         if 'delete'==self.operation:
             item=self.name[:-1]
-            @self.app.delete(self.api_url+self.name[:-1]+"/{"+self.id_variable+"}",tags=tags)
+            @self.app.delete(self.api_url+item+"/{"+self.id_variable+"}",tags=tags)
             @rename_function('delete_'+item)
             def delete_item(uid):
-                result=self.function()
+                result=self.function(uid)
                 return {"result":result}
             
             
             
         if 'delete_all'==self.operation:
             @self.app.delete(self.api_url+self.name,tags=tags)
             @rename_function('delete_all_'+self.name)
             def delete_item():
                 result=self.function()
                 return {"result":result}
-    
-    
+
         # if 'update' in self.operation:
         #     item=self.name[:-1]
         #     @self.app.put("/api/"+self.name+"/<id>")
         #     @rename_function('update_'+item)
         #     def update_item(id,name=self.name): #name=self.name because of late binding - otherwise, it would assign all endpoints with the same name
         #         cur = mysql.connection.cursor()
         #         column1 = request.get_json()[column_names[0]]
-                
+        #
         #         cur.execute("UPDATE "+self.name+" SET "+column_names[0]+" = '" + str(column1) + "' where id = " + id)
         #         mysql.connection.commit()
         #         result = {column_names[0]:column1}
-            
+        #
         #         return jsonify({"reuslt": result})
     
         # if 'delete' in self.operation:
         #     item=self.name[:-1]
         #     @self.app.delete("/api/"+self.name+"/<id>")
         #     @rename_function('delete_'+item)
         #     def delete_item(id,name=self.name): #name=self.name because of late binding - otherwise, it would assign all endpoints with the same name
@@ -167,26 +168,27 @@
             operations.append(v)
         else:
             operations=v
         #print(operations)
         for i,operation in enumerate(operations):
             if type(operation)==tuple:
                 #print("A",operation)
-                
+
+                body_template = operation[2]
                 function=operation[1]
                 operation=operation[0]
-                
+
                 #print("A",operation,function)
             else:
                 function=lambda *x:print(*x)
                 
                 #print("B",operation,function)
         
             #print(operation,function)
-            custom_endpoint=CustomEndpoint(app,k,operation,function,api_url=api_url,id_variable=id_variable)
+            custom_endpoint=CustomEndpoint(app,k,operation,function,body_template,api_url=api_url,id_variable=id_variable)
             custom_endpoint.initialize_custom_endpoint()
             
 #initialize_api_from_db_api_dict(app)
 
 # custom_endpoint1=CustomEndpoint(app,"workspaces","read",get_all_workspaces)
 # custom_endpoint1.initialize_custom_endpoint()
 # custom_endpoint2=CustomEndpoint(app,"nodes","read",get_all_nodes)
```

### Comparing `apidb-0.1.5/apidb.egg-info/PKG-INFO` & `apidb-0.2.0/apidb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidb
-Version: 0.1.5
+Version: 0.2.0
 Summary: Autogenerate API based on DB structure directly from Python using ORM
 Home-page: https://github.com/DovaX/apidb
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apidb-0.1.5/setup.py` & `apidb-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='apidb',
-    version='0.1.5',
+    version='0.2.0',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Autogenerate API based on DB structure directly from Python using ORM',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/apidb',
     packages=setuptools.find_packages(),
```

