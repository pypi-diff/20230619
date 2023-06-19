# Comparing `tmp/eFISHent-0.0.4.tar.gz` & `tmp/eFISHent-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFISHent-0.0.4.tar", last modified: Tue Mar 21 13:55:55 2023, max compression
+gzip compressed data, was "eFISHent-0.0.5.tar", last modified: Mon Jun 19 13:33:05 2023, max compression
```

## Comparing `eFISHent-0.0.4.tar` & `eFISHent-0.0.5.tar`

### file list

```diff
@@ -1,270 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:55:55.545272 eFISHent-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-21 13:55:34.000000 eFISHent-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-21 13:55:55.545272 eFISHent-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-03-21 13:55:34.000000 eFISHent-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:55:55.449271 eFISHent-0.0.4/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-21 13:55:34.000000 eFISHent-0.0.4/conda/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-21 13:55:34.000000 eFISHent-0.0.4/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:55:55.457271 eFISHent-0.0.4/eFISHent/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/basic_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:55:55.545272 eFISHent-0.0.4/eFISHent/data_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.coaxial.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.coaxial.dh
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.coaxstack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.coaxstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.dangle.dg
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.dangle.dh
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.dynalignmiscloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.hexaloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.hexaloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.int11.dg
--rw-r--r--   0 runner    (1001) docker     (123)    15847 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.int11.dh
--rw-r--r--   0 runner    (1001) docker     (123)    91487 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.int21.dg
--rw-r--r--   0 runner    (1001) docker     (123)    62673 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.int21.dh
--rw-r--r--   0 runner    (1001) docker     (123)   202949 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.int22.dg
--rw-r--r--   0 runner    (1001) docker     (123)   239533 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.int22.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.loop.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.miscloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.miscloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.specification.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.stack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.stack.dh
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.triloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.triloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackcoax.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackcoax.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackh.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackh.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki1n.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki1n.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki23.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki23.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackm.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackm.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/coaxial.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/coaxial.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/coaxstack.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/coaxstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dangle.dat
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dangle.dh
--rw-r--r--   0 runner    (1001) docker     (123)    41352 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/design.DNA.Helices.dat
--rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/design.DNA.Loops.dat
--rw-r--r--   0 runner    (1001) docker     (123)    40310 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/design.RNA.Helices.dat
--rw-r--r--   0 runner    (1001) docker     (123)    20189 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/design.RNA.Loops.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.coaxial.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.coaxial.dh
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.coaxstack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.coaxstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.dangle.dg
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.dangle.dh
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.dynalignmiscloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.dynalignmiscloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.hexaloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.hexaloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.int11.dg
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.int11.dh
--rw-r--r--   0 runner    (1001) docker     (123)    33241 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.int21.dg
--rw-r--r--   0 runner    (1001) docker     (123)    35488 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.int21.dh
--rw-r--r--   0 runner    (1001) docker     (123)    56145 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.int22.dg
--rw-r--r--   0 runner    (1001) docker     (123)    62705 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.int22.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.loop.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.loop.dh
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.miscloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.miscloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.specification.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.stack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.stack.dh
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.triloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.triloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstackcoax.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstackcoax.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstackh.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstackh.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki1n.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki1n.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki23.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki23.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstackm.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dna.tstackm.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnacoaxial.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnacoaxial.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnacoaxstack.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnacoaxstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnadangle.dat
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnadangle.dh
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnadynalignmiscloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnadynalignmiscloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnahexaloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnahexaloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnaint11.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnaint11.dh
--rw-r--r--   0 runner    (1001) docker     (123)    39870 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnaint21.dat
--rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnaint21.dh
--rw-r--r--   0 runner    (1001) docker     (123)    68371 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnaint22.dat
--rw-r--r--   0 runner    (1001) docker     (123)    69001 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnaint22.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnaloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnaloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnamiscloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnamiscloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnastack.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnastack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatriloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatriloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstack.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstackcoax.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstackcoax.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstackh.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstackh.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstacki.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstacki.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstacki1n.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstacki1n.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstacki23.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstacki23.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstackm.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dnatstackm.dh
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/dynalignmiscloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/fam_hmm_pars.dat
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/helix.dat
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/helixdr.dat
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/hexaloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/hexaloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/int11.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/int11.dh
--rw-r--r--   0 runner    (1001) docker     (123)    39823 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/int21.dat
--rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/int21.dh
--rw-r--r--   0 runner    (1001) docker     (123)    67786 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/int22-exp.dh
--rw-r--r--   0 runner    (1001) docker     (123)    68297 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/int22.dat
--rw-r--r--   0 runner    (1001) docker     (123)    71577 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/int22.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/loop.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/loop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.coaxial.dg
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.coaxstack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.dangle.dg
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.hexaloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.int11.dg
--rw-r--r--   0 runner    (1001) docker     (123)    83200 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.int21.dg
--rw-r--r--   0 runner    (1001) docker     (123)   197554 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.int22.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.loop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.miscloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.specification.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.stack.dg
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.tloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.triloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.tstack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.tstackcoax.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.tstackh.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.tstacki.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.tstacki1n.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.tstacki23.dg
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/m6A.tstackm.dg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/miscloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/miscloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/pseudconst.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.coaxial.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.coaxial.dh
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.coaxstack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.coaxstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)  1332032 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.cov.dg
--rw-r--r--   0 runner    (1001) docker     (123)  1336808 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.cov.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.dangle.dg
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.dangle.dh
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.dynalignmiscloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.hexaloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.hexaloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.int11.dg
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.int11.dh
--rw-r--r--   0 runner    (1001) docker     (123)    33238 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.int21.dg
--rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.int21.dh
--rw-r--r--   0 runner    (1001) docker     (123)    56398 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.int22.dg
--rw-r--r--   0 runner    (1001) docker     (123)    66417 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.int22.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.loop.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.loop.dh
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.miscloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.miscloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)  7768638 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.param_map.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.specification.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.stack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.stack.dh
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.triloop.dg
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.triloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstack.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstackcoax.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstackcoax.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstackh.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstackh.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki1n.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki1n.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki23.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki23.dh
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstackm.dg
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/rna.tstackm.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/stack.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/stack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/stackdr.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/stackdr.dh
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/triloop.dat
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/triloop.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstack.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstack.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstackcoax.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstackcoax.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstackh.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstackh.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstacki.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstacki.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstacki1n.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstacki1n.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstacki23.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstacki23.dh
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstackm.dat
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/data_tables/tstackm.dh
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/generate_probes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/kmers.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/luigi.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/prepare_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/secondary_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-03-21 13:55:34.000000 eFISHent-0.0.4/eFISHent/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 13:55:55.457271 eFISHent-0.0.4/eFISHent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-21 13:55:55.000000 eFISHent-0.0.4/eFISHent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-03-21 13:55:55.000000 eFISHent-0.0.4/eFISHent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 13:55:55.000000 eFISHent-0.0.4/eFISHent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-21 13:55:55.000000 eFISHent-0.0.4/eFISHent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 13:55:55.000000 eFISHent-0.0.4/eFISHent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-21 13:55:55.000000 eFISHent-0.0.4/eFISHent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-21 13:55:55.000000 eFISHent-0.0.4/eFISHent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-21 13:55:34.000000 eFISHent-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-21 13:55:55.553272 eFISHent-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-21 13:55:34.000000 eFISHent-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:33:05.144121 eFISHent-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 13:32:50.000000 eFISHent-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-19 13:33:05.144121 eFISHent-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-19 13:32:50.000000 eFISHent-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:33:05.100120 eFISHent-0.0.5/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-19 13:32:50.000000 eFISHent-0.0.5/conda/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-19 13:32:50.000000 eFISHent-0.0.5/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:33:05.104120 eFISHent-0.0.5/eFISHent/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/basic_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:33:05.144121 eFISHent-0.0.5/eFISHent/data_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.coaxial.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.coaxial.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.coaxstack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.coaxstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.dangle.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.dangle.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.dynalignmiscloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.hexaloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.hexaloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.int11.dg
+-rw-r--r--   0 runner    (1001) docker     (123)    15847 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.int11.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    91487 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.int21.dg
+-rw-r--r--   0 runner    (1001) docker     (123)    62673 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.int21.dh
+-rw-r--r--   0 runner    (1001) docker     (123)   202949 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.int22.dg
+-rw-r--r--   0 runner    (1001) docker     (123)   239533 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.int22.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.loop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.miscloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.miscloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.specification.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.stack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.stack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.triloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.triloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackcoax.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackcoax.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackh.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackh.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki1n.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki1n.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki23.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki23.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackm.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackm.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/coaxial.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/coaxial.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/coaxstack.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/coaxstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dangle.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dangle.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    41352 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/design.DNA.Helices.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/design.DNA.Loops.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    40310 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/design.RNA.Helices.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    20189 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/design.RNA.Loops.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.coaxial.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.coaxial.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.coaxstack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.coaxstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.dangle.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.dangle.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.dynalignmiscloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.dynalignmiscloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.hexaloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.hexaloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.int11.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.int11.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    33241 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.int21.dg
+-rw-r--r--   0 runner    (1001) docker     (123)    35488 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.int21.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    56145 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.int22.dg
+-rw-r--r--   0 runner    (1001) docker     (123)    62705 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.int22.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.loop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.loop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.miscloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.miscloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.specification.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.stack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.stack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.triloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.triloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstackcoax.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstackcoax.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstackh.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstackh.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki1n.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki1n.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki23.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki23.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstackm.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dna.tstackm.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnacoaxial.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnacoaxial.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnacoaxstack.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnacoaxstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnadangle.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnadangle.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnadynalignmiscloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnadynalignmiscloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnahexaloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnahexaloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnaint11.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnaint11.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    39870 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnaint21.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnaint21.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    68371 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnaint22.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    69001 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnaint22.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnaloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnaloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnamiscloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnamiscloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnastack.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnastack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatriloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatriloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstack.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstackcoax.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstackcoax.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstackh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstackh.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstacki.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstacki.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstacki1n.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstacki1n.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstacki23.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstacki23.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstackm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dnatstackm.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/dynalignmiscloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/fam_hmm_pars.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/helix.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/helixdr.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/hexaloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/hexaloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/int11.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/int11.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    39823 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/int21.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/int21.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    67786 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/int22-exp.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    68297 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/int22.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    71577 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/int22.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/loop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/loop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.coaxial.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.coaxstack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.dangle.dg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.hexaloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.int11.dg
+-rw-r--r--   0 runner    (1001) docker     (123)    83200 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.int21.dg
+-rw-r--r--   0 runner    (1001) docker     (123)   197554 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.int22.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.loop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.miscloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.specification.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.stack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.tloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.triloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.tstack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.tstackcoax.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.tstackh.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.tstacki.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.tstacki1n.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.tstacki23.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/m6A.tstackm.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/miscloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/miscloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/pseudconst.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.coaxial.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.coaxial.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.coaxstack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.coaxstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)  1332032 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.cov.dg
+-rw-r--r--   0 runner    (1001) docker     (123)  1336808 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.cov.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.dangle.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.dangle.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.dynalignmiscloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.hexaloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.hexaloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.int11.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.int11.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    33238 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.int21.dg
+-rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.int21.dh
+-rw-r--r--   0 runner    (1001) docker     (123)    56398 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.int22.dg
+-rw-r--r--   0 runner    (1001) docker     (123)    66417 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.int22.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.loop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.loop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.miscloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.miscloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)  7768638 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.param_map.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.specification.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.stack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.stack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.triloop.dg
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.triloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstack.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstackcoax.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstackcoax.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstackh.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstackh.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki1n.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki1n.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki23.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki23.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstackm.dg
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/rna.tstackm.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/stack.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/stack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/stackdr.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/stackdr.dh
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/triloop.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/triloop.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstack.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstack.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstackcoax.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstackcoax.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstackh.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstackh.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstacki.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstacki.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstacki1n.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstacki1n.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstacki23.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstacki23.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstackm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/data_tables/tstackm.dh
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/generate_probes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/kmers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/luigi.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/prepare_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/secondary_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-19 13:32:50.000000 eFISHent-0.0.5/eFISHent/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:33:05.104120 eFISHent-0.0.5/eFISHent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-19 13:33:05.000000 eFISHent-0.0.5/eFISHent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-19 13:33:05.000000 eFISHent-0.0.5/eFISHent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:33:05.000000 eFISHent-0.0.5/eFISHent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-19 13:33:05.000000 eFISHent-0.0.5/eFISHent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:33:04.000000 eFISHent-0.0.5/eFISHent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 13:33:05.000000 eFISHent-0.0.5/eFISHent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 13:33:05.000000 eFISHent-0.0.5/eFISHent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-19 13:32:50.000000 eFISHent-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-19 13:33:05.144121 eFISHent-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-19 13:32:50.000000 eFISHent-0.0.5/setup.py
```

### Comparing `eFISHent-0.0.4/PKG-INFO` & `eFISHent-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFISHent
-Version: 0.0.4
+Version: 0.0.5
 Summary: RNA FISH oligos/probes design tool.
 Home-page: https://github.com/bbquercus/efishent/
 Author: Bastian Eichenberger
 Author-email: bastian@eichenbergers.ch
 License: MIT
 Project-URL: Documentation, https://github.com/BBQuercus/efishent/wiki
 Project-URL: Changelog, https://github.com/BBQuercus/efishent/releases
