# Comparing `tmp/autotraders-1.5.4.tar.gz` & `tmp/autotraders-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.5.4.tar", last modified: Sun Jun 18 21:54:42 2023, max compression
+gzip compressed data, was "autotraders-1.5.5.tar", last modified: Sun Jun 18 22:53:06 2023, max compression
```

## Comparing `autotraders-1.5.4.tar` & `autotraders-1.5.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.437183 autotraders-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-18 21:54:25.000000 autotraders-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 21:54:42.437183 autotraders-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-18 21:54:25.000000 autotraders-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.425183 autotraders-1.5.4/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.429183 autotraders-1.5.4/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.429183 autotraders-1.5.4/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.433183 autotraders-1.5.4/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.433183 autotraders-1.5.4/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.437183 autotraders-1.5.4/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/cargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/states.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-18 21:54:25.000000 autotraders-1.5.4/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.429183 autotraders-1.5.4/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 21:54:42.000000 autotraders-1.5.4/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-18 21:54:25.000000 autotraders-1.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 21:54:42.437183 autotraders-1.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:54:42.437183 autotraders-1.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-18 21:54:25.000000 autotraders-1.5.4/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.395029 autotraders-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-18 22:52:54.000000 autotraders-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 22:53:06.395029 autotraders-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-18 22:52:54.000000 autotraders-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/cargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-18 22:52:54.000000 autotraders-1.5.5/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 22:53:06.000000 autotraders-1.5.5/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-18 22:52:54.000000 autotraders-1.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 22:53:06.395029 autotraders-1.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:53:06.391029 autotraders-1.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-18 22:52:54.000000 autotraders-1.5.5/tests/test_util.py
```

### Comparing `autotraders-1.5.4/LICENSE` & `autotraders-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/PKG-INFO` & `autotraders-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.4
+Version: 1.5.5
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.4/README.md` & `autotraders-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/agent.py` & `autotraders-1.5.5/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/faction/__init__.py` & `autotraders-1.5.5/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/faction/contract.py` & `autotraders-1.5.5/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/map/system.py` & `autotraders-1.5.5/autotraders/map/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/map/waypoint.py` & `autotraders-1.5.5/autotraders/map/waypoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from autotraders.space_traders_entity import SpaceTradersEntity
 
 
 class Waypoint(SpaceTradersEntity):
     waypoint_type: str
     faction: Optional[str]
     traits: Optional[list[Trait]]
-    marketplace: bool
-    shipyard: bool
+    marketplace: Optional[bool]
+    shipyard: Optional[bool]
     symbol: MapSymbol
     x: int
     y: int
 
     def __init__(
         self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
     ):
@@ -39,20 +39,24 @@
         else:
             self.faction = None
         self.traits = None
         if "traits" in data:
             self.traits = []
             for trait in data["traits"]:
                 self.traits.append(Trait(trait))
-        self.marketplace = (
-            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
-        )
-        self.shipyard = (
-            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
-        )
+        if self.traits is not None:
+            self.marketplace = (
+                len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
+            )
+            self.shipyard = (
+                len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+            )
+        else:
+            self.marketplace = None
+            self.shipyard = None
 
     @staticmethod
     def all(session, system_symbol, page: int = 1) -> PaginatedList:
         def paginated_func(p, num_per_page):
             r = session.get(
                 session.base_url
                 + "systems/"
```

### Comparing `autotraders-1.5.4/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.5.5/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.5.5/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.5.5/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.5.5/autotraders/map/waypoint_types/shipyard.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/paginated_list.py` & `autotraders-1.5.5/autotraders/paginated_list.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/session.py` & `autotraders-1.5.5/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/shared_models/map_symbol.py` & `autotraders-1.5.5/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/shared_models/transaction.py` & `autotraders-1.5.5/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/ship/__init__.py` & `autotraders-1.5.5/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/ship/cargo.py` & `autotraders-1.5.5/autotraders/ship/cargo.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/ship/nav.py` & `autotraders-1.5.5/autotraders/ship/nav.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/ship/ship_components.py` & `autotraders-1.5.5/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/space_traders_entity.py` & `autotraders-1.5.5/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/status.py` & `autotraders-1.5.5/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders/util.py` & `autotraders-1.5.5/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/autotraders.egg-info/PKG-INFO` & `autotraders-1.5.5/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.5.4
+Version: 1.5.5
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.5.4/autotraders.egg-info/SOURCES.txt` & `autotraders-1.5.5/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/pyproject.toml` & `autotraders-1.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.5.4"
+version = "1.5.5"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.5.4/tests/test_init.py` & `autotraders-1.5.5/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/tests/test_map.py` & `autotraders-1.5.5/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/tests/test_ship.py` & `autotraders-1.5.5/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.5.4/tests/test_util.py` & `autotraders-1.5.5/tests/test_util.py`

 * *Files identical despite different names*

