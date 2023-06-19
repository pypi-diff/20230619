# Comparing `tmp/hotpot-zzy-0.2.6.tar.gz` & `tmp/hotpot-zzy-0.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zzy/hotpot/dist/.tmp-srry8bzz/hotpot-zzy-0.2.6.tar", last modified: Sun Jun 18 14:25:56 2023, max compression
+gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-_8xl5tum/hotpot-zzy-0.3.0.0.tar", last modified: Mon Jun 19 12:52:24 2023, max compression
```

## Comparing `hotpot-zzy-0.2.6.tar` & `hotpot-zzy-0.3.0.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.088475 hotpot-zzy-0.2.6/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       17 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/MANIFEST.in
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       54 2023-06-18 14:25:56.088475 hotpot-zzy-0.2.6/PKG-INFO
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     6765 2023-06-14 13:37:58.000000 hotpot-zzy-0.2.6/README.md
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.080475 hotpot-zzy-0.2.6/hotpot/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      437 2023-06-16 03:28:06.000000 hotpot-zzy-0.2.6/hotpot/__init__.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)    40667 2023-06-16 06:34:10.000000 hotpot-zzy-0.2.6/hotpot/_io.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)    19026 2023-06-16 06:43:48.000000 hotpot-zzy-0.2.6/hotpot/bundle.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)   102878 2023-06-17 15:22:25.000000 hotpot-zzy-0.2.6/hotpot/cheminfo.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.080475 hotpot-zzy-0.2.6/hotpot/data/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       71 2023-06-16 12:44:21.000000 hotpot-zzy-0.2.6/hotpot/data/atom_single_point.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.080475 hotpot-zzy-0.2.6/hotpot/data/force_field/
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.080475 hotpot-zzy-0.2.6/hotpot/data/force_field/UFF/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     4710 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.080475 hotpot-zzy-0.2.6/hotpot/data/force_field/aMaterials/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1742 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/force_field/aMaterials/SiC.tersoff
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       88 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/force_field/contents.json
--rw-rw-r--   0 zzy       (1002) zzy       (1002)   238863 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/periodic_table.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.088475 hotpot-zzy-0.2.6/hotpot/data/solvents/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      973 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,1,1-trichloroethane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1068 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      783 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,1,2-trichloroethene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,1-dichloroethene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2586 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,1-diethoxypropane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1447 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,1-dimethoxymethane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      970 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,2-dichloroethane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,2-dichloroethene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1731 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,2-dimethoxyethane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1558 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1,4-dioxane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1-butanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1912 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1-pentanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1342 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/1-propanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/2,2-dimethoxypropane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/2-butanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1727 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/2-ethoxyethanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1443 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/2-methoxyethanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1636 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/2-methyl-1-propanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1760 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/3-methyl-1-butanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      670 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/DCM.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1335 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/DMF.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1146 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/DMSO.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1638 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/N,N-dimethylacetamide.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1756 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/N-methylpyrrolidone.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1455 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/THF.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      963 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/acetic_acid.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1149 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/acetone.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      774 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/acetonitrile.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1364 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/benzene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2104 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/butylacetate.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      687 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/carbon_tetrachloride.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1370 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/chlorobenzene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      677 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/chloroform.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2218 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/cumene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/cyclohexane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1629 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/diethylether.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2298 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/diisopropylamine.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1054 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/ethanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/ethyl_formate.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1534 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/ethylacetate.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1156 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/ethyleneglycol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      771 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/formamide.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      678 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/formic_acid.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2384 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/heptane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2098 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/hexane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2108 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/isobutyl_acetate.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2671 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/isooctane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1343 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/isopropanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1823 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/isopropylacetate.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2201 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/isopropylether.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/meta-xylene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      770 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/methanol.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1751 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/methoxybenzene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/methylacetate.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2014 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/methylbutylketone.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2229 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/methylcyclohexane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1444 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/methylethylketone.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/methylisobutylketone.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1733 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/methylisopropylketone.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1652 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/morpholine.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      869 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/nitromethane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1939 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/ortho-xylene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/para-xylene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1814 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/pentane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1820 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/propylacetate.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1270 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/pyridine.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1651 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/sulfolane.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/t-butylmethylether.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2340 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/tetralin.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1649 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/toluene.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/trichloroacetic_acid.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/trifluoroacetic_acid.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      482 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/solvents/water.mol2
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      195 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/data/units.json
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.088475 hotpot-zzy-0.2.6/hotpot/tanks/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      217 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/tanks/__init__.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     5096 2023-06-17 13:54:21.000000 hotpot-zzy-0.2.6/hotpot/tanks/cc.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      161 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/tanks/features.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.088475 hotpot-zzy-0.2.6/hotpot/tanks/lmp/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      284 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/tanks/lmp/__init__.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     8118 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/tanks/lmp/base.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     8789 2023-06-14 00:55:16.000000 hotpot-zzy-0.2.6/hotpot/tanks/lmp/gcmc.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     9577 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/tanks/lmp/materials.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     7916 2023-06-16 12:06:52.000000 hotpot-zzy-0.2.6/hotpot/tanks/quantum.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2949 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/tmo.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2882 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/tools.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.088475 hotpot-zzy-0.2.6/hotpot/utils/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      134 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/utils/__init__.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1717 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/utils/load_chem_lib.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      669 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.088475 hotpot-zzy-0.2.6/hotpot_zzy.egg-info/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       54 2023-06-18 14:25:56.000000 hotpot-zzy-0.2.6/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     3854 2023-06-18 14:25:56.000000 hotpot-zzy-0.2.6/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)        1 2023-06-18 14:25:56.000000 hotpot-zzy-0.2.6/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       51 2023-06-18 14:25:56.000000 hotpot-zzy-0.2.6/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)        7 2023-06-18 14:25:56.000000 hotpot-zzy-0.2.6/hotpot_zzy.egg-info/top_level.txt
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      312 2023-06-18 12:37:09.000000 hotpot-zzy-0.2.6/pyproject.toml
--rw-rw-r--   0 zzy       (1002) zzy       (1002)       38 2023-06-18 14:25:56.088475 hotpot-zzy-0.2.6/setup.cfg
-drwxrwxr-x   0 zzy       (1002) zzy       (1002)        0 2023-06-18 14:25:56.088475 hotpot-zzy-0.2.6/test/
--rw-rw-r--   0 zzy       (1002) zzy       (1002)      550 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/test/test_amorphous_maker.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     1157 2023-06-14 09:02:54.000000 hotpot-zzy-0.2.6/test/test_bundle.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     2419 2023-06-16 02:14:06.000000 hotpot-zzy-0.2.6/test/test_chemif.py
--rw-rw-r--   0 zzy       (1002) zzy       (1002)     7081 2023-06-13 07:03:55.000000 hotpot-zzy-0.2.6/test/test_lmp.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)       17 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/MANIFEST.in
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       56 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/PKG-INFO
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     6765 2023-06-14 13:37:58.000000 hotpot-zzy-0.3.0.0/README.md
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      437 2023-06-19 12:37:49.000000 hotpot-zzy-0.3.0.0/hotpot/__init__.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)    40667 2023-06-16 06:34:10.000000 hotpot-zzy-0.3.0.0/hotpot/_io.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)    19026 2023-06-16 06:43:48.000000 hotpot-zzy-0.3.0.0/hotpot/bundle.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)   103045 2023-06-19 12:12:28.000000 hotpot-zzy-0.3.0.0/hotpot/cheminfo.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/data/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)       71 2023-06-16 12:44:21.000000 hotpot-zzy-0.3.0.0/hotpot/data/atom_single_point.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/data/force_field/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/data/force_field/UFF/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     4710 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.142557 hotpot-zzy-0.3.0.0/hotpot/data/force_field/aMaterials/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1742 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rwxrwx---   0 zz1       (1005) zz1       (1008)       88 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/force_field/contents.json
+-rwxrwx---   0 zz1       (1005) zz1       (1008)   238863 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/periodic_table.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.150557 hotpot-zzy-0.3.0.0/hotpot/data/solvents/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      973 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,1-trichloroethane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1068 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      783 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,2-trichloroethene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-dichloroethene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2586 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-diethoxypropane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1447 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-dimethoxymethane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      970 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dichloroethane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      780 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dichloroethene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1731 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dimethoxyethane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1558 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,4-dioxane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-butanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1912 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-pentanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1342 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-propanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2,2-dimethoxypropane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1626 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-butanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1727 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-ethoxyethanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1443 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methoxyethanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1636 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methyl-1-propanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1760 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/3-methyl-1-butanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      670 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/DCM.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1335 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/DMF.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1146 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/DMSO.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1638 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/N,N-dimethylacetamide.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1756 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/N-methylpyrrolidone.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1455 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/THF.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      963 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetic_acid.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1149 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetone.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      774 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetonitrile.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1364 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/benzene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2104 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/butylacetate.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      687 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/carbon_tetrachloride.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1370 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/chlorobenzene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      677 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/chloroform.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2218 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/cumene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/cyclohexane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1629 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/diethylether.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2298 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/diisopropylamine.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1054 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethyl_formate.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1534 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethylacetate.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1156 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethyleneglycol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      771 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/formamide.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      678 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/formic_acid.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2384 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/heptane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2098 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/hexane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2108 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isobutyl_acetate.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2671 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isooctane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1343 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1823 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropylacetate.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2201 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropylether.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/meta-xylene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      770 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methanol.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1751 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methoxybenzene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1250 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylacetate.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2014 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylbutylketone.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2229 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylcyclohexane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1444 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylethylketone.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2017 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylisobutylketone.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1733 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylisopropylketone.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1652 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/morpholine.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      869 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/nitromethane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1939 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/ortho-xylene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1938 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/para-xylene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1814 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/pentane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1820 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/propylacetate.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1270 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/pyridine.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1651 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/sulfolane.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1920 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/t-butylmethylether.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2340 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/tetralin.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1649 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/toluene.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/trichloroacetic_acid.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      972 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/trifluoroacetic_acid.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      482 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/solvents/water.mol2
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      195 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/data/units.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/hotpot/tanks/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      217 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/__init__.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     9486 2023-06-19 11:51:27.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/cc.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      161 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/features.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      284 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/__init__.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     8118 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/base.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     8789 2023-06-14 00:55:16.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/gcmc.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     9577 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/materials.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     8286 2023-06-19 12:05:14.000000 hotpot-zzy-0.3.0.0/hotpot/tanks/quantum.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2949 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tmo.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2882 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/tools.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/hotpot/utils/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      134 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/utils/__init__.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1717 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/utils/load_chem_lib.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      669 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       56 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     3854 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       51 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-06-19 12:52:24.000000 hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/top_level.txt
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      314 2023-06-19 12:51:44.000000 hotpot-zzy-0.3.0.0/pyproject.toml
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/setup.cfg
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-19 12:52:24.154557 hotpot-zzy-0.3.0.0/test/
+-rwxrwx---   0 zz1       (1005) zz1       (1008)      550 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/test/test_amorphous_maker.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     1157 2023-06-14 09:02:54.000000 hotpot-zzy-0.3.0.0/test/test_bundle.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     2419 2023-06-16 02:14:06.000000 hotpot-zzy-0.3.0.0/test/test_chemif.py
+-rwxrwx---   0 zz1       (1005) zz1       (1008)     7081 2023-06-13 07:03:55.000000 hotpot-zzy-0.3.0.0/test/test_lmp.py
```

### Comparing `hotpot-zzy-0.2.6/README.md` & `hotpot-zzy-0.3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/_io.py` & `hotpot-zzy-0.3.0.0/hotpot/_io.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/bundle.py` & `hotpot-zzy-0.3.0.0/hotpot/bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/cheminfo.py` & `hotpot-zzy-0.3.0.0/hotpot/cheminfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,24 @@
     The _set_attrs method is used to set any keyword attribute, the attribute names, in the wrapper context, are defined
     by the keys from returned dict of _attr_setters; the values of the returned dict of _attr_setters are a collection
     of specific private method to wrapper and call openbabel method to set the attributes in openbabel object.
     """
     _data = {}  # all attributes of wrappers are stored into
 
     @property
+    def _ob_obj(self) -> Union[ob.OBMol, ob.OBAtom, ob.OBBond, ob.OBAngle, ob.OBUnitCell]:
+        return self._data.get('ob_obj')
+
+    @property
     def _protected_data(self):
         """
         the protected attr in data which could not be replaced by call methods:
             - update_attr_data()
         """
-        return ('ob_object',)
+        return ('ob_obj',)
 
     def _set_attrs(self, **kwargs):
         """    Set any atomic attributes by name    """
         attr_setters = self._attr_setters
         for name, value in kwargs.items():
             setter = attr_setters.get(name)
 
@@ -116,31 +120,57 @@
                 setter(value)
 
     @property
     @abstractmethod
     def _attr_setters(self) -> Dict[str, Callable]:
         raise NotImplemented
 
+    def _get_ob_comment_data(self, data_name: str):
+        """ Retrieve OBCommentData according to specific data_name """
+        comment = self._ob_obj.GetData(data_name)
+        if comment:
+            comment = ob.toCommentData(comment)
+            return comment.GetData()
+        return None
+
     @property
     def data(self) -> dict:
         """ Get the clone of attributes data dict """
         return copy.copy(self._data)
 
     def kwargs_setters(self):
         list_setters = [f'{k}: {s.__doc__}' for k, s in self._attr_setters.items()]
         print("\n".join(list_setters))
 
+    def remove_ob_data(self, data_name: str):
+        """ Remove specific OBData item by given data_name """
+        self._ob_obj.DeleteData(data_name)
+
     def replace_attr_data(self, data: Dict):
         """ Replace the core data dict directly """
         self._data = data
 
+    def set_ob_comment_data(self, attr_name: str, value: str):
+        """ Set the OBCommentData for ob_obj """
+        comment_data = ob.OBCommentData()
+
+        comment_data.SetAttribute(attr_name)
+        comment_data.SetData(value)
+
+        self._ob_obj.CloneData(comment_data)
+
     @property
     def setter_keys(self):
         return list(self._attr_setters.keys())
 
+    @property
+    def temp_label(self):
+        """ Retrieve the temp label """
+        return self._get_ob_comment_data('temp_label')
+
     def update_attr_data(self, data: dict):
         """ update the attribute data by give dict """
         for data_attr in self._protected_data:
             if data.get(data_attr):
                 data.pop(data_attr)
 
         self._data.update(data)
@@ -164,15 +194,15 @@
     )
 
     def __init__(self, ob_mol: ob.OBMol = None, _data: dict = None, **kwargs):
         if _data:
             self._data: dict = _data
         else:
             self._data: dict = {
-                'ob_object': ob_mol if ob_mol else ob.OBMol()
+                'ob_obj': ob_mol if ob_mol else ob.OBMol()
             }
         self._set_attrs(**kwargs)
         self._load_atoms()
         self._load_bonds()
 
     def __repr__(self):
         return f'Mol({self.ob_mol.GetSpacedFormula()})'
@@ -260,14 +290,23 @@
 
     def __eq__(self, other):
         """ if two molecule with 1.0 similarity in 2FP fingerprint they are identical """
         if self.similarity(other) == 1.0:
             return True
         return False
 
+    def _add_temp_atom_labels(self):
+        """
+        Add temp atom label, These label will assist in the implementation of certain functions,
+        say Molecule.components. These label should be deleted after the assisted functions have
+        been fulfilled, by call method _delete_temp_atom_labels(self)
+        """
+        for i, atom in enumerate(self.atoms):
+            atom.set_ob_comment_data('temp_label', str(i))
+
     @staticmethod
     def _assign_coordinates(the_mol: 'Molecule', coordinates: np.ndarray):
         """ Assign coordinates for all atoms in the Molecule """
         if len(the_mol.atoms) != coordinates.shape[-2]:
             raise AttributeError('the coordinate matrix do not match the number of atoms')
 
         for new_mol_atom, new_atom_coord in zip(the_mol.atoms, coordinates):
@@ -293,14 +332,19 @@
         }
 
     def _create_ob_unit_cell(self):
         """ Create New OBUnitCell for the Molecule """
         ob_unit_cell = ob.OBUnitCell()
         self.ob_mol.CloneData(ob_unit_cell)
 
+    def _delete_atom_temp_label(self):
+        """ Remove temp label of all label """
+        for a in self.atoms:
+            a.remove_ob_data('temp_label')
+
     def _get_critical_params(self, name: str):
         critical_params = self._data.get('critical_params')
         if critical_params is None:
             critical_params = json.load(open(ptj(data_root, 'thermo', 'critical.json'))).get(self.smiles)
             if critical_params:
                 self._data['critical_params'] = critical_params
                 return critical_params[name]
@@ -377,24 +421,26 @@
 
         # atoms = {i: atoms.get(i, Atom(self.ob_mol.GetAtomById(i), mol=self)) for i in set_ob_atoms_idx}
 
         self._data['atoms'] = atoms
 
         return atoms
 
-    def _load_bonds(self) -> Dict[int, 'Bond']:
+    def _load_bonds(self) -> Dict[Tuple[int], 'Bond']:
         """
         Construct bonds dict according to the OBBond in the OBMol,
         where the keys of the dict are the ob_id of OBBond and the values are the the constructed Bond objects
         the constructed dict would be place into the _data dict
         Returns:
             dict of bonds
         """
         bonds: Dict = self._data.get('bonds', {})  # Get the stored bonds
-        set_ob_bonds_id = {obb.GetId() for obb in ob.OBMolBondIter(self.ob_mol)}  # Get obBonds
+        set_ob_bonds_id = {
+            obb.GetId() for obb in ob.OBMolBondIter(self.ob_mol)
+        }  # Get obBonds
 
         set_bonds_id = set(bonds.keys())
 
         # Compare the stored bond with the obBonds in obMol
         to_pop_bond_idx = set_bonds_id.difference(set_ob_bonds_id)
 
         # Pop redundant stored bonds
@@ -452,15 +498,15 @@
             for item in items:
                 merge_attr(item)
 
         return self
 
     @property
     def _protected_data(self):
-        return 'ob_object', 'atoms', 'bonds', 'angles'
+        return 'ob_obj', 'atoms', 'bonds', 'angles'
 
     def _reorganize_atom_indices(self):
         """ reorganize or rearrange the indices for all atoms """
         for i, ob_atom in enumerate(ob.OBMolAtomIter(self.ob_mol)):
             ob_atom.SetId(i)
 
     def _set_atoms(self, atoms_kwargs: List[Dict[str, Any]]):
@@ -645,15 +691,15 @@
         if isinstance(atom, str):
             atom = Atom(symbol=atom, **atom_kwargs)
         elif isinstance(atom, int):
             atom = Atom(atomic_number=atom, **atom_kwargs)
         elif isinstance(atom, Atom):
             data = atom.data  # copy the atom's data dict
 
-            data.pop('ob_object')  # delete the ob_atom item in data dict
+            data.pop('ob_obj')  # delete the ob_atom item in data dict
             if data.get('mol'):
                 data.pop('mol')  # delete the _mol item in data dict
 
             atom = Atom(atomic_number=atom.atomic_number)
             atom.update_attr_data(data)
 
         # Avoid add an existed atom into the molecule
@@ -666,15 +712,15 @@
             # Get the last OBAtom
             ob_atom_in_ob_mol = list(ob.OBMolAtomIter(self.ob_mol))[-1]
 
             # Get the attribute dict and replace the 'OBAtom' and 'mol' items
             # The 'OBAtom' is the OBAtom has been stored in the self(Molecule)
             # The 'mol' is the self(Molecule)
             new_atom_data = atom.data
-            new_atom_data['ob_object'] = ob_atom_in_ob_mol
+            new_atom_data['ob_obj'] = ob_atom_in_ob_mol
             new_atom_data['mol'] = self
 
             # replace the attr data dict
             atom = Atom()
             atom.replace_attr_data(new_atom_data)
 
             # add the new atom into atoms list directly
@@ -771,18 +817,22 @@
         return [Angle(self, a_idx) for a_idx in ob.OBMolAngleIter(self.ob_mol)]
 
     def assign_bond_types(self):
         self.ob_mol.PerceiveBondOrders()
 
     def atom(self, id_label: Union[int, str]) -> 'Atom':
         """ get atom by label or idx """
-        if not self.is_labels_unique:
-            print(AttributeError('the molecule atoms labels are not unique!'))
-
         if isinstance(id_label, str):
+
+            if not self.is_labels_unique:
+                raise AttributeError(
+                    'the label is not unique, cannot get atom by label. try to get atom by ob_id '
+                    'or normalize the label before'
+                )
+
             for atom in self.atoms:
                 if atom.label == id_label:
                     return atom
             raise KeyError(f'No atom with label {id_label}')
 
         elif isinstance(id_label, int):
             return self.atoms_dict[id_label]
@@ -879,15 +929,15 @@
 
     @property
     def bonds(self):
         bonds = self._load_bonds()
         return list(bonds.values())
 
     @property
-    def bonds_dict(self):
+    def bonds_dict(self) -> Dict[Tuple[int], 'Bond']:
         return self._load_bonds()
 
     def build_bonds(self):
         self.ob_mol.ConnectTheDots()
 
     def build_conformer(self, force_field: str = 'UFF', steps: int = 50):
         """ build 3D coordinates for the molecule """
@@ -926,39 +976,28 @@
 
         if pop:
             return all_coordinates
 
     @property
     def components(self):
         """ get all fragments don't link each by any bonds """