```

### Comparing `eFISHent-0.0.4/README.md` & `eFISHent-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 conda env create bbquercus/efishent  
 
 # Activate environment
 conda activate efishent
 
 # Install efishent via pypi
 pip install efishent
-
 ```
 
 Any updates can then simply be done via pypi (`pip install --upgrade efishent`).
 
 ## Usage
 
 A detailed usage guide can be found on the [GitHub wiki](https://github.com/bbquercus/eFISHent/wiki) but here is a quick example:
@@ -52,34 +51,32 @@
 
 ## Component overview
 
 eFISHent is built up modularly using the following components...
 
 Index creation workflow:
 
-* Bowtie index (`indexing.py`)
-* Blast database (`indexing.py`)
-* Jellyfish indices (`kmers.py`)
+* Bowtie index
+* Jellyfish indices
 
 Probe filtering workflow:
 
-* Download / prepare sequences (`prepare_sequences.py`)
-* Generate candidate probes (`generate_probes.py`)
-* Filter with basic filters (`basic_filtering.py`)
-* Align probes to reference genome (`alignment.py`)
-* Filter based on alignment score and uniqueness (`alignment.py`)
-* Filter reoccuring k-mers (`kmers.py`)
-* Filter based on secondary structure prediction (`secondary_structure.py`)
-* Create final list of probes (`optimization.py`)
-* Write final list of probes to file with report (`cleanup.py`)
+* Download / prepare sequences
+* Generate candidate probes
+* Filter with basic filters
+* Align probes to reference genome
+* Filter based on alignment score and uniqueness
+* Filter reoccuring k-mers
+* Filter based on secondary structure prediction
+* Create final list of probes
+* Write final list of probes to file with report
 
 Probe set analysis plotting:
 
-* Create a simple overview over the key parameters (`analyze.py`)
-* (Using inputs from most other files)
+* Create a simple overview over the key parameters
 
 ## TODO
 
 * [ ] Add more detailed documentation as wiki page(s)
   * [x] Add links to genomes and RNAseq databases
   * [x] Add examples from multiple sources
   * [ ] Add benchmarks for deltaG, counts
```

