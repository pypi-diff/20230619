# Comparing `tmp/astropy-iers-data-0.2023.6.15.21.10.12.tar.gz` & `tmp/astropy-iers-data-0.2023.6.19.1.16.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astropy-iers-data-0.2023.6.15.21.10.12.tar", last modified: Thu Jun 15 21:11:22 2023, max compression
+gzip compressed data, was "astropy-iers-data-0.2023.6.19.1.16.11.tar", last modified: Mon Jun 19 01:17:21 2023, max compression
```

## Comparing `astropy-iers-data-0.2023.6.15.21.10.12.tar` & `astropy-iers-data-0.2023.6.19.1.16.11.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:22.781683 astropy-iers-data-0.2023.6.15.21.10.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-15 21:11:22.777683 astropy-iers-data-0.2023.6.15.21.10.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:22.769682 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-15 21:11:22.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:22.773682 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/Leap_Second.dat
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/ReadMe.eopc04
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/ReadMe.finals2000A
--rw-r--r--   0 runner    (1001) docker     (123)  4909837 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/eopc04.1962-now
--rw-r--r--   0 runner    (1001) docker     (123)  3543800 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/finals2000A.all
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:22.777683 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:11:22.769682 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-15 21:11:22.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-15 21:11:22.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:11:22.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 21:11:22.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 21:11:22.000000 astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:11:22.781683 astropy-iers-data-0.2023.6.15.21.10.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-15 21:11:03.000000 astropy-iers-data-0.2023.6.15.21.10.12/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:17:21.100783 astropy-iers-data-0.2023.6.19.1.16.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-19 01:17:21.100783 astropy-iers-data-0.2023.6.19.1.16.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:17:21.088783 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-19 01:17:20.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:17:21.096783 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/Leap_Second.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/ReadMe.eopc04
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/ReadMe.finals2000A
+-rw-r--r--   0 runner    (1001) docker     (123)  4910494 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/eopc04.1962-now
+-rw-r--r--   0 runner    (1001) docker     (123)  3543800 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/finals2000A.all
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:17:21.100783 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:17:21.092783 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-19 01:17:21.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-19 01:17:21.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 01:17:21.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 01:17:21.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 01:17:21.000000 astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 01:17:21.100783 astropy-iers-data-0.2023.6.19.1.16.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-19 01:17:00.000000 astropy-iers-data-0.2023.6.19.1.16.11/tox.ini
```

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/LICENSE.rst` & `astropy-iers-data-0.2023.6.19.1.16.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/PKG-INFO` & `astropy-iers-data-0.2023.6.19.1.16.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astropy-iers-data
-Version: 0.2023.6.15.21.10.12
+Version: 0.2023.6.19.1.16.11
 Summary: IERS Earth Rotation and Leap Second tables for the astropy core package
 Author-email: Astropy Developers <astropy.team@gmail.com>
 License: Copyright (c) 2023, Astropy Developers
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/README.rst` & `astropy-iers-data-0.2023.6.19.1.16.11/README.rst`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/__init__.py` & `astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/__init__.py`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/Leap_Second.dat` & `astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/Leap_Second.dat`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/ReadMe.eopc04` & `astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/ReadMe.eopc04`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/ReadMe.finals2000A` & `astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/ReadMe.finals2000A`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/eopc04.1962-now` & `astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/eopc04.1962-now`

 * *Files 0% similar despite different names*

```diff
@@ -22387,15 +22387,15 @@
 2023   4  11   0  60045.00   -0.004073    0.431351  -0.0290184    0.000282    0.000065    0.001211    0.002627   0.0000866    0.000059    0.000053   0.0000390    0.000071    0.000083    0.000072    0.000067   0.0000242
 2023   4  12   0  60046.00   -0.002903    0.434183  -0.0290346    0.000308    0.000070    0.000922    0.002788  -0.0000344    0.000057    0.000053   0.0000396    0.000074    0.000088    0.000072    0.000073   0.0000237
 2023   4  13   0  60047.00   -0.002436    0.436715  -0.0289857    0.000337    0.000028    0.000425    0.002499  -0.0000349    0.000057    0.000057   0.0000333    0.000075    0.000083    0.000075    0.000083   0.0000223
 2023   4  14   0  60048.00   -0.001750    0.439264  -0.0290056    0.000359   -0.000027    0.000681    0.002527   0.0001070    0.000059    0.000060   0.0000263    0.000076    0.000073    0.000078    0.000086   0.0000228
 2023   4  15   0  60049.00   -0.001196    0.441724  -0.0292618    0.000350   -0.000046    0.000823    0.002234   0.0003882    0.000065    0.000061   0.0000198    0.000075    0.000068    0.000085    0.000084   0.0000217
 2023   4  16   0  60050.00    0.000214    0.443555  -0.0298215    0.000317   -0.000053    0.001587    0.001700   0.0007070    0.000071    0.000063   0.0000158    0.000068    0.000061    0.000085    0.000081   0.0000226
 2023   4  17   0  60051.00    0.001716    0.445308  -0.0306441    0.000280   -0.000052    0.001430    0.001697   0.0009188    0.000067    0.000060   0.0000133    0.000063    0.000052    0.000075    0.000078   0.0000231
