# Comparing `tmp/wow_commodities-1.0.0.tar.gz` & `tmp/wow_commodities-1.0.1.tar.gz`

## Comparing `wow_commodities-1.0.0.tar` & `wow_commodities-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/app.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/src/__about__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/src/get_commodities.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/src/get_token.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/src/region_locale.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/.gitignore
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 wow_commodities-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/app.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/src/__about__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/src/get_commodities.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/src/get_token.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/src/region_locale.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/.gitignore
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 wow_commodities-1.0.1/PKG-INFO
```

### Comparing `wow_commodities-1.0.0/app.py` & `wow_commodities-1.0.1/app.py`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.0/src/get_commodities.py` & `wow_commodities-1.0.1/src/get_commodities.py`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.0/src/get_token.py` & `wow_commodities-1.0.1/src/get_token.py`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.0/.gitignore` & `wow_commodities-1.0.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
+pypirc
 .env
 .venv
 .hatch
 env/
 venv/
 ENV/
 env.bak/
```

### Comparing `wow_commodities-1.0.0/LICENSE.txt` & `wow_commodities-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.0/README.md` & `wow_commodities-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 -----
 
 **WoW Commodities** is a tool to download [World of Warcraft](https://worldofwarcraft.blizzard.com/) commodities auction data using [Blizzard API](https://develop.battle.net/documentation).
 
 ## Installation
 
 ```console
-pip install wow-commodities
+pip install WoW_Commodities
 ```
 
 ## Usage
 
 **WoW Commodities** needs tree positional arguments (in that order): 
 - id: a client ID from the Blizzard API.
 - secret: a secret from the Blizzard API.
```

### Comparing `wow_commodities-1.0.0/pyproject.toml` & `wow_commodities-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.0/PKG-INFO` & `wow_commodities-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WoW_Commodities
-Version: 1.0.0
+Version: 1.0.1
 Summary: Download World of Warcraft commodities auction data for the specified region.
 Project-URL: Documentation, https://github.com/Godrigos/wow-commodities#readme
 Project-URL: Issues, https://github.com/Godrigos/wow-commodities/issues
 Project-URL: Source, https://github.com/Godrigos/wow-commodities
 Author-email: "Aluizio, R." <gambit01@bol.com.br>
 License-Expression: LGPL-3.0-or-later
 License-File: LICENSE.txt
@@ -26,15 +26,15 @@
 -----
 
 **WoW Commodities** is a tool to download [World of Warcraft](https://worldofwarcraft.blizzard.com/) commodities auction data using [Blizzard API](https://develop.battle.net/documentation).
 
 ## Installation
 
 ```console
-pip install wow-commodities
+pip install WoW_Commodities
 ```
 
 ## Usage
 
 **WoW Commodities** needs tree positional arguments (in that order): 
 - id: a client ID from the Blizzard API.
 - secret: a secret from the Blizzard API.
```