-        if not self.has_3d:
-            self.build_conformer()
-
-        # split to fragment
-        separated_obmol = self.ob_mol.Separate()
-        components = [Molecule(ob_mol) for ob_mol in separated_obmol]
-
-        # match parents_atoms to children atoms
-        atoms = self.atoms
-        parent_atoms_coordinates = [a.coordinates for a in atoms]
-        match_atoms: Dict[Atom, Atom] = \
-            {atoms[parent_atoms_coordinates.index(a.coordinates)]: a for c in components for a in c.atoms}
-
-        # transfer the parent atoms attribute to the children
-        for pa, ca in match_atoms.items():
-            ca_data = ca.data()
-            pa_data = pa.data()
-
-            # Remove the ob_atom and molecule information
-            pa_data.pop('ob_object')
-            pa_data.pop('mol')
+        # Add temp label for each atom first
+        self._add_temp_atom_labels()
+        parent_atom_dict = {a.temp_label: a.data for a in self.atoms}
+
+        components = [self.__class__(obc) for obc in self.ob_mol.Separate()]
+
+        # Transfer the parent data attr to the children
+        for c in components:
+            for a in c.atoms:
+                a.update_attr_data(parent_atom_dict[a.temp_label])
+                a.remove_ob_data('temp_label')
 
