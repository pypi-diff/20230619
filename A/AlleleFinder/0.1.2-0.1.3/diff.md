# Comparing `tmp/AlleleFinder-0.1.2.tar.gz` & `tmp/AlleleFinder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adamkoziol/PycharmProjects/AlleleFinder/dist/tmpljkxth4p/AlleleFinder-0.1.2.tar", last modified: Thu Jun  1 18:10:45 2023, max compression
+gzip compressed data, was "/home/adamkoziol/PycharmProjects/AlleleFinder/dist/tmpafl07hzr/AlleleFinder-0.1.3.tar", last modified: Mon Jun 19 18:23:23 2023, max compression
```

## Comparing `AlleleFinder-0.1.2.tar` & `AlleleFinder-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/
--rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)     1113 2023-02-24 20:49:53.000000 AlleleFinder-0.1.2/setup.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1077 2023-03-10 15:09:59.000000 AlleleFinder-0.1.2/LICENSE
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/PKG-INFO
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      702 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       19 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/top_level.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/PKG-INFO
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        1 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/AlleleFinder.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     8402 2023-06-01 18:07:22.000000 AlleleFinder-0.1.2/README.md
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/allele_tools/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    24429 2023-03-24 14:27:36.000000 AlleleFinder-0.1.2/allele_tools/allele_profiler.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    30190 2023-06-01 15:06:39.000000 AlleleFinder-0.1.2/allele_tools/stec.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-06-22 16:34:50.000000 AlleleFinder-0.1.2/allele_tools/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6368 2023-03-13 14:59:24.000000 AlleleFinder-0.1.2/allele_tools/profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    85988 2023-06-01 15:06:40.000000 AlleleFinder-0.1.2/allele_tools/methods.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       51 2023-06-01 18:07:22.000000 AlleleFinder-0.1.2/allele_tools/version.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    28340 2023-03-24 18:52:09.000000 AlleleFinder-0.1.2/allele_tools/allele_updater.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35343 2023-03-24 19:36:21.000000 AlleleFinder-0.1.2/allele_tools/allele_translate_reduce.py
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/tests/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4599 2023-06-01 15:06:40.000000 AlleleFinder-0.1.2/tests/test_5_stec_allele_find.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6584 2023-06-01 15:06:40.000000 AlleleFinder-0.1.2/tests/test_1_allele_translate_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4628 2023-03-13 20:02:00.000000 AlleleFinder-0.1.2/tests/test_3_stec_profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1866 2023-03-24 19:31:09.000000 AlleleFinder-0.1.2/tests/test_6_stec_aa_allele_find.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2022-03-21 20:37:30.000000 AlleleFinder-0.1.2/tests/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2829 2023-02-28 19:59:56.000000 AlleleFinder-0.1.2/tests/test_0_profile_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3245 2023-03-24 19:29:12.000000 AlleleFinder-0.1.2/tests/test_7_stec_allele_split.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     7795 2023-06-01 15:06:39.000000 AlleleFinder-0.1.2/tests/test_2_allele_updater.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3042 2023-03-13 19:11:01.000000 AlleleFinder-0.1.2/tests/test_4_stec_allele_translate_reduce.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       38 2023-06-01 18:10:45.000000 AlleleFinder-0.1.2/setup.cfg
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/
+-rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)     1113 2023-02-24 20:49:53.000000 AlleleFinder-0.1.3/setup.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1077 2023-03-10 15:09:59.000000 AlleleFinder-0.1.3/LICENSE
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/PKG-INFO
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      742 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       19 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/top_level.txt
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      265 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/PKG-INFO
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        1 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/AlleleFinder.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     8402 2023-06-01 18:07:22.000000 AlleleFinder-0.1.3/README.md
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/allele_tools/
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    24429 2023-03-24 14:27:36.000000 AlleleFinder-0.1.3/allele_tools/allele_profiler.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35564 2023-06-19 15:26:07.000000 AlleleFinder-0.1.3/allele_tools/stec.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-06-22 16:34:50.000000 AlleleFinder-0.1.3/allele_tools/__init__.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6368 2023-03-13 14:59:24.000000 AlleleFinder-0.1.3/allele_tools/profile_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    96996 2023-06-19 16:12:53.000000 AlleleFinder-0.1.3/allele_tools/methods.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       51 2023-06-19 16:18:22.000000 AlleleFinder-0.1.3/allele_tools/version.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    28340 2023-03-24 18:52:09.000000 AlleleFinder-0.1.3/allele_tools/allele_updater.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    35343 2023-03-24 19:36:21.000000 AlleleFinder-0.1.3/allele_tools/allele_translate_reduce.py
+drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/tests/
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4680 2023-06-19 16:07:38.000000 AlleleFinder-0.1.3/tests/test_5_stec_allele_find.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     6584 2023-06-01 15:06:40.000000 AlleleFinder-0.1.3/tests/test_1_allele_translate_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4628 2023-03-13 20:02:00.000000 AlleleFinder-0.1.3/tests/test_3_stec_profile_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2107 2023-06-19 16:16:44.000000 AlleleFinder-0.1.3/tests/test_6_stec_aa_allele_find.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2022-03-21 20:37:30.000000 AlleleFinder-0.1.3/tests/__init__.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     2829 2023-02-28 19:59:56.000000 AlleleFinder-0.1.3/tests/test_0_profile_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3249 2023-06-19 15:57:17.000000 AlleleFinder-0.1.3/tests/test_7_stec_allele_split.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     4265 2023-06-19 15:58:02.000000 AlleleFinder-0.1.3/tests/test_8_stec_allele_concatenate.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     7795 2023-06-01 15:06:39.000000 AlleleFinder-0.1.3/tests/test_2_allele_updater.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3042 2023-03-13 19:11:01.000000 AlleleFinder-0.1.3/tests/test_4_stec_allele_translate_reduce.py
+-rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       38 2023-06-19 18:23:23.000000 AlleleFinder-0.1.3/setup.cfg
```

### Comparing `AlleleFinder-0.1.2/setup.py` & `AlleleFinder-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/LICENSE` & `AlleleFinder-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/AlleleFinder.egg-info/SOURCES.txt` & `AlleleFinder-0.1.3/AlleleFinder.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 tests/test_0_profile_reduce.py
 tests/test_1_allele_translate_reduce.py
 tests/test_2_allele_updater.py
 tests/test_3_stec_profile_reduce.py
 tests/test_4_stec_allele_translate_reduce.py
 tests/test_5_stec_allele_find.py
 tests/test_6_stec_aa_allele_find.py
-tests/test_7_stec_allele_split.py
+tests/test_7_stec_allele_split.py
+tests/test_8_stec_allele_concatenate.py
```

### Comparing `AlleleFinder-0.1.2/README.md` & `AlleleFinder-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/allele_tools/allele_profiler.py` & `AlleleFinder-0.1.3/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/allele_tools/stec.py` & `AlleleFinder-0.1.3/allele_tools/stec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 #!/usr/bin/env python
 
 """
 Run allele finding specifically for the co-located subunits of STEC genes
 """
 
 # Standard imports
-from argparse import \
-    ArgumentParser, \
+from argparse import (
+    ArgumentParser,
     RawTextHelpFormatter
-import multiprocessing
+)
 from glob import glob
 import logging
+import multiprocessing
 import sys
 import os
 
 # Third party inputs
-from olctools.accessoryFunctions.accessoryFunctions import make_path, MetadataObject
+from olctools.accessoryFunctions.accessoryFunctions import (
+    make_path,
+    MetadataObject,
+)
 
 # Local imports
+from allele_tools.allele_profiler import (
+    allele_prep,
+    parseable_blast_outputs,
+    read_profile
+)
 from allele_tools.allele_translate_reduce import Translate
 from allele_tools.profile_reduce import ProfileReduce
 from allele_tools.version import __version__
