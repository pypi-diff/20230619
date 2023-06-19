# Comparing `tmp/pyrodigal-2.1.0.tar.gz` & `tmp/pyrodigal-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrodigal-2.1.0.tar", last modified: Tue Feb 21 10:55:09 2023, max compression
+gzip compressed data, was "pyrodigal-2.2.0.tar", last modified: Mon Jun 19 20:04:51 2023, max compression
```

## Comparing `pyrodigal-2.1.0.tar` & `pyrodigal-2.2.0.tar`

### file list

```diff
@@ -1,177 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.502482 pyrodigal-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17260 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-02-21 10:55:09.502482 pyrodigal-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-21 10:55:09.000000 pyrodigal-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.442481 pyrodigal-2.1.0/pyrodigal/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/_connection.h
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/_connection.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/_pyrodigal.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/_pyrodigal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   197046 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/_pyrodigal.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/_sequence.h
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/_sequence.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/_unicode.pxd
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.442481 pyrodigal-2.1.0/pyrodigal/cpu_features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/cpu_features/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/cpu_features/aarch64.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/cpu_features/arm.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/cpu_features/x86.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.446482 pyrodigal-2.1.0/pyrodigal/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/avx.c
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/avx.h
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/avx.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/generic.c
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/generic.h
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/generic.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/mmx.c
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/mmx.h
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/mmx.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/neon.c
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/neon.h
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/neon.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/sse.c
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/sse.h
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/sse.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/impl/template.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.446482 pyrodigal-2.1.0/pyrodigal/prodigal/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/prodigal/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/prodigal/bitmap.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/prodigal/dprog.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/prodigal/gene.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/prodigal/metagenomic.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/prodigal/node.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/prodigal/sequence.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/prodigal/training.pxd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.450482 pyrodigal-2.1.0/pyrodigal/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.458482 pyrodigal-2.1.0/pyrodigal/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   737378 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/GCF_001457455.1_NCTC11397_genomic.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)   558392 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/GCF_001457455.1_NCTC11397_genomic.tinf_closed.bin
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.meta+mask.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.meta.faa.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.meta.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.single.faa.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.single.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)    89413 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.faa.gz
--rw-r--r--   0 runner    (1001) docker     (123)   139037 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)    87775 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.meta+mask.faa.gz
--rw-r--r--   0 runner    (1001) docker     (123)   129127 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.meta+mask.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)    89491 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.meta.faa.gz
--rw-r--r--   0 runner    (1001) docker     (123)   132891 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.meta.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)    90959 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.single.faa.gz
--rw-r--r--   0 runner    (1001) docker     (123)   134986 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.single.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)    23514 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.meta.faa.gz
--rw-r--r--   0 runner    (1001) docker     (123)    22885 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.meta.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.meta.gff
--rw-r--r--   0 runner    (1001) docker     (123)   169907 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.meta.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.single.faa.gz
--rw-r--r--   0 runner    (1001) docker     (123)    23382 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.single.fna.gz
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.training.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/test_connection_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/test_gene.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/test_genes.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/test_orf_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/pyrodigal/tests/test_training_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.442481 pyrodigal-2.1.0/pyrodigal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-02-21 10:55:09.000000 pyrodigal-2.1.0/pyrodigal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-02-21 10:55:09.000000 pyrodigal-2.1.0/pyrodigal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 10:55:09.000000 pyrodigal-2.1.0/pyrodigal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-21 10:55:09.000000 pyrodigal-2.1.0/pyrodigal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 10:55:09.000000 pyrodigal-2.1.0/pyrodigal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-21 10:55:09.000000 pyrodigal-2.1.0/pyrodigal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-02-21 10:55:09.502482 pyrodigal-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    25857 2023-02-21 10:54:53.000000 pyrodigal-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.434481 pyrodigal-2.1.0/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.494482 pyrodigal-2.1.0/vendor/Prodigal/
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/bitmap.c
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/bitmap.h
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/dprog.c
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/dprog.h
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/fptr.h
--rw-r--r--   0 runner    (1001) docker     (123)    20587 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/gene.c
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/gene.h
--rw-r--r--   0 runner    (1001) docker     (123)    27933 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/main.c
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/metagenomic.c
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/metagenomic.h
--rw-r--r--   0 runner    (1001) docker     (123)    60473 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/node.c
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/node.h
--rw-r--r--   0 runner    (1001) docker     (123)    27652 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/sequence.c
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/sequence.h
--rw-r--r--   0 runner    (1001) docker     (123) 25752586 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/training.c
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-02-21 10:54:55.000000 pyrodigal-2.1.0/vendor/Prodigal/training.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.494482 pyrodigal-2.1.0/vendor/cpu_features/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.494482 pyrodigal-2.1.0/vendor/cpu_features/ci/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/ci/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.494482 pyrodigal-2.1.0/vendor/cpu_features/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/cmake/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.494482 pyrodigal-2.1.0/vendor/cpu_features/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/cpu_features_cache_info.h
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/cpu_features_macros.h
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/cpuinfo_aarch64.h
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/cpuinfo_arm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/cpuinfo_mips.h
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/cpuinfo_ppc.h
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/cpuinfo_x86.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.498482 pyrodigal-2.1.0/vendor/cpu_features/include/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/internal/bit_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/internal/cpuid_x86.h
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/internal/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/internal/hwcaps.h
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/internal/stack_line_reader.h
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/include/internal/string_view.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.498482 pyrodigal-2.1.0/vendor/cpu_features/ndk_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/ndk_compat/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/ndk_compat/cpu-features.c
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/ndk_compat/cpu-features.h
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/ndk_compat/ndk-compat-test.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.502482 pyrodigal-2.1.0/vendor/cpu_features/src/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/copy.inl
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/define_introspection.inl
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/define_introspection_and_hwcaps.inl
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/equals.inl
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/filesystem.c
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/hwcaps.c
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/impl_aarch64_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/impl_arm_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/impl_mips_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/impl_ppc_linux.c
--rw-r--r--   0 runner    (1001) docker     (123)    76257 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/impl_x86__base_implementation.inl
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/impl_x86_freebsd.c
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/impl_x86_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/impl_x86_macos.c
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/impl_x86_windows.c
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/stack_line_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/string_view.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.502482 pyrodigal-2.1.0/vendor/cpu_features/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/src/utils/list_cpu_features.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:55:09.502482 pyrodigal-2.1.0/vendor/cpu_features/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/test/filesystem_for_testing.h
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-02-21 10:54:57.000000 pyrodigal-2.1.0/vendor/cpu_features/test/hwcaps_for_testing.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.160326 pyrodigal-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-19 20:04:51.160326 pyrodigal-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-19 20:04:50.000000 pyrodigal-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.104325 pyrodigal-2.2.0/pyrodigal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/_connection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/_connection.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/_pyrodigal.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/_pyrodigal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   197223 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/_pyrodigal.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/_sequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/_sequence.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/_unicode.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.108325 pyrodigal-2.2.0/pyrodigal/cpu_features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/cpu_features/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/cpu_features/aarch64.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/cpu_features/arm.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/cpu_features/x86.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.108325 pyrodigal-2.2.0/pyrodigal/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/avx.c
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/avx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/avx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/generic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/generic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/generic.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/mmx.c
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/mmx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/mmx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/neon.h
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/neon.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/sse.c
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/sse.h
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/sse.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/impl/template.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.112325 pyrodigal-2.2.0/pyrodigal/prodigal/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/prodigal/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/prodigal/bitmap.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/prodigal/dprog.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/prodigal/gene.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/prodigal/metagenomic.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/prodigal/node.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/prodigal/sequence.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/prodigal/training.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.112325 pyrodigal-2.2.0/pyrodigal/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.120325 pyrodigal-2.2.0/pyrodigal/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   737378 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/GCF_001457455.1_NCTC11397_genomic.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   558392 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/GCF_001457455.1_NCTC11397_genomic.tinf_closed.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.meta+mask.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.meta.faa.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.meta.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.single.faa.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.single.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    89413 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.faa.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   139037 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    87775 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.meta+mask.faa.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   129127 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.meta+mask.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    89491 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.meta.faa.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   132891 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.meta.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    90959 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.single.faa.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   134986 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.single.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    23514 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.meta.faa.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    22885 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.meta.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.meta.gff
+-rw-r--r--   0 runner    (1001) docker     (123)   169907 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.meta.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.single.faa.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    23382 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.single.fna.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.training.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/test_connection_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/test_gene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/test_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/test_orf_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/pyrodigal/tests/test_training_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.108325 pyrodigal-2.2.0/pyrodigal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-19 20:04:51.000000 pyrodigal-2.2.0/pyrodigal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-19 20:04:51.000000 pyrodigal-2.2.0/pyrodigal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:04:51.000000 pyrodigal-2.2.0/pyrodigal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-19 20:04:51.000000 pyrodigal-2.2.0/pyrodigal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:04:51.000000 pyrodigal-2.2.0/pyrodigal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 20:04:51.000000 pyrodigal-2.2.0/pyrodigal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 20:04:51.000000 pyrodigal-2.2.0/pyrodigal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-19 20:04:51.160326 pyrodigal-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    25826 2023-06-19 20:04:35.000000 pyrodigal-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.100325 pyrodigal-2.2.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:04:51.160326 pyrodigal-2.2.0/vendor/Prodigal/
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/bitmap.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/bitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/dprog.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/dprog.h
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/fptr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20587 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/gene.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/gene.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27933 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/metagenomic.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/metagenomic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60473 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/node.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/node.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27652 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/sequence.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/sequence.h
+-rw-r--r--   0 runner    (1001) docker     (123) 25752586 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/training.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-06-19 20:04:36.000000 pyrodigal-2.2.0/vendor/Prodigal/training.h
```

### Comparing `pyrodigal-2.1.0/CHANGELOG.md` & `pyrodigal-2.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,29 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/pyrodigal/compare/v2.1.0...HEAD
+[Unreleased]: https://github.com/althonos/pyrodigal/compare/v2.2.0...HEAD
+
+
+## [v2.2.0] - 2023-06-19
+[v2.2.0]: https://github.com/althonos/pyrodigal/compare/v2.1.0...v2.2.0
+
+### Changed
+- Release GIL while masking sequence regions in `Sequence.__init__`.
+- Use [`archspec`](https://pypi.org/project/archspec) instead of `cpu_features` for runtime feature detection.
+
+### Added
+- CLI flag to run ORF detection in parallel when input contains several contigs.
+
+### Removed
+- Support for Python 3.5.
 
 
 ## [v2.1.0] - 2023-02-20
 [v2.1.0]: https://github.com/althonos/pyrodigal/compare/v2.0.4...v2.1.0
 
 ### Changed
 - Update Prodigal to `v2.6.3+c1e2d36` to fix a bug with Shine-Dalgarno detection on reverse contig edge ([hyattpd/Prodigal#100](https://github.com/hyattpd/Prodigal/pull/100)).
```

### Comparing `pyrodigal-2.1.0/CITATION.cff` & `pyrodigal-2.2.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/CONTRIBUTING.md` & `pyrodigal-2.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/COPYING` & `pyrodigal-2.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/PKG-INFO` & `pyrodigal-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrodigal
-Version: 2.1.0
+Version: 2.2.0
 Summary: Cython bindings and Python interface to Prodigal, an ORF finder for genomes and metagenomes.
 Home-page: https://github.com/althonos/pyrodigal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pyrodigal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyrodigal/issues
@@ -18,28 +18,28 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: isal
 License-File: COPYING
 
 # 🔥 Pyrodigal [![Stars](https://img.shields.io/github/stars/althonos/pyrodigal.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pyrodigal/stargazers)
 
 *Cython bindings and Python interface to [Prodigal](https://github.com/hyattpd/Prodigal/), an ORF
 finder for genomes and metagenomes. **Now with SIMD!***
 
@@ -265,15 +265,14 @@
 in the [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) format.
 
 
 ## ⚖️ License
 
 This library is provided under the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/).
 The Prodigal code was written by [Doug Hyatt](https://github.com/hyattpd) and is distributed under the
-terms of the GPLv3 as well. See `vendor/Prodigal/LICENSE` for more information. The `cpu_features` library was written by [Guillaume Chatelet](https://github.com/gchatelet) and is
-licensed under the terms of the [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/). See `vendor/cpu_features/LICENSE` for more information.
+terms of the GPLv3 as well. See `vendor/Prodigal/LICENSE` for more information.
 
 *This project is in no way not affiliated, sponsored, or otherwise endorsed
 by the [original Prodigal authors](https://github.com/hyattpd). It was developed
 by [Martin Larralde](https://github.com/althonos/) during his PhD project
 at the [European Molecular Biology Laboratory](https://www.embl.de/) in
 the [Zeller team](https://github.com/zellerlab).*
```

### Comparing `pyrodigal-2.1.0/README.md` & `pyrodigal-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,14 @@
 in the [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) format.
 
 
 ## ⚖️ License
 
 This library is provided under the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/).
 The Prodigal code was written by [Doug Hyatt](https://github.com/hyattpd) and is distributed under the
-terms of the GPLv3 as well. See `vendor/Prodigal/LICENSE` for more information. The `cpu_features` library was written by [Guillaume Chatelet](https://github.com/gchatelet) and is
-licensed under the terms of the [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/). See `vendor/cpu_features/LICENSE` for more information.
+terms of the GPLv3 as well. See `vendor/Prodigal/LICENSE` for more information.
 
 *This project is in no way not affiliated, sponsored, or otherwise endorsed
 by the [original Prodigal authors](https://github.com/hyattpd). It was developed
 by [Martin Larralde](https://github.com/althonos/) during his PhD project
 at the [European Molecular Biology Laboratory](https://www.embl.de/) in
 the [Zeller team](https://github.com/zellerlab).*
```

### Comparing `pyrodigal-2.1.0/pyrodigal/__init__.py` & `pyrodigal-2.2.0/pyrodigal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/_connection.h` & `pyrodigal-2.2.0/pyrodigal/_connection.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/_connection.pxd` & `pyrodigal-2.2.0/pyrodigal/_connection.pxd`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/_pyrodigal.pxd` & `pyrodigal-2.2.0/pyrodigal/_pyrodigal.pxd`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/_pyrodigal.pyi` & `pyrodigal-2.2.0/pyrodigal/_pyrodigal.pyi`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/_pyrodigal.pyx` & `pyrodigal-2.2.0/pyrodigal/_pyrodigal.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -138,16 +138,29 @@
 
 import array
 import itertools
 import textwrap
 import threading
 import warnings
 
+import archspec.cpu
+
 include "_version.py"
 
+# --- Patch for PyPy 3.9 -----------------------------------------------------
+
+IF not HAS_PYINTERPRETERSTATE_GETID:
+    cdef extern from *:
+        """
+        int64_t PyInterpreterState_GetID(PyInterpreterState *interp) {
+            return 0;
+        }
+        """
+
+
 # --- Module-level constants -------------------------------------------------
 
 cdef size_t MIN_MASKS_ALLOC      = 8
 cdef size_t MIN_GENES_ALLOC      = 8
 cdef size_t MIN_NODES_ALLOC      = 8 * MIN_GENES_ALLOC
 cdef int    _IDEAL_SINGLE_GENOME = 100000
 cdef int    _MIN_SINGLE_GENOME   = 20000
@@ -545,20 +558,21 @@
                     data,
                     self.slen,
                     &self.gc,
                     self.digits,
                 )
 
         if mask:
-            Sequence._mask(
-                self.digits,
-                self.slen,
-                self.masks,
-                mask_size,
-            )
+            with nogil:
+                Sequence._mask(
+                    self.digits,
+                    self.slen,
+                    self.masks,
+                    mask_size,
+                )
 
     def __dealloc__(self):
         PyMem_Free(self.digits)
 
     def __len__(self):
         """__len__(self)\n--
 
@@ -1065,37 +1079,34 @@
 
         return phase
 
 
 # --- Connection Scorer ------------------------------------------------------
 
 _TARGET_CPU           = TARGET_CPU
+_HOST_CPU             = archspec.cpu.host()
 _AVX2_RUNTIME_SUPPORT = False
 _NEON_RUNTIME_SUPPORT = False
 _SSE2_RUNTIME_SUPPORT = False
 _MMX_RUNTIME_SUPPORT  = False
 _AVX2_BUILD_SUPPORT   = False
 _NEON_BUILD_SUPPORT   = False
 _SSE2_BUILD_SUPPORT   = False
 _MMX_BUILD_SUPPORT    = False
 
 IF TARGET_CPU == "x86" and TARGET_SYSTEM in ("freebsd", "linux_or_android", "macos", "windows"):
-    from pyrodigal.cpu_features.x86 cimport GetX86Info, X86Info
-    cdef X86Info cpu_info = GetX86Info()
     _MMX_BUILD_SUPPORT    = MMX_BUILD_SUPPORT
     _SSE2_BUILD_SUPPORT   = SSE2_BUILD_SUPPORT
     _AVX2_BUILD_SUPPORT   = AVX2_BUILD_SUPPORT
-    _MMX_RUNTIME_SUPPORT  = cpu_info.features.mmx  != 0
-    _SSE2_RUNTIME_SUPPORT = cpu_info.features.sse2 != 0
-    _AVX2_RUNTIME_SUPPORT = cpu_info.features.avx2 != 0
+    _MMX_RUNTIME_SUPPORT  = "mmx" in _HOST_CPU.features
+    _SSE2_RUNTIME_SUPPORT = "sse2" in _HOST_CPU.features
+    _AVX2_RUNTIME_SUPPORT = "avx2" in _HOST_CPU.features
 ELIF TARGET_CPU == "arm" and TARGET_SYSTEM == "linux_or_android":
-    from pyrodigal.cpu_features.arm cimport GetArmInfo, ArmInfo
-    cdef ArmInfo cpu_info = GetArmInfo()
     _NEON_BUILD_SUPPORT   = NEON_BUILD_SUPPORT
-    _NEON_RUNTIME_SUPPORT = cpu_info.features.neon != 0
+    _NEON_RUNTIME_SUPPORT = "neon" in _HOST_CPU.features
 ELIF TARGET_CPU == "aarch64":
     _NEON_BUILD_SUPPORT   = NEON_BUILD_SUPPORT
     _NEON_RUNTIME_SUPPORT = NEON_BUILD_SUPPORT
 
 cdef enum simd_backend:
     NONE = 0
     MMX = 1
@@ -3464,15 +3475,15 @@
             width (`int`): The width to use to wrap sequence lines. Prodigal
                 uses 70 for nucleotide sequences.
 
         Returns:
             `int`: The number of bytes written to the file.
 
         .. versionchanged:: 2.0.0
-            Replaced optional``prefix`` argument with ``sequence_id``.
+            Replaced optional ``prefix`` argument with ``sequence_id``.
 
         """
         cdef Gene    gene
         cdef int     i
         cdef ssize_t n    = 0
 
         for i, gene in enumerate(self):
```

### Comparing `pyrodigal-2.1.0/pyrodigal/_sequence.h` & `pyrodigal-2.2.0/pyrodigal/_sequence.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/_sequence.pxd` & `pyrodigal-2.2.0/pyrodigal/_sequence.pxd`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/_unicode.pxd` & `pyrodigal-2.2.0/pyrodigal/_unicode.pxd`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/cli.py` & `pyrodigal-2.2.0/pyrodigal/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """The Pyrodigal CLI, emulating the original Prodigal command line.
 """
 
 import argparse
 import contextlib
 import sys
 import os
+import multiprocessing.pool
 
 from . import __name__, __author__, __version__
 from ._pyrodigal import TRANSLATION_TABLES, OrfFinder, TrainingInfo
 from .tests.fasta import parse
 
 
 def argument_parser():
@@ -86,14 +87,23 @@
     parser.add_argument(
         "-t",
         required=False,
         metavar="training_file",
         help="Write a training file (if none exists); otherwise, read and use the specified training file.",
     )
     parser.add_argument(
+        "-j",
+        "--jobs",
+        type=int,
+        required=False,
+        default=1,
+        metavar="jobs",
+        help="The number of threads to use if input contains multiple sequences."
+    )
+    parser.add_argument(
         "-h", "--help", action="help", help="Show this help message and exit."
     )
     parser.add_argument(
         "-V",
         "--version",
         help="Show version number and exit.",
         action="version",
@@ -152,55 +162,65 @@
                         training_info = TrainingInfo.load(f)
                 else:
                     training_info = None
             else:
                 training_info = None
 
             # initialize the ORF finder
-            pyrodigal = OrfFinder(
+            orf_finder = OrfFinder(
                 meta=args.p == "meta",
                 closed=args.c,
                 mask=args.m,
                 training_info=training_info,
                 min_gene=args.min_gene,
                 min_edge_gene=args.min_edge_gene,
                 max_overlap=args.max_overlap,
             )
 
             # pre-train if in training mode
             if args.p == "single":
                 # use the same interleaving logic as Prodigal
                 sequences = list(parse(args.i))
-                training_info = pyrodigal.train(
+                training_info = orf_finder.train(
                     *(seq.seq for seq in sequences),
                     force_nonsd=args.n,
                     translation_table=args.g
                 )
                 # save the training info is desired
                 if args.t is not None and not os.path.exists(args.t):
                     with open(args.t, "wb") as f:
                         training_info.dump(f)
             else:
                 sequences = parse(args.i)
 
-            # find genes
-            for i, seq in enumerate(sequences):
-                # find genes with Pyrodigal
-                preds = pyrodigal.find_genes(seq.seq)
+            # get the number of jobs
+            if args.jobs == 0:
+                args.jobs = os.cpu_count() or 1
+            if args.jobs > 1:
+                pool = ctx.enter_context(multiprocessing.pool.ThreadPool(args.jobs))
+                parallel_map = pool.map
+            else:
+                parallel_map = map
+
+            # find genes in parallel
+            def process(sequence):
+                return (sequence.id, orf_finder.find_genes(sequence.seq))
+
+            for seq_id, preds in parallel_map(process, sequences):
                 # write output in GFF format
                 if args.f == "gff":
-                    preds.write_gff(out_file, seq.id)
+                    preds.write_gff(out_file, seq_id)
                 # if asked, write nucleotide sequences of genes
                 if nuc_file is not None:
-                    preds.write_genes(nuc_file, seq.id)
+                    preds.write_genes(nuc_file, seq_id)
                 # if asked, write amino acide sequences of proteins
                 if prot_file is not None:
-                    preds.write_translations(prot_file, seq.id)
+                    preds.write_translations(prot_file, seq_id)
                 # if asked, write scores
                 if scores_file is not None:
-                    preds.write_scores(scores_file, seq.id)
+                    preds.write_scores(scores_file, seq_id)
 
         except Exception as err:
             print("Error: {}".format(err))
             return getattr(err, "errno", 1)
         else:
             return 0
```

### Comparing `pyrodigal-2.1.0/pyrodigal/cpu_features/aarch64.pxd` & `pyrodigal-2.2.0/pyrodigal/cpu_features/aarch64.pxd`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/cpu_features/arm.pxd` & `pyrodigal-2.2.0/pyrodigal/cpu_features/arm.pxd`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/impl/avx.c` & `pyrodigal-2.2.0/pyrodigal/impl/avx.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/impl/generic.h` & `pyrodigal-2.2.0/pyrodigal/impl/generic.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/impl/mmx.c` & `pyrodigal-2.2.0/pyrodigal/impl/mmx.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/impl/neon.c` & `pyrodigal-2.2.0/pyrodigal/impl/neon.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/impl/sse.c` & `pyrodigal-2.2.0/pyrodigal/impl/sse.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/impl/template.h` & `pyrodigal-2.2.0/pyrodigal/impl/template.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/prodigal/gene.pxd` & `pyrodigal-2.2.0/pyrodigal/prodigal/gene.pxd`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/prodigal/node.pxd` & `pyrodigal-2.2.0/pyrodigal/prodigal/node.pxd`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/prodigal/sequence.pxd` & `pyrodigal-2.2.0/pyrodigal/prodigal/sequence.pxd`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/__init__.py` & `pyrodigal-2.2.0/pyrodigal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/GCF_001457455.1_NCTC11397_genomic.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/GCF_001457455.1_NCTC11397_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/GCF_001457455.1_NCTC11397_genomic.tinf_closed.bin` & `pyrodigal-2.2.0/pyrodigal/tests/data/GCF_001457455.1_NCTC11397_genomic.tinf_closed.bin`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.meta+mask.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.meta+mask.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.meta.faa.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.meta.faa.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.meta.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.meta.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.single.faa.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.single.faa.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/KK037166.single.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/KK037166.single.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.faa.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.faa.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.meta+mask.faa.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.meta+mask.faa.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.meta+mask.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.meta+mask.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.meta.faa.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.meta.faa.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.meta.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.meta.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.single.faa.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.single.faa.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/MIIJ01000039.single.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/MIIJ01000039.single.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.meta.faa.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.meta.faa.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.meta.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.meta.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.meta.gff` & `pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.meta.gff`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.meta.tsv` & `pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.meta.tsv`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.single.faa.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.single.faa.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.single.fna.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.single.fna.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/SRR492066.training.bin.gz` & `pyrodigal-2.2.0/pyrodigal/tests/data/SRR492066.training.bin.gz`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/data/__init__.py` & `pyrodigal-2.2.0/pyrodigal/tests/data/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import contextlib
 import gzip
 import io
 
 try:
     try:
-        from importlib import resources
+        from importlib.resources import files
     except ImportError:
-        import importlib_resources as resources
+        from importlib_resources import files
 except ImportError:
-    resources = None
+    files = None
 
 from ..fasta import parse
 
 @contextlib.contextmanager
 def load(name, mode="rt"):
-     with resources.open_binary(__name__, name) as src:
+     with files(__name__).joinpath(name).open("rb") as src:
         if name.endswith(".gz"):
             src = gzip.open(src, mode=mode)
         elif mode != "rb":
             src = io.TextIOWrapper(src)
         yield src 
 
 def load_record(name):
```

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/test_connection_scorer.py` & `pyrodigal-2.2.0/pyrodigal/tests/test_connection_scorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,23 +51,23 @@
         self.assertEqual(n1.gc_cont, n2.gc_cont)
         self.assertAlmostEqual(n1.score, n2.score)
         self.assertAlmostEqual(n1.cscore, n2.cscore)
         self.assertAlmostEqual(n1.rscore, n2.rscore)
         self.assertAlmostEqual(n1.sscore, n2.sscore)
         self.assertAlmostEqual(n1.tscore, n2.tscore)
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_score_connections_final(self):
         record = data.load_record("MIIJ01000039.fna.gz")
         nodes_expected = scored_nodes(record, final=True, backend=None)
         nodes_actual = scored_nodes(record, final=True, backend=self.backend)
         for n1, n2 in zip(nodes_expected, nodes_actual):
             self.assertNodeEqual(n1, n2)
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_score_connections_train(self):
         record = data.load_record("GCF_001457455.1_NCTC11397_genomic.fna.gz")
         nodes_expected = scored_nodes(record, final=False, backend=None)
         nodes_actual = scored_nodes(record, final=False, backend=self.backend)
         for n1, n2 in zip(nodes_expected, nodes_actual):
             self.assertNodeEqual(n1, n2)
```

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/test_doctest.py` & `pyrodigal-2.2.0/pyrodigal/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/test_gene.py` & `pyrodigal-2.2.0/pyrodigal/tests/test_gene.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import unittest
 import warnings
 
 from .. import OrfFinder
 from . import data
 
 
-@unittest.skipUnless(data.resources, "importlib.resources not available")
+@unittest.skipUnless(data.files, "importlib.resources not available")
 class TestGene(unittest.TestCase):
     @classmethod
     def find_genes(cls, seq):
         p = OrfFinder(meta=True)
         return p.find_genes(seq)
 
     @classmethod
```

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/test_genes.py` & `pyrodigal-2.2.0/pyrodigal/tests/test_genes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import unittest
 import pickle
 
 from .. import OrfFinder, METAGENOMIC_BINS
 from . import data
 
 
-@unittest.skipUnless(data.resources, "importlib.resources not available")
+@unittest.skipUnless(data.files, "importlib.resources not available")
 class TestGenes(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.record = data.load_record("SRR492066.fna.gz")
         cls.p = OrfFinder(meta=True)
         cls.genes = cls.p.find_genes(str(cls.record.seq))
```

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/test_mask.py` & `pyrodigal-2.2.0/pyrodigal/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/test_nodes.py` & `pyrodigal-2.2.0/pyrodigal/tests/test_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
         self.assertEqual(n1.cscore, n2.cscore, "cscores differ")
         self.assertEqual(n1.gc_cont, n2.gc_cont, "GC contents differ")
         self.assertEqual(n1.score, n2.score, "GC contents differ")
         self.assertEqual(n1.rscore, n2.rscore, "rscores differ")
         self.assertEqual(n1.sscore, n2.sscore, "sscores differ")
         self.assertEqual(n1.tscore, n2.tscore, "tscores differ")
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_add_nodes_metagenomic_bins(self):
         record = data.load_record("SRR492066.fna.gz")
         seq = Sequence(record.seq)
         nodes = Nodes()
         # nodes should start empty
         self.assertEqual(len(nodes), 0)
         # numbers below obtained directly in Prodigal by `printf`-ing the
         # node numbers on a normal run
         for bin, expected in [(0, 2970), (2, 2970), (11, 2293), (24, 2293)]:
             tt = METAGENOMIC_BINS[bin].training_info.translation_table
             self.assertEqual(nodes.extract(seq, translation_table=tt), expected)
             self.assertEqual(len(nodes), expected)
             nodes.clear()
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_copy(self):
         record = data.load_record("SRR492066.fna.gz")
         tt = METAGENOMIC_BINS[0].training_info.translation_table
         seq = Sequence(record.seq)
         nodes1 = Nodes()
         nodes1.extract(seq, translation_table=tt)
         nodes2 = nodes1.copy()
@@ -53,15 +53,15 @@
 
     def test_copy_empty(self):
         nodes = Nodes()
         copy = nodes.copy()
         self.assertEqual(len(nodes), 0)
         self.assertEqual(len(copy), 0)
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_pickle(self):
         record = data.load_record("SRR492066.fna.gz")
         tt = METAGENOMIC_BINS[0].training_info.translation_table
         seq = Sequence(record.seq)
         nodes1 = Nodes()
         nodes1.extract(seq, translation_table=tt)
         nodes2 = pickle.loads(pickle.dumps(nodes1))
```

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/test_orf_finder.py` & `pyrodigal-2.2.0/pyrodigal/tests/test_orf_finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,35 +95,35 @@
         self.assertStartTypesEqual(predictions, proteins)
         self.assertRbsSpacersEqual(predictions, proteins)
         self.assertGCContentEqual(predictions, proteins)
         self.assertGeneDataEqual(predictions, proteins)
 
 
 class _TestMode(_OrfFinderTestCase):
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_find_genes_KK037166(self):
         record = data.load_record("KK037166.fna.gz")
         proteins = data.load_records("KK037166.{}.faa.gz".format(self.mode))
         genes = data.load_records("KK037166.{}.fna.gz".format(self.mode))
 
         preds = self.find_genes(self.get_sequence(record))
         self.assertGenesEqual(preds, genes)
         self.assertPredictionsEqual(preds, proteins)
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_find_genes_SRR492066(self):
         record = data.load_record("SRR492066.fna.gz")
         proteins = data.load_records("SRR492066.{}.faa.gz".format(self.mode))
         genes = data.load_records("SRR492066.{}.fna.gz".format(self.mode))
 
         preds = self.find_genes(self.get_sequence(record))
         self.assertGenesEqual(preds, genes)
         self.assertPredictionsEqual(preds, proteins)
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_find_genes_MIIJ01000039(self):
         record = data.load_record("MIIJ01000039.fna.gz")
         proteins = data.load_records("MIIJ01000039.{}.faa.gz".format(self.mode))
         genes = data.load_records("MIIJ01000039.{}.fna.gz".format(self.mode))
 
         preds = self.find_genes(self.get_sequence(record))
         self.assertGenesEqual(preds, genes)
@@ -185,15 +185,15 @@
         self.assertRaises(ValueError, OrfFinder, max_overlap=-1)
 
     def test_invalid_min_gene(self):
         self.assertRaises(ValueError, OrfFinder, min_gene=-1)
 
 
 class TestMeta(_OrfFinderTestCase, unittest.TestCase):
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_train(self):
         record = data.load_record("SRR492066.fna.gz")
         p = OrfFinder(meta=True)
         self.assertRaises(RuntimeError, p.train, str(record.seq))
 
     def test_overflow(self):
         # > 180195.SAMN03785337.LFLS01000089
@@ -229,37 +229,37 @@
 
     def test_empty_sequence(self):
         p = OrfFinder(meta=True)
         genes = p.find_genes("")
         self.assertEqual(len(genes), 0)
         self.assertRaises(StopIteration, next, iter(genes))
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_find_genes_masked_MIIJ01000039(self):
         record = data.load_record("MIIJ01000039.fna.gz")
         proteins = data.load_records("MIIJ01000039.{}.faa.gz".format("meta+mask"))
         genes = data.load_records("MIIJ01000039.{}.fna.gz".format("meta+mask"))
 
         orf_finder = OrfFinder(meta=True, mask=True)
         preds = orf_finder.find_genes(record.seq)
         self.assertEqual(len(preds.sequence.masks), 1)
         self.assertGenesEqual(preds, genes)
         self.assertPredictionsEqual(preds, proteins)
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_find_genes_large_minsize(self):
         record = data.load_record("KK037166.fna.gz")
         genes = data.load_records("KK037166.{}.fna.gz".format("meta+mask"))
         large_genes = [gene for gene in genes if len(gene.seq) >= 200]
 
         orf_finder = OrfFinder(meta=True, min_gene=200, min_edge_gene=200, mask=True)
         preds = orf_finder.find_genes(record.seq)
         self.assertEqual(len(preds), len(large_genes))
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_find_genes_small_minsize(self):
         record = data.load_record("KK037166.fna.gz")
         genes = data.load_records("KK037166.{}.fna.gz".format("meta+mask"))
 
         orf_finder = OrfFinder(
             meta=True, min_gene=30, min_edge_gene=20, max_overlap=20, mask=True
         )
@@ -296,15 +296,15 @@
             self.assertEqual(genes[0].end, 347)
             self.assertEqual(genes[1].start_type, "ATG")
             self.assertEqual(genes[1].begin, 426)
             self.assertEqual(genes[1].end, 590)
 
 
 class TestSingle(_OrfFinderTestCase, unittest.TestCase):
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_train_info(self):
         record = data.load_record("SRR492066.fna.gz")
         p = OrfFinder(meta=False)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             info = p.train(record.seq)
 
@@ -315,57 +315,57 @@
         self.assertEqual(info.bias[1], 0.17260535063729165)
         self.assertEqual(info.bias[2], 0.1503420711765898)
         self.assertEqual(info.type_weights[0], 0.71796361273324)
         self.assertEqual(info.type_weights[1], -1.3722361344058844)
         self.assertEqual(info.type_weights[2], -2.136731395763296)
         self.assertTrue(info.uses_sd)
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_train_not_called(self):
         record = data.load_record("SRR492066.fna.gz")
         p = OrfFinder(meta=False)
         self.assertRaises(RuntimeError, p.find_genes, str(record.seq))
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_training_info_deallocation(self):
         record = data.load_record("SRR492066.fna.gz")
         proteins = data.load_records("SRR492066.{}.faa.gz".format("single"))
         p = OrfFinder(meta=False)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             p.train(str(record.seq))
         genes = p.find_genes(str(record.seq))
         del p  # normally should not deallocate training info since it's RC
         self.assertEqual(genes[0].translate(), str(proteins[0].seq))
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_short_sequences(self):
         record = data.load_record("SRR492066.fna.gz")
         seq = "AATGTAGGAAAAACAGCATTTTCATTTCGCCATTTT"
         p = OrfFinder(meta=False)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             p.train(str(record.seq[:20000]))
         for i in range(1, len(seq)):
             genes = p.find_genes(seq[:i])
             self.assertEqual(len(genes), 0)
             self.assertRaises(StopIteration, next, iter(genes))
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_empty_sequence(self):
         record = data.load_record("SRR492066.fna.gz")
         p = OrfFinder(meta=False)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             p.train(str(record.seq[:20000]))
         genes = p.find_genes("")
         self.assertEqual(len(genes), 0)
         self.assertRaises(StopIteration, next, iter(genes))
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_pickle(self):
         record = data.load_record("SRR492066.fna.gz")
         # train separately
         p1 = OrfFinder(meta=False, min_gene=60)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             p1.train(str(record.seq[:20000]))
@@ -375,15 +375,15 @@
         g1 = p1.find_genes(record.seq)
         g2 = p2.find_genes(record.seq)
         # make sure genes are the same
         self.assertEqual(len(g1), len(g2))
         for gene1, gene2 in zip(g1, g2):
             self.assertGeneEqual(gene1, gene2)
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_training_info_pickle(self):
         record = data.load_record("SRR492066.fna.gz")
         # train separately
         p1 = OrfFinder(meta=False, min_gene=60)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             p1.train(str(record.seq[:20000]))
```

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/test_sequence.py` & `pyrodigal-2.2.0/pyrodigal/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/pyrodigal/tests/test_training_info.py` & `pyrodigal-2.2.0/pyrodigal/tests/test_training_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 dst.write(b"not ok\n")
             with open(filename, "rb") as src:
                 self.assertRaises(EOFError, TrainingInfo.load, src)
         finally:
             if os.path.exists(filename):
                 os.remove(filename)
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     def test_pickle(self):
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
             record = data.load_record("SRR492066.fna.gz")
             t1 = OrfFinder().train(record.seq)
         t2 = pickle.loads(pickle.dumps(t1))
         self.assertTrainingInfoEqual(t1, t2)
@@ -80,15 +80,15 @@
         with self.assertRaises(RuntimeError):
             t1.bias = (0.0, 0.0, 0.0)
         with self.assertRaises(RuntimeError):
             t1.gc = 0.50
         with self.assertRaises(RuntimeError):
             t1.uses_sd = False
 
-    @unittest.skipUnless(data.resources, "importlib.resources not available")
+    @unittest.skipUnless(data.files, "importlib.resources not available")
     @unittest.skipUnless(platform.machine() == "x86_64", "Reference training file was created on x86-64")
     @unittest.skipUnless(sys.platform == "linux", "Reference training file was created on Linux")
     def test_train_closed(self):
         records = data.load_records("GCF_001457455.1_NCTC11397_genomic.fna.gz")
         with data.load("GCF_001457455.1_NCTC11397_genomic.tinf_closed.bin", "rb") as f:
             expected = TrainingInfo.load(f)
         orf_finder = OrfFinder(closed=True)
```

### Comparing `pyrodigal-2.1.0/pyrodigal.egg-info/PKG-INFO` & `pyrodigal-2.2.0/pyrodigal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrodigal
-Version: 2.1.0
+Version: 2.2.0
 Summary: Cython bindings and Python interface to Prodigal, an ORF finder for genomes and metagenomes.
 Home-page: https://github.com/althonos/pyrodigal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pyrodigal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyrodigal/issues
@@ -18,28 +18,28 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: isal
 License-File: COPYING
 
 # 🔥 Pyrodigal [![Stars](https://img.shields.io/github/stars/althonos/pyrodigal.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pyrodigal/stargazers)
 
 *Cython bindings and Python interface to [Prodigal](https://github.com/hyattpd/Prodigal/), an ORF
 finder for genomes and metagenomes. **Now with SIMD!***
 
@@ -265,15 +265,14 @@
 in the [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) format.
 
 
 ## ⚖️ License
 
 This library is provided under the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/).
 The Prodigal code was written by [Doug Hyatt](https://github.com/hyattpd) and is distributed under the
-terms of the GPLv3 as well. See `vendor/Prodigal/LICENSE` for more information. The `cpu_features` library was written by [Guillaume Chatelet](https://github.com/gchatelet) and is
-licensed under the terms of the [Apache License 2.0](https://choosealicense.com/licenses/apache-2.0/). See `vendor/cpu_features/LICENSE` for more information.
+terms of the GPLv3 as well. See `vendor/Prodigal/LICENSE` for more information.
 
 *This project is in no way not affiliated, sponsored, or otherwise endorsed
 by the [original Prodigal authors](https://github.com/hyattpd). It was developed
 by [Martin Larralde](https://github.com/althonos/) during his PhD project
 at the [European Molecular Biology Laboratory](https://www.embl.de/) in
 the [Zeller team](https://github.com/zellerlab).*
```

### Comparing `pyrodigal-2.1.0/setup.cfg` & `pyrodigal-2.2.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 	Programming Language :: C
 	Programming Language :: Cython
-	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
@@ -39,21 +38,27 @@
 	Paper = https://doi.org/10.21105/joss.04296
 	PyPI = https://pypi.org/project/pyrodigal
 
 [options]
 zip_safe = false
 packages = pyrodigal, pyrodigal.tests, pyrodigal.tests.data
 include_package_data = true
-python_requires = >=3.5
+python_requires = >=3.6
 setup_requires = 
 	setuptools >=46.4
 	cython ~=0.29.16
+install_requires = 
+	archspec ~=0.2.0
 tests_require = 
 	importlib-resources ; python_version < '3.7'
 
+[options.extras_require]
+isal = 
+	isal ~=1.1
+
 [options.entry_points]
 console_scripts = 
 	pyrodigal = pyrodigal.cli:main
 
 [options.package_data]
 pyrodigal = py.typed, *.pyi, *.pxd
 pyrodigal.tests = data/*
```

### Comparing `pyrodigal-2.1.0/setup.py` & `pyrodigal-2.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,14 +262,54 @@
                     __m64 a = _mm_set1_pi16(1);
                     short x = (short) _m_to_int(a);
                     return (x == 1) ? 0 : 1;
                 }}
             """,
         )
 
+    def _check_getid(self):
+        _eprint('checking whether `PyInterpreterState_GetID` is available')
+
+        base = "have_getid"
+        testfile = os.path.join(self.build_temp, "{}.c".format(base))
+        objects = []
+
+        self.mkpath(self.build_temp)
+        with open(testfile, "w") as f:
+            f.write("""
+            #include <stdint.h>
+            #include <stdlib.h>
+            #include <Python.h>
+
+            int main(int argc, char *argv[]) {{
+                PyInterpreterState_GetID(NULL);
+                return 0;
+            }}
+            """)
+
+        if self.compiler.compiler_type == "msvc":
+            flags = ["/WX"]
+        else:
+            flags = ["-Werror=implicit-function-declaration"]
+
+        try:
+            self.mkpath(self.build_temp)
+            objects = self.compiler.compile([testfile], extra_postargs=flags)
+        except CompileError:
+            _eprint("no")
+            return False
+        else:
+            _eprint("yes")
+            return True
+        finally:
+            os.remove(testfile)
+            for obj in filter(os.path.isfile, objects):
+                os.remove(obj)
+
+
     # --- Build code ---
 
     def build_simd_code(self, ext):
         # build platform-specific code
         for simd, sources in ext.platform_sources.items():
             if self._simd_supported[simd] and not self._simd_disabled[simd]:
                 objects = [
@@ -338,14 +378,15 @@
         cython_args = {
             "include_path": ["include"],
             "compiler_directives": {
                 "cdivision": True,
                 "nonecheck": False,
             },
             "compile_time_env": {
+                "HAS_PYINTERPRETERSTATE_GETID": self._check_getid(),
                 "SYS_IMPLEMENTATION_NAME": sys.implementation.name,
                 "SYS_VERSION_INFO_MAJOR": sys.version_info.major,
                 "SYS_VERSION_INFO_MINOR": sys.version_info.minor,
                 "SYS_VERSION_INFO_MICRO": sys.version_info.micro,
                 "TARGET_CPU": self.target_cpu,
                 "TARGET_SYSTEM": self.target_system,
                 "AVX2_BUILD_SUPPORT": False,
@@ -518,30 +559,14 @@
         self.make_file(
             [self.training_file],
             self.training_temp,
             self._split_training_source,
             (self.training_file, self.training_temp)
         )
 
-        # detect if a custom file needs to be included for `cpu_features`
-        impl_path = os.path.join(
-            "vendor", 
-            "cpu_features", 
-            "src", 
-            "impl_{}_{}.c".format(self.target_cpu, self.target_system)
-        )
-        if os.path.exists(impl_path):
-            self.get_library("cpu_features").sources.append(impl_path)
-
-        # check for functions required for libcpu_features on OSX
-        if self.target_system == "macos":
-            _patch_osx_compiler(self.compiler, self.target_machine)
-            if self._check_function("sysctlbyname", "sys/sysctl.h", args="(NULL, NULL, 0, NULL, 0)"):
-                self.compiler.define_macro("HAVE_SYSCTLBYNAME", 1)
-
         # build each library only if the sources are outdated
         self.mkpath(self.build_clib)
         for library in libraries:
             libname = self.compiler.library_filename(library.name, output_dir=self.build_clib)
             self.make_file(library.sources, libname, self.build_library, (library,))
 
     def build_library(self, library):
@@ -639,23 +664,14 @@
                     "node",
                     "sequence",
                     "training"
                 ]
             ],
             include_dirs=[os.path.join("vendor", "Prodigal")]
         ),
-        Library(
-            "cpu_features",
-            sources=list(filter(os.path.exists, [
-                os.path.join("vendor", "cpu_features", "src", "{}.c".format(base))
-                for base in ["filesystem", "stack_line_reader", "string_view"]
-            ])),
-            include_dirs=[os.path.join("vendor", "cpu_features", "include")],
-            define_macros=[("STACK_LINE_READER_BUFFER_SIZE", 1024)]
-        ),
     ],
     ext_modules=[
         Extension(
             "pyrodigal._pyrodigal",
             sources=[
                 "pyrodigal/_pyrodigal.pyx",
                 "pyrodigal/impl/generic.c"
@@ -665,19 +681,17 @@
                 "NEON": ["pyrodigal/impl/neon.c"],
                 "SSE2": ["pyrodigal/impl/sse.c"],
                 "MMX": ["pyrodigal/impl/mmx.c"],
             },
             include_dirs=[
                 "pyrodigal",
                 os.path.join("vendor", "Prodigal"),
-                os.path.join("vendor", "cpu_features", "include"),
             ],
             libraries=[
                 "prodigal",
-                "cpu_features",
             ],
         ),
     ],
     cmdclass={
         "sdist": sdist,
         "build_ext": build_ext,
         "build_clib": build_clib,
```

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/CHANGES` & `pyrodigal-2.2.0/vendor/Prodigal/CHANGES`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/LICENSE` & `pyrodigal-2.2.0/vendor/Prodigal/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/Makefile` & `pyrodigal-2.2.0/vendor/Prodigal/Makefile`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/README.md` & `pyrodigal-2.2.0/vendor/Prodigal/README.md`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/bitmap.c` & `pyrodigal-2.2.0/vendor/Prodigal/bitmap.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/bitmap.h` & `pyrodigal-2.2.0/vendor/Prodigal/bitmap.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/dprog.c` & `pyrodigal-2.2.0/vendor/Prodigal/dprog.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/dprog.h` & `pyrodigal-2.2.0/vendor/Prodigal/dprog.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/gene.c` & `pyrodigal-2.2.0/vendor/Prodigal/gene.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/gene.h` & `pyrodigal-2.2.0/vendor/Prodigal/gene.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/main.c` & `pyrodigal-2.2.0/vendor/Prodigal/main.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/metagenomic.c` & `pyrodigal-2.2.0/vendor/Prodigal/metagenomic.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/metagenomic.h` & `pyrodigal-2.2.0/vendor/Prodigal/metagenomic.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/node.c` & `pyrodigal-2.2.0/vendor/Prodigal/node.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/node.h` & `pyrodigal-2.2.0/vendor/Prodigal/node.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/sequence.c` & `pyrodigal-2.2.0/vendor/Prodigal/sequence.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/sequence.h` & `pyrodigal-2.2.0/vendor/Prodigal/sequence.h`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/training.c` & `pyrodigal-2.2.0/vendor/Prodigal/training.c`

 * *Files identical despite different names*

### Comparing `pyrodigal-2.1.0/vendor/Prodigal/training.h` & `pyrodigal-2.2.0/vendor/Prodigal/training.h`

 * *Files identical despite different names*