### Comparing `eFISHent-0.0.4/conda/meta.yaml` & `eFISHent-0.0.5/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/analyze.py` & `eFISHent-0.0.5/eFISHent/analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,42 +200,37 @@
         """Layout to build the figure."""
         fig = plt.figure(figsize=(15, 18))
         plt.suptitle(
             f"Analysis of probe set - {util.get_gene_name(False)}", y=1, fontsize=20
         )
         shape = (4, 3)
 
-        # Row 1
+        # Row 1 - length, TM, GC
         ax = plt.subplot2grid(shape, (0, 0))
         self.add_length(ax)
         ax = plt.subplot2grid(shape, (0, 1))
         self.add_melting_temperature(ax)
         ax = plt.subplot2grid(shape, (0, 2))
         self.add_gc_content(ax)
 
-        # Row 2
+        # Row 2 - G-quadruplet, kmer, deltaG
         ax = plt.subplot2grid(shape, (1, 0))
         self.add_g_quadruplet(ax)
         ax = plt.subplot2grid(shape, (1, 1))
         self.add_kmers(ax)
         ax = plt.subplot2grid(shape, (1, 2))
         self.add_free_energy(ax)
 
-        # Row 3
+        # Row 3 - off target count, affinity
         ax = plt.subplot2grid(shape, (2, 0))
         self.add_off_targets(ax)
         ax = plt.subplot2grid(shape, (2, 1))
         self.add_binding_affinity(ax, fig)
 
