# Comparing `tmp/valve_gfx_ci.gfxinfo-0.1.2.tar.gz` & `tmp/valve_gfx_ci.gfxinfo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valve_gfx_ci.gfxinfo-0.1.2.tar", last modified: Wed Feb  1 08:17:25 2023, max compression
+gzip compressed data, was "valve_gfx_ci.gfxinfo-0.1.3.tar", last modified: Tue Jun 13 10:01:06 2023, max compression
```

## Comparing `valve_gfx_ci.gfxinfo-0.1.2.tar` & `valve_gfx_ci.gfxinfo-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:17:25.337927 valve_gfx_ci.gfxinfo-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-01-31 12:54:55.000000 valve_gfx_ci.gfxinfo-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      866 2023-02-01 08:17:25.337927 valve_gfx_ci.gfxinfo-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-02-01 08:17:25.337927 valve_gfx_ci.gfxinfo-0.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:17:25.335927 valve_gfx_ci.gfxinfo-0.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:17:25.335927 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:17:25.337927 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/
--rw-r--r--   0 root         (0) root         (0)    87069 2023-02-01 08:17:16.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/DeviceInfo.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2137 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    11127 2023-02-01 08:08:25.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/amdgpu.py
--rw-rw-rw-   0 root         (0) root         (0)     9533 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/gfxinfo_vulkan.py
--rw-rw-rw-   0 root         (0) root         (0)     1435 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/intel.py
--rw-rw-rw-   0 root         (0) root         (0)      739 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/pcidevice.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/test_gfxinfo.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-01-31 10:16:47.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/virt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:17:25.336927 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci.gfxinfo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      866 2023-02-01 08:17:25.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci.gfxinfo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      682 2023-02-01 08:17:25.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci.gfxinfo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 08:17:25.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci.gfxinfo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-02-01 08:17:25.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci.gfxinfo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-02-01 08:17:25.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci.gfxinfo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-01 08:17:25.000000 valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci.gfxinfo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:01:06.643209 valve_gfx_ci.gfxinfo-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      889 2023-06-13 10:01:06.643209 valve_gfx_ci.gfxinfo-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1775 2023-06-13 10:01:06.643209 valve_gfx_ci.gfxinfo-0.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:01:06.640209 valve_gfx_ci.gfxinfo-0.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:01:06.640209 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:01:06.642209 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/
+-rw-rw-rw-   0 root         (0) root         (0)     2663 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2302 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9679 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/amdgpu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:01:06.643209 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/dbs/
+-rw-r--r--   0 root         (0) root         (0)    89895 2023-06-13 10:00:53.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/dbs/DeviceInfo.cpp
+-rw-r--r--   0 root         (0) root         (0)    24104 2023-06-13 10:01:02.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/dbs/i915_pciids.h
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-13 10:00:54.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/dbs/xe_pciids.h
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/devicetree.py
+-rw-rw-rw-   0 root         (0) root         (0)     9537 2023-06-13 07:52:59.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/gfxinfo_vulkan.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/gpudb.py
+-rw-rw-rw-   0 root         (0) root         (0)     8939 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/intel.py
+-rw-rw-rw-   0 root         (0) root         (0)      739 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/pcidevice.py
+-rw-rw-rw-   0 root         (0) root         (0)    14574 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/test_gfxinfo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2023-06-13 04:40:34.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/virt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:01:06.641209 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci.gfxinfo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      889 2023-06-13 10:01:06.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci.gfxinfo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      843 2023-06-13 10:01:06.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci.gfxinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 10:01:06.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci.gfxinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-13 10:01:06.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci.gfxinfo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-13 10:01:06.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci.gfxinfo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 10:01:06.000000 valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci.gfxinfo.egg-info/top_level.txt
```

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/LICENSE` & `valve_gfx_ci.gfxinfo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/PKG-INFO` & `valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci.gfxinfo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: valve_gfx_ci.gfxinfo
-Version: 0.1.2
+Name: valve-gfx-ci.gfxinfo
+Version: 0.1.3
 Summary: Generate a list of tags that describe the environment running a GFX workload
 Home-page: https://gitlab.freedesktop.org/mupuf/valve-infra/-/tree/master/gfxinfo
 Author: Martin Roukala
 Author-email: martin.roukala@mupuf.org
 Project-URL: Bug Tracker, https://gitlab.freedesktop.org/mupuf/valve-infra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: vulkan
 License-File: LICENSE
 
 # GFXInfo
 
 Access the list of supported GPUs, from their codename to the environment they
 are used in. The primary purpose is to generate a list of tags that can be used
 to compare the results coming from machines running automated testing.
```

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/setup.cfg` & `valve_gfx_ci.gfxinfo-0.1.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 [metadata]
 name = valve_gfx_ci.gfxinfo
