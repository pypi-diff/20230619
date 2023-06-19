# Comparing `tmp/rdf_doctor-0.8.2-py3-none-any.whl.zip` & `tmp/rdf_doctor-0.8.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17606 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-13 05:40 doctor/__init__.py
--rw-r--r--  2.0 unx      631 b- defN 23-Jun-05 08:08 doctor/consts.py
--rw-r--r--  2.0 unx    27880 b- defN 23-Jun-09 07:04 doctor/doctor.py
--rw-r--r--  2.0 unx    20305 b- defN 23-Jun-05 06:43 doctor/reference/correct-prefixes.tsv
--rw-r--r--  2.0 unx       90 b- defN 23-Jun-13 05:09 doctor/reference/refine-classes.tsv
--rw-r--r--  2.0 unx      679 b- defN 23-Jun-05 06:43 doctor/reference/refine-prefixes.tsv
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-13 05:45 rdf_doctor-0.8.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     8789 b- defN 23-Jun-13 05:45 rdf_doctor-0.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 05:45 rdf_doctor-0.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jun-13 05:44 rdf_doctor-0.8.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-13 05:44 rdf_doctor-0.8.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      994 b- defN 23-Jun-13 05:45 rdf_doctor-0.8.2.dist-info/RECORD
-12 files, 60602 bytes uncompressed, 15922 bytes compressed:  73.7%
+Zip file size: 18117 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-19 02:18 doctor/__init__.py
+-rw-r--r--  2.0 unx      631 b- defN 23-Jun-19 02:18 doctor/consts.py
+-rw-r--r--  2.0 unx    29745 b- defN 23-Jun-19 02:18 doctor/doctor.py
+-rw-r--r--  2.0 unx    20305 b- defN 23-Jun-19 02:18 doctor/reference/correct-prefixes.tsv
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-19 02:18 doctor/reference/refine-classes.tsv
+-rw-r--r--  2.0 unx      679 b- defN 23-Jun-19 02:18 doctor/reference/refine-prefixes.tsv
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8844 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jun-19 02:22 rdf_doctor-0.8.3.dist-info/RECORD
+12 files, 62522 bytes uncompressed, 16433 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-classes.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefixes.tsv
 Comment: 
 
-Filename: rdf_doctor-0.8.2.dist-info/LICENSE
+Filename: rdf_doctor-0.8.3.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-0.8.2.dist-info/METADATA
+Filename: rdf_doctor-0.8.3.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-0.8.2.dist-info/WHEEL
+Filename: rdf_doctor-0.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-0.8.2.dist-info/entry_points.txt
+Filename: rdf_doctor-0.8.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.2.dist-info/top_level.txt
+Filename: rdf_doctor-0.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-0.8.2.dist-info/RECORD
+Filename: rdf_doctor-0.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.8.2"
+__version__ = "0.8.3"
```

## doctor/doctor.py

```diff
@@ -2,14 +2,15 @@
 import sys
 import argparse
 import gzip
 import rdflib
 import re
 import csv
 import codecs
+import datetime
 from doctor.consts import VERSION_FILE, REPORT_FORMAT_SHEX, REPORT_FORMAT_MD, REPORT_FORMAT_MARKDOWN, \
                             TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, EXTENSION_GZ, CORRECT_PREFIXES_FILE_PATH, \
                             CLASS_ERRATA_FILE_PATH, PREFIX_ERRATA_FILE_PATH, HELP_LINK_URL
 from shexer.shaper import Shaper
 from shexer.consts import NT, TURTLE, GZ, MIXED_INSTANCES
 from unidecode import unidecode
 from collections import defaultdict
@@ -47,14 +48,17 @@
         # Output result to specified destination (standard output or file)
         if args.output is None:
             print("".join(output_result))
         else:
             with open(args.output, "w", encoding="utf-8") as f:
                 f.write("".join(output_result))
 