-        # TODO add a way to display off target expression percentages?
-        # if ProbeConfig().encode_count_table:
-        #     ax = plt.subplot2grid(shape, (2, 2))
-        #     self.add_expression_percentages(ax)
-
-        # Row 4
+        # Row 4 - coverage
         ax = plt.subplot2grid(shape, (3, 0), colspan=3)
         self.add_probe_coverage(ax)
 
         plt.tight_layout()
         plt.savefig(self.output().path)
 
     def run(self):
```

### Comparing `eFISHent-0.0.4/eFISHent/basic_filtering.py` & `eFISHent-0.0.5/eFISHent/basic_filtering.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,31 @@
 from .config import ProbeConfig
 from .generate_probes import GenerateAllProbes
 
 
 def get_melting_temp(
     sequence: Bio.Seq.Seq, na_concentration: float, formamide_concentration: float
 ) -> float:
-    """Get melting temperature of candidate."""
-    tm_raw = Bio.SeqUtils.MeltingTemp.Tm_NN(sequence, Na=na_concentration)
+    """Get melting temperature of candidate assuming DNA/RNA hybrid."""
+    rna_sequence = sequence.transcribe()
+    tm_raw = Bio.SeqUtils.MeltingTemp.Tm_NN(
+        rna_sequence,
+        c_seq=rna_sequence.complement_rna(),
+        nn_table=Bio.SeqUtils.MeltingTemp.R_DNA_NN1,
+        Na=na_concentration,
+    )
     melting_temp = Bio.SeqUtils.MeltingTemp.chem_correction(
         tm_raw, fmd=formamide_concentration
     )
     return float(melting_temp)
 
 
 def get_gc_content(sequence: Bio.Seq.Seq) -> float:
     """Get GC content of candidate."""
