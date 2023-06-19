# Comparing `tmp/pyswtools-0.6.0.tar.gz` & `tmp/pyswtools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyswtools-0.6.0.tar", max compression
+gzip compressed data, was "pyswtools-0.7.0.tar", max compression
```

## Comparing `pyswtools-0.6.0.tar` & `pyswtools-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0    35149 2023-05-26 12:38:39.604629 pyswtools-0.6.0/LICENSE
--rw-r--r--   0        0        0     4081 2023-05-27 11:49:27.007898 pyswtools-0.6.0/README.md
--rw-r--r--   0        0        0      807 2023-05-27 11:49:17.907991 pyswtools-0.6.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-05-03 14:11:07.498269 pyswtools-0.6.0/pyswtools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.6.0/pyswtools/auto_exporter/__init__.py
--rw-r--r--   0        0        0     5406 2023-05-04 20:45:17.566358 pyswtools-0.6.0/pyswtools/auto_exporter/main.py
--rw-r--r--   0        0        0     3415 2023-05-04 08:30:28.502483 pyswtools-0.6.0/pyswtools/config.py
--rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.6.0/pyswtools/copy_full_assembly/__init__.py
--rw-r--r--   0        0        0     1807 2023-05-04 15:28:13.720447 pyswtools-0.6.0/pyswtools/copy_full_assembly/main.py
--rw-r--r--   0        0        0      787 2023-05-27 11:49:17.907991 pyswtools-0.6.0/pyswtools/main.py
--rw-r--r--   0        0        0        0 2023-05-03 11:48:07.729317 pyswtools-0.6.0/pyswtools/ready_dxf/__init__.py
--rw-r--r--   0        0        0     1326 2023-05-03 13:47:31.066860 pyswtools-0.6.0/pyswtools/ready_dxf/dxf_utilities.py
--rw-r--r--   0        0        0      645 2023-05-03 13:47:31.062860 pyswtools-0.6.0/pyswtools/ready_dxf/file_utilities.py
--rw-r--r--   0        0        0      502 2023-05-03 13:47:31.058860 pyswtools-0.6.0/pyswtools/ready_dxf/main.py
--rw-r--r--   0        0        0        0 2023-05-27 11:49:17.907991 pyswtools-0.6.0/pyswtools/stat/__init__.py
--rw-r--r--   0        0        0     5434 2023-05-27 11:49:17.907991 pyswtools-0.6.0/pyswtools/stat/main.py
--rw-r--r--   0        0        0      454 2023-05-27 11:36:54.314563 pyswtools-0.6.0/pyswtools/utils.py
--rw-r--r--   0        0        0     4962 1970-01-01 00:00:00.000000 pyswtools-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-26 12:38:39.604629 pyswtools-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4899 2023-06-19 17:20:17.563884 pyswtools-0.7.0/README.md
+-rw-r--r--   0        0        0      807 2023-06-19 17:22:30.798020 pyswtools-0.7.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-03 14:11:07.498269 pyswtools-0.7.0/pyswtools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.7.0/pyswtools/auto_exporter/__init__.py
+-rw-r--r--   0        0        0     5406 2023-05-04 20:45:17.566358 pyswtools-0.7.0/pyswtools/auto_exporter/main.py
+-rw-r--r--   0        0        0        0 2023-06-19 17:20:17.563884 pyswtools-0.7.0/pyswtools/clean/__init__.py
+-rw-r--r--   0        0        0     2058 2023-06-19 17:20:17.563884 pyswtools-0.7.0/pyswtools/clean/main.py
+-rw-r--r--   0        0        0     3415 2023-05-04 08:30:28.502483 pyswtools-0.7.0/pyswtools/config.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.7.0/pyswtools/copy_full_assembly/__init__.py
+-rw-r--r--   0        0        0     1596 2023-06-19 17:20:17.567880 pyswtools-0.7.0/pyswtools/copy_full_assembly/main.py
+-rw-r--r--   0        0        0     1345 2023-06-19 17:20:17.567880 pyswtools-0.7.0/pyswtools/helper_sw.py
+-rw-r--r--   0        0        0      841 2023-06-19 17:22:58.195772 pyswtools-0.7.0/pyswtools/main.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:48:07.729317 pyswtools-0.7.0/pyswtools/ready_dxf/__init__.py
+-rw-r--r--   0        0        0     1326 2023-06-19 17:19:43.848800 pyswtools-0.7.0/pyswtools/ready_dxf/dxf_utilities.py
+-rw-r--r--   0        0        0      645 2023-05-03 13:47:31.062860 pyswtools-0.7.0/pyswtools/ready_dxf/file_utilities.py
+-rw-r--r--   0        0        0      502 2023-05-27 12:07:20.884752 pyswtools-0.7.0/pyswtools/ready_dxf/main.py
+-rw-r--r--   0        0        0        0 2023-05-27 11:49:17.907991 pyswtools-0.7.0/pyswtools/stat/__init__.py
+-rw-r--r--   0        0        0    11391 2023-06-19 17:20:17.567880 pyswtools-0.7.0/pyswtools/stat/main.py
+-rw-r--r--   0        0        0      454 2023-05-27 11:36:54.314563 pyswtools-0.7.0/pyswtools/utils.py
+-rw-r--r--   0        0        0     5780 1970-01-01 00:00:00.000000 pyswtools-0.7.0/PKG-INFO
```

### Comparing `pyswtools-0.6.0/LICENSE` & `pyswtools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswtools-0.6.0/README.md` & `pyswtools-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 
 List of ressources that can be helpful when starting with the solidworks API:
 - [Solidworks API](https://help.solidworks.com/2022/french/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1)
 - [Python examples](https://mycad.visiativ.com/sites/default/files/questions/answer/15/11/2019/solidworks_python_api.pdf)
 
 ## List of modules
 
+- CLI: handle all the modules
+- Config: handle the configuration
+- Ready-dxf: Prep the dxf outputed from SW to be laser cutted
+- Copy-full-assembly: Update the relative link from an assembly after a copy
+- Auto-export: export all the parts to `.stl` or `.dxf`
+- Stat: List all the parts from an assembly with their mass and density
+- Clean: List all the unused files from an assembly
+
 ### CLI
 It is the main module of this project. It allows you to select the actions that you want to apply. To directly get help from the tool simply type:
 ```
 pyswtools
 ```
 
 ### Config
@@ -75,19 +83,14 @@
 
 ```
 pyswtools ready-dxf /path/to/directory
 ```
 
 It will output a `directory_cleaned` directory with all the cleaned dxf. Do not include the `/` or `\` at the end of the path of the directory
 
-#### Features to come
-- [ ] Combine Lines
-- [ ] Combine Files
-- [ ] Add auto coloring
-- [ ] Add tests
 
 ### Copy-full-assembly
 This tool help you when copying multiple file or assembly. It will help you by updating path reference to new path reference:
 - In the equation manager
 #### How to use
 ```
 pyswtools copy-full-assembly PATH_TO_DIR SRC_REPLACE TARGET_REPLACE
@@ -115,22 +118,35 @@
 ```
 pyswtools auto-export PATH/TO/DIR MODE
 ```
 
 With `Mode` being `AUTO`, `DXF` or `STL`. It will create directory with the extension used  and the corresponding files in it.
 
 ### Stat
-This tool help you get stat on an assembly. It can gives you recursive information about the mass of each component of an assembly.
+This tool help you get stat on an assembly. It can gives you recursive information about the mass and the density of each component of an assembly.
 
 #### How to use
 
 ```
 pyswtools stat PATH/TO/ASSEMBLY OPTIONS
 ```
 
-You can select the display mode:
-- `--tree`: (default) It will follow the structure from the assembly file
-- `--list`: It will output to a single list
-
-You can select the sort:
-- `--mass`: (default) sort with a decreasing mass
-- `--name`: sort with alphabetical order
+You can select the display mode with `--type-output`:
+- `tree`: (default) It will follow the structure from the assembly file
+- `list`: It will output to a single list
+
+You can select the sort mode with `--type-sort`:
+- `mass`: (default) sort with a decreasing total mass
+- `mass-part`: sort with a decreasing part mass
+- `name`: sort with alphabetical order
+
+You can get only the elements with a default density (1000 Kg/m³) with the option `--only-default-density`. This option only works with a `type `list`
+
+### Clean
+This tool help you clean the directory of your project and remove unused files
+
+#### How to use
+
+```
+pyswtools clean PATH/TO/DIR/PROJECT/ PATH/TO/MAIN/ASSEMBLY
+```
+It will output all the solidworks files in `PATH/TO/DIR/PROJECT/` that are not used in the assembly.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyswtools-0.6.0/pyproject.toml` & `pyswtools-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyswtools"
-version = "0.6.0"
+version = "0.7.0"
 description = "Set of tools to improve Solidworks usage"
 authors = ["ldevillez <louis.devillez@gmail.com>"]
 license = "GNU General Public License"
 readme = "README.md"
 homepage = "https://github.com/ldevillez/pySwTools"
 repository = "https://github.com/ldevillez/pySwTools"
```

### Comparing `pyswtools-0.6.0/pyswtools/auto_exporter/main.py` & `pyswtools-0.7.0/pyswtools/auto_exporter/main.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.6.0/pyswtools/config.py` & `pyswtools-0.7.0/pyswtools/config.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.6.0/pyswtools/copy_full_assembly/main.py` & `pyswtools-0.7.0/pyswtools/copy_full_assembly/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,16 @@
 Make a copy of a directory but update all the paths to reference the new paths
 """
 
 import os
 import click
 
 # pylint: disable=relative-beyond-top-level
-from ..utils import check_system, check_system_verbose
-from ..config import get_config
-
-if check_system():
-    # pylint: disable=import-error
-    import win32com.client
+from ..utils import check_system_verbose
+from ..helper_sw import open_app, is_file, is_temp
 
 
 @click.command()
 @click.help_option("-h", "--help")
 @click.argument(
     "input_path",
     type=click.Path(exists=True),
@@ -32,25 +28,22 @@
     """
     Make a copy of a directory but update all the paths to reference the new paths
     """
 
     if not check_system_verbose():
         return
 
-    # Function + auto config
-    conf = get_config()
-    sw_app = win32com.client.Dispatch(
-        f"SldWorks.Application.{(int(conf.sw_version)-2012+20)}"
-    )
+    # Open app
+    sw_app = open_app()
 
     # Walk though the directory and each subdirectory
     for root, _, files in os.walk(input_path):
         for file in files:
             curr_path = os.path.abspath(os.path.join(root, file))
-            if ".SLDPRT" not in file or "~$" in file:
+            if not is_file(file) or is_temp(file):
                 continue
             print(f"- {file}")
 
             # Open the new doc
             sw_doc = sw_app.OpenDoc(curr_path, 1)
 
             # Get the equation manager
```

### Comparing `pyswtools-0.6.0/pyswtools/main.py` & `pyswtools-0.7.0/pyswtools/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import click
 
 from .config import config
 from .ready_dxf.main import ready_dxf
 from .copy_full_assembly.main import copy_full_assembly
 from .auto_exporter.main import auto_export
 from .stat.main import stat
+from .clean.main import clean
 
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 __author__ = "Devillez Louis"
-__maintainer__ = "Deville Louis"
+__maintainer__ = "Devillez Louis"
 __email__ = "louis.devillez@gmail.com"
 
 
 @click.group()
 @click.version_option(__version__, "-v", "--version")
 @click.help_option("-h", "--help")
 def cli() -> None:
@@ -27,10 +28,11 @@
 
 
 cli.add_command(config)
 cli.add_command(ready_dxf)
 cli.add_command(copy_full_assembly)
 cli.add_command(auto_export)
 cli.add_command(stat)
+cli.add_command(clean)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `pyswtools-0.6.0/pyswtools/ready_dxf/dxf_utilities.py` & `pyswtools-0.7.0/pyswtools/ready_dxf/dxf_utilities.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.6.0/pyswtools/ready_dxf/file_utilities.py` & `pyswtools-0.7.0/pyswtools/ready_dxf/file_utilities.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.6.0/PKG-INFO` & `pyswtools-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswtools
-Version: 0.6.0
+Version: 0.7.0
 Summary: Set of tools to improve Solidworks usage
 Home-page: https://github.com/ldevillez/pySwTools
 License: GNU General Public License
 Author: ldevillez
 Author-email: louis.devillez@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -46,14 +46,22 @@
 
 List of ressources that can be helpful when starting with the solidworks API:
 - [Solidworks API](https://help.solidworks.com/2022/french/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1)
 - [Python examples](https://mycad.visiativ.com/sites/default/files/questions/answer/15/11/2019/solidworks_python_api.pdf)
 
 ## List of modules
 
+- CLI: handle all the modules
+- Config: handle the configuration
+- Ready-dxf: Prep the dxf outputed from SW to be laser cutted
+- Copy-full-assembly: Update the relative link from an assembly after a copy
+- Auto-export: export all the parts to `.stl` or `.dxf`
+- Stat: List all the parts from an assembly with their mass and density
+- Clean: List all the unused files from an assembly
+
 ### CLI
 It is the main module of this project. It allows you to select the actions that you want to apply. To directly get help from the tool simply type:
 ```
 pyswtools
 ```
 
 ### Config
@@ -98,19 +106,14 @@
 
 ```
 pyswtools ready-dxf /path/to/directory
 ```
 
 It will output a `directory_cleaned` directory with all the cleaned dxf. Do not include the `/` or `\` at the end of the path of the directory
 
-#### Features to come
-- [ ] Combine Lines
-- [ ] Combine Files
-- [ ] Add auto coloring
-- [ ] Add tests
 
 ### Copy-full-assembly
 This tool help you when copying multiple file or assembly. It will help you by updating path reference to new path reference:
 - In the equation manager
 #### How to use
 ```
 pyswtools copy-full-assembly PATH_TO_DIR SRC_REPLACE TARGET_REPLACE
@@ -138,23 +141,35 @@
 ```
 pyswtools auto-export PATH/TO/DIR MODE
 ```
 
 With `Mode` being `AUTO`, `DXF` or `STL`. It will create directory with the extension used  and the corresponding files in it.
 
 ### Stat
-This tool help you get stat on an assembly. It can gives you recursive information about the mass of each component of an assembly.
+This tool help you get stat on an assembly. It can gives you recursive information about the mass and the density of each component of an assembly.
 
 #### How to use
 
 ```
 pyswtools stat PATH/TO/ASSEMBLY OPTIONS
 ```
 
-You can select the display mode:
-- `--tree`: (default) It will follow the structure from the assembly file
-- `--list`: It will output to a single list
-
-You can select the sort:
-- `--mass`: (default) sort with a decreasing mass
-- `--name`: sort with alphabetical order
+You can select the display mode with `--type-output`:
+- `tree`: (default) It will follow the structure from the assembly file
+- `list`: It will output to a single list
+
+You can select the sort mode with `--type-sort`:
+- `mass`: (default) sort with a decreasing total mass
+- `mass-part`: sort with a decreasing part mass
+- `name`: sort with alphabetical order
+
+You can get only the elements with a default density (1000 Kg/m³) with the option `--only-default-density`. This option only works with a `type `list`
 
+### Clean
+This tool help you clean the directory of your project and remove unused files
+
+#### How to use
+
+```
+pyswtools clean PATH/TO/DIR/PROJECT/ PATH/TO/MAIN/ASSEMBLY
+```
+It will output all the solidworks files in `PATH/TO/DIR/PROJECT/` that are not used in the assembly.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