-from allele_tools.methods import \
-        setup_arguments, \
-        common_allele_find_errors, \
-        pathfinder, \
-        query_prep, \
-        blast_alleles, \
-        create_gene_names, \
-        parse_colocated_results, \
-        create_nt_allele_comprehension, \
-        create_aa_allele_comprehension, \
-        create_frozen_allele_comprehension, \
-        match_profile, \
-        create_stec_report, \
-        split_alleles, \
-        parse_aa_blast, \
-        analyse_aa_alleles, \
-        report_aa_alleles
-from allele_tools.allele_profiler import \
-    allele_prep, \
-    parseable_blast_outputs, \
-    read_profile
-
+from allele_tools.methods import (
+    analyse_aa_alleles,
+    blast_alleles,
+    common_allele_find_errors,
+    concatenate_alleles,
+    create_aa_allele_comprehension,
+    create_frozen_allele_comprehension,
+    create_gene_names,
+    create_nt_allele_comprehension,
+    create_stec_report,
+    error_print,
+    load_alleles,
+    match_profile,
+    parse_aa_blast,
+    parse_colocated_results,
+    pathfinder,
+    profile_allele_check,
+    query_prep,
+    report_aa_alleles,
+    setup_arguments,
+    split_alleles,
+    write_concatenated_sequences
+)
 
 __author__ = 'adamkoziol'
 
 
 class STEC:
     """
     Perform the STEC-specific allele finding
@@ -328,14 +338,97 @@
         self.extended_fieldnames.insert(14, 'percent_match')
         self.outfmt = '6 qseqid sseqid nident mismatch gaps evalue bitscore qlen slen length ' \
                       'qstart qend sstart send qseq sseq'
         # A string of the header to use for formatting the profile file, and the report headers
         self.data = str()
 
 
+class AlleleConcatenate:
+
+    """
+    Concatenate stx subunits. Read in profile files. Load alleles. Concatenate alleles with appropriate linker
+    """
+
+    def main(self):
+        """
+        Run the necessary methods for AlleleConcatenate
+        """
+        self.gene, self.nt_alleles = load_alleles(
+            allele_path=self.nt_allele_path,
+            allele_order=self.allele_order
+        )
+        self.gene, self.aa_alleles = load_alleles(
+            allele_path=self.aa_allele_path,
+            allele_order=self.allele_order
+        )
+        self.concatenated_nt_seq = concatenate_alleles(
+            profile_data=self.nt_profile_data,
+            allele_dict=self.nt_alleles,
+            allele_order=self.allele_order,
+            stx_gene=self.gene,
+            linker_length_dict=self.linker_length_dict,
+            molecule='nt'
+        )
+        self.concatenated_aa_seq = concatenate_alleles(
+            profile_data=self.aa_profile_data,
+            allele_dict=self.aa_alleles,
+            allele_order=self.allele_order,
+            stx_gene=self.gene,
+            linker_length_dict=self.linker_length_dict,
+            molecule='aa'
+        )
+        write_concatenated_sequences(
+            concatenated_sequences=self.concatenated_nt_seq,
+            concatenate_path=self.concatenate_path,
+            file_name=self.gene_allele[self.gene],
+            molecule='nt'
+        )
+        write_concatenated_sequences(
+            concatenated_sequences=self.concatenated_aa_seq,
+            concatenate_path=self.concatenate_path,
+            file_name=self.gene_allele[self.gene],
+            molecule='aa'
+        )
+
+    def __init__(
+            self,
+            nt_allele_path,
+            aa_allele_path,
+            nt_profile_file,
+            aa_profile_file,
+            concatenate_path):
+        self.nt_allele_path = pathfinder(path=nt_allele_path)
+        self.aa_allele_path = pathfinder(path=aa_allele_path)
+        self.nt_profile_file = pathfinder(path=nt_profile_file)
+        self.aa_profile_file = pathfinder(path=aa_profile_file)
+        self.nt_profile_path = os.path.dirname(self.nt_profile_file)
+        self.aa_profile_path = os.path.dirname(self.aa_profile_file)
+        self.concatenate_path = pathfinder(path=concatenate_path)
+        self.linker_length_dict = {
+            'stx1': 9,
+            'stx2': 12,
+        }
+        # Set the appropriate order for the genes in the report (stx1 genes are not in numerical order)
+        self.allele_order = {
+            'stx1': ['ECs2974', 'ECs2973'],
+            'stx2': ['ECs1205', 'ECs1206']
+        }
+        self.gene_allele = {
+            'stx1': 'ECs2974_ECs2973',
+            'stx2': 'ECs1205_ECs1206'
+        }
+        self.nt_profile_data = read_profile(profile_file=self.nt_profile_file)
+        self.aa_profile_data = read_profile(profile_file=self.aa_profile_file)
+        self.gene = str()
+        self.nt_alleles = {}
+        self.aa_alleles = {}
+        self.concatenated_nt_seq = []
+        self.concatenated_aa_seq = []
+
+
 def profile_reduce(args):
     """
     Reduce the Enterobase profile to only the genes of interest
     :param args: type ArgumentParser arguments
     """
     # Create the gene names file if it doesn't exist or is empty
     genes_path = os.path.dirname(args.gene_names)
@@ -440,20 +533,15 @@
         args=args,
         errors=errors,
         amino_acid=False
     )
     if not os.path.isfile(args.nt_profile):
         errors.append(f'Could not locate supplied nucleotide profile file: {args.nt_profile}')
     if errors:
-        error_string = '\n'.join(errors)
-        was_were = 'was' if len(errors) == 1 else 'were'
-        correct = 'error' if len(errors) == 1 else 'errors'
-        logging.error(
-            'There %s %s %s when attempting to run your command: \n%s', was_were, len(errors), correct, error_string)
-        raise SystemExit
+        error_print(errors=errors)
     stec = STEC(
         allele_path=args.nt_alleles,
         aa_allele_path=args.aa_alleles,
         profile_file=args.nt_profile,
         aa_profile_file=args.aa_profile,
         query_path=args.query_path,
         report_path=args.report_path
@@ -473,20 +561,15 @@
     # Find errors for amino acid and query checks
     errors = common_allele_find_errors(
         args=args,
         errors=errors,
         amino_acid=True
     )
     if errors:
-        error_string = '\n'.join(errors)
-        was_were = 'was' if len(errors) == 1 else 'were'
-        correct = 'error' if len(errors) == 1 else 'errors'
-        logging.error(
-            'There %s %s %s when attempting to run your command: \n%s', was_were, len(errors), correct, error_string)
-        raise SystemExit
+        error_print(errors=errors)
     aa_stec = AASTEC(
         aa_allele_path=args.aa_alleles,
         query_path=args.query_path,
         report_path=args.report_path,
         cutoff=args.cutoff
     )
     aa_stec.main()
@@ -505,26 +588,46 @@
         errors.append(f'Could not find supplied nucleotide allele folder: {args.query_path}')
     else:
         if not allele_files:
             errors.append(
                 f'Could not locate sequence files in supplied allele folder: {args.query_path}'
             )
     if errors:
-        error_string = '\n'.join(errors)
-        was_were = 'was' if len(errors) == 1 else 'were'
-        correct = 'error' if len(errors) == 1 else 'errors'
-        logging.error(
-            'There %s %s %s when attempting to run your command: \n%s', was_were, len(errors), correct, error_string)
-        raise SystemExit
+        error_print(errors=errors)
     split_alleles(
         allele_files=allele_files,
         output_path=args.output_path
     )
 
 
+def allele_concatenate(args):
+    """
+    Concatenate subunit files with linkers. Provide linkages between nucleotide and amino acid files
+    :param args: type ArgumentParser arguments
+    """
+    logging.info('Concatenating allele subunits')
+    errors = []
+    # Determine if the profile file, the allele folder, and the alleles all exist
+    errors = profile_allele_check(
+        args=args,
+        errors=errors
+    )
+    # If there were any errors with the supplied arguments, print them, and exit
+    if errors:
+        error_print(errors=errors)
+    concatenate = AlleleConcatenate(
+        nt_allele_path=args.nt_alleles,
+        aa_allele_path=args.aa_alleles,
+        nt_profile_file=args.nt_profile,
+        aa_profile_file=args.aa_profile,
+        concatenate_path=args.concatenate_path
+    )
+    concatenate.main()
+
+
 def cli():
     """
     Collect the arguments, create an object, and run the script
     """
     # Parser for arguments
     parser = ArgumentParser(
         description='Determines STEC subunit profiles'
@@ -703,15 +806,15 @@
         '-c', '--cutoff',
         metavar='cutoff',
         default=90,
         choices=[percent for percent in range(90, 101)],
         help='Specify the percent identity cutoff for matches. Allowed values are between 90 and 100. Default is 100'
     )
     aa_allele_find_subparser.set_defaults(func=aa_allele_find)
-    # Create a subparser for allele discovery
+    # Create a subparser for splitting multi-FASTA files of alleles
     allele_split_subparser = subparsers.add_parser(
         parents=[parent_parser],
         name='allele_split',
         description='Split combined allele files into individual files',
         formatter_class=RawTextHelpFormatter,
         help='Split combined allele files into individual files'
     )
@@ -726,14 +829,58 @@
         '-o', '--output_path',
         metavar='output_path',
         default=os.path.join(os.getcwd(), 'split_alleles'),
         help='Specify name and path of folder into which the split allele files are to be written. '
              'If not provided, the split_alleles folder in the current working directory will be used'
     )
     allele_split_subparser.set_defaults(func=allele_split)
+    # Create a subparser for concatenating stx subunits
+    allele_concatenate_subparser = subparsers.add_parser(
+        parents=[parent_parser],
+        name='allele_concatenate',
+        description='Concatenate stx toxin subunit alleles with linkers',
+        formatter_class=RawTextHelpFormatter,
+        help='Concatenate stx toxin subunit alleles with linkers'
+    )
+    allele_concatenate_subparser.add_argument(
+        '--nt_profile',
+        metavar='nt_profile',
+        default=os.path.join(os.getcwd(), 'nt_profile', 'profile.txt'),
+        help='Specify name and path of nucleotide profile file. If not provided, profile.txt in '
+             'the nt_profile folder in the current working directory will be used by default'
+    )
+    allele_concatenate_subparser.add_argument(
+        '--aa_profile',
+        metavar='aa_profile',
+        default=os.path.join(os.getcwd(), 'aa_profile', 'profile.txt'),
+        help='Specify name and path of amino acid profile file. If not provided, profile.txt in '
+             'the aa_profile folder in the current working directory will be used by default'
+    )
+    allele_concatenate_subparser.add_argument(
+        '--nt_alleles',
+        metavar='nt_alleles',
+        default=os.path.join(os.getcwd(), 'nt_alleles'),
+        help='Specify name and path of folder containing nucleotide alleles. If not provided, the '
+             'nt_allele folder in the current working directory will be used by default'
+    )
+    allele_concatenate_subparser.add_argument(
+        '--aa_alleles',
+        metavar='aa_alleles',
+        default=os.path.join(os.getcwd(), 'aa_alleles'),
+        help='Specify name and path of folder containing amino acid alleles. If not provided, the '
+             'aa_allele folder in the current working directory will be used by default'
+    )
+    allele_concatenate_subparser.add_argument(
+        '-c', '--concatenate_path',
+        metavar='concatenate_path',
+        default=os.path.join(os.getcwd(), 'concatenated_alleles'),
+        help='Specify name and path of folder into which concatenated subunit files are to be placed. If not '
+             'provided, the concatenated_alleles folder in the current working directory will be used'
+    )
+    allele_concatenate_subparser.set_defaults(func=allele_concatenate)
     # Get the arguments into an object
     arguments = setup_arguments(parser=parser)
     # Prevent the arguments being printed to the console (they are returned in order for the tests to work)
     sys.stderr = open(os.devnull, 'w', encoding='utf-8')
     return arguments
```

### Comparing `AlleleFinder-0.1.2/allele_tools/profile_reduce.py` & `AlleleFinder-0.1.3/allele_tools/profile_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/allele_tools/methods.py` & `AlleleFinder-0.1.3/allele_tools/methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 #!/usr/bin/env python
 
 """
 Collection of methods for Allele finding
 """
 
 # Standard imports
+from argparse import ArgumentParser
 from csv import DictReader
 from glob import glob
-import logging
 import json
+import logging
 import math
 import os
 
 # Third party inputs
-from olctools.accessoryFunctions.accessoryFunctions import GenObject, \
-    make_path, \
-    MetadataObject, \
+from olctools.accessoryFunctions.accessoryFunctions import (
+    GenObject,
+    make_path,
+    MetadataObject,
     relative_symlink
+ )
 from Bio.Blast.Applications import NcbiblastnCommandline, NcbiblastpCommandline
 from Bio.Data.CodonTable import TranslationError
 from Bio.SeqRecord import SeqRecord
 from Bio.Seq import Seq
 from Bio import SeqIO
 import coloredlogs
 
@@ -47,15 +50,15 @@
     # Change the default log format to be the time prepended to the appropriately formatted 
     # message string
     coloredlogs.DEFAULT_LOG_FORMAT = '%(asctime)s %(message)s'
     # Set the logging level
     coloredlogs.install(level=arguments.verbosity.upper())
 
 
-def setup_arguments(parser):
+def setup_arguments(parser: ArgumentParser):
     """
     Finalise setting up the ArgumentParser arguments into an object, and running subparser
     functions, or displaying the help message
     :param parser: type: ArgumentParser object
     :return: parsed ArgumentParser object
     """
     # Get the arguments into an object
@@ -81,15 +84,18 @@
         # If there were no subparsers specified (the list of keys in the arguments is empty),
         # use the basic help
         except IndexError:
             parser.parse_args(['-h'])
     return arguments
 
 
-def common_allele_find_errors(args, errors, amino_acid):
+def common_allele_find_errors(
+        args: ArgumentParser.parse_args,
+        errors: list,
+        amino_acid: bool):
     """
     Perform checks for arguments shared between allele finding scripts
     :param args: type ArgumentParser arguments
     :param errors: List of errors with supplied arguments
     :param amino_acid: Boolean of whether the query sequence is amino acid or nucleotide
     :return: Updated list of errors
     """
@@ -103,31 +109,85 @@
             )
         else:
             if amino_acid:
                 errors = detect_protein(
                     query_path=args.query_path,
                     errors=errors
                 )
-    # Amino acid allele checks
-    if not os.path.isdir(args.aa_alleles):
-        errors.append(f'Could not find supplied amino acid allele folder: {args.aa_alleles}')
-    else:
-        if not glob(os.path.join(args.aa_alleles, '*.fasta')):
-            errors.append(
-                f'Could not locate sequence files in supplied amino acid allele folder: {args.aa_alleles}'
-            )
+    # Nucleotide and amino acid checks
+    errors = profile_allele_check(
+        args=args,
+        errors=errors
+    )
+    return errors
+
+
+def profile_allele_check(
+        args: ArgumentParser.parse_args,
+        errors: list):
+    """
+    Perform checks for arguments pertaining to profile and allele files
+    :param args: type ArgumentParser arguments
+    :param errors: List of errors with supplied arguments
+    :return: Updated list of errors
+    """
+    # Nucleotide checks
+    try:
+        if not os.path.isdir(args.nt_alleles):
+            errors.append(f'Could not find supplied nucleic acid allele folder: {args.nt_alleles}')
+        else:
+            if not glob(os.path.join(args.nt_alleles, '*.fasta')):
+                errors.append(
+                    f'Could not locate sequence files in supplied nucleic acid allele folder: {args.nt_alleles}'
+                )
+    # Allows for checks in analyses without nucleotide sequences
+    except AttributeError:
+        pass
+    try:
+        if not os.path.isfile(args.nt_profile):
+            errors.append(f'Could not locate supplied nucleic acid profile file: {args.nt_profile}')
+    except AttributeError:
+        pass
+    # Amino acid checks
+    try:
+        if not os.path.isdir(args.aa_alleles):
+            errors.append(f'Could not find supplied amino acid allele folder: {args.aa_alleles}')
+        else:
+            if not glob(os.path.join(args.aa_alleles, '*.fasta')):
+                errors.append(
+                    f'Could not locate sequence files in supplied amino acid allele folder: {args.aa_alleles}'
+                )
+    except AttributeError:
+        pass
     try:
         if not os.path.isfile(args.aa_profile):
             errors.append(f'Could not locate supplied amino acid profile file: {args.aa_profile}')
     except AttributeError:
         pass
     return errors
 
 
-def detect_protein(query_path, errors):
+def error_print(
+        errors: list):
+    """
+    Log grammatically correct error messages and exit
+    :param errors: List of errors with supplied arguments
+    """
+    # Create variables to allow for grammatically correct error messages
+    error_string = '\n'.join(errors)
+    was_were = 'was' if len(errors) == 1 else 'were'
+    correct = 'error' if len(errors) == 1 else 'errors'
+    logging.error(
+        'There %s %s %s when attempting to run your command: \n%s', was_were, len(errors), correct, error_string)
+    raise SystemExit
+
+
+def detect_protein(
+        query_path: str,
+        errors: list):
     """
     Attempt to determine whether a supplied file contains protein sequence
     :param query_path: String of absolute path to folder containing sequence files
     :param errors: List of errors with supplied arguments
     :return: Updated list of errors
     """
     # Create a list of all the FASTA files in the query path
@@ -149,15 +209,15 @@
                 aa = True
         # Update the errors if the file appears to be DNA
         if not aa:
             errors.append(f'Query file {seq_file} does not appear to be protein')
     return errors
 
 
-def pathfinder(path):
+def pathfinder(path: str):
     """
     Create absolute path user-supplied path. Allows for tilde expansion from
     :param path: String of path supplied by user. Could be relative, tilde expansion, or absolute
     :return: out_path: String of absolute path provided by user.
     """
     # Determine if the path requires path expansion
     if path.startswith('~'):
@@ -165,32 +225,35 @@
         out_path = os.path.abspath(os.path.expanduser(os.path.join(path)))
     else:
         # Create the absolute path from the path
         out_path = os.path.abspath(os.path.join(path))
     return out_path
 
 
-def query_prep(query_path, runmetadata, clear_report=True):
+def query_prep(
+        query_path: str,
+        runmetadata: MetadataObject,
+        clear_report=True):
     """
