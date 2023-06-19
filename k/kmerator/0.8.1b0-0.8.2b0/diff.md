# Comparing `tmp/kmerator-0.8.1b0.tar.gz` & `tmp/kmerator-0.8.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerator-0.8.1b0.tar", last modified: Thu Jun 15 13:05:40 2023, max compression
+gzip compressed data, was "kmerator-0.8.2b0.tar", last modified: Mon Jun 19 12:58:10 2023, max compression
```

## Comparing `kmerator-0.8.1b0.tar` & `kmerator-0.8.2b0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-15 13:05:40.573857 kmerator-0.8.1b0/
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.8.1b0/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-15 13:05:40.569773 kmerator-0.8.1b0/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11626 2023-06-15 12:20:25.000000 kmerator-0.8.1b0/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-15 13:05:40.452747 kmerator-0.8.1b0/kmerator/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.8.1b0/kmerator/__init__.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.8.1b0/kmerator/color.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.8.1b0/kmerator/config.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19683 2023-05-16 08:28:01.000000 kmerator-0.8.1b0/kmerator/dataset.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.8.1b0/kmerator/exit.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-06-15 12:58:43.000000 kmerator-0.8.1b0/kmerator/info.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    11984 2023-06-15 12:31:45.000000 kmerator-0.8.1b0/kmerator/kmerator.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    18618 2023-06-15 12:55:37.000000 kmerator-0.8.1b0/kmerator/kmerize.py
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.8.1b0/kmerator/longest_transcript.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.8.1b0/kmerator/mk_geneinfo.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.8.1b0/kmerator/mk_transcriptome.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    12152 2023-05-16 08:26:02.000000 kmerator-0.8.1b0/kmerator/options.py
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-15 13:05:40.553502 kmerator-0.8.1b0/kmerator.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/requires.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-06-15 13:05:40.576299 kmerator-0.8.1b0/setup.cfg
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1109 2023-06-15 12:34:30.000000 kmerator-0.8.1b0/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-19 12:58:10.619572 kmerator-0.8.2b0/
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.8.2b0/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-19 12:58:10.616210 kmerator-0.8.2b0/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11626 2023-06-15 12:20:25.000000 kmerator-0.8.2b0/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-19 12:58:10.493702 kmerator-0.8.2b0/kmerator/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.8.2b0/kmerator/__init__.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.8.2b0/kmerator/color.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.8.2b0/kmerator/config.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19683 2023-05-16 08:28:01.000000 kmerator-0.8.2b0/kmerator/dataset.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.8.2b0/kmerator/exit.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-06-19 12:54:05.000000 kmerator-0.8.2b0/kmerator/info.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    11984 2023-06-15 12:31:45.000000 kmerator-0.8.2b0/kmerator/kmerator.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    18699 2023-06-19 12:33:32.000000 kmerator-0.8.2b0/kmerator/kmerize.py
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.8.2b0/kmerator/longest_transcript.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.8.2b0/kmerator/mk_geneinfo.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.8.2b0/kmerator/mk_transcriptome.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    12678 2023-06-19 12:52:43.000000 kmerator-0.8.2b0/kmerator/options.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-19 12:58:10.599860 kmerator-0.8.2b0/kmerator.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-06-19 12:58:10.622067 kmerator-0.8.2b0/setup.cfg
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1109 2023-06-15 12:34:30.000000 kmerator-0.8.2b0/setup.py
```

### Comparing `kmerator-0.8.1b0/PKG-INFO` & `kmerator-0.8.2b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.8.1b0
+Version: 0.8.2b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.8.1b0/README.md` & `kmerator-0.8.2b0/README.md`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.1b0/kmerator/config.py` & `kmerator-0.8.2b0/kmerator/config.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.1b0/kmerator/dataset.py` & `kmerator-0.8.2b0/kmerator/dataset.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.1b0/kmerator/info.py` & `kmerator-0.8.2b0/kmerator/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Genral informations on to the program.
 """
 
 APPNAME = "kmerator"
 SHORTDESC = "Find specific gene or transcript kmers. And more."
 LICENCE = "GPL3"
-VERSION = "0.8.1-beta"
+VERSION = "0.8.2-beta"
 AUTHOR = 'Sébastien RIQUIER, IRMB, Montpellier'
 AUTHOR_EMAIL = "sebastien.riquier@ucd.ie"
 CONTIBUTORS = [
     'Chloe BESSIERE chloe.bessiere@inserm.fr>'
     'Benoit GUIBERT <benoit.guibert@inserm.fr>',
 ]
 DOC = f"""
```