-            ca_data.update(pa_data)
-
-            ca.replace_attr_data(ca_data)
+        # remove temp labels of all atoms
+        self._delete_atom_temp_label()
 
         return components
 
     @property
     def configure_number(self):
         all_coordinates = self._data.get('all_coordinates')
         if isinstance(all_coordinates, np.ndarray):
@@ -1007,64 +1046,29 @@
         """
         return np.array([atom.coordinates for atom in self.atoms], dtype=np.float64)
 
     def copy(self) -> 'Molecule':
         """ Get a clone of this Molecule """
         clone = Molecule(self.ob_copy())
         clone._load_atoms()
-        clone._load_atoms()
+        clone._load_bonds()
 
         # Copy the Molecule's attr data to the clone one
         clone.update_attr_data(self.data)
         # Copy the Atoms' attr data to the clone ones
         for atom in clone.atoms:
             atom.update_attr_data(self.atoms_dict[atom.ob_id].data)
             atom.molecule = clone
         # Copy the Bonds' attr data to the lone ones
-        for bond in clone.atoms:
+        for bond in clone.bonds:
             bond.update_attr_data(self.bonds_dict[bond.ob_id].data)
             bond.molecule = clone
 
         return clone
 
-    # TODO: Discarding in last version
-    def copy1(self) -> 'Molecule':
-        """ Copy the Molecule """
-        # Create the new data sheet
-        new_data = {
-            'ob_object': ob.OBMol(),
-            'atoms': {},
-            'bonds': {}
-        }
-
-        # Copy all attribute except for 'OBMol', 'atoms' and 'bonds'
-        for name, value in self._data.items():
-            if name not in new_data:
-                new_data[name] = copy.copy(value)
-
-        # Create new Molecule
-        clone_mol = self.__class__()
-        clone_mol._data = new_data
-        clone_mol.identifier = self.identifier
-
-        # Clone the old UnitCell data into new
-        cell_data = self.ob_mol.GetData(12)  # the UnitCell of OBmol save with idx 12
-        if cell_data:
-            clone_mol.ob_mol.CloneData(cell_data)
-
-        # copy, in turn, each Atom in this molecule and add them into new Molecule
-        for atom in self.atoms:
-            clone_mol.add_atom(atom)
-
-        # generate Bonds in new Molecule with same graph pattern in this Molecule
-        for bond in self.bonds:
-            clone_mol.add_bond(bond.atom1.label, bond.atom2.label, bond_type=bond.type)
-
-        return clone_mol
-
     def compact_crystal(self, inplace=False):
         """"""
         mol = self if inplace else self.copy()
         lattice_params = np.concatenate((self.xyz_diff, [90., 90., 90.]))
 
         mol.make_crystal(*lattice_params)
 
@@ -1283,24 +1287,24 @@
         if not self.has_3d:
             self.build_conformer()
 
         # Make the input gjf script
         script = self.dump('gjf', *args, link0=link0, route=route, **kwargs)
 
         # Run Gaussian16
-        gaussian = Gaussian(g16root)
-        stdout, stderr = gaussian.run(script, args, **kwargs)
+        with Gaussian(g16root) as gaussian:
+            stdout, stderr = gaussian.run(script, args, **kwargs)
 
-        # save the calculate result into the molecule data dict
-        self._data['gaussian_output'] = stdout
-        self._data['gaussian_parse_data'] = gaussian.data
-
-        # Inplace the self attribute according to the result from gaussian
-        if inplace_attrs:
-            self._set_attrs(**gaussian.molecule_setter_dict)
+            # save the calculate result into the molecule data dict
+            self._data['gaussian_output'] = stdout
+            self._data['gaussian_parse_data'] = gaussian.data
+
+            # Inplace the self attribute according to the result from gaussian
+            if inplace_attrs:
+                self._set_attrs(**gaussian.molecule_setter_dict)
 
         # Save log file
         if path_log_file:
             with open(path_log_file, 'w') as writer:
                 writer.write(stdout)
 
         # Save error file
@@ -1345,19 +1349,15 @@
             metal_symbol: which metal element link to the ligand
             acceptor_atoms: which elements to be acceptor atom to link to metal
             opti_force_field: which force field could be used to optimize the configuration of ligand and M-L pair.
 
         Return:
             A generator for M-L pair
         """