-    Create metadata objects for each sample
+    Create MetadataObjects for each sample
     :param query_path: String of absolute path to folder containing sequence files
-    :param runmetadata: List of metadata objects for each query
+    :param runmetadata: MetadataObject with list of GenObjects for each query
     :param clear_report: Boolean of whether to clear previous iterations of BLAST reports. Default is True
-    :return runmetadata: Metadata object updated with query information
+    :return runmetadata: MetadataObject updated with query information
     """
     logging.info('Preparing query files')
     # Find all the sequence files in the path
     fasta_files = sorted(glob(os.path.join(query_path, '*.fasta')))
     for fasta in fasta_files:
         name = os.path.splitext(os.path.basename(fasta))[0]
         if name != 'combinedtargets':
-            # Create a metadata object for each sample
+            # Create a MetadataObject for each sample
             metadata = MetadataObject()
             metadata.samples = []
-            # Populate the metadata object with the required attributes
+            # Populate the MetadataObject with the required attributes
             metadata.name = name
             metadata.general = GenObject()
             metadata.commands = GenObject()
             metadata.alleles = GenObject()
             metadata.alleles.outputdirectory = os.path.join(query_path, metadata.name)
             # Set the name of the BLAST output file
             metadata.alleles.blast_report = os.path.join(
@@ -212,18 +275,23 @@
                 export_output=True
             )
             metadata.samples.append(metadata)
             runmetadata.samples.append(metadata)
     return runmetadata
 
 
-def blast_alleles(runmetadata, amino_acid, combined_targets, cpus, outfmt):
+def blast_alleles(
+        runmetadata: MetadataObject,
+        amino_acid: bool,
+        combined_targets: str,
+        cpus: int,
+        outfmt: str):
     """
     Run the BLAST analyses on the query
