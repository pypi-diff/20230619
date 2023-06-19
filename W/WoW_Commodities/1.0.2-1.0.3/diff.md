# Comparing `tmp/wow_commodities-1.0.2.tar.gz` & `tmp/wow_commodities-1.0.3.tar.gz`

## Comparing `wow_commodities-1.0.2.tar` & `wow_commodities-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/app.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/src/__about__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/src/get_commodities.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/src/get_token.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/src/region_locale.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/.gitignore
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 wow_commodities-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/app.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/src/__about__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/src/get_commodities.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/src/get_token.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/src/region_locale.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/.gitignore
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 wow_commodities-1.0.3/PKG-INFO
```

### Comparing `wow_commodities-1.0.2/app.py` & `wow_commodities-1.0.3/app.py`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.2/src/get_commodities.py` & `wow_commodities-1.0.3/src/get_commodities.py`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.2/src/get_token.py` & `wow_commodities-1.0.3/src/get_token.py`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.2/.gitignore` & `wow_commodities-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.2/LICENSE.txt` & `wow_commodities-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.2/README.md` & `wow_commodities-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,24 @@
 
 **WoW Commodities** may also take optional arguments defining the region of the downloaded data. The supported regions are:
 
 - us = North America
 - eu = Europe
 - kr = Korea
 - tw = Taiwan
+- cn = China
 
 Defaults to `us`.
 
 And a localization paramenter for language translations. The supported localization are:
 - US Region: en_US, es_MX, pt_BR
 - EU Region: en_GB, es_ES, fr_FR, ru_RU, de_DE, pt_PT, it_IT
 - KR Region: ko_KR
 - TW Region: zh_TW.
+- CN Region: zh_CN
 
 Bear in mind that not all combinations of Regions and Localizations are valid. For more details on those combinations read [this article](https://develop.battle.net/documentation/guides/regionality-and-apis).
 
 Defaults to `en_US`.
 
 With optional arguments:
 ```console
```

### Comparing `wow_commodities-1.0.2/pyproject.toml` & `wow_commodities-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wow_commodities-1.0.2/PKG-INFO` & `wow_commodities-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WoW_Commodities
-Version: 1.0.2
+Version: 1.0.3
 Summary: Download World of Warcraft commodities auction data for the specified region.
 Project-URL: Documentation, https://github.com/Godrigos/WoW_Commodities#readme
 Project-URL: Issues, https://github.com/Godrigos/WoW_Commodities/issues
 Project-URL: Source, https://github.com/Godrigos/WoW_Commodities
 Author-email: "Aluizio, R." <gambit01@bol.com.br>
 License-Expression: LGPL-3.0-or-later
 License-File: LICENSE.txt
@@ -44,22 +44,24 @@
 
 **WoW Commodities** may also take optional arguments defining the region of the downloaded data. The supported regions are:
 
 - us = North America
 - eu = Europe
 - kr = Korea
 - tw = Taiwan
+- cn = China
 
 Defaults to `us`.
 
 And a localization paramenter for language translations. The supported localization are:
 - US Region: en_US, es_MX, pt_BR
 - EU Region: en_GB, es_ES, fr_FR, ru_RU, de_DE, pt_PT, it_IT
 - KR Region: ko_KR
 - TW Region: zh_TW.
+- CN Region: zh_CN
 
 Bear in mind that not all combinations of Regions and Localizations are valid. For more details on those combinations read [this article](https://develop.battle.net/documentation/guides/regionality-and-apis).
 
 Defaults to `en_US`.
 
 With optional arguments:
 ```console
```