-        # self.normalize_labels()
         ligand = self.copy()
-        ligand.localed_optimize(opti_force_field)  # locally optimize the ligand
-        # ligand.normalize_labels()
-
         for atom in ligand.atoms:
             if atom.symbol in acceptor_atoms:
                 # copy the ligand as the embryo of metal-ligand pairs
                 pair = ligand.copy()
 
                 # Replace the correspondent atom in the pair embryo, i.e., the accepting atom
                 acc_atom = pair.atom(atom.ob_id)
@@ -1381,17 +1381,14 @@
                 while acc_atom.valence > acc_atom.valence_max and acc_atom.neighbours_hydrogen:
                     pair.remove_atoms(acc_atom.neighbours_hydrogen[0], remove_hydrogens=True)
 
                 # localize optimization of M-L pair by classical force field, if the pair has 3d
                 if pair.has_3d:
                     pair.localed_optimize(opti_force_field)
 
-                # TODO: must refresh the property of ligands, otherwise, the program could break out with unknown reason
-                # TODO: identifying for cause is needed in the later.
-                # _ = ligand.smiles
                 pair.identifier = pair.smiles
 
                 yield pair
 
     def generate_pairs_bundle(
             self, metal_symbol: str, acceptor_atoms: Sequence = ('O',), opti_force_field: str = 'UFF'
     ) -> 'PairBundle':