-    :param runmetadata: List of metadata objects for each query
+    :param runmetadata: MetadataObject with list of GenObjects for each query
     :param amino_acid: Boolean of whether the query sequence is amino acid or nucleotide
     :param combined_targets: String of absolute path to file containing all sequences in other files in folder
     :param cpus: Integer of number of threads to use for BLAST analyses
     :param outfmt: String of BLAST fields to include in the report
     """
     logging.info('Running BLAST analyses')
     # Iterate through the samples
@@ -249,15 +317,17 @@
                 num_threads=cpus,
                 outfmt=outfmt,
                 out=sample.alleles.blast_report
             )
         blast()
 
 
-def create_gene_names(path=os.getcwd(), name='genes.txt'):
+def create_gene_names(
+        path=os.getcwd(),
+        name='genes.txt'):
     """
     Create a file with gene names to use in reducing a wgMLST profile by finding any .fasta files
     in a folder and adding them to the file (one per line)
     :param path: type: String of the path in which the genes file is to be created
     :param name: type: String of the name of the gene file
     """
     # Find all the .fasta files in the path
@@ -279,49 +349,60 @@
         logging.error(
             'Created gene file, %s, is empty. Please ensure that directory %s has files with '
             '.fasta extensions', gene_file, path
             )
         raise SystemExit
 
 
-def create_blast_dict(sample, extended_fieldnames):
+def create_blast_dict(
+        sample: MetadataObject,
+        extended_fieldnames: list):
     """
     Use DictReader to open and read a BLAST report into a dictionary
-    :param sample: Metadata object
+    :param sample: MetadataObject with list of GenObjects for each query
     :param extended_fieldnames: List of the BLAST fields used, as well as the additional percent
     match in index 14
     """
     # Open the BLAST report as a dictionary
     blastdict = DictReader(
         open(sample.alleles.blast_report,
              encoding='utf-8'),
         fieldnames=extended_fieldnames,
         dialect='excel-tab'
     )
     return blastdict
 
 
-def parse_colocated_results(runmetadata, fieldnames, extended_fieldnames, amino_acid, gene_names, nt_allele_path,
-                            aa_allele_path, report_path, overlap_range=50, cutoff=90):
+def parse_colocated_results(
+        runmetadata: MetadataObject,
+        fieldnames: list,
+        extended_fieldnames: list,
+        amino_acid: bool,
+        gene_names: list,
+        nt_allele_path: str,
+        aa_allele_path: str,
+        report_path: str,
+        overlap_range=50,
+        cutoff=90):
     """
     Parse BLAST outputs. Ensure co-location of genes that must be co-located
-    :param runmetadata: List of metadata objects
+    :param runmetadata: MetadataObject with list of GenObjects for each query
     :param fieldnames: List of the BLAST fields used
     :param extended_fieldnames: List of the BLAST fields used, as well as the additional percent
     match in index 14
-    :param amino_acid: Variable on whether targets are protein
+    :param amino_acid: Boolean of whether targets are protein
     :param gene_names: List of all gene names in the analysis
     :param nt_allele_path: String of the absolute path to the folder containing nucleotide allele files
     :param aa_allele_path: String of the absolute path to the folder containing amino acid allele files
     :param report_path: String of the absolute path to the folder into which reports are to be written
     :param overlap_range: Integer of the maximum distance allowed between two genes in order for
     them to be considered co-located. Default is 50 bp
     :param cutoff: Integer of the minimum percent identity between query and subject sequence.
     Default is 100%
-    :return: runmetadata: Updated list of metadata objects
+    :return: runmetadata: Updated MetadataObjects
     :return: notes: List of contig:query_range-specific notes
     """
     logging.info('Parsing BLAST outputs')
     notes = {}
     for sample in runmetadata.samples:
         # Initialise GenObjects as required
         sample.alleles.blastlist = []
@@ -436,15 +517,15 @@
                     nt_allele_id = find_next_allele(
                         gene=base_gene,
                         allele_path=nt_allele_path
                     )
                     # Add the base gene name to the allele identifier
                     nt_allele = f'{base_gene}_{nt_allele_id}'
                     # Update the allele database with the new allele
-                    notes[contig][query_range_tuple] = update_allele_databases(
+                    notes[contig][query_range_tuple], nt_allele = update_allele_databases(
                         query_sequence=nt_querysequence,
                         header=nt_allele,
                         filtered=filtered,
                         gene=base_gene,
                         report_path=report_path,
                         allele_path=nt_allele_path,
                         notes=notes[contig][query_range_tuple],
@@ -453,15 +534,15 @@
                 # Add unfiltered novel aa alleles to the database
                 if not aa_allele and not filtered:
                     aa_allele_id = find_next_allele(
                         gene=base_gene,
                         allele_path=aa_allele_path
                     )
                     aa_allele = f'{base_gene}_{aa_allele_id}'
-                    notes[contig][query_range_tuple] = update_allele_databases(
+                    notes[contig][query_range_tuple], aa_allele = update_allele_databases(
                         query_sequence=aa_querysequence,
                         header=aa_allele,
                         filtered=filtered,
                         gene=base_gene,
                         report_path=report_path,
                         allele_path=aa_allele_path,
                         notes=notes[contig][query_range_tuple],
@@ -488,28 +569,28 @@
                         'query_ranges': [query_range],
                         'target': [nt_allele]
                     }
                 # If the keys already exist, append to the lists
                 else:
                     colocation_dict[contig]['query_ranges'].append(query_range)
                     colocation_dict[contig]['target'].append(nt_allele)
-            # Store the BLAST outputs in the metadata object
+            # Store the BLAST outputs in the MetadataObject
             sample.alleles.blastresults = resultdict
         # Populate missing results with 'NA' values
         if len(resultdict) == 0:
             sample.alleles.blastresults = 'NA'
         sample.alleles.overlap_dict = colocation_calculation(
             colocation_dict=colocation_dict,
             gene_names=gene_names,
             overlap_range=overlap_range
         )
     return runmetadata, notes
 
 
-def translate_sequence(nt_seq):
+def translate_sequence(nt_seq: str):
     """
     Uses BioPython to translate a nucleotide sequence to protein, and trims it to the first stop
     codon
     :param nt_seq: String of the nucleotide sequence
     :return aa_seq: String of the trimmed amino acid sequence
     """
     # Create a sequence object from the nucleotide sequence
@@ -524,15 +605,19 @@
         seq = Seq(allele_seq)
         aa_seq_object = str(seq.translate())
     # Split the sting on stop codons, keep only the first part of the split
     aa_seq = str(aa_seq_object).split('*', maxsplit=1)[0] + '*'
     return str(aa_seq)
 
 
-def aa_allele_lookup(aa_seq, gene, aa_allele_path, notes):
+def aa_allele_lookup(
+        aa_seq: str,
+        gene: str,
+        aa_allele_path: str,
+        notes: list):
     """
     Read in the amino acid allele file. Search for exact matches to the current sequence
     :param aa_seq: String of the amino acid sequence
     :param gene: Sting of the gene name
     :param aa_allele_path: String of the absolute path to the folder containing the amino acid
     allele files
     :param notes: List of notes for the current contig: query_range
@@ -553,15 +638,19 @@
         aa_seq=aa_seq,
         gene=gene,
         notes=notes
     )
     return filtered, notes
 
 