+        if args.verbose:
+            print(get_dt_now() + " -- Done!")
+
     except ValueError as e:
         print(e)
 
     except:
         print("An exception error occurred. Input data format may not be correct. Please review the data.")
 
     return
@@ -82,33 +86,38 @@
                                     formatter_class=argparse.RawDescriptionHelpFormatter)
 
     # Version info(-v, --version)
     parser.add_argument("-v","--version",
                         action="version",
                         version="%(prog)s " + get_version(VERSION_FILE))
 
+    # show progress while processing (-e、--verbose)
+    parser.add_argument("-e","--verbose",
+                        action="store_true",
+                        help="show progress while processing")
+
     # Input RDF file (-i、--input [RDF-FILE]、required)
     parser.add_argument("-i","--input", type=str,
                         required=True,
                         nargs="+",
                         help="input RDF file(s)(.ttl or .nt or gzip-compressed versions of them). Use the same extension when specifying multiple.",
                         metavar="RDF-FILE")
 
-    # Report format (-r、--report、default: shex)
+    # Report format (-r、--report [FORMAT]、default: shex)
     parser.add_argument("-r","--report", type=str,
                         default=REPORT_FORMAT_SHEX,
                         help="set the output format/serializer of report to one of: shex (defalut) or md or markdown(same as md)",
                         metavar="FORMAT")
 
     # Output report file (-o、--output [FILE]、default: Standard output)
     parser.add_argument("-o","--output", type=str,
                         help="write to file instead of stdout",
                         metavar="FILE")
 
-    # Target class(-c、--classes、default: all、Multiple can be specified.)
+    # Target class(-c、--classes [URL1, URL2,...]、default: all、Multiple can be specified.)
     parser.add_argument("-c","--classes", type=str,
                         default=[TARGET_CLASS_ALL],
                         nargs="+",
                         help="set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...",
                         metavar="URL")
 
     # Prefix errata file path(-p, --prefix-dict [FILE]、default: reference/refine-prefixes.tsv)
@@ -240,31 +249,40 @@
 
 
 # Processing when the report format is "shex"
 def get_shex_result(args, input_format, compression_mode):
 
     # Get Prefix when input file is turtle format
     if input_format == TURTLE:
+        if args.verbose:
+            print(get_dt_now() + " -- Getting prefixes from input file...")
+
         input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
     else:
         input_prefixes = []
         duplicated_prefixes = []
 
     shaper_result = get_shaper_result(args, input_format, compression_mode, input_prefixes)
 
     # Prefixes with the same QName but different URIs at the same time
+    if args.verbose:
+        print(get_dt_now() + " -- Checking for duplicate prefixes...")
+
     result_duplicated_prefixes = []
     if len(duplicated_prefixes) != 0:
         result_duplicated_prefixes.append("# Duplicate prefixes found.\n")
         result_duplicated_prefixes.append("\n")
         result_duplicated_prefixes.append("# Input QName\tURI\n")
         result_duplicated_prefixes.extend(["# " + s for s in duplicated_prefixes])
         result_duplicated_prefixes.append("\n\n")
 
     # Suggest QName based on URI of validation expression output by sheXer and correct-prefixes.tsv
+    if args.verbose:
+        print(get_dt_now() + " -- Creating suggestions for QName...")
+
     result_suggested_qname = []
     correct_prefixes = get_correct_prefixes()
     suggested_qname = get_suggested_qname(shaper_result, input_prefixes, correct_prefixes)
     if len(suggested_qname) != 0:
         result_suggested_qname.append("# There may be a better QName.\n\n")
         result_suggested_qname.append("# Input QName\tSuggested QName\tURI\n")
         result_suggested_qname.extend(["# " + s for s in suggested_qname])
@@ -284,34 +302,43 @@
 
 # Processing when the report format is "md/markdown"
 def get_markdown_result(args, input_format, compression_mode):
 
     # Processing related to prefixes ------------------
     # Get Prefix when input file is turtle format
     if input_format == TURTLE:
+        if args.verbose:
+            print(get_dt_now() + " -- Getting prefixes from input file...")
+
         input_prefixes, duplicated_prefixes = get_input_prefixes(args.input, compression_mode)
     else:
         input_prefixes = []
         duplicated_prefixes = []
 
-    # Get list for result output about prefix reuse rate
+    # Get list for result output about prefix reuse percentage
+    if args.verbose:
+        print(get_dt_now() + " -- Calculating prefix reuse percentage...")
+
     result_prefix_reuse_percentage = []
     result_prefix_reuse_percentage.append("## Prefix reuse percentage ([?](" + HELP_LINK_URL + "))\n")
     result_prefix_reuse_percentage.append("Percentage of prefixes used in the input file that are included in the predefined prefix list inside rdf-doctor.\n")
     prefix_reuse_percentage = get_prefix_reuse_percentage(input_prefixes)
     if prefix_reuse_percentage == None:
         result_prefix_reuse_percentage.append("```\n")
         result_prefix_reuse_percentage.append("Not calculated because there is no prefix defined.\n")
         result_prefix_reuse_percentage.append("```\n\n")
     else:
         result_prefix_reuse_percentage.append("```\n")
         result_prefix_reuse_percentage.append(str(prefix_reuse_percentage) + "%\n")
         result_prefix_reuse_percentage.append("```\n\n")
 
     # Refer to the errata of prefixes and obtain a list for result output that combines incorrect prefixes and correct prefixes
+    if args.verbose:
+        print(get_dt_now() + " -- Comparing with prefix dictionary (errata)...")
+
     result_prefix_errata = []
     prefix_comparison_result = get_prefix_comparison_result(input_prefixes, args.prefix_dict)
     # When there is data to output
     if len(prefix_comparison_result) != 0:
         result_prefix_errata.append("Found prefixes that looks incorrect.\n")
         result_prefix_errata.append("```\n")
         result_prefix_errata.append("Prefix\tInput URI\tSuggested URI\n")
@@ -323,30 +350,39 @@
         result_duplicated_prefixes.append("Duplicate prefixes found.\n")
         result_duplicated_prefixes.append("```\n")
         result_duplicated_prefixes.append("Input QName\tURI\n")
         result_duplicated_prefixes.extend([s for s in duplicated_prefixes])
         result_duplicated_prefixes.append("```\n\n")
     # -------------------------------------------------
 
+    if args.verbose:
+        print(get_dt_now() + " -- Getting classes from input file...")
+
     # Processing related to classes -------------------
     input_classes = get_input_classes(args.input, input_format, compression_mode, args.classes)
 
     # Refers to the errata list of the class, acquires the list for result output that combines the incorrect class and the correct class,
     # and returns the class corresponding to each key in fingerprint format stored in dictionary format.
+    if args.verbose:
+        print(get_dt_now() + " -- Comparing with class dictionary (errata)...")
+
     result_class_errata = []
     class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_dict)
     # When there is data to output
     if len(class_comparison_result) != 0:
         result_class_errata.append("Found class names that looks incorrect.\n")
         result_class_errata.append("```\n")
         result_class_errata.append("Input class name\tSuggested class name\n")
         result_class_errata.extend(class_comparison_result)
         result_class_errata.append("```\n\n")
 
     # Get a result output list to notify about different class strings with the same key as a result of fingerprinting
+    if args.verbose:
+        print(get_dt_now() + " -- Comparing with fingerprint method results...")
+
     result_class_fingerprint = []
     fingerprint_comparison_result = get_fingerprint_comparison_result(fingerprint_class_dict)
     # When there is data to output
     if len(fingerprint_comparison_result) != 0:
         result_class_fingerprint.append("Found multiple strings that appear to represent the same class name.\n")
         result_class_fingerprint.append("```")
         result_class_fingerprint.extend(fingerprint_comparison_result)