@@ -1470,44 +1467,44 @@
 
     def ob_copy(self):
         """ Return a clone of OBMol of the Molecule """
         return ob.OBMol(self.ob_mol)
 
     @property
     def ob_mol(self):
-        return self._data['ob_object']
+        return self._data['ob_obj']
 
     def ob_mol_pop(self):
         data: dict = self._data
 
         atoms: Dict[int, Atom] = data.get('atoms')
         if atoms:
             for ob_id, atom in atoms.items():
                 atom.ob_atom_pop()
 
         bonds: Dict[int, Bond] = data.get('bonds')
         if bonds:
             for ob_idx, bond in bonds.items():
                 bond.ob_bond_pop()
 
-        return self._data.pop('ob_object')
+        return self._data.pop('ob_obj')
 
     def ob_mol_rewrap(self, ob_mol: ob.OBMol):
         if not isinstance(ob_mol, ob.OBMol):
             raise TypeError('the ob_mol should be OBMol object')
 
         atoms = self._data.get('atoms')
         bonds = self._data.get('bonds')
 
         if any(oba.GetId() not in atoms for oba in ob.OBMolAtomIter(ob_mol)):
             raise ValueError('the atom number between the wrapper and the core OBMol is not match')
         if any(obb.GetIdx() not in bonds for obb in ob.OBMolBondIter(ob_mol)):
             raise ValueError('the bond number between the wrapper and the core OBMol is not match')
 
