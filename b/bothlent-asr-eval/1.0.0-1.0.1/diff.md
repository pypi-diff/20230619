# Comparing `tmp/bothlent_asr_eval-1.0.0-py3-none-any.whl.zip` & `tmp/bothlent_asr_eval-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10093 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      118 b- defN 23-Jun-19 14:50 bothlent_asr_eval/__init__.py
--rw-rw-rw-  2.0 fat     2919 b- defN 21-Apr-14 00:25 bothlent_asr_eval/__main__.py
--rw-rw-rw-  2.0 fat    14200 b- defN 23-Jun-19 14:10 bothlent_asr_eval/asr_evaluation.py
+Zip file size: 10108 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      130 b- defN 23-Jun-19 15:12 bothlent_asr_eval/__init__.py
+-rw-rw-rw-  2.0 fat     2940 b- defN 23-Jun-19 15:13 bothlent_asr_eval/__main__.py
+-rw-rw-rw-  2.0 fat    14200 b- defN 23-Jun-19 15:04 bothlent_asr_eval/asr_evaluation.py
 -rw-rw-rw-  2.0 fat        9 b- defN 22-Sep-19 16:17 bothlent_asr_eval/package_data.dat
 -rw-rw-rw-  2.0 fat       43 b- defN 22-Sep-19 16:17 bothlent_asr_eval/simple.py
--rw-rw-rw-  2.0 fat        9 b- defN 22-Sep-19 16:17 bothlent_asr_eval-1.0.0.data/data/bothlent_asr_eval_data/data_file
--rw-rw-rw-  2.0 fat     1081 b- defN 23-Jun-19 14:58 bothlent_asr_eval-1.0.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2277 b- defN 23-Jun-19 14:58 bothlent_asr_eval-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 14:58 bothlent_asr_eval-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       47 b- defN 23-Jun-19 14:58 bothlent_asr_eval-1.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-19 14:58 bothlent_asr_eval-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1099 b- defN 23-Jun-19 14:58 bothlent_asr_eval-1.0.0.dist-info/RECORD
-12 files, 21912 bytes uncompressed, 8193 bytes compressed:  62.6%
+-rw-rw-rw-  2.0 fat        9 b- defN 22-Sep-19 16:17 bothlent_asr_eval-1.0.1.data/data/bothlent_asr_eval_data/data_file
+-rw-rw-rw-  2.0 fat     1081 b- defN 23-Jun-19 15:37 bothlent_asr_eval-1.0.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2277 b- defN 23-Jun-19 15:37 bothlent_asr_eval-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 15:37 bothlent_asr_eval-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Jun-19 15:37 bothlent_asr_eval-1.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-19 15:37 bothlent_asr_eval-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1099 b- defN 23-Jun-19 15:37 bothlent_asr_eval-1.0.1.dist-info/RECORD
+12 files, 21945 bytes uncompressed, 8208 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -9,29 +9,29 @@
 
 Filename: bothlent_asr_eval/package_data.dat
 Comment: 
 
 Filename: bothlent_asr_eval/simple.py
 Comment: 
 
-Filename: bothlent_asr_eval-1.0.0.data/data/bothlent_asr_eval_data/data_file
+Filename: bothlent_asr_eval-1.0.1.data/data/bothlent_asr_eval_data/data_file
 Comment: 
 
-Filename: bothlent_asr_eval-1.0.0.dist-info/LICENSE.txt
+Filename: bothlent_asr_eval-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: bothlent_asr_eval-1.0.0.dist-info/METADATA
+Filename: bothlent_asr_eval-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: bothlent_asr_eval-1.0.0.dist-info/WHEEL
+Filename: bothlent_asr_eval-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: bothlent_asr_eval-1.0.0.dist-info/entry_points.txt
+Filename: bothlent_asr_eval-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: bothlent_asr_eval-1.0.0.dist-info/top_level.txt
+Filename: bothlent_asr_eval-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bothlent_asr_eval-1.0.0.dist-info/RECORD
+Filename: bothlent_asr_eval-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bothlent_asr_eval/__init__.py

```diff
@@ -1,5 +1,5 @@
 def main():
     """Entry point for the application script"""
-    from . import __main__
+    from bothlent_asr_eval import __main__
     __main__.main()
-    
+
```

## bothlent_asr_eval/__main__.py

```diff
@@ -18,17 +18,17 @@
 Contains the main method for the CLI.
 """
 
 import argparse
 
 # For some reason Python 2 and Python 3 disagree about how to import this.
 try:
-    from asr_evaluation.asr_evaluation import main as other_main
+    from bothlent_asr_eval.asr_evaluation import main as other_main
 except Exception:
-    from asr_evaluation import main as other_main
+    from bothlent_asr_eval.asr_evaluation import main as other_main
 
 def get_parser():
     """Parse the CLI args."""
     parser = argparse.ArgumentParser(description='Evaluate an ASR transcript against a reference transcript.')
     parser.add_argument('ref', type=argparse.FileType('r'), help='Reference transcript filename')
     parser.add_argument('hyp', type=argparse.FileType('r'), help='ASR hypothesis filename')
     print_args = parser.add_mutually_exclusive_group()
```