@@ -387,36 +423,35 @@
     if TARGET_CLASS_ALL in args.classes:
         target_classes = None
         all_classes_mode = True
     else:
         target_classes = args.classes
         all_classes_mode = False
 
-    namespaces_dict = {}
-    for input_prefix in input_prefixes:
-        namespaces_dict[input_prefix[1]] = input_prefix[0].replace(":","")
-
-    if len(args.input) == 1:
-        graph_file_input = args.input[0]
-        graph_list_of_files_input = None
+    if input_format == NT:
+        namespaces_dict = default_namespaces()
     else:
-        graph_file_input = None
-        graph_list_of_files_input = args.input
-    # Init shexer's shaper class
-    shaper = Shaper(graph_file_input=graph_file_input,
-                    graph_list_of_files_input=graph_list_of_files_input,
+        namespaces_dict = {}
+        for input_prefix in input_prefixes:
+            namespaces_dict[input_prefix[1]] = input_prefix[0].replace(":","")
+
+    # Get instance of shexer's shaper class
+    shaper = Shaper(graph_list_of_files_input=args.input,
                     target_classes=target_classes,
                     all_classes_mode=all_classes_mode,
                     input_format=input_format,
                     namespaces_dict=namespaces_dict,
+                    disable_exact_cardinality=True,
                     compression_mode=compression_mode,
                     instances_report_mode=MIXED_INSTANCES,
                     detect_minimal_iri=True)
 
-    return shaper.shex_graph(string_output=True)
+    return shaper.shex_graph(string_output=True,
+                            verbose=args.verbose,
+                            acceptance_threshold=0.05)
 
 
 # Calculates the percentage of prefixes in the input file that exist in the prefix list file prepared in advance,
 # and returns it after rounding to the second decimal place.
 # If the prefix is not detected, do not calculate and return None.
 def get_prefix_reuse_percentage(input_prefixes):
     correct_prefixes = get_correct_prefixes()
@@ -634,7 +669,24 @@
 def fingerprint(string):
     string = string.lower()
     string = re.sub("[^A-Za-z0-9 ]+", "", string)
     string = unidecode(string)
     words = string.split()
     words = sorted(list(set(words)))
     return " ".join(words)
+
+# A dictionary of namespaces to pass to sheXer
+# This function is used only when the input file is N-Triples.
+def default_namespaces():
+    return {
+            "http://www.w3.org/2002/07/owl#": "owl",
+            "http://www.w3.org/1999/02/22-rdf-syntax-ns#": "rdf",
+            "http://www.w3.org/2000/01/rdf-schema#": "rdfs",
+            "http://www.w3.org/2001/XMLSchema#": "xsd",
+            "http://www.w3.org/XML/1998/namespace": "xml",
+            }
+
+# Get current date and time
+# dd/MM/yyyy HH:mm:ss
+# This function will only be called if verbose parameter is True.
+def get_dt_now():
+    return datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')
```

## Comparing `rdf_doctor-0.8.2.dist-info/LICENSE` & `rdf_doctor-0.8.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-0.8.2.dist-info/METADATA` & `rdf_doctor-0.8.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 0.8.2
+Version: 0.8.3
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -50,14 +50,15 @@
 usage: rdf-doctor -i RDF-FILE [Options]
 
 Home page: https://github.com/dbcls/rdf-doctor
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
+  -e, --verbose         show progress while processing
   -i RDF-FILE [RDF-FILE ...], --input RDF-FILE [RDF-FILE ...]
                         input RDF file(s)(.ttl or .nt or gzip-compressed versions of them). Use the same extension when specifying multiple.
   -r FORMAT, --report FORMAT
                         set the output format/serializer of report to one of: shex (defalut) or md or markdown(same as md)
   -o FILE, --output FILE
                         write to file instead of stdout
   -c URL [URL ...], --classes URL [URL ...]
```