-        self._data['ob_object'] = ob_mol
+        self._data['ob_obj'] = ob_mol
         for ob_atom in ob.OBMolAtomIter(ob_mol):
             atom = atoms.get(ob_atom.GetId())
             atom.ob_atom_rewrap(ob_atom)
 
         for ob_bond in ob.OBMolBondIter(ob_mol):
             bond = bonds.get(ob_bond.GetIdx())
             bond.ob_bond_rewrap(ob_bond)
@@ -2058,40 +2055,40 @@
     def __init__(
             self,
             ob_atom: ob.OBAtom = None,
             **kwargs
     ):
         # Contain all data to reappear this Atom
         self._data: Dict[str, Any] = {
-            'ob_object': ob_atom if ob_atom else ob.OBAtom(),
+            'ob_obj': ob_atom if ob_atom else ob.OBAtom(),
         }
 
         self._set_attrs(**kwargs)
 
     def __eq__(self, other):
         if isinstance(other, Atom):
             # return self.symbol == other.symbol
             return self.ob_atom == other.ob_atom
 
     def __hash__(self):
         return hash(f'Atom({self.atomic_number})')
 
     @property
     def ob_atom(self):
-        return self._data['ob_object']
+        return self._data['ob_obj']
 
     @ob_atom.setter
     def ob_atom(self, oba):
