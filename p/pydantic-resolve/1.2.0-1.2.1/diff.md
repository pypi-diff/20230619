# Comparing `tmp/pydantic_resolve-1.2.0.tar.gz` & `tmp/pydantic_resolve-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.2.0.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.2.1.tar", max compression
```

## Comparing `pydantic_resolve-1.2.0.tar` & `pydantic_resolve-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.2.0/LICENSE
--rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.2.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.2.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2217 2023-06-18 14:39:54.866965 pydantic_resolve-1.2.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.2.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     5140 2023-06-18 15:07:09.605671 pydantic_resolve-1.2.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     3898 2023-06-18 01:11:55.489541 pydantic_resolve-1.2.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-06-18 15:00:21.348884 pydantic_resolve-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5694 2023-06-18 15:05:30.997444 pydantic_resolve-1.2.0/README.md
--rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 pydantic_resolve-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.2.1/LICENSE
+-rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.2.1/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-18 14:32:47.738157 pydantic_resolve-1.2.1/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2217 2023-06-18 14:39:54.866965 pydantic_resolve-1.2.1/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.2.1/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     5170 2023-06-19 10:02:56.509176 pydantic_resolve-1.2.1/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     3898 2023-06-18 01:11:55.489541 pydantic_resolve-1.2.1/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-06-19 10:06:48.583578 pydantic_resolve-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7293 2023-06-19 07:27:48.337999 pydantic_resolve-1.2.1/README.md
+-rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 pydantic_resolve-1.2.1/PKG-INFO
```

### Comparing `pydantic_resolve-1.2.0/LICENSE` & `pydantic_resolve-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.0/pydantic_resolve/__init__.py` & `pydantic_resolve-1.2.1/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.0/pydantic_resolve/core.py` & `pydantic_resolve-1.2.1/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.0/pydantic_resolve/resolver.py` & `pydantic_resolve-1.2.1/pydantic_resolve/resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,27 +101,28 @@
             val = await val
 
         # start to resolve
         val = await self.resolve(val)  
         # all children is resolved
         target.__setattr__(target_attr_name, val)
 
-        # execute post methods, accept no params
-        for post_key in core.iter_over_object_post_methods(target):
-            post_attr_name = post_key.replace(POST_PREFIX, '')
-            if not hasattr(target, post_attr_name):
-                raise ResolverTargetAttrNotFound(f"fail to run {post_key}(), attribute {post_attr_name} not found")
-
-            post_method = target.__getattribute__(post_key)
-            post_method()
 
     async def resolve(self, target: T) -> T:
         """ entry: resolve dataclass object or pydantic object / or list in place """
 
         if isinstance(target, (list, tuple)):
             await asyncio.gather(*[self.resolve(t) for t in target])
 
         if core.is_acceptable_type(target):
             await asyncio.gather(*[self.resolve_obj(target, field) 
                                    for field in core.iter_over_object_resolvers(target)])
 
+            # execute post methods, accept no params
+            for post_key in core.iter_over_object_post_methods(target):
+                post_attr_name = post_key.replace(POST_PREFIX, '')
+                if not hasattr(target, post_attr_name):
+                    raise ResolverTargetAttrNotFound(f"fail to run {post_key}(), attribute {post_attr_name} not found")
+
+                post_method = target.__getattribute__(post_key)
+                post_method()
+
         return target