-def evaluate_translated_allele(aa_seq, gene, notes, aa=False):
+def evaluate_translated_allele(
+        aa_seq: str,
+        gene: str,
+        notes: list,
+        aa=False):
     """
     Evaluate whether an aa sequence passes the necessary length thresholds after trimming of an interior stop codons
     :param aa_seq: String of the amino acid sequence to evaluate
     :param gene: String of the name of the gene (no allele information) being evaluated
     :param notes: List of notes for the current contig: query_range
     :param aa: Boolean of whether the query sequence is amino acid. Triggers filtering if sequence doesn't end with a
     stop codon
@@ -589,32 +678,42 @@
         gene=gene,
         notes=notes,
         filtered=filtered
     )
     return filtered, notes
 
 
-def update_allele_databases(query_sequence, header, filtered, gene, report_path, allele_path, notes, molecule):
+def update_allele_databases(
+        query_sequence: SeqIO.parse,
+        header: str,
+        filtered: bool,
+        gene: str,
+        report_path: str,
+        allele_path: str,
+        notes: list,
+        molecule: str):
     """
     Update the appropriate allele file depending on quality filter status and molecule
     :param query_sequence: SEQIO sequence object of the novel allele
     :param header: String of the allele name (gene_allele ID)
     :param filtered: Boolean of whether the allele has been quality filtered
     :param gene: String of the name of the gene
     :param report_path: String of the absolute path to the folder into which the reports are to be written
     :param allele_path: String of the absolute path to the folder containing the allele database
     :param notes: List of notes on the alleles
     :param molecule: String of the current molecule. Options are Nucleotide and Amino acid
     :return: notes: Updated list of notes
     """
     # Create a SeqRecord of the allele using the novel allele name and sequence
-    new_record = SeqRecord(seq=Seq(query_sequence),
-                           id=header,
-                           name='',
-                           description='')
+    new_record = SeqRecord(
+        seq=Seq(query_sequence),
+        id=header,
+        name='',
+        description=''
+    )
     # Create a string to prepend to allele file names
     molecule_str = 'nt' if molecule == 'Nucleotide' else 'aa'
     # Set the correct files depending on the filtering status
     if not filtered:
         new_alleles = os.path.join(report_path, f'{molecule_str}_{gene}_novel_alleles.fasta')
         allele_file = os.path.join(allele_path, f'{gene}.fasta')
     else:
@@ -626,35 +725,44 @@
         for record in SeqIO.parse(allele_file, 'fasta'):
             # Append all the records to the list
             records.append(record)
     # Check to see if the query sequence is novel in the database
     if query_sequence not in [str(seq.seq) for seq in records]:
         # Append the SeqRecord to the novel alleles file
         with open(new_alleles, 'a+', encoding='utf-8') as novel:
-            SeqIO.write(sequences=new_record,
-                        handle=novel,
-                        format='fasta')
+            SeqIO.write(
+                sequences=new_record,
+                handle=novel,
+                format='fasta'
+            )
         records.append(new_record)
         # Overwrite the existing allele database file with the updated list of records
         with open(allele_file, 'w', encoding='utf-8') as alleles:
-            SeqIO.write(sequences=records,
-                        handle=alleles,
-                        format='fasta')
+            SeqIO.write(
+                sequences=records,
+                handle=alleles,
+                format='fasta'
+            )
         remove_combined_db_files(allele_path=allele_path)
         notes.append(f'{molecule} allele {header} is novel')
     # Non-novel sequences will have updated notes with the match
     else:
         for record in records:
             if str(query_sequence) == record.seq:
                 # Append the previous finding to the notes
                 notes.append(f'{molecule} matches previous result: {record.id}')
-    return notes
+                # Set the header to the corresponding record.id on a match
+                header = record.id
+    return notes, header
 
 
-def colocation_calculation(colocation_dict, gene_names, overlap_range):
+def colocation_calculation(
+        colocation_dict: dict,
+        gene_names: list,
+        overlap_range: int):
     """
     Determine if gene results are co-located on a contig
     :param colocation_dict: Dictionary of contig: {'query_ranges': [query_range],
     'target': [allele_id]}
     :param gene_names: List of all genes in the analysis
     :param overlap_range: Integer of the maximum distance allowed between two separate hits before
     they can no longer be considered co-located on a contig
@@ -721,16 +829,23 @@
                     }
                 # Append the current allele identifier to the list of alleles
                 overlap_dict[contig][tuple_range][gene]['allele'].append(current_allele)
     return overlap_dict
 
 
 def positive_overlap(
-        info_dict, other_iterator, query_range, other_range, overlap_dict,
-        current_allele, contig, gene_names, overlap):
+        info_dict: dict,
+        other_iterator: int,
+        query_range: range,
+        other_range: range,
+        overlap_dict: dict,
+        current_allele: str,
+        contig: str,
+        gene_names: list,
+        overlap: bool):
     """
     Determine the combined range of two overlapping ranges, extract gene names corresponding to
     allele names, populate dictionary of range overlaps
     :param info_dict: Dictionary of {'query_ranges': [query_range], 'target': [allele_id]}
     :param other_iterator: Integer of the iterator corresponding to the current other_range from the
     dictionary of other_range: iterator
     :param query_range: Range of hit corresponding to current_allele in info_dict
@@ -775,15 +890,17 @@
     overlap_dict[contig][full_range][gene_pair]['allele'].append(current_allele)
     # Set processed to True to indicate that there was an overlap and that the
     # dictionary was populated
     processed = True
     return overlap_dict, processed
 
 
-def calculate_full_range(query_range, other_range):
+def calculate_full_range(
+        query_range: range,
+        other_range: range):
     """
     Determine if two ranges overlap
     :param query_range: Range of hit corresponding to current_allele
     :param other_range: Range of hit corresponding to non-current allele
     :return full_range: Tuple of minimum coordinate from both ranges, maximum coordinate from
     both ranges
     """
@@ -795,15 +912,20 @@
     max_range = (max(query_range[1], other_range[1]))
     # The full range is a tuple of (min_range, max_range)
     # full_range = (100, 1000)
     full_range = tuple(sorted([min_range, max_range]))
     return full_range
 
 
-def evaluate_translated_length(aa_seq, length_dict, gene, notes, filtered):
+def evaluate_translated_length(
+        aa_seq: str,
+        length_dict: dict,
+        gene: str,
+        notes: list,
+        filtered: bool):
     """
     Evaluate whether a translated sequence passes a length filter and starts with a methionine
     residue
     :param aa_seq: String of the amino acid sequence to evaluate
     :param length_dict: Dictionary of minimum acceptable length for each gene in the analysis
     :param gene: String of the name of the gene
     :param notes: List of notes on the alleles
@@ -820,15 +942,21 @@
         filtered = True
         notes.append(
             f'{gene} amino acid sequence was {len(aa_seq)} amino acid residues. Minimum allowed '
             f'length is {length_dict[gene]} amino acid residues')
     return filtered, notes
 
 
-def generic_evaluate_translated_length(aa_seq, sequence, gene, notes, filtered, cutoff=0.95):
+def generic_evaluate_translated_length(
+        aa_seq: str,
+        sequence: str,
+        gene: str,
+        notes: list,
+        filtered: bool,
+        cutoff=0.95):
     """
     Evaluate whether a translated sequence passes a generic length filter and starts with a methionine
     residue
     :param aa_seq: String of the amino acid sequence to evaluate
     :param sequence: String of untrimmed nucleotide sequence
     :param gene: String of the name of the gene
     :param notes: List of notes on the alleles
@@ -850,15 +978,18 @@
         filtered = True
         notes.append(
             f'{gene} amino acid sequence was trimmed to {aa_seq_length} residues '
             f'the minimum length allowed is {minimum_length} residues')
     return filtered, notes
 
 
-def find_next_allele(gene, allele_path, extension='.fasta'):
+def find_next_allele(
+        gene: str,
+        allele_path: str,
+        extension='.fasta'):
     """
     Update the allele database with the novel allele extracted above
     :param gene: Name of the current gene being examined
     :param allele_path: Name and absolute path to folder containing allele files
     :param extension: String of the file extension. Default is .fasta
     :return: last_id: Number of the last alleles in the current database
     """
@@ -877,30 +1008,32 @@
         last_id = 0
     # Make it clear that these are novel profiles by starting at 1000000
     if last_id < 1000000:
         last_id = 999999
     return last_id + 1
 
 
-def remove_combined_db_files(allele_path):
+def remove_combined_db_files(allele_path: str):
     """
     Remove all the combined gene files used in BLAST analyses
     :param allele_path: String of the absolute path to the folder containing the alleles
     """
     # Find all the files in the directory with the word combined in the name
     combined_files = glob(os.path.join(allele_path, 'combined*'))
     # Remove each of the files
     for file in combined_files:
         os.remove(file)
 
 
-def create_nt_allele_comprehension(runmetadata, gene_names):
+def create_nt_allele_comprehension(
+        runmetadata: MetadataObject,
+        gene_names: list):
     """
     Create gene: nucleotide allele ID comprehensions for each contig: range combination with hits
-    :param runmetadata: List of metadata objects
+    :param runmetadata: MetadataObject with list of GenObjects for each query
     :param gene_names: List of all gene names in the analysis
     :return: allele_comprehension: nucleotide allele comprehension. allele_comprehension[contig][full_range] =
     {gene:allele}
     """
     logging.info('Determining nucleotide allele profiles')
     # Initialise an empty allele comprehension dictionary
     allele_comprehension = {}
@@ -965,18 +1098,20 @@
                 # Update the dictionary with the negative result
                 allele_comprehension[contig][full_range].update(
                                 {gene: '0'}
                             )
     return allele_comprehension
 
 
-def create_aa_allele_comprehension(runmetadata, gene_names):
+def create_aa_allele_comprehension(
+        runmetadata: MetadataObject,
+        gene_names: list):
     """
     Create gene: amino acid allele ID comprehensions for each contig: range combination with hits
