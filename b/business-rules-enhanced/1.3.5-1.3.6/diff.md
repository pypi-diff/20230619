# Comparing `tmp/business-rules-enhanced-1.3.5.tar.gz` & `tmp/business-rules-enhanced-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "business-rules-enhanced-1.3.5.tar", last modified: Wed Jun  7 10:21:05 2023, max compression
+gzip compressed data, was "business-rules-enhanced-1.3.6.tar", last modified: Mon Jun 19 18:33:55 2023, max compression
```

## Comparing `business-rules-enhanced-1.3.5.tar` & `business-rules-enhanced-1.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/business_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    58368 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/six.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-07 10:21:05.000000 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 10:21:05.000000 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:21:05.000000 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 10:21:05.000000 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:33:55.746492 business-rules-enhanced-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-19 18:33:55.746492 business-rules-enhanced-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:33:55.746492 business-rules-enhanced-1.3.6/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/business_rules/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/business_rules/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/business_rules/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58428 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/business_rules/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/business_rules/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/business_rules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/business_rules/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:33:55.746492 business-rules-enhanced-1.3.6/business_rules_enhanced.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-19 18:33:55.000000 business-rules-enhanced-1.3.6/business_rules_enhanced.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 18:33:55.000000 business-rules-enhanced-1.3.6/business_rules_enhanced.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:33:55.000000 business-rules-enhanced-1.3.6/business_rules_enhanced.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 18:33:55.000000 business-rules-enhanced-1.3.6/business_rules_enhanced.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:33:55.746492 business-rules-enhanced-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-19 18:33:26.000000 business-rules-enhanced-1.3.6/setup.py
```

### Comparing `business-rules-enhanced-1.3.5/LICENSE` & `business-rules-enhanced-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.5/PKG-INFO` & `business-rules-enhanced-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: business-rules-enhanced
-Version: 1.3.5
+Version: 1.3.6
 Summary: Fork of Venmo-Business-Rules: Python DSL for setting up business intelligence rules that can be configured without code  History -------  1.0.1 +++++ released 2016-3-16  - Fixes a packaging bug preventing 1.0.0 from being installed on some platforms.  1.0.0 +++++ released 2016-3-16  - Removes caching layer on rule decorator 
 Home-page: https://github.com/cdisc-org/business-rules
 Author: cdisc-org
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `business-rules-enhanced-1.3.5/README.md` & `business-rules-enhanced-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.5/business_rules/actions.py` & `business-rules-enhanced-1.3.6/business_rules/actions.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.5/business_rules/engine.py` & `business-rules-enhanced-1.3.6/business_rules/engine.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.5/business_rules/operators.py` & `business-rules-enhanced-1.3.6/business_rules/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -856,21 +856,22 @@
         return pd.Series(results)
 
     @type_operator(FIELD_DATAFRAME)
     def is_unique_set(self, other_value):
         target = self.replace_prefix(other_value.get("target"))
         comparator = other_value.get("comparator")
         values = [target, comparator]
-        target_data = flatten_list(values)
+        target_data = flatten_list(self.value, values)
         target_names = []
         for target_name in target_data:
             target_name = self.replace_prefix(target_name)
             if target_name in self.value.columns:
                 target_names.append(target_name)
-        counts = self.value[target_names].groupby(target_names)[target].transform('size')
+        target_names = list(set(target_names))
+        counts = self.value[target_names].groupby(target_names)[target].transform('size') 
         results = np.where(counts <= 1, True, False)
         return pd.Series(results)
 
     @type_operator(FIELD_DATAFRAME)
     def is_not_unique_relationship(self, other_value) -> pd.Series:
         """
         Validates one-to-one relationship between two columns (target and comparator) against a dataset.
```

### Comparing `business-rules-enhanced-1.3.5/business_rules/six.py` & `business-rules-enhanced-1.3.6/business_rules/six.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.5/business_rules/utils.py` & `business-rules-enhanced-1.3.6/business_rules/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,21 +145,23 @@
 
 def apply_regex(regex: str, val: str):
     result = re.findall(regex, val)
     if result:
         return result[0]
     else:
         return None
-    
-def flatten_list(l):
-    for item in l:
-        if isinstance(item, list):
-            yield from flatten_list(item)
-        else:
-            yield item
+def flatten_list(data, l):
+   for item in l:
+       if isinstance(item, list):
+           yield from flatten_list(data, item)
+       elif item in data and isinstance(data[item].iloc[0], list):
+           for val in data[item].iloc[0]:
+               yield val
+       else:
+           yield item
 
 vectorized_apply_regex = np.vectorize(apply_regex)
 vectorized_is_complete_date = np.vectorize(is_complete_date)
 vectorized_compare_dates = np.vectorize(compare_dates)
 vectorized_is_valid = np.vectorize(is_valid_date)
 vectorized_get_dict_key = np.vectorize(get_dict_key_val)
 vectorized_is_in = np.vectorize(is_in)
```

### Comparing `business-rules-enhanced-1.3.5/business_rules/variables.py` & `business-rules-enhanced-1.3.6/business_rules/variables.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/PKG-INFO` & `business-rules-enhanced-1.3.6/business_rules_enhanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: business-rules-enhanced
-Version: 1.3.5
+Version: 1.3.6
 Summary: Fork of Venmo-Business-Rules: Python DSL for setting up business intelligence rules that can be configured without code  History -------  1.0.1 +++++ released 2016-3-16  - Fixes a packaging bug preventing 1.0.0 from being installed on some platforms.  1.0.0 +++++ released 2016-3-16  - Removes caching layer on rule decorator 
 Home-page: https://github.com/cdisc-org/business-rules
 Author: cdisc-org
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `business-rules-enhanced-1.3.5/setup.py` & `business-rules-enhanced-1.3.6/setup.py`

 * *Files identical despite different names*