-2023   4  18   0  60052.00    0.002942    0.446930  -0.0316096    0.000249   -0.000049    0.001235    0.001626   0.0009803    0.000068    0.000058   0.0000121    0.000058    0.000046    0.000070    0.000081   0.0000235
+2023   4  18   0  60052.00    0.002942    0.446930  -0.0316096    0.000249   -0.000050    0.001235    0.001626   0.0009803    0.000068    0.000058   0.0000121    0.000058    0.000046    0.000070    0.000081   0.0000235
 2023   4  19   0  60053.00    0.004306    0.448627  -0.0325371    0.000260   -0.000054    0.001416    0.001755   0.0008834    0.000064    0.000054   0.0000117    0.000067    0.000051    0.000066    0.000079   0.0000223
 2023   4  20   0  60054.00    0.005723    0.450456  -0.0333578    0.000289   -0.000060    0.001529    0.001976   0.0007316    0.000063    0.000053   0.0000108    0.000082    0.000061    0.000063    0.000076   0.0000230
 2023   4  21   0  60055.00    0.007430    0.452633  -0.0339749    0.000321   -0.000060    0.001766    0.002358   0.0004803    0.000061    0.000057   0.0000099    0.000096    0.000070    0.000061    0.000075   0.0000231
 2023   4  22   0  60056.00    0.009155    0.455143  -0.0342997    0.000333   -0.000028    0.001670    0.002638   0.0001878    0.000057    0.000056   0.0000094    0.000092    0.000067    0.000062    0.000077   0.0000221
 2023   4  23   0  60057.00    0.010695    0.457843  -0.0343744    0.000334    0.000015    0.001640    0.002760  -0.0000276    0.000053    0.000055   0.0000091    0.000078    0.000058    0.000060    0.000079   0.0000225
 2023   4  24   0  60058.00    0.012615    0.460612  -0.0342760    0.000332    0.000047    0.002125    0.002635  -0.0001638    0.000053    0.000054   0.0000088    0.000063    0.000048    0.000060    0.000079   0.0000235
 2023   4  25   0  60059.00    0.014950    0.462927  -0.0340746    0.000331    0.000056    0.002422    0.002163  -0.0002294    0.000052    0.000051   0.0000087    0.000053    0.000041    0.000058    0.000077   0.0000226
@@ -22416,7 +22416,10 @@
 2023   5  10   0  60074.00    0.043548    0.484305  -0.0381955    0.000419   -0.000201    0.001754    0.001513   0.0001209    0.000059    0.000056   0.0000119    0.000069    0.000080    0.000063    0.000077   0.0000243
 2023   5  11   0  60075.00    0.045281    0.485514  -0.0383861    0.000400   -0.000164    0.001829    0.001111   0.0002941    0.000058    0.000053   0.0000124    0.000072    0.000086    0.000065    0.000082   0.0000261
 2023   5  12   0  60076.00    0.047344    0.486618  -0.0388214    0.000381   -0.000124    0.002128    0.001101   0.0005745    0.000060    0.000054   0.0000123    0.000075    0.000091    0.000067    0.000077   0.0000252
 2023   5  13   0  60077.00    0.049455    0.487750  -0.0395385    0.000396   -0.000115    0.002367    0.001214   0.0008647    0.000063    0.000053   0.0000123    0.000077    0.000094    0.000071    0.000075   0.0000240
 2023   5  14   0  60078.00    0.052341    0.489096  -0.0405378    0.000425   -0.000123    0.003216    0.001445   0.0011312    0.000066    0.000051   0.0000125    0.000082    0.000098    0.000070    0.000073   0.0000243
 2023   5  15   0  60079.00    0.055853    0.490619  -0.0417757    0.000448   -0.000134    0.003551    0.001600   0.0013088    0.000060    0.000051   0.0000132    0.000087    0.000103    0.000071    0.000072   0.0000251
 2023   5  16   0  60080.00    0.059171    0.492264  -0.0430984    0.000452   -0.000140    0.003165    0.001518   0.0012961    0.000056    0.000053   0.0000143    0.000091    0.000107    0.000068    0.000069   0.0000254
+2023   5  17   0  60081.00    0.062111    0.493466  -0.0442928    0.000382   -0.000115    0.002699    0.001107   0.0010916    0.000055    0.000052   0.0000144    0.000101    0.000118    0.000064    0.000071   0.0000246
+2023   5  18   0  60082.00    0.064515    0.494600  -0.0452544    0.000291   -0.000082    0.002295    0.001120   0.0008148    0.000053    0.000051   0.0000143    0.000116    0.000136    0.000063    0.000067   0.0000257
+2023   5  19   0  60083.00    0.066867    0.495722  -0.0459063    0.000212   -0.000051    0.002389    0.001051   0.0004982    0.000054    0.000050   0.0000144    0.000129    0.000151    0.000063    0.000066   0.0000266
```

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data/data/finals2000A.all` & `astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data/data/finals2000A.all`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data.egg-info/PKG-INFO` & `astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astropy-iers-data
-Version: 0.2023.6.15.21.10.12
+Version: 0.2023.6.19.1.16.11
 Summary: IERS Earth Rotation and Leap Second tables for the astropy core package
 Author-email: Astropy Developers <astropy.team@gmail.com>
 License: Copyright (c) 2023, Astropy Developers
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/astropy_iers_data.egg-info/SOURCES.txt` & `astropy-iers-data-0.2023.6.19.1.16.11/astropy_iers_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/pyproject.toml` & `astropy-iers-data-0.2023.6.19.1.16.11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.15.21.10.12/tox.ini` & `astropy-iers-data-0.2023.6.19.1.16.11/tox.ini`

 * *Files identical despite different names*