-        self._data['ob_object'] = oba
+        self._data['ob_obj'] = oba
 
     def ob_atom_pop(self):
-        return self._data.pop('ob_object')
+        return self._data.pop('ob_obj')
 
     def ob_atom_rewrap(self, ob_atom):
-        self._data['ob_object'] = ob_atom
+        self._data['ob_obj'] = ob_atom
 
     def __repr__(self):
         return f"Atom({self.label if self.label else self.symbol})"
 
     @property
     def _attr_setters(self) -> Dict[str, Callable]:
         return {
@@ -2130,15 +2127,20 @@
 
         self._data['force_vector'] = force_vector
 
     def _set_ob_id(self, ob_id):
         self.ob_atom.SetId(ob_id)
 
     def _set_label(self, label):
-        self._data['label'] = label
+        label_data = ob.OBCommentData()
+
+        label_data.SetAttribute('label')
+        label_data.SetData(label)
+
+        self.ob_atom.CloneData(label_data)
 
     def _set_molecule(self, molecule: Molecule):
         self._data['mol'] = molecule
 
     def _set_partial_charge(self, charge):
         self.ob_atom.SetPartialCharge(charge)
 
@@ -2172,15 +2174,15 @@
         """ the array of coordinates """
         return np.array(self.coordinates)
 
     def copy(self):
         """ Make a copy of self """
         # Extract old data
         data = self.data
-        data.pop('ob_object')  # Remove the old OBAtom
+        data.pop('ob_obj')  # Remove the old OBAtom
         # Remove molecule if the parent atom in a molecule
         if self.molecule:
             data.pop('mol')
 
         # Copy the information contained in OBAtom
         new_attrs = {
             "atomic_number": self.atomic_number,
@@ -2313,15 +2315,21 @@
 
     @property
     def is_metal(self):
         return self.ob_atom.IsMetal()
 
     @property
     def label(self):
-        return self._data.get('label', self.symbol)
+        label_data = self.ob_atom.GetData('label')
+
+        if label_data:
+            label_data = ob.toCommentData(label_data)
+            return label_data.GetValue()
+        else:
+            return self.symbol
 
     @label.setter
     def label(self, value):
         self._set_label(value)
 
     @property
     def link_degree(self) -> int:
@@ -2459,15 +2467,15 @@
 
 
 class Bond(Wrapper, ABC):
     """"""
 
     def __init__(self, ob_bond: ob.OBBond, _mol: Molecule):
         self._data = {
-            'ob_object': ob_bond,
+            'ob_obj': ob_bond,
             'mol': _mol
         }
 
     def __repr__(self):
         return f"Bond({self.atoms[0].label}, {self.atoms[1].label}, {self.type_name})"
 
     def __eq__(self, other: 'Bond'):
@@ -2475,21 +2483,21 @@
             return self.pair_key == other.pair_key
 
     def __hash__(self):
         return hash(self.pair_key)
 
     @property
     def ob_bond(self):
-        return self._data['ob_object']
+        return self._data['ob_obj']
 
     def ob_bond_pop(self):
-        return self._data.pop('ob_object')
+        return self._data.pop('ob_obj')
 
     def ob_bond_rewrap(self, ob_bond):
-        self._data['ob_object'] = ob_bond
+        self._data['ob_obj'] = ob_bond
 
     @property
     def _attr_setters(self) -> Dict[str, Callable]:
         return {
         }
 
     @property
@@ -2509,15 +2517,15 @@
         return self.ob_bond.GetEndAtom().GetAtomicNum()
 
     @property
     def atoms(self):
         return self.atom1, self.atom2
 
     @property
-    def begin_end_ob_id(self):
+    def begin_end_ob_id(self) -> (int, int):
         return self.ob_bond.GetBeginAtom().GetId(), self.ob_bond.GetEndAtom().GetId()
 
     @property
     def begin_end_atomic_number(self):
         return self.ob_bond.GetBeginAtom().GetAtomicNum(), self.ob_bond.GetEndAtom().GetAtomicNum()
 
     @property
```

### Comparing `hotpot-zzy-0.2.6/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.3.0.0/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.3.0.0/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/periodic_table.json` & `hotpot-zzy-0.3.0.0/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,1,1-trichloroethane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,1-trichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,1,1-trifluroethanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,1-trifluroethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,1,2-trichloroethene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1,2-trichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,1-dichloroethene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,1-diethoxypropane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-diethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,1-dimethoxymethane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,1-dimethoxymethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,2-dichloroethane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,2-dichloroethene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,2-dimethoxyethane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,2-dimethoxyethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1,4-dioxane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1,4-dioxane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1-butanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1-pentanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-pentanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/1-propanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/2,2-dimethoxypropane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2,2-dimethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/2-butanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/2-ethoxyethanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-ethoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/2-methoxyethanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/2-methyl-1-propanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methyl-1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/2-methyltetrahydrofuran.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/2-methyltetrahydrofuran.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/3-methyl-1-butanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/3-methyl-1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/DCM.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/DCM.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/DMF.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/DMF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/DMSO.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/DMSO.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/N,N-dimethylacetamide.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/N,N-dimethylacetamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/N-methylpyrrolidone.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/N-methylpyrrolidone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/THF.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/THF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/acetic_acid.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/acetone.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/acetonitrile.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/acetonitrile.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/benzene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/benzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/butylacetate.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/butylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/carbon_tetrachloride.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/carbon_tetrachloride.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/chlorobenzene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/chlorobenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/chloroform.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/chloroform.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/cumene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/cumene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/cyclohexane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/cyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/diethylether.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/diethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/diisopropylamine.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/diisopropylamine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/ethanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/ethyl_formate.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethyl_formate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/ethylacetate.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/ethyleneglycol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ethyleneglycol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/formamide.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/formamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/formic_acid.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/formic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/heptane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/heptane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/hexane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/hexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/isobutyl_acetate.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isobutyl_acetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/isooctane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isooctane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/isopropanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/isopropylacetate.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/isopropylether.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/isopropylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/meta-xylene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/meta-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/methanol.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/methoxybenzene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methoxybenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/methylacetate.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/methylbutylketone.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylbutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/methylcyclohexane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylcyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/methylethylketone.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylethylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/methylisobutylketone.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylisobutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/methylisopropylketone.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/methylisopropylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/morpholine.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/morpholine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/nitromethane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/nitromethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/ortho-xylene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/ortho-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/para-xylene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/para-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/pentane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/pentane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/propylacetate.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/propylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/pyridine.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/pyridine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/sulfolane.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/sulfolane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/t-butylmethylether.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/t-butylmethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/tetralin.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/tetralin.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/toluene.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/toluene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/trichloroacetic_acid.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/trichloroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/data/solvents/trifluoroacetic_acid.mol2` & `hotpot-zzy-0.3.0.0/hotpot/data/solvents/trifluoroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.3.0.0/hotpot/tanks/lmp/materials.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/tanks/quantum.py` & `hotpot-zzy-0.3.0.0/hotpot/tanks/quantum.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,24 @@
             self.g16root = str(g16root)
         else:
             raise TypeError('the g16root should be str or os.PathLike type!')
 
         self.envs = self._set_environs()
         self._set_resource_limits(report_set_resource_error)
 
-        self.data = None
+        self.data = None  # to receive the data from the cclib parser
+        self.g16process = None  # to link to the g16 subprocess
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        print(f'{exc_type}, {exc_val}, {exc_tb}, {self.g16process.poll()}')
+        if self.g16process.poll():
+            self.g16process.kill()
 
     def _set_environs(self):
         """Sets up the environment variables required for running Gaussian 16.
 
         This method sets the environment variables required for Gaussian 16 to function correctly. If the
         `g16root` attribute is not set, the method sets it to the user's home directory.
 
@@ -157,20 +166,20 @@
             *args: Additional arguments to pass to subprocess.Popen.
             **kwargs: Additional keyword arguments to pass to subprocess.Popen.
 
         Returns:
             Tuple[str, str]: A tuple of the standard output and standard error of the process.
         """
         # Run Gaussian using subprocess
-        g16_process = subprocess.Popen(
+        self.g16process = subprocess.Popen(
             'g16', bufsize=-1, stdin=subprocess.PIPE,
             stdout=subprocess.PIPE, stderr=subprocess.PIPE,
             env=self.envs, universal_newlines=True
         )
-        stdout, stderr = g16_process.communicate(script)
+        stdout, stderr = self.g16process.communicate(script)
 
         self.parse_log(stdout)
 
         return stdout, stderr
 
     def parse_log(self, stdout: str):
         """ Parse the gaussian log file and save them into self """
```

### Comparing `hotpot-zzy-0.2.6/hotpot/tmo.py` & `hotpot-zzy-0.3.0.0/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/tools.py` & `hotpot-zzy-0.3.0.0/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/utils/load_chem_lib.py` & `hotpot-zzy-0.3.0.0/hotpot/utils/load_chem_lib.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot/utils/units_convert.py` & `hotpot-zzy-0.3.0.0/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/hotpot_zzy.egg-info/SOURCES.txt` & `hotpot-zzy-0.3.0.0/hotpot_zzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/test/test_amorphous_maker.py` & `hotpot-zzy-0.3.0.0/test/test_amorphous_maker.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/test/test_bundle.py` & `hotpot-zzy-0.3.0.0/test/test_bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/test/test_chemif.py` & `hotpot-zzy-0.3.0.0/test/test_chemif.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.6/test/test_lmp.py` & `hotpot-zzy-0.3.0.0/test/test_lmp.py`

 * *Files identical despite different names*