-    :param runmetadata: List of metadata objects
+    :param runmetadata: MetadataObject with list of GenObjects for each query
     :param gene_names: List of all gene names in the analysis
     :return: allele_comprehension: amino acid allele comprehension. allele_comprehension[contig][full_range] =
     {gene:allele}
     """
     logging.info('Determining amino acid allele profiles')
     # Initialise a dictionary to store contig:query_range gene:alleleID results
     allele_comprehension = {}
@@ -1038,15 +1173,15 @@
                         if gene not in allele_comprehension[contig][full_range]:
                             allele_comprehension[contig][full_range].update(
                                     {gene: '0'}
                                 )
     return allele_comprehension
 
 
-def create_frozen_allele_comprehension(allele_comprehension):
+def create_frozen_allele_comprehension(allele_comprehension: dict):
     """
     Freeze allele comprehension dictionaries
     :param allele_comprehension: Dictionary of contig:full_range: {gene:allele}
     :return: frozen_allele_comprehension: Dictionary of contig:query_range: json.dumps({gene:allele}, sort_keys=True)
     """
     # Initialise a dictionary to store the frozen allele comprehensions
     frozen_allele_comprehension = {}
@@ -1061,19 +1196,25 @@
             frozen_allele_dict = json.dumps(allele_dict, sort_keys=True)
             # Update the dictionary with the range and the frozen allele string
             if query_range not in frozen_allele_comprehension[contig]:
                 frozen_allele_comprehension[contig][query_range] = frozen_allele_dict
     return frozen_allele_comprehension
 
 
-def extract_novel_alleles(sample, gene, genome_query, amino_acid, allele_path, report_path,
-                          cutoff=75):
+def extract_novel_alleles(
+        sample: MetadataObject,
+        gene: str,
+        genome_query: bool,
+        amino_acid: bool,
+        allele_path: str,
+        report_path: str,
+        cutoff=75):
     """
     Extract the sequence of novel alleles from samples that do not have a 100% match
-    :param sample: Metadata object
+    :param sample: MetadataObject with list of GenObjects for each query
     :param gene: Name of current gene
     :param genome_query: Boolean of whether the allele or the genome are the query
     :param amino_acid: Variable indicating whether the current analyses are on DNA or
     amino acid sequences
     :param allele_path: Name and absolute path to folder containing allele files
     :param report_path: Name and absolute path to folder in which reports are to be created
     :param cutoff: The minimum percent identity cutoff to allow when considering the presence of a
@@ -1126,15 +1267,20 @@
             allele_path=allele_path,
             report_path=report_path,
             amino_acid=amino_acid,
         )
     return sample, novel_allele, query_sequence
 
 
-def update_allele_database(gene, query_sequence, allele_path, report_path, amino_acid):
+def update_allele_database(
+        gene: str,
+        query_sequence: str,
+        allele_path: str,
+        report_path: str,
+        amino_acid: bool):
     """
     Update the allele database with the novel allele extracted above
     :param gene: Name of the current gene being examined
     :param query_sequence: Sequence of the novel allele
     :param allele_path: Name and absolute path to folder containing allele files
     :param report_path: Name and absolute path to folder in which reports are to be created
     :param amino_acid: Variable indicating whether the current analyses are on DNA or
@@ -1192,19 +1338,19 @@
             sequences=records,
             handle=alleles,
             format='fasta'
         )
     return novel_allele
 
 
-def translate(runmetadata):
+def translate(runmetadata: MetadataObject):
     """
     Use BioPython to translate DNA to amino acid
-    :param runmetadata: List of metadata objects for each query
-    :return: Updated list of metadata objects
+    :param runmetadata: MetadataObject with list of GenObjects for each query
+    :return: Updated MetadataObject
     """
     logging.info('Translating allele sequences to amino acid')
     for sample in runmetadata.samples:
         # Initialise the dictionary to store the translated sequence
         sample.alleles.nt_alleles_translated = {}
         for allele, allele_sequence_list in sample.alleles.targetsequence.items():
             for allele_sequence in allele_sequence_list:
@@ -1222,16 +1368,22 @@
                 # Ensure that the allele name exists (isn't an empty string) before adding
                 # allele name: translated sequence to the dictionary
                 if allele:
                     sample.alleles.nt_alleles_translated[allele] = aa_seq
     return runmetadata
 
 
-def match_profile(profile_data, frozen_allele_comprehension, report_path, profile_file, genes,
-                  allele_comprehension, molecule):
+def match_profile(
+        profile_data: dict,
+        frozen_allele_comprehension: dict,
+        report_path: str,
+        profile_file: str,
+        genes: list,
+        allele_comprehension: dict,
+        molecule: str):
     """
     Match current profiles to any previously created profiles
     :param profile_data: Dictionary of seq_type: {gene name: allele ID}
     :param frozen_allele_comprehension: Dictionary of json.dumps({gene name: allele ID}, sort_keys=True): seq_type
     :param report_path: Name and absolute path to folder in which reports are to be created
     :param profile_file: Name and path of file containing reduced profiles
     :param genes: List of all genes in the analysis
@@ -1269,18 +1421,23 @@
                 profile_matches[contig][query_range] = update_profiles(
                     profile_file=profile_file,
                     report_path=report_path,
                     genes=genes,
                     allele_dict=allele_comprehension[contig][query_range],
                     molecule=molecule
                 )
+                # Update the profile_data dictionary with the new sequence type
+                profile_data[profile_matches[contig][query_range]] = allele_comprehension[contig][query_range]
+                frozen_profiles = freeze_profiles(
+                    profile_data=profile_data
+                )
     return profile_matches, frozen_profiles
 
 
-def freeze_profiles(profile_data):
+def freeze_profiles(profile_data: dict):
     """
     Freeze profiles, so that the frozen {gene:allele} dictionary can be used as the key and the corresponding sequence
     type as the value
     :param profile_data: Dictionary of all profiles in seq_type: {gene name: allele ID} format
     :return: frozen_profiles: Dictionary of json.dumps({gene name: allele ID}, sort_keys=True): seq_type
     """
     # Initialise a dictionary to store the frozen profiles information
@@ -1290,15 +1447,20 @@
         # Freeze the allele comprehension
         frozen_allele_comprehension = json.dumps(allele_comprehension, sort_keys=True)
         # Populate the dictionary with frozen_allele_comprehension: seq_type
         frozen_profiles[frozen_allele_comprehension] = seq_type
     return frozen_profiles
 
 
-def update_profiles(profile_file, report_path, genes, allele_dict, molecule):
+def update_profiles(
+        profile_file: str,
+        report_path: str,
+        genes: list,
+        allele_dict: dict,
+        molecule: str):
     """
     Run methods to add novel profiles to the profile file. Determine the sequence type to use, and update the file
     :param profile_file: Name and path of file containing reduced profiles
     :param report_path: Name and absolute path to folder in which reports are to be created
     :param genes: List of all genes in the analysis
     :param allele_dict: Dictionary of a single allele comprehension. Extracted from
     allele_comprehension[contig][query_range] = {gene: allele}
@@ -1306,26 +1468,28 @@
     :return: next_seq_type: Integer of the sequence type assigned to the novel profile
     """
     # Extract the sequence type to use for the novel profile
     next_seq_type = return_next_seq_type(
         profile_file=profile_file
     )
     # Update the profile file
