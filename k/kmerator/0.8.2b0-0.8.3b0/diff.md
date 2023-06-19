# Comparing `tmp/kmerator-0.8.2b0.tar.gz` & `tmp/kmerator-0.8.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerator-0.8.2b0.tar", last modified: Mon Jun 19 12:58:10 2023, max compression
+gzip compressed data, was "kmerator-0.8.3b0.tar", last modified: Mon Jun 19 13:20:48 2023, max compression
```

## Comparing `kmerator-0.8.2b0.tar` & `kmerator-0.8.3b0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-19 12:58:10.619572 kmerator-0.8.2b0/
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.8.2b0/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-19 12:58:10.616210 kmerator-0.8.2b0/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11626 2023-06-15 12:20:25.000000 kmerator-0.8.2b0/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-19 12:58:10.493702 kmerator-0.8.2b0/kmerator/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.8.2b0/kmerator/__init__.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.8.2b0/kmerator/color.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.8.2b0/kmerator/config.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19683 2023-05-16 08:28:01.000000 kmerator-0.8.2b0/kmerator/dataset.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.8.2b0/kmerator/exit.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-06-19 12:54:05.000000 kmerator-0.8.2b0/kmerator/info.py
--rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    11984 2023-06-15 12:31:45.000000 kmerator-0.8.2b0/kmerator/kmerator.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    18699 2023-06-19 12:33:32.000000 kmerator-0.8.2b0/kmerator/kmerize.py
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.8.2b0/kmerator/longest_transcript.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.8.2b0/kmerator/mk_geneinfo.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.8.2b0/kmerator/mk_transcriptome.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    12678 2023-06-19 12:52:43.000000 kmerator-0.8.2b0/kmerator/options.py
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-19 12:58:10.599860 kmerator-0.8.2b0/kmerator.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/requires.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-06-19 12:58:10.000000 kmerator-0.8.2b0/kmerator.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-06-19 12:58:10.622067 kmerator-0.8.2b0/setup.cfg
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1109 2023-06-15 12:34:30.000000 kmerator-0.8.2b0/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-19 13:20:48.153756 kmerator-0.8.3b0/
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.8.3b0/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-19 13:20:48.149656 kmerator-0.8.3b0/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11626 2023-06-15 12:20:25.000000 kmerator-0.8.3b0/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-19 13:20:48.047197 kmerator-0.8.3b0/kmerator/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.8.3b0/kmerator/__init__.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.8.3b0/kmerator/color.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.8.3b0/kmerator/config.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19683 2023-05-16 08:28:01.000000 kmerator-0.8.3b0/kmerator/dataset.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.8.3b0/kmerator/exit.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-06-19 13:16:24.000000 kmerator-0.8.3b0/kmerator/info.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    11984 2023-06-15 12:31:45.000000 kmerator-0.8.3b0/kmerator/kmerator.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    18699 2023-06-19 12:33:32.000000 kmerator-0.8.3b0/kmerator/kmerize.py
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.8.3b0/kmerator/longest_transcript.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.8.3b0/kmerator/mk_geneinfo.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.8.3b0/kmerator/mk_transcriptome.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    12706 2023-06-19 13:15:40.000000 kmerator-0.8.3b0/kmerator/options.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-19 13:20:48.133468 kmerator-0.8.3b0/kmerator.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-19 13:20:47.000000 kmerator-0.8.3b0/kmerator.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-06-19 13:20:47.000000 kmerator-0.8.3b0/kmerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-06-19 13:20:47.000000 kmerator-0.8.3b0/kmerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-06-19 13:20:47.000000 kmerator-0.8.3b0/kmerator.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-06-19 13:20:47.000000 kmerator-0.8.3b0/kmerator.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-06-19 13:20:47.000000 kmerator-0.8.3b0/kmerator.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-06-19 13:20:48.156279 kmerator-0.8.3b0/setup.cfg
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1109 2023-06-15 12:34:30.000000 kmerator-0.8.3b0/setup.py
```

### Comparing `kmerator-0.8.2b0/PKG-INFO` & `kmerator-0.8.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.8.2b0
+Version: 0.8.3b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.8.2b0/README.md` & `kmerator-0.8.3b0/README.md`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.2b0/kmerator/config.py` & `kmerator-0.8.3b0/kmerator/config.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.2b0/kmerator/dataset.py` & `kmerator-0.8.3b0/kmerator/dataset.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.2b0/kmerator/info.py` & `kmerator-0.8.3b0/kmerator/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Genral informations on to the program.
 """
 
 APPNAME = "kmerator"
 SHORTDESC = "Find specific gene or transcript kmers. And more."
 LICENCE = "GPL3"
-VERSION = "0.8.2-beta"
+VERSION = "0.8.3-beta"
 AUTHOR = 'Sébastien RIQUIER, IRMB, Montpellier'
 AUTHOR_EMAIL = "sebastien.riquier@ucd.ie"
 CONTIBUTORS = [
     'Chloe BESSIERE chloe.bessiere@inserm.fr>'
     'Benoit GUIBERT <benoit.guibert@inserm.fr>',
 ]
 DOC = f"""
```

### Comparing `kmerator-0.8.2b0/kmerator/kmerator.py` & `kmerator-0.8.3b0/kmerator/kmerator.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.2b0/kmerator/kmerize.py` & `kmerator-0.8.3b0/kmerator/kmerize.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.2b0/kmerator/longest_transcript.py` & `kmerator-0.8.3b0/kmerator/longest_transcript.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.2b0/kmerator/mk_geneinfo.py` & `kmerator-0.8.3b0/kmerator/mk_geneinfo.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.2b0/kmerator/mk_transcriptome.py` & `kmerator-0.8.3b0/kmerator/mk_transcriptome.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.8.2b0/kmerator/options.py` & `kmerator-0.8.3b0/kmerator/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,19 +211,20 @@
     if not os.path.isdir(args.datadir):
         sys.exit(f"{ERROR}Error: {args.datadir!r} not found or not a directory.{ENDCOL}")
     if not os.access(args.datadir, os.R_OK) or not os.access(args.datadir, os.X_OK):
         sys.exit(f"{ERROR}Error: insufficient rights in {args.datadir!r}.{ENDCOL}")
     ### --fasta-file - check if query fasta file is present
     if args.fasta_file and not os.path.isfile(args.fasta_file):
         sys.exit(f"{ERROR}Error: {args.fasta_file!r} not found.{ENDCOL}")
-    check_fasta_file(args)
     ### --fasta-file - Check query fasta file extension
     if args.fasta_file and args.fasta_file.split('.')[-1] not in ("fa", "fasta"):
         sys.exit(f" {ERROR}Error: {os.path.basename(args.fasta_file)} " \
                 f"Does not appears to be a fasta file.{ENDCOL}")
+    if args.fasta_file:
+        check_fasta_file(args)
     ### --selection - Check Gene Select option
     if args.selection:
         for gene in args.selection:
             if gene.startswith('ENS') and '.' in gene:
                 sys.exit(f"{ERROR}ENSEMBL annotations with version (point) like "
                         f"ENSTXXXXXXXX.1 is forbidden, just remove the '.1'."
                         )
```

### Comparing `kmerator-0.8.2b0/kmerator.egg-info/PKG-INFO` & `kmerator-0.8.3b0/kmerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.8.2b0
+Version: 0.8.3b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
```

### Comparing `kmerator-0.8.2b0/setup.py` & `kmerator-0.8.3b0/setup.py`

 * *Files identical despite different names*