-    return float(Bio.SeqUtils.GC(sequence))
+    return float(Bio.SeqUtils.gc_fraction(sequence)) * 100
 
 
 def get_g_quadruplet_count(sequence: Bio.Seq.Seq) -> int:
     """Get number of G quadruplets in candidate."""
     return int(sequence.count("GGGG"))
 
 
@@ -61,15 +67,17 @@
         if config.min_gc > config.max_gc:
             raise ValueError("Max GC has to be greater or equal the min GC!")
 
         sequence = candidate.seq
         gc_content = get_gc_content(sequence)
         g_quadruplets = get_g_quadruplet_count(sequence)
         melting_temp = get_melting_temp(
-            sequence, config.na_concentration, config.formamide_concentration
+            Bio.Seq.Seq(sequence),
+            config.na_concentration,
+            config.formamide_concentration,
         )
 
         if (
             config.min_gc <= gc_content <= config.max_gc
             and config.min_tm <= melting_temp <= config.max_tm
             and g_quadruplets == 0
         ):
```

### Comparing `eFISHent-0.0.4/eFISHent/cleanup.py` & `eFISHent-0.0.5/eFISHent/cleanup.py`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/cli.py` & `eFISHent-0.0.5/eFISHent/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 import os
 import sys
 import tempfile
 
 import luigi
 
-# from .indexing import BuildBlastDatabase
+from . import __version__
 from .analyze import AnalyzeProbeset
 from .cleanup import CleanUpOutput
 from .constants import CLI_SHORTFORM
 from .constants import CONFIG_CLASSES
 from .indexing import BuildBowtieIndex
 from .kmers import BuildJellyfishIndex
 from .util import UniCode
@@ -63,15 +63,15 @@
         default=argparse.SUPPRESS,
         help="Show this message.",
     )
     utility.add_argument(
         "-V",
         "--version",
         action="version",
-        version="%(prog)s 0.0.1",
+        version="%(prog)s " + str(__version__),
         help="Show %(prog)s's version number.",
     )
     utility.add_argument(
         "-s",
         "--silent",
         action="store_true",
         help="Change the program output to silent hiding information on progress.",
```