### Comparing `kmerator-0.8.1b0/kmerator/kmerator.py` & `kmerator-0.8.2b0/kmerator/kmerator.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.1b0/kmerator/kmerize.py` & `kmerator-0.8.2b0/kmerator/kmerize.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,24 +183,25 @@
 
         i = 1
         for mer, abund_in_tr in kmercounts_transcriptome_dict.items():
 
             kmer_pos = i
             try:
                 abund_in_ge = int(kmercounts_genome_dict[mer])    # abundance in genome for this kmer
-            except KeyError:
+            except KeyError as err:
                 if len(mer) != len(next(iter(kmercounts_genome_dict))):
                     raise KeyError(f"ErrorIndexLength: length of kmer expected: {self.args['kmer_length']}\n"
                                    f"  Genome kmer index length: {len(next(iter(kmercounts_genome_dict)))}\n"
                                    f"  Transcriptome kmer index length (dataset): {len(mer)}")
                 revcomp = self.__revcomp(mer)
                 if revcomp in kmercounts_genome_dict:
                     raise KeyError("ErrorGenomeIndex: The jellyfish indexes of the genome and "
                                    "transcriptome do not match.\nA possible error is that the "
                                    "genome index was built with the jellyfish '-C' option.")
+                raise KeyError(f"Error: kmer not found in genome: {err}")
 
             if level == 'gene':
                 ### if the kmer is present/unique or does not exist (splicing?) on the genome
                 if abund_in_ge <= 1:
 
                     isoforms_with_mer = [enst for enst, seq in isoforms_dict.items() if mer in seq]
                     isoforms_with_mer_nb = len(isoforms_with_mer)
```

### Comparing `kmerator-0.8.1b0/kmerator/longest_transcript.py` & `kmerator-0.8.2b0/kmerator/longest_transcript.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.1b0/kmerator/mk_geneinfo.py` & `kmerator-0.8.2b0/kmerator/mk_geneinfo.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.1b0/kmerator/mk_transcriptome.py` & `kmerator-0.8.2b0/kmerator/mk_transcriptome.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.1b0/kmerator/options.py` & `kmerator-0.8.2b0/kmerator/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,14 +211,15 @@
     if not os.path.isdir(args.datadir):
         sys.exit(f"{ERROR}Error: {args.datadir!r} not found or not a directory.{ENDCOL}")
     if not os.access(args.datadir, os.R_OK) or not os.access(args.datadir, os.X_OK):
         sys.exit(f"{ERROR}Error: insufficient rights in {args.datadir!r}.{ENDCOL}")
     ### --fasta-file - check if query fasta file is present
     if args.fasta_file and not os.path.isfile(args.fasta_file):
         sys.exit(f"{ERROR}Error: {args.fasta_file!r} not found.{ENDCOL}")
+    check_fasta_file(args)
     ### --fasta-file - Check query fasta file extension
     if args.fasta_file and args.fasta_file.split('.')[-1] not in ("fa", "fasta"):
         sys.exit(f" {ERROR}Error: {os.path.basename(args.fasta_file)} " \
                 f"Does not appears to be a fasta file.{ENDCOL}")
     ### --selection - Check Gene Select option
     if args.selection:
         for gene in args.selection:
@@ -246,14 +247,29 @@
             sys.exit(f"{ERROR}Error: temporary directory not found ({args.tmpdir}).{ENDCOL}")
         else:
             args.tmpdir = tempfile.mkdtemp(prefix="kmerator_", dir=args.tmpdir)
     else:
         args.tmpdir = args.output
 
 
+def check_fasta_file(args):
+    headers = set()
+    with open(args.fasta_file) as fh:
+        nb = 1
+        for row in fh:
+            if row.startswith('>'):
+                header = row.split(' ')[0]
+                if header in headers:
+                    sys.exit(f"{ERROR}ErrorFastaFile: sequence identifier must be unique.\n"
+                                    f"    {header.rstrip()!r} is not unique (line {nb}).")
+                headers.add(header)
+            nb += 1
+    del headers
+
+
 '''
 def is_transcriptome_ensembl_file(first_row):
     """Checks if the line matches the Ensembl transcriptome file format"""
     line = first_row.split()
     try:
         if (not line[6].startswith('gene_symbol:') or
             not line[0].startswith('>ENST') or
```

### Comparing `kmerator-0.8.1b0/kmerator.egg-info/PKG-INFO` & `kmerator-0.8.2b0/kmerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.8.1b0
+Version: 0.8.2b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.8.1b0/setup.py` & `kmerator-0.8.2b0/setup.py`

 * *Files identical despite different names*