```

### Comparing `pydantic_resolve-1.2.0/pydantic_resolve/util.py` & `pydantic_resolve-1.2.1/pydantic_resolve/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.2.0/pyproject.toml` & `pydantic_resolve-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.2.0"
+version = "1.2.1"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.2.0/PKG-INFO` & `pydantic_resolve-1.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.2.0
+Version: 1.2.1
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
@@ -31,77 +31,100 @@
 > A small yet powerful package which can run resolvers to generate deep nested datasets.
 
 [Change log](./changelog.md)
 
 **example**:
 
 ```python
-# define loader functions
+import asyncio
+from typing import List, Optional
+from pydantic import BaseModel
+from pydantic_resolve import Resolver, mapper, LoaderDepend
+
+# define dataset and loader functions
 async def friends_batch_load_fn(names):
     mock_db = {
         'tangkikodo': ['tom', 'jerry'],
         'john': ['mike', 'wallace'],
         'trump': ['sam', 'jim'],
         'sally': ['sindy', 'lydia'],
     }
     return [mock_db.get(name, []) for name in names]
 
 async def contact_batch_load_fn(names):
     mock_db = {
-        'tom': 100, 'jerry':200, 'mike': 3000, 'wallace': 400, 'sam': 500,
-        'jim': 600, 'sindy': 700, 'lydia': 800, 'tangkikodo': 900, 'john': 1000,
-        'trump': 1200, 'sally': 1300,
+        'tom': 1001, 'jerry': 1002, 'mike': 1003, 'wallace': 1004, 'sam': 1005,
+        'jim': 1006, 'sindy': 1007, 'lydia': 1008, 'tangkikodo': 1009, 'john': 1010,
+        'trump': 2011, 'sally': 2012,
     }
-    return [mock_db.get(name, None) for name in names]
+    result = []
+    for name in names:
+        n = mock_db.get(name, None)
+        result.append({'number': n} if n else None)
+    return result
 
-# define schemas
+# define data schemas
 class Contact(BaseModel):
     number: Optional[int]
 
 class Friend(BaseModel):
     name: str
 
     contact: Optional[Contact] = None
-    @mapper(lambda n: Contact(number=n))
-    def resolve_contact(self, loader=LoaderDepend(contact_batch_load_fn)):
-        return loader.load(self.name)
+    @mapper(Contact)                                          # 1. resolve dataloader and map return dict to Contact object
+    def resolve_contact(self, contact_loader=LoaderDepend(contact_batch_load_fn)):
+        return contact_loader.load(self.name)
+
+    is_contact_10: bool = False
+    def post_is_contact_10(self):                             # 3. after resolve_contact executed, do extra computation
+        if self.contact:
+            if str(self.contact.number).startswith('10'):
+                self.is_contact_10 = True
+        else:
+            self.is_contact_10 = False
 
 class User(BaseModel):
     name: str
     age: int
 
     greeting: str = ''
-    def resolve_greeting(self):
+    async def resolve_greeting(self):
+        await asyncio.sleep(1)
         return f"hello, i'm {self.name}, {self.age} years old."
 
     contact: Optional[Contact] = None
-    @mapper(lambda n: Contact(number=n))
-    def resolve_contact(self, loader=LoaderDepend(contact_batch_load_fn)):
-        return loader.load(self.name)
+    @mapper(Contact)
+    def resolve_contact(self, contact_loader=LoaderDepend(contact_batch_load_fn)):
+        return contact_loader.load(self.name)
 
     friends: List[Friend] = []
-    @mapper(lambda items: [Friend(name=item) for item in items])  # transform after data received
-    def resolve_friends(self, loader=LoaderDepend(friends_batch_load_fn)):
-        return loader.load(self.name)
+    @mapper(lambda names: [Friend(name=name) for name in names])
+    def resolve_friends(self, friend_loader=LoaderDepend(friends_batch_load_fn)):
+        return friend_loader.load(self.name)
+
+    friend_count: int = 0
+    def post_friend_count(self):
+        self.friend_count = len(self.friends)
 
 class Root(BaseModel):
     users: List[User] = []
     @mapper(lambda items: [User(**item) for item in items])
     def resolve_users(self):
         return [
             {"name": "tangkikodo", "age": 19},
             {"name": "john", "age": 20},
-            # {"name": "trump", "age": 21},
-            # {"name": "sally", "age": 22},
-            # {"name": "no man", "age": 23},
+            {"name": "trump", "age": 21},
+            {"name": "sally", "age": 22},
+            {"name": "no man", "age": 23},
         ]
 
 async def main():
     import json
-    root = await Resolver().resolve(Root())
+    root = Root()
+    root = await Resolver().resolve(root)                 # 4. run it
     dct = root.dict()
     print(json.dumps(dct, indent=4))
 
 asyncio.run(main())
 ```
 
 **output**:
@@ -110,79 +133,135 @@
 {
   "users": [
     {
       "name": "tangkikodo",
       "age": 19,
       "greeting": "hello, i'm tangkikodo, 19 years old.",
       "contact": {
-        "number": 900
+        "number": 1009
       },
       "friends": [
         {
           "name": "tom",
           "contact": {
-            "number": 100
-          }
+            "number": 1001
+          },
+          "is_contact_10": true
         },
         {
           "name": "jerry",
           "contact": {
-            "number": 200
-          }
+            "number": 1002
+          },
+          "is_contact_10": true
         }
-      ]
+      ],
+      "friend_count": 2
     },
     {
       "name": "john",
-      "age": 21,
-      "greeting": "hello, i'm john, 21 years old.",
+      "age": 20,
+      "greeting": "hello, i'm john, 20 years old.",
       "contact": {
-        "number": 1000
+        "number": 1010
       },
       "friends": [
         {
           "name": "mike",
           "contact": {
-            "number": 3000
-          }
+            "number": 1003
+          },
+          "is_contact_10": true
         },
         {
           "name": "wallace",
           "contact": {
-            "number": 400
-          }
+            "number": 1004
+          },
+          "is_contact_10": true
         }
-      ]
+      ],
+      "friend_count": 2
+    },
+    {
+      "name": "trump",
+      "age": 21,
+      "greeting": "hello, i'm trump, 21 years old.",
+      "contact": {
+        "number": 2011
+      },
+      "friends": [
+        {
+          "name": "sam",
+          "contact": {
+            "number": 1005
+          },
+          "is_contact_10": true
+        },
+        {
+          "name": "jim",
+          "contact": {
+            "number": 1006
+          },
+          "is_contact_10": true
+        }
+      ],
+      "friend_count": 2
+    },
+    {
+      "name": "sally",
+      "age": 22,
+      "greeting": "hello, i'm sally, 22 years old.",
+      "contact": {
+        "number": 2012
+      },
+      "friends": [
+        {
+          "name": "sindy",
+          "contact": {
+            "number": 1007
+          },
+          "is_contact_10": true
+        },
+        {
+          "name": "lydia",
+          "contact": {
+            "number": 1008
+          },
+          "is_contact_10": true
+        }
+      ],
+      "friend_count": 2
+    },
+    {
+      "name": "no man",
+      "age": 23,
+      "greeting": "hello, i'm no man, 23 years old.",
+      "contact": null,
+      "friends": [],
+      "friend_count": 0
     }
   ]
 }
 ```
 
-- Full-feature [example](./examples/6_sqlalchemy_loaderdepend_global_filter.py) which includes `dataloader`, `LoaderDepend` and global `loader_filters`
-- Helps you asynchoronously, resursively resolve a pydantic object (or dataclass object)
-- When used in conjunction with aiodataloader, allows you to easily generate nested data structures without worrying about generating N+1 queries.
-- say byebye to contextvars when using dataloader.
-- Inspired by [GraphQL](https://graphql.org/) and [graphene](https://graphene-python.org/)
-
 ## Install
 
 ```shell
 pip install pydantic-resolve
-
-pip install "pydantic-resolve[dataloader]"  # install with aiodataloader, from v1.0, aiodataloader is a default dependency, [dataloader] is removed.
 ```
 
 - use `resolve` for simple scenario,
 - use `Resolver` and `LoaderDepend` for complicated nested batch query.
 
 ```python
 from pydantic_resolve import (
     resolve,                     # handle simple resolving task
     Resolver, LoaderDepend,      # handle schema resolving with LoaderDepend and DataLoader
-    ResolverTargetAttrNotFound, DataloaderDependCantBeResolved, LoaderFieldNotProvidedError
+    ResolverTargetAttrNotFound, DataloaderDependCantBeResolved, LoaderFieldNotProvidedError  # errors
 )
 ```
 
 ## Run FastAPI example
 
 ```shell
 poetry shell
```

