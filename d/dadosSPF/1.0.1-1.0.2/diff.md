# Comparing `tmp/dadosSPF-1.0.1.tar.gz` & `tmp/dadosSPF-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dadosSPF-1.0.1.tar", last modified: Tue Jun 13 13:23:37 2023, max compression
+gzip compressed data, was "dist/dadosSPF-1.0.2.tar", last modified: Mon Jun 19 14:29:51 2023, max compression
```

## Comparing `dadosSPF-1.0.1.tar` & `dadosSPF-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      781 2023-06-13 13:23:21.000000 dadosSPF-1.0.1/README.md
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.1/dadosSPF/__init__.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)    37006 2023-06-13 13:21:19.000000 dadosSPF-1.0.1/dadosSPF/dadosSPF.py
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1328 2023-06-13 13:22:55.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-13 13:21:19.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      459 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/top_level.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/setup.cfg
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      533 2023-06-13 13:23:28.000000 dadosSPF-1.0.1/setup.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      781 2023-06-13 13:23:21.000000 dadosSPF-1.0.2/README.md
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/dadosSPF/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.2/dadosSPF/__init__.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)    37018 2023-06-19 14:26:52.000000 dadosSPF-1.0.2/dadosSPF/dadosSPF.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/dadosSPF.egg-info/
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1328 2023-06-13 13:22:55.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-13 13:21:19.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      528 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/top_level.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/setup.cfg
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      545 2023-06-19 14:27:45.000000 dadosSPF-1.0.2/setup.py
```

### Comparing `dadosSPF-1.0.1/PKG-INFO` & `dadosSPF-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.1/README.md` & `dadosSPF-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.1/dadosSPF/dadosSPF.py` & `dadosSPF-1.0.2/dadosSPF/dadosSPF.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ =     "CARLOS PIVETA"
 __collaborators__ = "CARLOS PIVETA"
 __license__ =    "DADOS"
-__version__ =    "1.0.1"
+__version__ =    "1.0.2"
 __maintainer__ = "CARLOS PIVETA"
 __status__ =     "Production"
 
 import os
 import re
 import sys
 import glob
@@ -626,15 +626,15 @@
         
         hora = str(datetime.now()+timedelta(hours=-3)).replace('-','').replace(':','').replace(' ','_')[:15]
         arquivo = "{}{}_{}.csv".format(caminhoArquivo,nomeArquivo,hora)
         try:
             if tpDf.upper() == 'SPARK':
                     df.coalesce(1).write.option('header', 'True').format('csv').save(arquivo)
             elif tpDf.upper() == 'PANDAS':
-                    df.to_csv(arquivo, sep=';')
+                    df.to_csv(arquivo, sep=';',index=False)
             else:
                 raise ValueError("ERRO! Formato NÃO suportado !!!")
             print("csv {} salvo !!!".format(nomeArquivo))   
         except Exception as e:
             print("ERRO! csv {} NÃO salvo !!!".format(nomeArquivo))
             print(e)
```

### Comparing `dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.1/dadosSPF.egg-info/PKG-INFO` & `dadosSPF-1.0.2/dadosSPF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.1/setup.py` & `dadosSPF-1.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='dadosSPF',
-    version='1.0.1',
+    version='1.0.2',
     url='https://gitlab.com.br/dadosSPF',
     license='MIT License',
     author='Carlos Piveta',
 	long_description=readme,
     long_description_content_type="text/markdown",
     author_email='cepo496@gmail.com',
     keywords='Pacote',
     description='Pacote de funções uteis para o desenvolvimento na cloudera',
     packages=['dadosSPF'],
-    install_requires=['pandas','impyla','holidays']
+    install_requires=['pandas','impyla','holidays','unidecode']
 )
```