### Comparing `eFISHent-0.0.4/eFISHent/config.py` & `eFISHent-0.0.5/eFISHent/config.py`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/constants.py` & `eFISHent-0.0.5/eFISHent/constants.py`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.coaxial.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.coaxial.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.coaxial.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.coaxial.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.coaxstack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.coaxstack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.coaxstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.coaxstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.dangle.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.dangle.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.dangle.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.dangle.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.dynalignmiscloop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.dynalignmiscloop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.int11.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.int11.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.int11.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.int11.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.int21.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.int21.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.int21.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.int21.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.int22.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.int22.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.int22.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.int22.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.loop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.loop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.miscloop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.miscloop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.miscloop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.miscloop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.specification.dat` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.specification.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.stack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.stack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.stack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.stack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackcoax.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackcoax.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackcoax.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackcoax.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackh.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackh.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackh.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackh.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki1n.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki1n.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki1n.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki1n.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki23.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki23.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstacki23.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstacki23.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackm.dg` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackm.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/b-test.tstackm.dh` & `eFISHent-0.0.5/eFISHent/data_tables/b-test.tstackm.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/coaxial.dat` & `eFISHent-0.0.5/eFISHent/data_tables/coaxial.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/coaxial.dh` & `eFISHent-0.0.5/eFISHent/data_tables/coaxial.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/coaxstack.dat` & `eFISHent-0.0.5/eFISHent/data_tables/coaxstack.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/coaxstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/coaxstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dangle.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dangle.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dangle.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dangle.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/design.DNA.Helices.dat` & `eFISHent-0.0.5/eFISHent/data_tables/design.DNA.Helices.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/design.DNA.Loops.dat` & `eFISHent-0.0.5/eFISHent/data_tables/design.DNA.Loops.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/design.RNA.Helices.dat` & `eFISHent-0.0.5/eFISHent/data_tables/design.RNA.Helices.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/design.RNA.Loops.dat` & `eFISHent-0.0.5/eFISHent/data_tables/design.RNA.Loops.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.coaxial.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.coaxial.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.coaxial.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.coaxial.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.coaxstack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.coaxstack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.coaxstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.coaxstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.dangle.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.dangle.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.dangle.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.dangle.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.dynalignmiscloop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.dynalignmiscloop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.dynalignmiscloop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.dynalignmiscloop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.int11.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.int11.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.int11.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.int11.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.int21.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.int21.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.int21.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.int21.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.int22.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.int22.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.int22.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.int22.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.loop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.loop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.loop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.loop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.miscloop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.miscloop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.miscloop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.miscloop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.specification.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dna.specification.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.stack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.stack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.stack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.stack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstackcoax.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstackcoax.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstackcoax.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstackcoax.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstackh.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstackh.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstackh.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstackh.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki1n.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki1n.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki1n.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki1n.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki23.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki23.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstacki23.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstacki23.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstackm.dg` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstackm.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dna.tstackm.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dna.tstackm.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnacoaxial.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnacoaxial.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnacoaxial.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnacoaxial.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnacoaxstack.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnacoaxstack.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnacoaxstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnacoaxstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnadangle.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnadangle.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnadangle.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnadangle.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnadynalignmiscloop.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnadynalignmiscloop.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnadynalignmiscloop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnadynalignmiscloop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnaint11.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnaint11.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnaint11.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnaint11.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnaint21.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnaint21.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnaint21.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnaint21.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnaint22.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnaint22.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnaint22.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnaint22.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnaloop.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnaloop.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnaloop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnaloop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnamiscloop.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnamiscloop.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnamiscloop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnamiscloop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnastack.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnastack.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnastack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnastack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatloop.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnatloop.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstack.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstack.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstackcoax.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstackcoax.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstackcoax.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstackcoax.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstackh.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstackh.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstackh.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstackh.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstacki.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstacki.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstacki.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstacki.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstacki1n.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstacki1n.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstacki1n.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstacki1n.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstacki23.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstacki23.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstacki23.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstacki23.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstackm.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstackm.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dnatstackm.dh` & `eFISHent-0.0.5/eFISHent/data_tables/dnatstackm.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/dynalignmiscloop.dat` & `eFISHent-0.0.5/eFISHent/data_tables/dynalignmiscloop.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/fam_hmm_pars.dat` & `eFISHent-0.0.5/eFISHent/data_tables/fam_hmm_pars.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/int11.dat` & `eFISHent-0.0.5/eFISHent/data_tables/int11.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/int11.dh` & `eFISHent-0.0.5/eFISHent/data_tables/int11.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/int21.dat` & `eFISHent-0.0.5/eFISHent/data_tables/int21.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/int21.dh` & `eFISHent-0.0.5/eFISHent/data_tables/int21.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/int22-exp.dh` & `eFISHent-0.0.5/eFISHent/data_tables/int22-exp.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/int22.dat` & `eFISHent-0.0.5/eFISHent/data_tables/int22.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/int22.dh` & `eFISHent-0.0.5/eFISHent/data_tables/int22.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/loop.dat` & `eFISHent-0.0.5/eFISHent/data_tables/loop.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/loop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/loop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.coaxial.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.coaxial.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.coaxstack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.coaxstack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.dangle.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.dangle.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.int11.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.int11.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.int21.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.int21.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.int22.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.int22.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.loop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.loop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.miscloop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.miscloop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.specification.dat` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.specification.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.stack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.stack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.tstack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.tstack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.tstackcoax.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.tstackcoax.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.tstackh.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.tstackh.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.tstacki.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.tstacki.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.tstacki1n.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.tstacki1n.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.tstacki23.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.tstacki23.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/m6A.tstackm.dg` & `eFISHent-0.0.5/eFISHent/data_tables/m6A.tstackm.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/miscloop.dat` & `eFISHent-0.0.5/eFISHent/data_tables/miscloop.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/miscloop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/miscloop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/pseudconst.dat` & `eFISHent-0.0.5/eFISHent/data_tables/pseudconst.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.coaxial.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.coaxial.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.coaxial.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.coaxial.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.coaxstack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.coaxstack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.coaxstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.coaxstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.cov.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.cov.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.cov.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.cov.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.dangle.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.dangle.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.dangle.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.dangle.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.dynalignmiscloop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.dynalignmiscloop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.int11.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.int11.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.int11.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.int11.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.int21.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.int21.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.int21.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.int21.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.int22.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.int22.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.int22.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.int22.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.loop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.loop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.loop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.loop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.miscloop.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.miscloop.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.miscloop.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.miscloop.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.param_map.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.param_map.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.specification.dat` & `eFISHent-0.0.5/eFISHent/data_tables/rna.specification.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.stack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.stack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.stack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.stack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstack.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstack.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstackcoax.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstackcoax.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstackcoax.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstackcoax.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstackh.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstackh.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstackh.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstackh.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki1n.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki1n.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki1n.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki1n.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki23.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki23.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstacki23.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstacki23.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstackm.dg` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstackm.dg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/rna.tstackm.dh` & `eFISHent-0.0.5/eFISHent/data_tables/rna.tstackm.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/stack.dat` & `eFISHent-0.0.5/eFISHent/data_tables/stack.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/stack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/stack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/stackdr.dat` & `eFISHent-0.0.5/eFISHent/data_tables/stackdr.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/stackdr.dh` & `eFISHent-0.0.5/eFISHent/data_tables/stackdr.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstack.dat` & `eFISHent-0.0.5/eFISHent/data_tables/tstack.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstack.dh` & `eFISHent-0.0.5/eFISHent/data_tables/tstack.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstackcoax.dat` & `eFISHent-0.0.5/eFISHent/data_tables/tstackcoax.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstackcoax.dh` & `eFISHent-0.0.5/eFISHent/data_tables/tstackcoax.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstackh.dat` & `eFISHent-0.0.5/eFISHent/data_tables/tstackh.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstackh.dh` & `eFISHent-0.0.5/eFISHent/data_tables/tstackh.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstacki.dat` & `eFISHent-0.0.5/eFISHent/data_tables/tstacki.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstacki.dh` & `eFISHent-0.0.5/eFISHent/data_tables/tstacki.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstacki1n.dat` & `eFISHent-0.0.5/eFISHent/data_tables/tstacki1n.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstacki1n.dh` & `eFISHent-0.0.5/eFISHent/data_tables/tstacki1n.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstacki23.dat` & `eFISHent-0.0.5/eFISHent/data_tables/tstacki23.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstacki23.dh` & `eFISHent-0.0.5/eFISHent/data_tables/tstacki23.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstackm.dat` & `eFISHent-0.0.5/eFISHent/data_tables/tstackm.dat`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/data_tables/tstackm.dh` & `eFISHent-0.0.5/eFISHent/data_tables/tstackm.dh`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/generate_probes.py` & `eFISHent-0.0.5/eFISHent/generate_probes.py`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/indexing.py` & `eFISHent-0.0.5/eFISHent/indexing.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,40 +8,14 @@
 import luigi
 import pandas as pd
 
 from . import util
 from .config import GeneralConfig
 
 
