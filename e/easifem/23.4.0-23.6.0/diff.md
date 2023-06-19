# Comparing `tmp/easifem-23.4.0.tar.gz` & `tmp/easifem-23.6.0.tar.gz`

## Comparing `easifem-23.4.0.tar` & `easifem-23.6.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/__init__.py
--rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/cmake.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/console.py
--rwxr-xr-x   0        0        0     2668 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/easifem.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/install.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/parsers.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/run.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/setenv.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/test.py
--rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/utils.py
--rw-r--r--   0        0        0    32396 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/utils_install.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 easifem-23.4.0/src/easifem/utils_setenv.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easifem-23.4.0/tests/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 easifem-23.4.0/tests/hello.F90
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 easifem-23.4.0/tests/hello.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 easifem-23.4.0/tests/test2.F90
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 easifem-23.4.0/tests/test2.md
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 easifem-23.4.0/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 easifem-23.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 easifem-23.4.0/README.md
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 easifem-23.4.0/pyproject.toml
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 easifem-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/clean.py
+-rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/cmake.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/components.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/console.py
+-rwxr-xr-x   0        0        0     3711 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/easifem.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/install.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/parsers.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/run.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/setenv.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/test.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/uninstall.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_clean.py
+-rw-r--r--   0        0        0    32343 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_install.py
+-rw-r--r--   0        0        0    10907 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_run.py
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_setenv.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_uninstall.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/hello.F90
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/hello.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/test2.F90
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/test2.md
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 easifem-23.6.0/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 easifem-23.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 easifem-23.6.0/README.md
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 easifem-23.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 easifem-23.6.0/PKG-INFO
```

### Comparing `easifem-23.4.0/src/easifem/install.py` & `easifem-23.6.0/src/easifem/install.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,53 @@
+import argparse
+ 
+_DESCRIPTION = """
+The [install] subcommand helps you installing the components of  
+EASIFEM, such as extpkgs, base, classes, materials, kernels, etc.
+
+In order to install a component you should specify following environment variables:
+A) EASIFEM_ROOT_DIR: the place where easifem is installed. 
+B) EASIFEM_BUILD_DIR: the place where easifem is build. 
+C) EASIFEM_SOURCE_DIR: the place where the source of easifem will be stored.
+
+You can specify them by using
+
+easifem setenv --build= --install= --source=
+
+For more see,
+easifem setenv --help 
+
+Use:
+
+easifem install option
+
+Option can be:
+
+all: Install everything
+extpkgs: install external packages
+openblas : install OpenBlas
+lapack95: install LAPACK95
+sparsekit: install Sparsekit
+fftw: install FFTW
+superlu: install SuperLU
+arpack: install ARPACK
+lis: install LIS
+base: install easifemBase
+classes: install easifemClasses
+materials: install easifemMaterials
+kernels: install easifemKernels
+"""
+
 def parser(subparser):
 
     ans = subparser.add_parser(
         "install",
         help="Install components of easifem.",
-        description="""
-        The [install] subcommand helps you installing the components of \n 
-        EASIFEM, such as extpkgs, base, classes, materials, kernels, etc. \n
-        \n
-        In order to install a component you should specify following environment variables: \n
-        A) EASIFEM_ROOT_DIR: the place where easifem is installed. \n
-        B) EASIFEM_BUILD_DIR: the place where easifem is build. \n
-        C) EASIFEM_SOURCE_DIR: the place where the source of easifem will be stored. \n
-        \n
-        You can specify them by using \n
-        \n
-        easifem setenv --build= --install= --source=
-        \n
-        For more see,\n
-        easifem setenv --help \n
-        \n
-        """,
+        description=_DESCRIPTION,
+        formatter_class=argparse.RawTextHelpFormatter,
     )
 
     ans.add_argument(
         "-i",
         "--install",
         help="Location where easifem is installed, EASIFEM_INSTALL_DIR",
         required=False,
```

### Comparing `easifem-23.4.0/src/easifem/run.py` & `easifem-23.6.0/src/easifem/run.py`

 * *Files identical despite different names*

### Comparing `easifem-23.4.0/src/easifem/setenv.py` & `easifem-23.6.0/src/easifem/setenv.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,54 @@
+import argparse
+
+_DESCRIPTION = """
+The [setenv] subcommand sets the environment variable for easifem on your system.
+
+While setting the environment you can provide following details.
+A) EASIFEM_INSTALL_DIR
+B) EASIFEM_BUILD_DIR
+C) EASIFEM_SOURCE_DIR
+
+EASIFEM_INSTALL_DIR: denotes the root location where EASIFEM will
+be installed. It is specified by --install=value
+
+Following are the good choices for --install variable:
+1) ${HOME}
+2) ${HOME}/.local
+3) /opt
+The default value is ${HOME}.
+
+EASIFEM_SOURCE_DIR: specifies the location where the source code of
+the components of EASIFEM will be stored.
+It is specified by --source=value 
+
+Following are the good choices for --source variable:
+1) ${HOME}/code/
+The default value is ${HOME}/code.
+EASIFEM_BUILD_DIR: specifies the location where the components of 
+EASIFEM will be build. It is specified by --build=value 
+
+Following are the good choices for --root variable:
+1) ${HOME}/temp 
+The default value is ${HOME}/temp.
+
+Example:
+
+easifem setenv --install ${HOME} --build ${HOME}/temp --source ${HOME}/code
+easifem setenv -r ${HOME} -b ${HOME}/temp -s ${HOME}/code
+"""
+
+
 def parser(subparser):
 
     ans = subparser.add_parser(
         "setenv",
         help="Set environment variables for running easifem on your system.",
-        description="""
-        The [setenv] subcommand sets the environment variable \n
-        for running easifem on your system. \n
-        \n 
-        While setting the environment you can provide following details. \n
-        A) EASIFEM_INSTALL_DIR \n
-        B) EASIFEM_BUILD_DIR \n
-        C) EASIFEM_SOURCE_DIR \n
-        \n
-        EASIFEM_INSTALL_DIR: denotes the root location where EASIFEM will \n
-        be installed. It is specified by \n
-        --install=value. \n
-        \n
-        Following are the good choices for --install variable: \n
-        1) ${HOME} \n
-        2) ${HOME}/.local \n
-        3) /opt \n
-        \n
-        The default value is ${HOME}.
-        \n
-        EASIFEM_SOURCE_DIR: specifies the location where the source code of \n
-        the components of EASIFEM will be stored. \n
-        It is specified by\n
-        --source=value \n
-        \n
-        Following are the good choices for --source variable: \n
-        1) ${HOME}/code/\n
-        \n
-        The default value is ${HOME}/code.
-        \n
-        EASIFEM_BUILD_DIR: specifies the location where the components of \n
-        EASIFEM will be build. It is specified by\n
-        --build=value \n
-        \n
-        Following are the good choices for --root variable: \n
-        1) ${HOME}/temp \n
-        \n
-        The default value is ${HOME}/temp.
-        \n
-
-        Example
-
-        easifem setenv --install ${HOME} --build ${HOME}/temp --source ${HOME}/code
-        easifem setenv -r ${HOME} -b ${HOME}/temp -s ${HOME}/code
-        """,
+        description=_DESCRIPTION,
+        formatter_class=argparse.RawTextHelpFormatter,
     )
 
     ans.add_argument(
         "-i",
         "--install",
         help="Root directory for easifem, EASIFEM_INSTALL_DIR",
         required=False,
```

### Comparing `easifem-23.4.0/src/easifem/test.py` & `easifem-23.6.0/src/easifem/test.py`

 * *Files identical despite different names*

### Comparing `easifem-23.4.0/src/easifem/utils.py` & `easifem-23.6.0/src/easifem/utils_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,18 +94,15 @@
 def _makeEasifemLibsTree(easifemLibs):
     """
     Dependencies among easifem components
     """
     if easifemLibs == "easifemBase":
         return ("easifemBase",)
     elif easifemLibs == "easifemClasses":
-        return (
-            "easifemBase",
-            "easifemClasses",
-        )
+        return ("easifemClasses",)
     elif easifemLibs == "easifemMaterials":
         return (
             "easifemBase",
             "easifemClasses",
             "easifemMaterials",
         )
     elif easifemLibs == "easifemKernels":
@@ -137,14 +134,15 @@
         )
 
 
 def _makeExtpkgs(easifemLibs):
     """
     Dependencies of easifem components on external libs
     """
+    # return ""
     return (
         "LAPACK95",
         "Sparsekit",
         "arpackng",
         "OpenMP",
     )
```

### Comparing `easifem-23.4.0/src/easifem/utils_install.py` & `easifem-23.6.0/src/easifem/utils_install.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
-import sys
+
+# import sys
 import shutil
 import subprocess
 from easifem.console import console
 from rich.panel import Panel
 from rich.text import Text
-from rich.progress import Progress, BarColumn, TextColumn
 
-_easifem = "easifem"
+# _easifem = "easifem"
 
 _extpkgs = ["openblas", "lapack95", "sparsekit", "fftw", "superlu", "arpack", "lis"]
 
 _components = ["extpkgs", "base", "classes", "materials", "kernels"] + _extpkgs
 
 # _build0 = os.path.join(os.environ["HOME"], "temp")
 # _install0 = os.environ["HOME"]
```

### Comparing `easifem-23.4.0/src/easifem/utils_setenv.py` & `easifem-23.6.0/src/easifem/utils_setenv.py`

 * *Files 23% similar despite different names*

```diff
@@ -54,56 +54,66 @@
 
         for key in _keys:
             console.print(f"◌ {key}: {os.environ.get(key)}")
 
     _config_path = os.path.join(os.environ["HOME"], ".config", "easifem")
     os.makedirs(_config_path, exist_ok=True)
 
+    # -----------------------bash/zsh--------------------------------------
     _config_file_sh = os.path.join(_config_path, "easifemvar.sh")
     easifemrc = open(_config_file_sh, "w")
     # easifemrc.write("#!/bin/bash \n \n")
     easifemrc.write("\n")
     a = os.environ.get("EASIFEM_INSTALL_DIR")
     easifemrc.write(f"export EASIFEM_INSTALL_DIR={a} \n")
     a = os.environ.get("EASIFEM_BUILD_DIR")
     easifemrc.write(f"export EASIFEM_BUILD_DIR={a} \n")
     a = os.environ.get("EASIFEM_SOURCE_DIR")
     easifemrc.write(f"export EASIFEM_SOURCE_DIR={a} \n")
+
     for key in _keys:
         a = os.environ.get(key)
         easifemrc.write(f"export {key}={a} \n")
         easifemrc.write(
             "export LD_LIBRARY_PATH=" + '"${LD_LIBRARY_PATH}:${' + f"{key}" + '}/lib"\n'
         )
 
     easifemrc.write(
         "export PKG_CONFIG_PATH="
         + '"${PKG_CONFIG_PATH}:${EASIFEM_EXTPKGS}/lib/pkgconfig"\n'
     )
-    # export PKG_CONFIG_PATH="${PKG_CONFIG_PATH}:${EASIFEM_EXTPKGS}/lib/pkgconfig"
-    # export LD_LIBRARY_PATH="${LD_LIBRARY_PATH}:${EASIFEM_EXTPKGS}/lib"
-    # export LD_LIBRARY_PATH="${LD_LIBRARY_PATH}:${EASIFEM_CLASSES}/lib"
-    # export LD_LIBRARY_PATH="${LD_LIBRARY_PATH}:${EASIFEM_MATERIALS}/lib"
-    # export LD_LIBRARY_PATH="${LD_LIBRARY_PATH}:${EASIFEM_KERNELS}/lib"
-    # export LD_LIBRARY_PATH="${LD_LIBRARY_PATH}:${HOME}/.local/lib/"
-    # export LD_LIBRARY_PATH="${LD_LIBRARY_PATH}:${EASIFEM_BASE}/lib"
+
+    easifemrc.write("export PATH=" + '"${PATH}:${EASIFEM_EXTPKGS}/bin"\n')
+    easifemrc.write("export PATH=" + '"${PATH}:${EASIFEM_APP}/bin"\n')
+
     easifemrc.close()
 
+    # -----------------------fish--------------------------------------
     _config_file_fish = os.path.join(_config_path, "easifemvar.fish")
     easifemrc = open(_config_file_fish, "w")
     easifemrc.write("\n")
     a = os.environ.get("EASIFEM_INSTALL_DIR")
     easifemrc.write(f"set -gx EASIFEM_INSTALL_DIR {a} \n")
     a = os.environ.get("EASIFEM_BUILD_DIR")
     easifemrc.write(f"set -gx EASIFEM_BUILD_DIR {a} \n")
     a = os.environ.get("EASIFEM_SOURCE_DIR")
     easifemrc.write(f"set -gx EASIFEM_SOURCE_DIR {a} \n")
     for key in _keys:
         a = os.environ.get(key)
         easifemrc.write(f"set -gx {key} {a} \n")
+        easifemrc.write(
+            "set -gx LD_LIBRARY_PATH " + '$LD_LIBRARY_PATH $' + f"{key}" + '/lib\n'
+        )
+    easifemrc.write(
+        "set -gx PKG_CONFIG_PATH $PKG_CONFIG_PATH $EASIFEM_EXTPKGS/lib/pkgconfig\n"
+    )
+
+    easifemrc.write("set -gx PATH $PATH $EASIFEM_EXTPKGS/bin\n")
+    easifemrc.write("set -gx PATH $PATH $EASIFEM_APP/bin\n")
+
     easifemrc.close()
 
     console.print("\n Environment variables have been written in  ↓")
     console.print(Panel.fit(f"{_config_file_sh}\n\n" + f"{_config_file_fish}"))
 
     text = Text()
     text.append("\n🚀 Please perform the following task: ⤵\n\n", style="bold")
```

### Comparing `easifem-23.4.0/.gitignore` & `easifem-23.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `easifem-23.4.0/LICENSE.txt` & `easifem-23.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easifem-23.4.0/README.md` & `easifem-23.6.0/README.md`

 * *Files identical despite different names*

### Comparing `easifem-23.4.0/pyproject.toml` & `easifem-23.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easifem-23.4.0/PKG-INFO` & `easifem-23.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easifem
-Version: 23.4.0
+Version: 23.6.0
 Summary: easifem is a command line interface for using EASIFEM library. Expandable And Scalable Infrastructure for Finite Element Methods, EASIFEM, is Modern Fortran framework for solving partial differential equations (PDEs) using finite element methods.
 Project-URL: Documentation, https://github.com/vickysharma0812/easifem#readme
 Project-URL: Issues, https://github.com/vickysharma0812/easifem/issues
 Project-URL: Source, https://github.com/vickysharma0812/easifem
 Author-email: Vikas Sharma <Vickysharma0812@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