-version = 0.1.2
+version = 0.1.3
 author = Martin Roukala
 author_email = martin.roukala@mupuf.org
 description = Generate a list of tags that describe the environment running a GFX workload
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.freedesktop.org/mupuf/valve-infra/-/tree/master/gfxinfo
 project_urls = 
 	Bug Tracker = https://gitlab.freedesktop.org/mupuf/valve-infra/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
-Obsoletes-Dist = gfxinfo-mupuf
+obsoletes_dist = gfxinfo-mupuf
 
 [options]
 package_dir = 
 	= src
 install_requires = 
 	backports.cached-property;python_version<'3.8'
 	requests>=2,<3
-	chturne-vulkan
 tests_requires = 
 	coverage
 	pytest
 include_package_data = True
 packages = find_namespace:
 python_requires = >=3.6
 
+[options.extras_require]
+vulkan = 
+	chturne-vulkan
+
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	gfxinfo = valve_gfx_ci.gfxinfo.__main__:main
 
@@ -59,14 +62,14 @@
 deps = 
 	{[options]install_requires}
 	{[options]tests_requires}
 commands = 
 	coverage erase
 	coverage run --parallel-mode --source=src/valve_gfx_ci/gfxinfo -m pytest
 	coverage combine
-	coverage report --fail-under 100 -m --omit="src/valve_gfx_ci/gfxinfo/__init__.py,src/valve_gfx_ci/gfxinfo/__main__.py,src/valve_gfx_ci/gfxinfo/amdgpu.py,src/valve_gfx_ci/gfxinfo/gfxinfo_vulkan.py,src/valve_gfx_ci/gfxinfo/intel.py,src/valve_gfx_ci/gfxinfo/virt.py"
-	coverage report --fail-under 39
+	coverage report --fail-under 100 -m --omit="src/valve_gfx_ci/gfxinfo/__init__.py,src/valve_gfx_ci/gfxinfo/__main__.py,src/valve_gfx_ci/gfxinfo/gfxinfo_vulkan.py"
+	coverage report --fail-under 64
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/DeviceInfo.cpp` & `valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/dbs/DeviceInfo.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 //==============================================================================
-/// Copyright (c) 2020-2022 Advanced Micro Devices, Inc. All rights reserved.
+/// Copyright (c) 2020-2023 Advanced Micro Devices, Inc. All rights reserved.
 /// @author AMD Developer Tools Team
 /// @file
 /// @brief Device info table.
 //==============================================================================
 
 #include "DeviceInfo.h"
 