-    update_profile_file(
+    created = update_profile_file(
         profile_file=profile_file,
         next_seq_type=next_seq_type,
         allele_dict=allele_dict,
         genes=genes,
         report_path=report_path,
         molecule=molecule
     )
+    if not created:
+        next_seq_type = 'N/A'
     return next_seq_type
 
 
-def return_next_seq_type(profile_file):
+def return_next_seq_type(profile_file: str):
     """
     Parse the profile file, and return the value for the next sequence type to be used. Local profiles will start at
     1000000 in order to be distinct from Enterobase profiles
     :param profile_file: Name and path of file containing reduced profiles
     :return: last_seq_type + 1: Integer of the sequence type to be assigned to the novel profile
     """
     # Open the profile file
@@ -1342,35 +1506,44 @@
     # If the sequence type corresponds to an Enterobase number, use our local numbering scheme instead
     if int_last_seq_type < 1000000:
         int_last_seq_type = 999999
     # Return the last sequence type + 1 to give the next sequence type
     return int_last_seq_type + 1
 
 
-def update_profile_file(profile_file, next_seq_type, allele_dict, genes, report_path, molecule):
+def update_profile_file(
+        profile_file: str,
+        next_seq_type: int,
+        allele_dict: dict,
+        genes: list,
+        report_path: str,
+        molecule: str):
     """
     Update the profile file with novel profile. Additionally, either create or update the novel_profiles.txt file
     with the same profile
     :param profile_file: Name and path of file containing reduced profiles
     :param next_seq_type: Integer of the sequence type to be assigned to the novel profile
     :param allele_dict: Dictionary of a single allele comprehension. Extracted from
     allele_comprehension[contig][query_range] = {gene: allele}
     :param genes: List of all genes in the analysis
     :param report_path: Name and absolute path to folder in which reports are to be created
     :param molecule: String of the current molecule being processed. Options are "aa" and "nt"
+    :return bool: Boolean of whether the profile could be created or not
     """
 
     # Initialise a string to store the profile information with the novel sequence type
     seq_type_str = f'{next_seq_type}'
     # Initialise a header to store 'ST  gene1   gene2.......geneX\n'
     header = 'ST'
     # Iterate over all the genes in the analysis
     for gene in genes:
         # Extract the allele ID for each gene in the analysis
         allele = allele_dict[gene]
+        if not allele:
+            return False
         # Update the header with the gene
         header += f'\t{gene}'
         # Update the profile string with the allele ID
         seq_type_str += f'\t{allele}'
     # Open the profile file (to update) and write the novel profile
     with open(profile_file, 'a+', encoding='utf-8') as profile:
         profile.write(seq_type_str + '\n')
@@ -1382,22 +1555,31 @@
         with open(novel_profile_file, 'w', encoding='utf-8') as novel_profile:
             novel_profile.write(header + '\n')
             novel_profile.write(seq_type_str + '\n')
     # Otherwise, update the existing file with the novel profile
     else:
         with open(novel_profile_file, 'a+', encoding='utf-8') as novel_profile:
             novel_profile.write(seq_type_str + '\n')
+    return True
 
 
-def create_stec_report(runmetadata, nt_profile_matches, nt_alleles, aa_profile_matches,
-                       aa_alleles, report_file, gene_names, aa_profile_path, notes):
+def create_stec_report(
+        runmetadata: MetadataObject,
+        nt_profile_matches: dict,
+        nt_alleles: dict,
+        aa_profile_matches: dict,
+        aa_alleles: dict,
+        report_file: str,
+        gene_names: list,
+        aa_profile_path: str,
+        notes: list):
     """
     Create a STEC-specific report including the allele matches for each gene and sequence type for both nucleotide and
     amino acid sequence information
-    :param runmetadata: List of metadata objects for each query
+    :param runmetadata: MetadataObject with list of GenObjects for each query
     :param nt_profile_matches: Dictionary of contig:query_range:nucleotide seq_type_match
     :param nt_alleles: Dictionary of nucleotide contig:full_range:nucleotide seq_type_match
     :param aa_profile_matches: Dictionary of contig:query_range:amino acid seq_type_match
     :param aa_alleles: Dictionary of amino acid contig:full_range: {gene:allele}
     :param report_file: String of the name and path of the report file
     :param gene_names: List of all gene names in the analysis
     :param aa_profile_path: String of the absolute path of the folder in which the amino acid profile file is located
@@ -1494,15 +1676,19 @@
             report.write(data)
     # If the report already exists, write only the data string
     else:
         with open(report_file, 'a+', encoding='utf-8') as report:
             report.write(data)
 
 
-def update_profile_link_file(nt_seq_type, aa_seq_type, note, aa_profile_path):
+def update_profile_link_file(
+        nt_seq_type: str,
+        aa_seq_type: str,
+        note: list,
+        aa_profile_path: str):
     """
     Update the file linking amino acid sequence type to the (multiple) corresponding nucleotide sequence type(s)
     :param nt_seq_type: String of the nucleotide sequence type
     :param aa_seq_type: String of the amino acid sequence type
     :param note: List of notes on the alleles
     :param aa_profile_path: String of the absolute path of the folder in which the amino acid profile file is located
     :return: note: Update list of notes
@@ -1555,15 +1741,17 @@
     # Overwrite the profile link file with the updated links
     with open(link_file, 'w', encoding='utf-8') as profile_link:
         for record in records:
             profile_link.write(f'{record}\t{links[record]}\n')
     return note
 
 
-def split_alleles(allele_files, output_path):
+def split_alleles(
+        allele_files: list,
+        output_path: str):
     """
     Split FASTA files into individual sequences
     :param allele_files: List of absolute path to FASTA-formatted allele sequence files
     :param output_path: String of the absolute path into which the individual sequence files are to be written
     """
     # Create the output path if it doesn't already exist
     make_path(inpath=output_path)
@@ -1578,30 +1766,37 @@
             # Set the name of the file to be the FASTA header
             output_file = os.path.join(output_path, f'{record.id}.fasta')
             # Write the record to the new file
             with open(output_file, 'w', encoding='utf-8') as output:
                 SeqIO.write(record, output, 'fasta')
 
 
-def parse_aa_blast(runmetadata, extended_fieldnames, fieldnames, gene_names, notes, aa_allele_path,
-                   report_path, cutoff):
+def parse_aa_blast(
+        runmetadata: MetadataObject,
+        extended_fieldnames: list,
+        fieldnames: list,
+        gene_names: list,
+        notes: list,
+        aa_allele_path: str,
+        report_path: str,
+        cutoff: int):
     """
     Parse amino acid BLAST results
-    :param runmetadata: List of metadata objects
+    :param runmetadata: MetadataObject with list of GenObjects for each query
     :param extended_fieldnames: List of the BLAST fields used, as well as the additional percent
     match in index 14
     :param fieldnames: List of the BLAST fields used
     :param gene_names: List of all gene names in the analysis
     :param notes: List of sample-specific notes
     :param aa_allele_path: String of the absolute path to the folder containing amino acid allele files
     :param report_path: String of the absolute path to the folder into which reports are to be written
     them to be considered co-located. Default is 50 bp
     :param cutoff: Integer of the minimum percent identity between query and subject sequence.
     Default is 90
-    :return: runmetadata: Updated list of metadata objects
+    :return: runmetadata: Updated MetadataObject
     :return: filtered: Boolean of whether the sample fails quality/length checks
     :return: notes: Updated list of sample-specific notes
     """
     logging.info('Parsing BLAST outputs')
     # Initialise a boolean to track if the sequence fails checks
     filtered = False
     for sample in runmetadata.samples:
@@ -1645,15 +1840,15 @@
                 aa_allele_id = find_next_allele(
                     gene=gene,
                     allele_path=aa_allele_path
                 )
                 # Set the name of the allele as gene_alleleID
                 aa_allele = f'{gene}_{aa_allele_id}'
                 # Update the allele database with the novel allele
-                notes = update_allele_databases(
+                notes, aa_allele = update_allele_databases(
                     query_sequence=query_seq,
                     header=aa_allele,
                     filtered=filtered,
                     gene=gene,
                     report_path=report_path,
                     allele_path=aa_allele_path,
                     notes=notes,
@@ -1663,21 +1858,24 @@
                 if not filtered:
                     sample.alleles.blastlist.append(aa_allele)
                 # Update the processed boolean
                 processed = True
     return runmetadata, filtered, notes
 
 
-def analyse_aa_alleles(runmetadata, gene_names, notes):
+def analyse_aa_alleles(
+        runmetadata: MetadataObject,
+        gene_names: list,
+        notes: list):
     """
     Analyse supplied amino acid alleles to ensure that they pass quality checks
-    :param runmetadata: List of metadata objects
+    :param runmetadata: MetadataObject with list of GenObjects for each query
     :param gene_names: List of all gene names in the analysis
     :param notes: List of sample-specific notes
-    :return: runmetadata: Updated list of metadata objects
+    :return: runmetadata: Updated MetadataObject
     :return: notes: Updated list of sample-specific notes
     """
     # Iterate through all the samples
     for sample in runmetadata.samples:
         # Iterate over all the records in the file (should only be one, as these files must be split with the
         # split_alleles function)
         for record in SeqIO.parse(sample.general.bestassemblyfile, 'fasta'):
@@ -1689,35 +1887,169 @@
                 gene=gene,
                 notes=notes,
                 aa=True
             )
     return runmetadata, notes
 
 
-def report_aa_alleles(runmetadata, report_file, notes):
+def report_aa_alleles(
+        runmetadata: MetadataObject,
+        report_file: str,
+        notes: list):
     """
     Create an amino acid query-specific report with sample name, allele match, and notes
-    :param runmetadata: List of metadata objects
+    :param runmetadata: MetadataObject with list of GenObjects for each query
     :param report_file: String of absolute path to the report file
     :param notes: List of sample-specific notes
     """
     # Initialise the header string
     header = 'Sample\tMatch\tNotes\n'
     # Create an empty string to store the sample-specific results
     data = str()
     # Iterate over all the samples
     for sample in runmetadata.samples:
-        # Extract the list of hits from the metadata object, and join with semicolons
+        # Extract the list of hits from the MetadataObject, and join with semicolons
         matches = ';'.join(sample.alleles.blastlist)
         # Join the list of notes with
         note = ';'.join(notes)
         # Populate the data string with the matches and notes
         data += f'{sample.name}\t{matches}\t{note}\n'
     # If the report doesn't already exist write the header and data string
     if not os.path.isfile(report_file):
         with open(report_file, 'w', encoding='utf-8') as report:
             report.write(header)
             report.write(data)
     # Otherwise write only the data string
     else:
         with open(report_file, 'a+', encoding='utf-8') as report:
             report.write(data)
+
+
+def load_alleles(
+        allele_path: str,
+        allele_order: dict):
+    """
+    Use SeqIO to read in allele files
+    :param str allele_path: Name and path of folder containing allele files
+    :param dict allele_order: Dictionary of stx gene name: allele order to use
+    :return: str stx_gene: Name of stx gene (stx1 or stx2) being concatenated
+    :return: dict allele_dict: Dictionary of stx gene name: allele name: allele sequence
+    """
+    # Initialise variable to store the stx gene name being analysed and the sequence of the alleles
+    stx_gene = None
+    allele_dict = {}
+    # Find all the allele files in the folder
+    allele_files = glob(os.path.join(allele_path, '*.fasta'))
+    for allele_file in allele_files:
+        # Set the name of the subunit by splitting off the path information and the file extension from the file
+        allele_name = os.path.splitext(os.path.basename(allele_file))[0]
+        # Determine which stx gene is being processed
+        for gene_name, alleles in allele_order.items():
+            # The name of the current subunit is present in the list of subunits linked to the stx gene
+            if allele_name in alleles:
+                stx_gene = gene_name
+        # Initialise the subunit name in the dictionary as required
+        if allele_name not in allele_dict:
+            allele_dict[allele_name] = {}
+        # Use SeqIO to read in the allele file
+        for record in SeqIO.parse(handle=allele_file, format='fasta'):
+            # Add the name of the allele and its sequence to the dictionary
+            allele_dict[allele_name][record.id] = str(record.seq)
+    return stx_gene, allele_dict
+
+
+def concatenate_alleles(
+        profile_data: dict,
+        allele_dict: dict,
+        allele_order: dict,
+        stx_gene: str,
+        linker_length_dict: dict,
+        molecule: str):
+    """
+
+    :param profile_data: Dictionary of all profiles in seq_type: {gene name: allele ID} format
+    :param allele_dict: Dictionary of stx gene name: allele name: allele sequence
+    :param dict allele_order: Dictionary of stx gene name: allele order to use
+    :param str stx_gene: Name of stx gene (stx1 or stx2) being concatenated
+    :param dict linker_length_dict: Dictionary of gene name: length of linker sequence to use
+    :param str molecule: String of the current molecule. Options are "nt" (nucleotide) and "aa" (amino acid)
+    :return: concatenated_sequences: List of SeqRecords for all concatenated sequences
+    """
+    # Create a list to store SeqRecords of the concatenated sequences
+    concatenated_sequences = []
+    # Iterate over all the sequence type: profile pairs in profile_data
+    for seq_type, profile in profile_data.items():
+        # Initialise a string to store the concatenated sequences
+        concatenated_seq = str()
+        # Create a boolean to store if one (or both) of the allele subunits is missing
+        complete = True
+        # Iterate over the subunits in order from the allele_order dictionary
+        for subunit in allele_order[stx_gene]:
+            # Extract the allele number from the profile dictionary using the subunit as the key
+            allele_number = profile[subunit]
+            # If the allele number is 0, the subunit is absent, and the concatenated sequence will not be created
+            if allele_number == '0':
+                complete = False
+                continue
+            # Set the full allele name by joining the subunit with the allele number
+            full_allele_name = f'{subunit}_{allele_number}'
+            # Extract the string of the allele sequence from the allele dictionary
+            allele_seq = allele_dict[subunit][full_allele_name]
+            # If the first subunit is already present, simply append the second subunit to the string
+            if concatenated_seq:
+                concatenated_seq += allele_seq
+            # Otherwise the linker sequence must be created
+            else:
+                # Extract the gene-specific linker length from the dictionary
+                linker_length = linker_length_dict[stx_gene]
+                # Nucleotide sequences will use N as the linker sequence
+                if molecule == 'nt':
+                    linker = 'N' * linker_length
+                # Amino acid sequences will use X as the linker sequence, and will be reduced by a factor of three
+                else:
+                    linker = 'X' * int(linker_length / 3)
+                concatenated_seq += f'{allele_seq}{linker}'
+        # Do not add incomplete sequences to the list
+        if not complete:
+            continue
+        # Create a SeqRecord of the allele using the novel allele name and sequence
+        concatenated_sequences.append(
+            SeqRecord(
+                seq=Seq(concatenated_seq),
+                id=seq_type,
+                name='',
+                description=''
+            )
+        )
+    return concatenated_sequences
+
+
+def write_concatenated_sequences(
+        concatenated_sequences: list,
+        concatenate_path: str,
+        file_name: str,
+        molecule: str):
+    """
+    Write the concatenated sequences to file
+    :param list concatenated_sequences: List of all SeqRecord objects for the concatenated sequences
+    :param str concatenate_path: Name and absolute path of the folder into which the FASTA files of the concatenated
+    sequences are to be written
+    :param str file_name: File name to use. 'ECs2974_ECs2973' (stx1) and 'ECs1205_ECs1206' (stx2)
+    :param str molecule: String of the current molecule. Options are "nt" (nucleotide) and "aa" (amino acid)
+    """
+    # Set the name of the output path by adding the molecule to the supplied path
+    output_path = os.path.join(concatenate_path, molecule)
+    make_path(inpath=output_path)
+    # Clear out any previous iterations of this script
+    previous_fastas = glob(os.path.join(output_path, '*.fasta'))
+    for fasta in previous_fastas:
+        os.remove(fasta)
+    # Set the name of the file to use
+    concatenated_file = os.path.join(output_path, f'{file_name}.fasta')
+    # Iterate over all the concatenated sequences
+    for concatenated_seq in concatenated_sequences:
+        with open(concatenated_file, 'a+', encoding='utf-8') as output_file:
+            SeqIO.write(
+                sequences=concatenated_seq,
+                handle=output_file,
+                format='fasta'
+            )
```

### Comparing `AlleleFinder-0.1.2/allele_tools/allele_updater.py` & `AlleleFinder-0.1.3/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/allele_tools/allele_translate_reduce.py` & `AlleleFinder-0.1.3/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/tests/test_5_stec_allele_find.py` & `AlleleFinder-0.1.3/tests/test_5_stec_allele_find.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
             aa_alleles=variables.aa_allele_path,
             query_path=variables.query_path,
             report_path=variables.report_path
         )
         arguments = cli()
         allele_find(args=arguments)
 
+
 @patch('argparse.ArgumentParser.parse_args')
 def test_allele_find_integration(mock_args, variables):
     prepare_files(
         variables=variables,
         links=True
     )
     mock_args.return_value = argparse.Namespace(
@@ -92,15 +93,17 @@
     allele_find(args=arguments)
     variables.allele_report = os.path.join(variables.report_path, 'stec_report.tsv')
     assert os.path.isfile(variables.allele_report)
 
 
 def test_report_contents(variables):
     variables.report_contents = open(variables.allele_report, 'r', encoding='utf-8').readlines()
+    assert variables.report_contents[1] == \
+        '2013-SEQ-0039	6	9	241	6	2	68\t\n'
     assert variables.report_contents[16] == \
-           '2017-SEQ-0617	0	2	116	0		1000002	ECs1206 amino acid sequence does not start ' \
-           'with M; ECs1206 amino acid sequence was 14 amino acid residues. Minimum allowed length is ' \
-           '88 amino acid residues; Novel nt_seq_type 116, and aa_seq_type 1000002\n'
+           '2017-SEQ-0617	0	2	116	0		N/A	ECs1206 amino acid sequence does not start with M; ' \
+           'ECs1206 amino acid sequence was 14 amino acid residues. Minimum allowed length is 88 amino acid residues; ' \
+           'Novel nt_seq_type 116, and aa_seq_type N/A\n'
 
 
 def test_clean(variables):
     clean_outputs(variables=variables)
```

### Comparing `AlleleFinder-0.1.2/tests/test_1_allele_translate_reduce.py` & `AlleleFinder-0.1.3/tests/test_1_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/tests/test_3_stec_profile_reduce.py` & `AlleleFinder-0.1.3/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/tests/test_0_profile_reduce.py` & `AlleleFinder-0.1.3/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/tests/test_7_stec_allele_split.py` & `AlleleFinder-0.1.3/tests/test_7_stec_allele_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python
 
 """
-Unit and integration tests for allele_tools/profile_reduce.py
+Unit and integration tests for allele_tools/stec.py allele_split
 """
 
 # Standard imports
 from unittest.mock import patch
 from glob import glob
 import argparse
 import shutil
 import os
 
 # Third-party imports
 from Bio import SeqIO
 import pytest
 
 # Local imports
-from allele_tools.stec import \
-    allele_split, \
+from allele_tools.stec import (
+    allele_split,
     cli
+)
 
 
 @pytest.fixture(name='variables', scope='module')
 def setup():
     class Variables:
         def __init__(self):
             # Extract the connection string prior to running tests
@@ -59,14 +60,15 @@
         mock_args.return_value = argparse.Namespace(
             query_path=variables.query_path,
             output_path=variables.output_path
         )
         arguments = cli()
         allele_split(args=arguments)
 
+
 @patch('argparse.ArgumentParser.parse_args')
 def test_profile_reduce_missing_tilde_profile(mock_args, variables):
     prepare_files(variables=variables)
     mock_args.return_value = argparse.Namespace(
         query_path=variables.query_path,
         output_path=variables.output_path
     )
```

### Comparing `AlleleFinder-0.1.2/tests/test_2_allele_updater.py` & `AlleleFinder-0.1.3/tests/test_2_allele_updater.py`

 * *Files identical despite different names*

### Comparing `AlleleFinder-0.1.2/tests/test_4_stec_allele_translate_reduce.py` & `AlleleFinder-0.1.3/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

