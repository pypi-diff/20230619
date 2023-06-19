# Comparing `tmp/countess-minimap2-0.0.6.tar.gz` & `tmp/countess-minimap2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-minimap2-0.0.6.tar", last modified: Wed May 31 04:07:35 2023, max compression
+gzip compressed data, was "countess-minimap2-0.0.8.tar", last modified: Mon Jun 19 00:40:14 2023, max compression
```

## Comparing `countess-minimap2-0.0.6.tar` & `countess-minimap2-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:07:35.216711 countess-minimap2-0.0.6/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2023-04-13 01:52:34.000000 countess-minimap2-0.0.6/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2082 2023-05-31 04:07:35.216711 countess-minimap2-0.0.6/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1509 2023-05-31 04:06:44.000000 countess-minimap2-0.0.6/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 04:07:35.216711 countess-minimap2-0.0.6/countess_minimap2.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     2082 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      314 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       63 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       68 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       18 2023-05-31 04:07:35.000000 countess-minimap2-0.0.6/countess_minimap2.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     4217 2023-05-31 04:06:17.000000 countess-minimap2-0.0.6/countess_minimap2.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1086 2023-05-31 04:01:45.000000 countess-minimap2-0.0.6/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-31 04:07:35.216711 countess-minimap2-0.0.6/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-15 00:46:44.000000 countess-minimap2-0.0.6/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-19 00:40:14.434330 countess-minimap2-0.0.8/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1469 2023-04-13 01:52:34.000000 countess-minimap2-0.0.8/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2259 2023-06-19 00:40:14.434330 countess-minimap2-0.0.8/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1653 2023-06-19 00:39:02.000000 countess-minimap2-0.0.8/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-06-19 00:40:14.434330 countess-minimap2-0.0.8/countess_minimap2.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2259 2023-06-19 00:40:14.000000 countess-minimap2-0.0.8/countess_minimap2.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      314 2023-06-19 00:40:14.000000 countess-minimap2-0.0.8/countess_minimap2.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-06-19 00:40:14.000000 countess-minimap2-0.0.8/countess_minimap2.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       63 2023-06-19 00:40:14.000000 countess-minimap2-0.0.8/countess_minimap2.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       68 2023-06-19 00:40:14.000000 countess-minimap2-0.0.8/countess_minimap2.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       18 2023-06-19 00:40:14.000000 countess-minimap2-0.0.8/countess_minimap2.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4741 2023-06-19 00:39:19.000000 countess-minimap2-0.0.8/countess_minimap2.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1119 2023-06-19 00:38:56.000000 countess-minimap2-0.0.8/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-06-19 00:40:14.434330 countess-minimap2-0.0.8/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-15 00:46:44.000000 countess-minimap2-0.0.8/setup.py
```

### Comparing `countess-minimap2-0.0.6/LICENSE.txt` & `countess-minimap2-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-minimap2-0.0.6/PKG-INFO` & `countess-minimap2-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: countess-minimap2
-Version: 0.0.6
-Summary: CountESS Minimap2 Plugin
+Version: 0.0.8
+Summary: Sequence Alignment Plugin for CountESS, based in Minimap2
 Author-email: Nick Moore <nick@zoic.org>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# CountESS MiniMap2 Plugin v0.0.6