-# class BuildBlastDatabase(luigi.Task):
-#     """Build local nucleotide blast database."""
-
-#     logger = logging.getLogger("custom-logger")
-
-#     def output(self):
-#         return [
-#             luigi.LocalTarget(f"{util.get_genome_name()}.{extension}")
-#             for extension in ["nhr", "nin", "nsq"]
-#         ]
-
-#     def build_blast_index(self, fname: str, genome: str) -> None:
-#         args_blast = ["makeblastdb", "-dbtype", "nucl", "-in", fname, "-out", genome]
-#         self.logger.debug(f"Running bowtie with - {''.join(args_blast)}")
-#         subprocess.check_call(
-#             args_blast, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT
-#         )
-
-#     def run(self):
-#         self.build_blast_index(
-#             fname=os.path.abspath(GeneralConfig().reference_genome),
-#             genome=util.get_genome_name(),
-#         )
-#         self.logger.info("Finished building blast database.")
-
-
 class BuildBowtieIndex(luigi.Task):
     """Create bowtie index for a given reference genome."""
 
     logger = logging.getLogger("custom-logger")
 
     def output(self):
         return [
```

### Comparing `eFISHent-0.0.4/eFISHent/kmers.py` & `eFISHent-0.0.5/eFISHent/kmers.py`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/luigi.cfg` & `eFISHent-0.0.5/eFISHent/luigi.cfg`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/optimization.py` & `eFISHent-0.0.5/eFISHent/optimization.py`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/prepare_sequence.py` & `eFISHent-0.0.5/eFISHent/prepare_sequence.py`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent/secondary_structure.py` & `eFISHent-0.0.5/eFISHent/secondary_structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 from .kmers import KMerFiltering
 
 
 def get_free_energy(sequence: Bio.SeqRecord.SeqRecord) -> float:
     """Return the predicted free energy of the sequence.
 
     Using "Fold" as part of the RNAstructure package from the Mathews lab.
+
+    Not ideal to include Fold_osx executable but easiest solution since
+        there is no RNAstructure build on conda for MacOS and this is the only
+        dependency not available.
     """
     file_path = Path(__file__).resolve().parent.as_posix()
     data_table = os.path.join(file_path, "data_tables/")
     if sys.platform == "linux" or sys.platform == "linux2":
         fold_path = "Fold"
     if sys.platform == "darwin":
         fold_path = os.path.join(file_path, "Fold_osx")
```

### Comparing `eFISHent-0.0.4/eFISHent/util.py` & `eFISHent-0.0.5/eFISHent/util.py`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/eFISHent.egg-info/PKG-INFO` & `eFISHent-0.0.5/eFISHent.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFISHent
-Version: 0.0.4
+Version: 0.0.5
 Summary: RNA FISH oligos/probes design tool.
 Home-page: https://github.com/bbquercus/efishent/
 Author: Bastian Eichenberger
 Author-email: bastian@eichenbergers.ch
 License: MIT
 Project-URL: Documentation, https://github.com/BBQuercus/efishent/wiki
 Project-URL: Changelog, https://github.com/BBQuercus/efishent/releases
```

### Comparing `eFISHent-0.0.4/eFISHent.egg-info/SOURCES.txt` & `eFISHent-0.0.5/eFISHent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eFISHent-0.0.4/setup.py` & `eFISHent-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import textwrap
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     # Description
     name="eFISHent",
-    version="0.0.4",
+    version="0.0.5",
     license="MIT",
     description="RNA FISH oligos/probes design tool.",
     long_description_content_type="text/plain",
     long_description=textwrap.dedent(
         """
     eFISHent is a command-line based tool to facilitate the creation of eFISHent RNA FISH oligonucleotide probes.
     This is just the python code which is reliant on multiple compiled bioinformatics libaries.
```