@@ -304,23 +304,26 @@
     {GDT_ELLESMERE, 0x67C2, 0x02, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon (TM) Pro V7300X"},
     {GDT_ELLESMERE, 0x67C2, 0x03, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "67C2:03"},
     {GDT_ELLESMERE, 0x67C4, 0x00, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon (TM) Pro WX 7100 Graphics"},
     {GDT_ELLESMERE, 0x67C4, 0x80, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon Embedded E9560"},
     {GDT_ELLESMERE, 0x67C7, 0x00, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon (TM) Pro WX 5100 Graphics"},
     {GDT_ELLESMERE, 0x67C7, 0x80, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon Embedded E9390"},
     {GDT_ELLESMERE, 0x67D0, 0x01, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon (TM) Pro V7350x2"},
-    {GDT_ELLESMERE, 0x67FF, 0xE3, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon (TM) Pro WX 7100 Graphics"},
+    {GDT_ELLESMERE, 0x67FF, 0xE3, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon (TM) E9550"},
+    {GDT_ELLESMERE, 0x67FF, 0xF3, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon (TM) PRO E9565 Graphics"},
+    {GDT_ELLESMERE, 0x67FF, 0xF7, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon (TM) Pro WX 5100 Graphics"},
     {GDT_ELLESMERE, 0x67D0, 0x02, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon (TM) Pro V7300X"},
     {GDT_ELLESMERE, 0x67DF, 0x04, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "67DF:04"},
     {GDT_ELLESMERE, 0x67DF, 0x05, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "67DF:05"},
     {GDT_ELLESMERE, 0x67DF, 0xC4, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon (TM) RX 480 Graphics"},
     {GDT_ELLESMERE, 0x67DF, 0xC5, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon (TM) RX 470 Graphics"},
     {GDT_ELLESMERE, 0x67DF, 0xC7, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon (TM) RX 480 Graphics"},
     {GDT_ELLESMERE, 0x67DF, 0xCF, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon (TM) RX 470 Graphics"},
     {GDT_ELLESMERE, 0x67DF, 0xFF, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon RX 470 Series"},
+    {GDT_ELLESMERE, 0x67FF, 0xE7, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "AMD Radeon Embedded E9390"},
     {GDT_ELLESMERE, 0x67DF, 0xC0, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon Pro 580X"},
     {GDT_ELLESMERE, 0x67DF, 0xC1, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon RX 580 Series"},
     {GDT_ELLESMERE, 0x67DF, 0xC2, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon RX 570 Series"},
     {GDT_ELLESMERE, 0x67DF, 0xC3, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon RX 580 Series"},
     {GDT_ELLESMERE, 0x67DF, 0xC6, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon RX 570 Series"},
     {GDT_ELLESMERE, 0x67DF, 0xC7, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "Radeon (TM) RX 480 Graphics"},
     {GDT_ELLESMERE, 0x67DF, 0xCC, GDT_HW_GENERATION_VOLCANICISLAND, false, "Ellesmere", "67DF:CC"},
@@ -724,18 +727,19 @@
     {GDT_GFX10_3_1, 0x73C3, 0x00, GDT_HW_GENERATION_GFX103, false, "gfx1031", "73C3:00"},
     {GDT_GFX10_3_1, 0x73DF, 0x40, GDT_HW_GENERATION_GFX103, false, "gfx1031", "73DF:40"},
     {GDT_GFX10_3_1, 0x73DF, 0x41, GDT_HW_GENERATION_GFX103, false, "gfx1031", "73DF:41"},
     {GDT_GFX10_3_1, 0x73DF, 0xC0, GDT_HW_GENERATION_GFX103, false, "gfx1031", "AMD Radeon RX 6750 XT"},
     {GDT_GFX10_3_1, 0x73DF, 0xC1, GDT_HW_GENERATION_GFX103, false, "gfx1031", "AMD Radeon RX 6700 XT"},
     {GDT_GFX10_3_1, 0x73DF, 0xC5, GDT_HW_GENERATION_GFX103, false, "gfx1031", "AMD Radeon RX 6700 XT"},
     {GDT_GFX10_3_1, 0x73DF, 0xC7, GDT_HW_GENERATION_GFX103, false, "gfx1031", "73DF:C7"},
-    {GDT_GFX10_3_1, 0x73DF, 0xDF, GDT_HW_GENERATION_GFX103, false, "gfx1031", "73DF:DF"},
+    {GDT_GFX10_3_1, 0x73DF, 0xDF, GDT_HW_GENERATION_GFX103, false, "gfx1031", "AMD Radeon RX 6700"},
     {GDT_GFX10_3_1, 0x73DF, 0xC2, GDT_HW_GENERATION_GFX103, false, "gfx1031", "AMD Radeon RX 6800M"},
     {GDT_GFX10_3_1, 0x73DF, 0xC3, GDT_HW_GENERATION_GFX103, false, "gfx1031", "AMD Radeon RX 6800M"},
     {GDT_GFX10_3_1, 0x73DF, 0xCF, GDT_HW_GENERATION_GFX103, false, "gfx1031", "AMD Radeon RX 6700M"},
+    {GDT_GFX10_3_1, 0x73DF, 0xFF, GDT_HW_GENERATION_GFX103, false, "gfx1031", "AMD Radeon RX 6700"},
 
     // GFX10_3_2
     {GDT_GFX10_3_2, 0x73E0, 0x00, GDT_HW_GENERATION_GFX103, false, "gfx1032", "73E0:00"},
     {GDT_GFX10_3_2, 0x73EF, 0xC0, GDT_HW_GENERATION_GFX103, false, "gfx1032", "AMD Radeon RX 6800S"},
     {GDT_GFX10_3_2, 0x73EF, 0xC1, GDT_HW_GENERATION_GFX103, false, "gfx1032", "AMD Radeon RX 6650 XT"},
     {GDT_GFX10_3_2, 0x73EF, 0xC2, GDT_HW_GENERATION_GFX103, false, "gfx1032", "AMD Radeon RX 6700S"},
     {GDT_GFX10_3_2, 0x73EF, 0xC3, GDT_HW_GENERATION_GFX103, false, "gfx1032", "AMD Radeon RX 6650M"},
@@ -759,18 +763,18 @@
     {GDT_GFX10_3_4, 0x743F, 0xC7, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon RX 6400"},
     {GDT_GFX10_3_4, 0x743F, 0xD7, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon RX 6400"},
     {GDT_GFX10_3_4, 0x7421, 0x00, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon(TM) PRO W6500M"},
     {GDT_GFX10_3_4, 0x7423, 0x00, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon(TM) PRO W6300M"},
     {GDT_GFX10_3_4, 0x7423, 0x01, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon PRO W6300"},
     {GDT_GFX10_3_4, 0x743F, 0xC3, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon(TM) RX 6500M"},
     {GDT_GFX10_3_4, 0x743F, 0xCF, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon RX 6300M"},
-    {GDT_GFX10_3_4, 0x743F, 0xC8, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon RX 6500M"},
+    {GDT_GFX10_3_4, 0x743F, 0xC8, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon(TM) RX 6550M"},
     {GDT_GFX10_3_4, 0x743F, 0xCC, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon(TM) 6550S"},
-    {GDT_GFX10_3_4, 0x743F, 0xCE, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon RX 6400M"},
-    {GDT_GFX10_3_4, 0x743F, 0xD3, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon RX 6500M"},
+    {GDT_GFX10_3_4, 0x743F, 0xCE, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon(TM) RX 6450M"},
+    {GDT_GFX10_3_4, 0x743F, 0xD3, GDT_HW_GENERATION_GFX103, false, "gfx1034", "AMD Radeon(TM) RX 6550M"},
 
     // GFX10_3_5
     {GDT_GFX10_3_5, 0x164D, 0x00, GDT_HW_GENERATION_GFX103, true, "gfx1035", "AMD Radeon(TM) Graphics"},
     {GDT_GFX10_3_5, 0x164D, 0x01, GDT_HW_GENERATION_GFX103, true, "gfx1035", "AMD Radeon(TM) Graphics"},
     {GDT_GFX10_3_5, 0x164D, 0x02, GDT_HW_GENERATION_GFX103, true, "gfx1035", "AMD Radeon(TM) Graphics"},
     {GDT_GFX10_3_5, 0x164D, 0x03, GDT_HW_GENERATION_GFX103, true, "gfx1035", "AMD Radeon(TM) Graphics"},
     {GDT_GFX10_3_5, 0x164D, 0x11, GDT_HW_GENERATION_GFX103, true, "gfx1035", "AMD Radeon(TM) Graphics"},
@@ -857,23 +861,48 @@
     {GDT_GFX10_3_5, 0x1681, 0xDD, GDT_HW_GENERATION_GFX103, true, "gfx1035", "AMD Radeon(TM) Graphics"},
     {GDT_GFX10_3_5, 0x1681, 0xDE, GDT_HW_GENERATION_GFX103, true, "gfx1035", "AMD Radeon(TM) Graphics"},
     {GDT_GFX10_3_5, 0x1681, 0xDF, GDT_HW_GENERATION_GFX103, true, "gfx1035", "AMD Radeon(TM) Graphics"},
 
     // GFX11_0_0
     {GDT_GFX11_0_0, 0x73A8, 0x00, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) Graphics"},
     {GDT_GFX11_0_0, 0x744C, 0xC0, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) Graphics"},
-    {GDT_GFX11_0_0, 0x744C, 0xC8, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) RX 7900 XTX"},
-    {GDT_GFX11_0_0, 0x744C, 0xCC, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) RX 7900 XT"},
+    {GDT_GFX11_0_0, 0x744C, 0xC8, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon RX 7900 XTX"},
+    {GDT_GFX11_0_0, 0x744C, 0xCC, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon RX 7900 XT"},
     {GDT_GFX11_0_0, 0x744C, 0xCE, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) Graphics"},
     {GDT_GFX11_0_0, 0x744C, 0xE0, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) Graphics"},
     {GDT_GFX11_0_0, 0x744C, 0xEC, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) Graphics"},
     {GDT_GFX11_0_0, 0x744C, 0xEE, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) Graphics"},
     {GDT_GFX11_0_0, 0x744C, 0xCF, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) Graphics"},
     {GDT_GFX11_0_0, 0x7448, 0x00, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) Graphics"},
     {GDT_GFX11_0_0, 0x745E, 0xCC, GDT_HW_GENERATION_GFX11, true, "gfx1100", "AMD Radeon(TM) Graphics"},
+
+    // GFX11_0_2
+    {GDT_GFX11_0_2, 0x73F0, 0x3C, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0x3D, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0xF5, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0xF6, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0xF7, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x7480, 0xC0, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x7480, 0xCF, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x749F, 0xCF, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0x3E, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0x3F, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0xF1, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0xF2, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0xF3, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x73F0, 0xF4, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x7480, 0xC1, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon RX 7700S"},
+    {GDT_GFX11_0_2, 0x7480, 0xC3, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon RX 7600S"},
+    {GDT_GFX11_0_2, 0x7480, 0xC7, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon RX 7600M XT"},
+    {GDT_GFX11_0_2, 0x7483, 0xCF, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon RX 7600M"},
+    {GDT_GFX11_0_2, 0x7480, 0x00, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x7481, 0x00, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x7489, 0x00, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+    {GDT_GFX11_0_2, 0x748B, 0x00, GDT_HW_GENERATION_GFX11, true, "gfx1102", "AMD Radeon(TM) Graphics"},
+
 };
 
 GDT_DeviceInfo gs_deviceInfo[] = {
     {2, 10, 1, 8, 2, 64, 2, 7, 4, true},    // GDT_TAHITI_PRO
     {2, 10, 1, 8, 2, 64, 2, 8, 4, true},    // GDT_TAHITI_XT
     {2, 10, 1, 8, 2, 64, 2, 4, 4, true},    // GDT_PITCAIRN_PRO
     {2, 10, 1, 8, 2, 64, 2, 5, 4, true},    // GDT_PITCAIRN_XT
@@ -911,11 +940,12 @@
     {2, 20, 1, 16, 4, 64, 2, 10, 2, true},  // GDT_GFX10_1_1
     {4, 16, 1, 16, 4, 64, 2, 10, 2, true},  // GDT_GFX10_3_0
     {2, 16, 1, 16, 2, 64, 2, 10, 2, true},  // GDT_GFX10_3_1
     {2, 16, 1, 16, 2, 64, 2, 8, 2, true},   // GDT_GFX10_3_2
     {1, 16, 1, 16, 2, 64, 2, 8, 2, true},   // GDT_GFX10_3_4
     {1, 16, 1, 16, 1, 64, 2, 6, 2, true},   // GDT_GFX10_3_5
     {6, 16, 1, 8, 12, 64, 2, 8, 2, true},   // GDT_GFX11_0_0
+    {2, 16, 1, 16, 4, 64, 2, 8, 2, true},   // GDT_GFX11_0_2
 };
 
 size_t gs_cardInfoSize   = sizeof(gs_cardInfo) / sizeof(GDT_GfxCardInfo);
 size_t gs_deviceInfoSize = sizeof(gs_deviceInfo) / sizeof(GDT_DeviceInfo);
```

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/__init__.py` & `valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 
 from .pcidevice import PCIDevice
 from .amdgpu import AmdGpuDeviceDB
-from .intel import IntelGpuDeviceDB
+from .devicetree import DeviceTreeGPU
+from .intel import IntelI915GpuDeviceDB, IntelXeGpuDeviceDB
 from .virt import VirtIOGpuDeviceDB
 from .gfxinfo_vulkan import VulkanInfo
 
 
-SUPPORTED_GPU_DBS = [AmdGpuDeviceDB(), IntelGpuDeviceDB(), VirtIOGpuDeviceDB()]
+SUPPORTED_GPU_DBS = [AmdGpuDeviceDB(), IntelXeGpuDeviceDB(), IntelI915GpuDeviceDB(), VirtIOGpuDeviceDB()]
 
 
 def pci_devices():
     def readfile(root, filename):
         with open(os.path.join(root, filename)) as f:
             return f.read().strip()
 
@@ -26,31 +27,46 @@
                                 revision=int(readfile(root, "revision"), 16))
             pciids.append(pci_dev)
 
     return pciids
 
 
 def find_gpu():
-    """For now we only support single-gpu DUTs"""
-    devices = pci_devices()
+    def find_devicetree_gpu():
+        try:
+            with open("/proc/device-tree/gpu/compatible") as f:
+                return DeviceTreeGPU.from_compatible_str(f.read())
+        except OSError:
+            return None
+
+    def find_pci_gpu():
+        devices = pci_devices()
+
+        for pci_device in devices:
+            for gpu_db in SUPPORTED_GPU_DBS:
+                if gpu := gpu_db.from_pciid(pci_device):
+                    return gpu
 
-    for pci_device in devices:
+        # We could not find the GPU in our databases, update them
         for gpu_db in SUPPORTED_GPU_DBS:
-            if gpu := gpu_db.from_pciid(pci_device):
-                return gpu
+            gpu_db.update()
 
-    # We could not find the GPU in our databases, update them
-    for gpu_db in SUPPORTED_GPU_DBS:
-        gpu_db.update()
+        # Retry, now that we have updated our DBs
+        for pci_device in devices:
+            for gpu_db in SUPPORTED_GPU_DBS:
+                if gpu := gpu_db.from_pciid(pci_device):
+                    return gpu
 
-    # Retry, now that we have updated our DBs
-    for pci_device in devices:
-        for gpu_db in SUPPORTED_GPU_DBS:
-            if gpu := gpu_db.from_pciid(pci_device):
-                return gpu
+    """For now we only support single-gpu DUTs"""
+    if gpu := find_devicetree_gpu():
+        return gpu
+    elif gpu := find_pci_gpu():
+        return gpu
+    else:
+        return None
 
 
 def cache_db():
     for gpu_db in SUPPORTED_GPU_DBS:
         gpu_db.cache_db()
```

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/__main__.py` & `valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,32 @@
 def main():
     parser = argparse.ArgumentParser(prog='GFXInfo')
     parser.add_argument("-p", '--pciid')
     parser.add_argument('--check-db', action="store_true")
     args = parser.parse_args()
 
     if args.check_db:
-        sys.exit(0 if check_db() else 1)
-
-    elif args.pciid is None:
-        if gpu := find_gpu():
-            output_gpu_info(gpu)
+        ret = check_db()
+        if ret:
+            print("All databases passed their checks!")
         else:
-            json.dump({"error": "No suitable GPU found"}, sys.stdout)
-            sys.exit(1)
-    else:
+            print("ERROR: At least one database is invalid")
+        sys.exit(0 if ret else 1)
+
+    elif args.pciid:
         pciid = PCIDevice.from_str(args.pciid)
         if gpu := find_gpu_from_pciid(pciid):
             output_gpu_info(gpu, show_vk_info=False)
         else:
-            json.dump({"error": "No GPU found matching the PCIID '{args.pciid}'"}, sys.stdout)
+            json.dump({"error": f"No GPU found matching the PCIID '{args.pciid}'"}, sys.stdout)
+            sys.exit(1)
+
+    else:
+        if gpu := find_gpu():
+            output_gpu_info(gpu)
+        else:
+            json.dump({"error": "No suitable GPU found"}, sys.stdout)
             sys.exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/gfxinfo_vulkan.py` & `valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/gfxinfo_vulkan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 try:
     from functools import cached_property
 except ImportError:
     from backports.cached_property import cached_property
 from enum import Enum
-from cffi import FFI
 
 import sys
 import re
 
 try:
     import vulkan as vk
+    from cffi import FFI
 
     class VulkanHeap:
         DEVICE_LOCAL_BIT = vk.VK_MEMORY_PROPERTY_DEVICE_LOCAL_BIT
         VISIBLE_BIT = vk.VK_MEMORY_PROPERTY_HOST_VISIBLE_BIT
         COHERENT_BIT = vk.VK_MEMORY_PROPERTY_HOST_COHERENT_BIT
         HOST_CACHED_BIT = vk.VK_MEMORY_PROPERTY_HOST_CACHED_BIT
         LAZILY_ALLOCATED_BIT = vk.VK_MEMORY_PROPERTY_LAZILY_ALLOCATED_BIT
```

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/intel.py` & `valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/devicetree.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,49 @@
 from dataclasses import dataclass
 
+from .gpudb import GpuDevice
+
+import sys
+
 
 @dataclass
-class IntelGPU:
-    vendor_id: int
-    product_id: int
-    revision: int
-    gen_version: int
-    family: str
+class DeviceTreeGPU(GpuDevice):
+    vendor: str
+    model: str
 
     @property
     def base_name(self):
-        return 'intel' + self.gen_version
+        return f'{self.vendor}-{self.model}'
 
     @property
-    def pciid(self):
-        return f"{hex(self.vendor_id)}:{hex(self.product_id)}"
+    def pci_device(self):
+        return None
 
     @property
     def tags(self):
         return {
-            f"intelgpu:pciid:{self.pciid}",
-            f"intelgpu:family:{self.family}",
-            f"intelgpu:gen:{self.gen_version}",
+            f"dt_gpu:vendor:{self.vendor}",
+            f"dt_gpu:model:{self.model}",
         }
 
     @property
     def structured_tags(self):
         return {
-            "type": "intelgpu",
-            "family": self.family,
-            "gen": self.gen_version
+            "type": "devicetree",
+            "vendor": self.vendor,
+            "model": self.model
         }
 
     def __str__(self):
-        return f"<IntelGPU: PCIID {self.pciid} - gen{self.gen_version} - {self.family}>"
-
-
-class IntelGpuDeviceDB:
-    def cache_db(self):
-        # NOTHING TO DO
-        pass
+        return f"<DeviceTreeGPU: {self.vendor}/{self.model}>"
 
-    def update(self):
-        # NOTHING TO DO
-        pass
-
-    def check_db(self):
-        return True
-
-    def from_pciid(self, pciid):
-        if pciid.vendor_id != 0x8086:
+    @classmethod
+    def from_compatible_str(cls, compatible):
+        main_compatible = compatible.split('\0')[0]
+
+        fields = main_compatible.split(',')
+        if len(fields) == 2:
+            return cls(vendor=fields[0], model=fields[1])
+        else:
+            print(f"ERROR: The compatible '{main_compatible}' is not following the expected format 'vendor,model'",
+                  file=sys.stderr)
             return None
-
-        SUPPORTED_GPUS = {
-            0x3e9b: {
-                'gen_version': '9',
-                'family': 'COFFEELAKE'
-            },
-        }
-        if md := SUPPORTED_GPUS.get(pciid.product_id):
-            return IntelGPU(vendor_id=pciid.vendor_id, product_id=pciid.product_id, revision=pciid.revision, **md)
```

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci/gfxinfo/pcidevice.py` & `valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci/gfxinfo/pcidevice.py`

 * *Files identical despite different names*

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci.gfxinfo.egg-info/PKG-INFO` & `valve_gfx_ci.gfxinfo-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: valve-gfx-ci.gfxinfo
-Version: 0.1.2
+Name: valve_gfx_ci.gfxinfo
+Version: 0.1.3
 Summary: Generate a list of tags that describe the environment running a GFX workload
 Home-page: https://gitlab.freedesktop.org/mupuf/valve-infra/-/tree/master/gfxinfo
 Author: Martin Roukala
 Author-email: martin.roukala@mupuf.org
 Project-URL: Bug Tracker, https://gitlab.freedesktop.org/mupuf/valve-infra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: vulkan
 License-File: LICENSE
 
 # GFXInfo
 
 Access the list of supported GPUs, from their codename to the environment they
 are used in. The primary purpose is to generate a list of tags that can be used
 to compare the results coming from machines running automated testing.
```

### Comparing `valve_gfx_ci.gfxinfo-0.1.2/src/valve_gfx_ci.gfxinfo.egg-info/SOURCES.txt` & `valve_gfx_ci.gfxinfo-0.1.3/src/valve_gfx_ci.gfxinfo.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 setup.cfg
 src/valve_gfx_ci.gfxinfo.egg-info/PKG-INFO
 src/valve_gfx_ci.gfxinfo.egg-info/SOURCES.txt
 src/valve_gfx_ci.gfxinfo.egg-info/dependency_links.txt
 src/valve_gfx_ci.gfxinfo.egg-info/entry_points.txt
 src/valve_gfx_ci.gfxinfo.egg-info/requires.txt
 src/valve_gfx_ci.gfxinfo.egg-info/top_level.txt
-src/valve_gfx_ci/gfxinfo/DeviceInfo.cpp
 src/valve_gfx_ci/gfxinfo/__init__.py
 src/valve_gfx_ci/gfxinfo/__main__.py
 src/valve_gfx_ci/gfxinfo/amdgpu.py
+src/valve_gfx_ci/gfxinfo/devicetree.py
 src/valve_gfx_ci/gfxinfo/gfxinfo_vulkan.py
+src/valve_gfx_ci/gfxinfo/gpudb.py
 src/valve_gfx_ci/gfxinfo/intel.py
 src/valve_gfx_ci/gfxinfo/pcidevice.py
 src/valve_gfx_ci/gfxinfo/test_gfxinfo.py
-src/valve_gfx_ci/gfxinfo/virt.py
+src/valve_gfx_ci/gfxinfo/virt.py
+src/valve_gfx_ci/gfxinfo/dbs/DeviceInfo.cpp
+src/valve_gfx_ci/gfxinfo/dbs/i915_pciids.h
+src/valve_gfx_ci/gfxinfo/dbs/xe_pciids.h
```