## bothlent_asr_eval/asr_evaluation.py

 * *Ordering differences only*

```diff
@@ -52,16 +52,16 @@
 deletion_table = defaultdict(int)
 substitution_table = defaultdict(int)
 # These are the editdistance opcodes that are condsidered 'errors'
 error_codes = ['replace', 'delete', 'insert']
 
 
 # TODO - rename this function.  Move some of it into evaluate.py?
-    """Main method - this reads the hyp and ref files, and creates
 def main(args):
+    """Main method - this reads the hyp and ref files, and creates
     editdistance.SequenceMatcher objects to compute the edit distance.
     All the statistics necessary statistics are collected, and results are
     printed as specified by the command line options.
 
     This function doesn't not check to ensure that the reference and
     hypothesis file have the same number of lines.  It will stop after the
     shortest one runs out of lines.  This should be easy to fix...
```

## Comparing `bothlent_asr_eval-1.0.0.dist-info/LICENSE.txt` & `bothlent_asr_eval-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `bothlent_asr_eval-1.0.0.dist-info/METADATA` & `bothlent_asr_eval-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bothlent-asr-eval
-Version: 1.0.0
+Version: 1.0.1
 Summary: A asr evaluation tool.
 Home-page: 
 Author: bcui
 Author-email: bcui@bothlent.com
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
```

## Comparing `bothlent_asr_eval-1.0.0.dist-info/RECORD` & `bothlent_asr_eval-1.0.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-bothlent_asr_eval/__init__.py,sha256=jQDOOvEuh4Ly9oJtjJDIcwi6sZm_2ORP5VbZ_1WFZoY,118
-bothlent_asr_eval/__main__.py,sha256=LFnfK4V_R9pCveX__f589Hmk06e4X4fja50uBLEsv9E,2919
-bothlent_asr_eval/asr_evaluation.py,sha256=js6OPSzGMX5Y5-vJ7FTAKX9XjAwr48u8jHsob3VWDkg,14200
+bothlent_asr_eval/__init__.py,sha256=-itGxau3gbEK_Zn5ZZBLAmD-RNQATF16IsD3_guoYmE,130
+bothlent_asr_eval/__main__.py,sha256=gFDcGnkn2sUriv7tEgJedgKewoGhCWISSpy_mnBpT2c,2940
+bothlent_asr_eval/asr_evaluation.py,sha256=ES7OqB0gd6a9deoVS9U7tvhPIPS0Au4-f0z7njf2fXk,14200
 bothlent_asr_eval/package_data.dat,sha256=EweZDmulyhRes16ZGCqb7EZTG8VN32VqYCx4D6AkDe4,9
 bothlent_asr_eval/simple.py,sha256=jQxgMu2wujV5-EV7SIHDYnIfEhmJAzxyn2XKqYliCB0,43
-bothlent_asr_eval-1.0.0.data/data/bothlent_asr_eval_data/data_file,sha256=EweZDmulyhRes16ZGCqb7EZTG8VN32VqYCx4D6AkDe4,9
-bothlent_asr_eval-1.0.0.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
-bothlent_asr_eval-1.0.0.dist-info/METADATA,sha256=p6SQXUP-PuvvPGvzyJ-OMW3yLMxahjFqDQzENwZ9xbY,2277
-bothlent_asr_eval-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-bothlent_asr_eval-1.0.0.dist-info/entry_points.txt,sha256=ViuJ6ZnFL8oumW5Cl2vKEn6CVkAqmTXl_7IDGNEa9xY,47
-bothlent_asr_eval-1.0.0.dist-info/top_level.txt,sha256=eXMiFde-PA4V8_pneg6rsj1rIYmkCQRnB6v68vLw_H4,18
-bothlent_asr_eval-1.0.0.dist-info/RECORD,,
+bothlent_asr_eval-1.0.1.data/data/bothlent_asr_eval_data/data_file,sha256=EweZDmulyhRes16ZGCqb7EZTG8VN32VqYCx4D6AkDe4,9
+bothlent_asr_eval-1.0.1.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
+bothlent_asr_eval-1.0.1.dist-info/METADATA,sha256=fLyfwhmL1bPFHRTIUFIcaevXvLxKTVjymeRAsvl94B0,2277
+bothlent_asr_eval-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bothlent_asr_eval-1.0.1.dist-info/entry_points.txt,sha256=ViuJ6ZnFL8oumW5Cl2vKEn6CVkAqmTXl_7IDGNEa9xY,47
+bothlent_asr_eval-1.0.1.dist-info/top_level.txt,sha256=eXMiFde-PA4V8_pneg6rsj1rIYmkCQRnB6v68vLw_H4,18
+bothlent_asr_eval-1.0.1.dist-info/RECORD,,
```