+# CountESS MiniMap2 Plugin v0.0.8
 
 This is a plugin to allow [MiniMap2](https://github.com/lh3/minimap2) 
 to be used from within [CountESS](https://github.com/CountESS-Project/CountESS/)
 
 This might be useful, but it also stands as a handy example of how to write
 a CountESS plugin which wraps an external Python library.
 
@@ -28,14 +28,19 @@
 ### Output Column Prefix
 
 The default output column prefix is `mm` but this can be changed.
 
 ### Ref FA / Ref MMI
 
 A local FASTA or MMI file to look up the sequences in.
+Acceptable formats are MMI or FASTA, optionally gzipped.
+
+### Req Sequence
+
+Alternatively, enter a single reference DNA sequence directly here.
 
 ### Preset
 
 See [minimap2 Preset Options](https://lh3.github.io/minimap2/minimap2.html#8)
 
 ### Minimum Match Length
```

### Comparing `countess-minimap2-0.0.6/README.md` & `countess-minimap2-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS MiniMap2 Plugin v0.0.6
+# CountESS MiniMap2 Plugin v0.0.8
 
 This is a plugin to allow [MiniMap2](https://github.com/lh3/minimap2) 
 to be used from within [CountESS](https://github.com/CountESS-Project/CountESS/)
 
 This might be useful, but it also stands as a handy example of how to write
 a CountESS plugin which wraps an external Python library.
 
@@ -11,14 +11,19 @@
 ### Output Column Prefix
 
 The default output column prefix is `mm` but this can be changed.
 
 ### Ref FA / Ref MMI
 
 A local FASTA or MMI file to look up the sequences in.
+Acceptable formats are MMI or FASTA, optionally gzipped.
+
+### Req Sequence
+
+Alternatively, enter a single reference DNA sequence directly here.
 
 ### Preset
 
 See [minimap2 Preset Options](https://lh3.github.io/minimap2/minimap2.html#8)
 
 ### Minimum Match Length
```

### Comparing `countess-minimap2-0.0.6/countess_minimap2.egg-info/PKG-INFO` & `countess-minimap2-0.0.8/countess_minimap2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: countess-minimap2
-Version: 0.0.6
-Summary: CountESS Minimap2 Plugin
+Version: 0.0.8
+Summary: Sequence Alignment Plugin for CountESS, based in Minimap2
 Author-email: Nick Moore <nick@zoic.org>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# CountESS MiniMap2 Plugin v0.0.6
+# CountESS MiniMap2 Plugin v0.0.8
 
 This is a plugin to allow [MiniMap2](https://github.com/lh3/minimap2) 
 to be used from within [CountESS](https://github.com/CountESS-Project/CountESS/)
 
 This might be useful, but it also stands as a handy example of how to write
 a CountESS plugin which wraps an external Python library.
 
@@ -28,14 +28,19 @@
 ### Output Column Prefix
 
 The default output column prefix is `mm` but this can be changed.
 
 ### Ref FA / Ref MMI
 
 A local FASTA or MMI file to look up the sequences in.
+Acceptable formats are MMI or FASTA, optionally gzipped.
+
+### Req Sequence
+
+Alternatively, enter a single reference DNA sequence directly here.
 
 ### Preset
 
 See [minimap2 Preset Options](https://lh3.github.io/minimap2/minimap2.html#8)
 
 ### Minimum Match Length
```

### Comparing `countess-minimap2-0.0.6/countess_minimap2.py` & `countess-minimap2-0.0.8/countess_minimap2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """ CountESS Minimap2 Plugin"""
 
 import re
-from typing import Any, Mapping, Optional
+from typing import Mapping, Optional
 
 import pandas as pd
 
 import mappy  # type: ignore
 
 from countess.core.logger import Logger
 from countess.core.parameters import (
     BooleanParam,
     ChoiceParam,
     ColumnChoiceParam,
     IntegerParam,
     StringParam,
+    StringCharacterSetParam,
     FileParam,
 )
 from countess.core.plugins import PandasTransformPlugin
 
-VERSION = '0.0.6'
+VERSION = '0.0.8'
 
 CS_STRING_RE = r"(=[ACTGTN]+|:[0-9]+|(?:\*[ACGTN][ACGTN])+|\+[ACGTN]+|-[ACGTN]+)"
 MM2_PRESET_CHOICES = ["sr", "map-pb", "map-ont", "asm5", "asm10", "splice"]
 
 
 def cs_to_hgvs(cs_string: str, offset: int=1) -> str:
     """Turn the Minimap2 "difference string" into a HGVS string"""
@@ -43,15 +44,15 @@
         elif op[0] == "+":
             hgvs_ops.append(f"{offset}_{offset+1}ins{op[1]}")
             offset += 1
         elif op[0] == "-":
             hgvs_ops.append(f"{offset}del")
             offset += 1
     if len(hgvs_ops) == 0:
-        return "g.{offset}="
+        return "g.="
     elif len(hgvs_ops) == 1:
         return "g." + hgvs_ops[0]
     else:
         return "g.[" + ";".join(hgvs_ops) + "]"
 
 class MiniMap2Plugin(PandasTransformPlugin):
     """Turns a DNA sequence into a HGVS variant code"""
@@ -60,37 +61,46 @@
 
     name = "MiniMap2 Plugin"
     description = """
         Finds variants using Minimap2.  Note that the CIGAR string doesn't always
         show all variants.
     """
     version = VERSION
-    link = "https://github.com/nickzoic/countess-minimap2#readme"
+    link = "https://github.com/CountESS-Project/countess-minimap2#readme"
 
-    FILE_TYPES = [("MMI", "*.mmi"), ("FASTA", "*.fa(sta)?")]
+    FILE_TYPES = [("MMI", "*.mmi"), ("FASTA", "*.fa *.fasta *.fa.gz *.fasta.gz")]
+    CHARACTER_SET = set(['A', 'C', 'G', 'T'])
 
     parameters = {
         "column": ColumnChoiceParam("Input Column", "sequence"),
         "prefix": StringParam("Output Column Prefix", "mm"),
         "ref": FileParam("Ref FA / Ref MMI", file_types = FILE_TYPES),
+        "seq": StringCharacterSetParam("*OR* Ref Sequence", character_set=CHARACTER_SET),
         "preset": ChoiceParam("Preset", "sr", choices=MM2_PRESET_CHOICES),
         "min_length": IntegerParam("Minimum Match Length", 0),
         "drop": BooleanParam("Drop Unmatched", False),
     }
 
     def run_df(self, df: pd.DataFrame, logger: Logger) -> pd.DataFrame:
 
         assert isinstance(self.parameters['column'], ColumnChoiceParam)
 
         column = self.parameters['column'].get_column(df)
         prefix = self.parameters["prefix"].value
 
-        aligner = mappy.Aligner(
-            self.parameters["ref"].value, preset=self.parameters["preset"].value
-        )
+        if self.parameters["seq"].value:
+            aligner = mappy.Aligner(
+                seq=self.parameters["seq"].value, preset=self.parameters["preset"].value
+            )
+        elif self.parameters["ref"].value:
+            aligner = mappy.Aligner(
+                self.parameters["ref"].value, preset=self.parameters["preset"].value
+            )
+        else:
+            aligner = None
 
         if not aligner:
             logger.error("ERROR: failed to load/build index file")
             return pd.DataFrame()
 
         prefix = self.parameters["prefix"].value
         min_length = self.parameters["min_length"].value
@@ -115,14 +125,14 @@
                 prefix + "_r_en": 0,
                 prefix + "_strand": 0,
                 prefix + "_cigar": "",
                 prefix + "_cs": "",
                 prefix + "_hgvs": "",
             })
 
-
-        df = df.join(column.apply(process, convert_dtype=True))
+        dfx = column.apply(process, convert_dtype=True)
+        df = df.assign(**dict( (name, dfx[name]) for name in dfx.columns))
 
         if self.parameters["drop"].value:
             df = df.dropna(subset=[prefix + "_ctg"])
 
         return df
```

### Comparing `countess-minimap2-0.0.6/pyproject.toml` & `countess-minimap2-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 readme = "README.md"
 authors = [
     { name = "Nick Moore", email="nick@zoic.org" },
 ]
 maintainers = [
     { name = "Nick Moore", email="nick@zoic.org" },
 ]
-description = "CountESS Minimap2 Plugin"
+description = "Sequence Alignment Plugin for CountESS, based in Minimap2"
 requires-python = ">=3.10"
 license = { text = "BSD-3-Clause" }
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 dependencies = [
-    "countess>=0.0.26,<0.1",
+    "countess>=0.0.30,<0.1",
     "mappy~=2.24",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "countess[dev]>=0.0.29,<0.1",
+    "countess[dev]>=0.0.30,<0.1",
 ]
 
 [project.entry-points.countess_plugins]
 minimap2 = "countess_minimap2:MiniMap2Plugin"
 
 [tool.setuptools.dynamic]
 version = { attr = "countess_minimap2.VERSION" }
```

