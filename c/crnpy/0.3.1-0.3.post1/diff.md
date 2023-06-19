# Comparing `tmp/crnpy-0.3.1.tar.gz` & `tmp/crnpy-0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crnpy-0.3.1.tar", last modified: Mon Jun 19 19:16:47 2023, max compression
+gzip compressed data, was "crnpy-0.3.post1.tar", last modified: Fri Jun 16 23:49:30 2023, max compression
```

## Comparing `crnpy-0.3.1.tar` & `crnpy-0.3.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:16:47.348236 crnpy-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-19 19:16:30.000000 crnpy-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-19 19:16:47.348236 crnpy-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-19 19:16:30.000000 crnpy-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:16:47.348236 crnpy-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-19 19:16:30.000000 crnpy-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:16:47.344236 crnpy-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:16:47.348236 crnpy-0.3.1/src/crnpy/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-19 19:16:30.000000 crnpy-0.3.1/src/crnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53443 2023-06-19 19:16:30.000000 crnpy-0.3.1/src/crnpy/crnpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-19 19:16:30.000000 crnpy-0.3.1/src/crnpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:16:47.348236 crnpy-0.3.1/src/crnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-19 19:16:47.000000 crnpy-0.3.1/src/crnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-19 19:16:47.000000 crnpy-0.3.1/src/crnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:16:47.000000 crnpy-0.3.1/src/crnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 19:16:47.000000 crnpy-0.3.1/src/crnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 23:49:21.000000 crnpy-0.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 23:49:30.905187 crnpy-0.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-16 23:49:21.000000 crnpy-0.3.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 23:49:30.905187 crnpy-0.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-16 23:49:21.000000 crnpy-0.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.901188 crnpy-0.3.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/src/crnpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53443 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/crnpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/src/crnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/top_level.txt
```

### Comparing `crnpy-0.3.1/LICENSE` & `crnpy-0.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `crnpy-0.3.1/PKG-INFO` & `crnpy-0.3.post1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 Metadata-Version: 2.1
 Name: crnpy
-Version: 0.3.1
-Summary: A Python package for processing cosmic ray neutron data.
-Home-page: https://github.com/soilwater/crnpy
-Author: Joaquin Peraza, Andres Patrignani
-Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
-License: MIT
+Version: 0.3.post1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
-<img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
+<img src="/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from Cosmic-Ray Neutron Probes (CRNP) into accurate field-level soil moisture data.
 
 This library has been developed with the intent of providing a comprehensive yet easy-to-use workflow for processing raw data from a variety of CRNP, encompassing multiple manufacturers and models.
 
 ## Key Features
 - Versatility: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 - Modularity: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
-- Instrument agnostic: It can be used with any CRNP, allowing users to process data from multiple instruments with their own workflow.
+- Accuracy: The library shows excellent agreement with ground-based measurements, making it a reliable tool for scientific research and practical applications.
 - Correction Routines: The correction functions of the library have been effectively used to represent field and watershed scale soil moisture conditions.
 
-![CRNPy Processing Workflow](https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/workflow.png)
+![CRNPy Processing Workflow](docs/img/workflow.png)
 Overview of the proposed CRNPy processing workflow. Final user can choose to use the entire workflow, part of it, or build functions on top of it depending on their needs, dashed lines indicate optional steps.
 
 
 ## Installation
 
 To install the CRNPy library, you can use Python's package manager, pip. Simply open your command line or terminal and type:
 
 ```pip install crnpy```
 
 ## Authors
+The CRNPy library was conceived and developed by Joaquin Peraza and Andres Patrignani in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
 
-The CRNPy library was developed by:
-
-- Joaquin Peraza
-- Andres Patrignani
-
-in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
-
-The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. The authors would like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
+The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
```

### Comparing `crnpy-0.3.1/README.md` & `crnpy-0.3.post1/src/crnpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
+Metadata-Version: 2.1
+Name: crnpy
+Version: 0.3.post1
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
-<img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
+<img src="/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from Cosmic-Ray Neutron Probes (CRNP) into accurate field-level soil moisture data.
 
 This library has been developed with the intent of providing a comprehensive yet easy-to-use workflow for processing raw data from a variety of CRNP, encompassing multiple manufacturers and models.
 
 ## Key Features
 - Versatility: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 - Modularity: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
-- Instrument agnostic: It can be used with any CRNP, allowing users to process data from multiple instruments with their own workflow.
+- Accuracy: The library shows excellent agreement with ground-based measurements, making it a reliable tool for scientific research and practical applications.
 - Correction Routines: The correction functions of the library have been effectively used to represent field and watershed scale soil moisture conditions.
 
-![CRNPy Processing Workflow](https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/workflow.png)
+![CRNPy Processing Workflow](docs/img/workflow.png)
 Overview of the proposed CRNPy processing workflow. Final user can choose to use the entire workflow, part of it, or build functions on top of it depending on their needs, dashed lines indicate optional steps.
 
 
 ## Installation
 
 To install the CRNPy library, you can use Python's package manager, pip. Simply open your command line or terminal and type:
 
 ```pip install crnpy```
 
 ## Authors
+The CRNPy library was conceived and developed by Joaquin Peraza and Andres Patrignani in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
 
-The CRNPy library was developed by:
-
-- Joaquin Peraza
-- Andres Patrignani
-
-in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
-
-The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. The authors would like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
+The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
```

### Comparing `crnpy-0.3.1/src/crnpy/crnpy.py` & `crnpy-0.3.post1/src/crnpy/crnpy.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.3.1/src/crnpy/data.py` & `crnpy-0.3.post1/src/crnpy/data.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.3.1/src/crnpy.egg-info/PKG-INFO` & `crnpy-0.3.post1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,30 @@
-Metadata-Version: 2.1
-Name: crnpy
-Version: 0.3.1
-Summary: A Python package for processing cosmic ray neutron data.
-Home-page: https://github.com/soilwater/crnpy
-Author: Joaquin Peraza, Andres Patrignani
-Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
-<img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
+<img src="/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from Cosmic-Ray Neutron Probes (CRNP) into accurate field-level soil moisture data.
 
 This library has been developed with the intent of providing a comprehensive yet easy-to-use workflow for processing raw data from a variety of CRNP, encompassing multiple manufacturers and models.
 
 ## Key Features
 - Versatility: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 - Modularity: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
-- Instrument agnostic: It can be used with any CRNP, allowing users to process data from multiple instruments with their own workflow.
+- Accuracy: The library shows excellent agreement with ground-based measurements, making it a reliable tool for scientific research and practical applications.
 - Correction Routines: The correction functions of the library have been effectively used to represent field and watershed scale soil moisture conditions.
 
-![CRNPy Processing Workflow](https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/workflow.png)
+![CRNPy Processing Workflow](docs/img/workflow.png)
 Overview of the proposed CRNPy processing workflow. Final user can choose to use the entire workflow, part of it, or build functions on top of it depending on their needs, dashed lines indicate optional steps.
 
 
 ## Installation
 
 To install the CRNPy library, you can use Python's package manager, pip. Simply open your command line or terminal and type:
 
 ```pip install crnpy```
 
 ## Authors
+The CRNPy library was conceived and developed by Joaquin Peraza and Andres Patrignani in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
 
-The CRNPy library was developed by:
-
-- Joaquin Peraza
-- Andres Patrignani
-
-in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
-
-The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. The authors would like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
+The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
```

