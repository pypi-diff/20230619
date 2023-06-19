# Comparing `tmp/mckit_meshes-0.1.3.tar.gz` & `tmp/mckit_meshes-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mckit_meshes-0.1.3.tar", max compression
+gzip compressed data, was "mckit_meshes-0.1.4.tar", max compression
```

## Comparing `mckit_meshes-0.1.3.tar` & `mckit_meshes-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1063 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/LICENSE
--rw-r--r--   0        0        0     2443 2023-01-28 08:48:39.975317 mckit_meshes-0.1.3/README.rst
--rw-r--r--   0        0        0     7796 2023-01-28 08:48:39.975317 mckit_meshes-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       88 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/__init__.py
--rw-r--r--   0        0        0        0 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/cli/__init__.py
--rw-r--r--   0        0        0       89 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/cli/commands/__init__.py
--rw-r--r--   0        0        0     1468 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/cli/commands/mesh2npz.py
--rw-r--r--   0        0        0     1931 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/cli/commands/npz2vtk.py
--rw-r--r--   0        0        0     1894 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/cli/logging.py
--rw-r--r--   0        0        0        0 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/cli/py.typed
--rw-r--r--   0        0        0     2899 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/cli/runner.py
--rw-r--r--   0        0        0    42874 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/fmesh.py
--rw-r--r--   0        0        0      599 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/m_file_iterator.py
--rw-r--r--   0        0        0        0 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/mesh/__init__.py
--rw-r--r--   0        0        0    19566 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/mesh/geometry_spec.py
--rw-r--r--   0        0        0     2906 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/mesh2com.py
--rw-r--r--   0        0        0      929 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/particle_kind.py
--rw-r--r--   0        0        0       81 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/utils/__init__.py
--rw-r--r--   0        0        0     1043 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/utils/cartesian_product.py
--rw-r--r--   0        0        0     2538 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/utils/io.py
--rw-r--r--   0        0        0      831 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/utils/no_daemon_process.py
--rw-r--r--   0        0        0        0 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/utils/py.typed
--rw-r--r--   0        0        0    12243 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/utils/rebin.py
--rw-r--r--   0        0        0     1944 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/utils/resource.py
--rw-r--r--   0        0        0      783 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/utils/testing.py
--rw-r--r--   0        0        0      401 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/utils/utils.py
--rw-r--r--   0        0        0      585 2023-01-28 08:48:14.722970 mckit_meshes-0.1.3/src/mckit_meshes/version.py
--rw-r--r--   0        0        0    22898 2023-01-28 08:48:39.979317 mckit_meshes-0.1.3/src/mckit_meshes/wgtmesh.py
--rw-r--r--   0        0        0     3596 1970-01-01 00:00:00.000000 mckit_meshes-0.1.3/setup.py
--rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 mckit_meshes-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-19 11:45:37.949875 mckit_meshes-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2443 2023-06-19 11:45:37.949875 mckit_meshes-0.1.4/README.rst
+-rw-r--r--   0        0        0    16475 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:45:37.953875 mckit_meshes-0.1.4/src/mckit_meshes/cli/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1422 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/cli/commands/mesh2npz.py
+-rw-r--r--   0        0        0     1932 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/cli/commands/npz2vtk.py
+-rw-r--r--   0        0        0     1821 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/cli/logging.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:45:37.953875 mckit_meshes-0.1.4/src/mckit_meshes/cli/py.typed
+-rw-r--r--   0        0        0     2840 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/cli/runner.py
+-rw-r--r--   0        0        0    43448 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/fmesh.py
+-rw-r--r--   0        0        0      611 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/m_file_iterator.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:45:37.953875 mckit_meshes-0.1.4/src/mckit_meshes/mesh/__init__.py
+-rw-r--r--   0        0        0    19224 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/mesh/geometry_spec.py
+-rw-r--r--   0        0        0     2942 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/mesh2com.py
+-rw-r--r--   0        0        0      943 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/particle_kind.py
+-rw-r--r--   0        0        0       64 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/utils/__init__.py
+-rw-r--r--   0        0        0     1082 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/utils/cartesian_product.py
+-rw-r--r--   0        0        0     2555 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/utils/io.py
+-rw-r--r--   0        0        0      946 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/utils/no_daemon_process.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:45:37.953875 mckit_meshes-0.1.4/src/mckit_meshes/utils/py.typed
+-rw-r--r--   0        0        0    12762 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/utils/rebin.py
+-rw-r--r--   0        0        0      768 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/utils/resource.py
+-rw-r--r--   0        0        0      847 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/utils/testing.py
+-rw-r--r--   0        0        0      401 2023-06-19 11:45:37.953875 mckit_meshes-0.1.4/src/mckit_meshes/utils/utils.py
+-rw-r--r--   0        0        0      620 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/version.py
+-rw-r--r--   0        0        0    23236 2023-06-19 11:45:51.542097 mckit_meshes-0.1.4/src/mckit_meshes/wgtmesh.py
+-rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 mckit_meshes-0.1.4/PKG-INFO
```

### Comparing `mckit_meshes-0.1.3/LICENSE` & `mckit_meshes-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mckit_meshes-0.1.3/README.rst` & `mckit_meshes-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/cli/commands/mesh2npz.py` & `mckit_meshes-0.1.4/src/mckit_meshes/cli/commands/mesh2npz.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,48 +4,46 @@
 
 import typing as t
 
 import logging
 
 from pathlib import Path
 
-import mckit_meshes.fmesh as fmesh
-
-from ...utils.io import check_if_path_exists
+from mckit_meshes import fmesh
+from mckit_meshes.utils.io import check_if_path_exists
 
 __LOG = logging.getLogger(__name__)
 
 
-def revise_mesh_tallies(mesh_tallies) -> t.List[Path]:
+def revise_mesh_tallies(mesh_tallies) -> list[Path]:
     if mesh_tallies:
         return list(map(Path, mesh_tallies))
 
     cwd = Path.cwd()
     rv = list(cwd.glob("*.m"))
     if not rv:
-        errmsg = "No .m-files found in directory '{}', nothing to do.".format(cwd.absolute())
+        errmsg = f"No .m-files found in directory '{cwd.absolute()}', nothing to do."
         __LOG.warning(errmsg)
     return rv
 
 
 def mesh2npz(
-    prefix: str | Path, mesh_tallies: t.Iterable[str | Path], override: bool = False
+    prefix: str | Path,
+    mesh_tallies: t.Iterable[str | Path],
+    override: bool = False,
 ) -> None:
     """Convert MCNP meshtal file to a number of npz files, one for each mesh tally."""
     mesh_tallies = revise_mesh_tallies(mesh_tallies)
     single_input = len(mesh_tallies) == 1
     prefix = Path(prefix)
     for m in mesh_tallies:
-        m = Path(m)
-        if single_input:
-            p = prefix
-        else:
-            p = prefix / m.stem
-        __LOG.info("Processing {}".format(m))
-        __LOG.debug("Saving tallies with prefix {}".format(prefix))
+        _m = Path(m)
+        p = prefix if single_input else prefix / _m.stem
+        __LOG.info(f"Processing {_m}")
+        __LOG.debug(f"Saving tallies with prefix {prefix}")
         p.mkdir(parents=True, exist_ok=True)
-        with m.open() as stream:
+        with _m.open() as stream:
             fmesh.m_2_npz(
                 stream,
                 prefix=p,
                 check_existing_file_strategy=check_if_path_exists(override),
             )
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/cli/commands/npz2vtk.py` & `mckit_meshes-0.1.4/src/mckit_meshes/cli/commands/npz2vtk.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 import typing as t
 
 import logging
 
 from pathlib import Path
 
-import mckit_meshes.fmesh as fmesh
-
-from ...utils.io import check_if_path_exists
+from mckit_meshes import fmesh
+from mckit_meshes.utils.io import check_if_path_exists
 
 __LOG = logging.getLogger(__name__)
 
 
-def revise_npz_files(npz_files: t.Optional[t.Iterable[t.Any]]) -> t.List[Path]:
+def revise_npz_files(npz_files: t.Iterable[t.Any] | None) -> list[Path]:
     """Use specified list of file to process, if any, or find them in current directory.
 
     Args:
         npz_files: npz files to process passed from command line, optional.
 
     Returns:
         List of the specified or found files as Path objects.
@@ -43,19 +42,19 @@
         npz_files: files to process, optional
         override: define behaviour when output file, exists, default - rise FileExistsError.
     """
     npz_files = revise_npz_files(npz_files)
     prefix = Path(prefix)
     file_exists_strategy = check_if_path_exists(override)
     for npz in npz_files:
-        npz = Path(npz)
-        __LOG.info("Processing {}", npz)
+        _npz = Path(npz)
+        __LOG.info("Processing {}", _npz)
         __LOG.debug("Saving VTK file with prefix {}", prefix)
         prefix.mkdir(parents=True, exist_ok=True)
-        mesh = fmesh.FMesh.load_npz(npz)
+        mesh = fmesh.FMesh.load_npz(_npz)
         vtk_file_stem = f"{prefix / str(mesh.name)}"
         vtk_file_name = (
             vtk_file_stem + ".vtr"
         )  # TODO dvp: revise this when it comes to saving structured mesh
         file_exists_strategy(vtk_file_name)
         vtk = mesh.save2vtk(vtk_file_stem)
         __LOG.info("Saved VTK to {}", vtk)
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/cli/logging.py` & `mckit_meshes-0.1.4/src/mckit_meshes/cli/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Intercept log messages from the used libraries and pass them to `loguru`.
 
 See https://github.com/Delgan/loguru
 """
+from __future__ import annotations
+
 from typing import Final
 
 import logging
 import sys
 
 from os import environ
 
 from loguru import logger
 
 # class PropagateHandler(logging.Handler):
 #     """Send events from loguru to standard logging"""
 #     def emit(self, record):
-#         logging.getLogger(record.name).handle(record)
 #
 #
-# logger.add(PropagateHandler(), format="{message}")
 
 
 class InterceptHandler(logging.Handler):
     """Send events from standard logging to loguru."""
 
     def emit(self, record):
         # Get corresponding Loguru level if it exists
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/cli/runner.py` & `mckit_meshes-0.1.4/src/mckit_meshes/cli/runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 """The CLI application module.
 
 The module applies :meth:`click` API to organize CLI interface for McKit-meshes package.
 """
 from __future__ import annotations
 
-import typing as t
+from typing import TYPE_CHECKING
 
 import datetime
 
-from pathlib import Path
-
 import click
 import mckit_meshes.version as meta
 
 from mckit_meshes.cli.commands import do_mesh2npz, do_npz2vtk
-
-# from mckit_meshes.cli.commands.common import get_default_output_directory
 from mckit_meshes.cli.logging import init_logger, logger
 
-# from mckit_meshes.utils import MCNP_ENCODING
+if TYPE_CHECKING:
+    from pathlib import Path
 
 NAME = "mckit_meshes"
 VERSION = meta.__version__
-# LOG_FILE_RETENTION = 3
-# NO_LEVEL_BELOW = 30
 
 
 @click.group("mckit-meshes", help=meta.__summary__)
 @click.pass_context
 @click.option("--override/--no-override", is_flag=True, default=False)
 @click.option("--verbose/--no-verbose", is_flag=True, default=False, help="Log everything")
 @click.option(
@@ -35,15 +30,19 @@
     is_flag=True,
     default=False,
     help="Log only WARNINGS and above",
 )
 @click.option("--logfile", default=None, help="File to log to")
 @click.version_option(VERSION, prog_name=NAME)
 def mckit_meshes(
-    ctx: click.Context, verbose: bool, quiet: bool, logfile: str, override: bool
+    ctx: click.Context,
+    verbose: bool,
+    quiet: bool,
+    logfile: str,
+    override: bool,
 ) -> None:
     """McKit-meshes command line interface."""
     init_logger(logfile, quiet, verbose)
     # TODO dvp: add customized logger configuring from a configuration toml-file.
 
     obj = ctx.ensure_object(dict)
     obj["OVERRIDE"] = override
@@ -62,15 +61,15 @@
 @click.argument(
     "mesh_tallies",
     metavar="[<meshtally_file>...]",
     type=click.Path(exists=True),
     nargs=-1,
     required=False,
 )
-def mesh2npz(ctx: click.Context, prefix: str | Path, mesh_tallies: t.List[t.Any]) -> None:
+def mesh2npz(ctx: click.Context, prefix: str | Path, mesh_tallies: list[click.Path]) -> None:
     """Converts mesh files to npz files."""
     do_mesh2npz(prefix, mesh_tallies, ctx.obj["OVERRIDE"])
     #
 
 
 @mckit_meshes.command()
 @click.pass_context
@@ -85,18 +84,19 @@
 @click.argument(
     "npz_files",
     metavar="[<npz_file>...]",
     type=click.Path(exists=True),
     nargs=-1,
     required=False,
 )
-def npz2vtk(ctx: click.Context, prefix: str | Path, npz_files: t.List[t.Any]) -> None:
+def npz2vtk(ctx: click.Context, prefix: str | Path, npz_files: list[click.Path]) -> None:
     """Converts npz files to VTK files."""
     do_npz2vtk(prefix, npz_files, ctx.obj["OVERRIDE"])
     # Don't remove these comments: this makes flake8 happy on absent arguments in the docstring.
     #
 
 
 if __name__ == "__main__":
-    ct = datetime.datetime.now()
+    tz = datetime.timezone(datetime.timedelta(0))
+    ct = datetime.datetime.now(tz)
     mckit_meshes(obj={})
-    logger.success(f"Elapsed time: {datetime.datetime.now() - ct}")
+    logger.success(f"Elapsed time: {datetime.datetime.now(tz) - ct}")
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/fmesh.py` & `mckit_meshes-0.1.4/src/mckit_meshes/fmesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """Classes and functions for operations with fmesh tallies."""
 
 # TODO dvp: redesign this class as xarray data structure.
 #           multidimensional array with coordinates is more appropriate for this class.
 
 from __future__ import annotations
 
-from typing import Callable, Generator, Iterable, List, Optional, TextIO, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Generator, Iterable, TextIO
 
 import logging
 
 from pathlib import Path
+from textwrap import dedent
+
+import numpy as np
 
 import mckit_meshes.mesh.geometry_spec as gc
 import mckit_meshes.utils.no_daemon_process as ndp
-import mckit_meshes.utils.rebin as rebin
-import numpy as np
 
 from mckit_meshes.particle_kind import ParticleKind as Kind
+from mckit_meshes.utils import rebin
 from mckit_meshes.utils.io import raise_error_when_file_exists_strategy
-from numpy.typing import ArrayLike
 from pyevtk.hl import gridToVTK
 from toolz.itertoolz import concatv
 
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike
+
 __LOG = logging.getLogger(__name__)
 
 
 def _expand_args(args):
     """Adapter to invoke rebin.
 
     Args:
@@ -48,28 +52,28 @@
             This is used to check that the file is for FMesh object.
         NPZ_FORMAT: Identifies version of format of data stored in npz file.
     """
 
     NPZ_MARK = np.int16(5445)
     NPZ_FORMAT = np.int16(4)
 
-    class X(RuntimeError):
+    class FMeshError(RuntimeError):
         """FMesh class specific exception."""
 
     def __init__(
         self,
         name: int,
         kind: int | Kind,
         geometry_spec: gc.AbstractGeometrySpec,
         ebins: np.ndarray,
         data: np.ndarray,
         errors: np.ndarray,
-        totals: Optional[np.ndarray] = None,
-        totals_err: Optional[np.ndarray] = None,
-        comment: Optional[str] = None,
+        totals: np.ndarray | None = None,
+        totals_err: np.ndarray | None = None,
+        comment: str | None = None,
     ) -> None:
         """Construct FMesh instance object.
 
         Args:
             name: FMESH tally number
             kind: neutron, photon
             geometry_spec: mesh geometry specification
@@ -86,25 +90,25 @@
             totals_err: Can be provided with data from mesh file,
                     if there are more than 1 energy bin, optional.
             comment: Comment from a meshtal file (content of FC card in MCNP model).
         """
         self.name = int(name)
         self.kind = Kind(kind)
 
-        self._geometry_spec: Union[
-            gc.CartesianGeometrySpec, gc.CylinderGeometrySpec, gc.AbstractGeometrySpec
-        ] = geometry_spec
+        self._geometry_spec: gc.CartesianGeometrySpec | gc.CylinderGeometrySpec | gc.AbstractGeometrySpec = (
+            geometry_spec
+        )
         self.bins = {}
         self.bins["X"] = self._x = geometry_spec.ibins
         self.bins["Y"] = self._y = geometry_spec.jbins
         self.bins["Z"] = self._z = geometry_spec.kbins
         self.bins["E"] = self._e = gc.as_float_array(ebins)
         self.data = gc.as_float_array(data)
         self.errors = gc.as_float_array(errors)
-        if 2 < self._e.size:
+        if self._e.size > 2:
             if totals is None:
                 if totals_err is not None:
                     raise ValueError("totals are omitted but totals_err are provided")
                 self._totals = np.sum(self.data, axis=0)
                 non_zero = self._totals > 0.0
                 self._totals_err = np.zeros_like(self._totals)
                 self._totals_err[non_zero] = (
@@ -132,15 +136,15 @@
         """Check if there's more than 1 energy bin.
 
         If True, then totals and totals err should present.
 
         Returns:
             True if there are more than one energy bins.
         """
-        return 2 < self.e.size
+        return self.e.size > 2
 
     @property
     def ibins(self) -> np.ndarray:
         """Synonym to geometry bins x or R."""
         return self._geometry_spec.ibins
 
     @property
@@ -202,49 +206,54 @@
         Returns:
             True if this is a cylinder mesh.
         """
         return self._geometry_spec.cylinder
 
     @property
     def total_precision(self) -> float:
-        """"""
+        """Get total precision of this mesh.
+
+        Returns:
+            total precision from totals or errors, if there are no totals.
+        """
         if self.has_multiple_energy_bins:
             return self.totals_err[
                 -1
             ]  # TODO dvp: assumes max energy bin is most representative, check usage
-        else:
-            return self.errors[0, 0, 0, 0]
+        return self.errors[0, 0, 0, 0]
 
     def check_attributes(self) -> None:
         """Check consistency of attributes."""
-        assert 2 <= self._e.size
+        assert self._e.size >= 2
         assert self.data.shape == self.errors.shape
-        assert self.data.shape == (self.e.size - 1,) + self._geometry_spec.bins_shape
+        assert self.data.shape == (self.e.size - 1, *self._geometry_spec.bins_shape)
         assert (
             self._totals is None
             or isinstance(self._totals, np.ndarray)
             and isinstance(self._totals_err, np.ndarray)
             and self._totals.shape == self._totals_err.shape
             and self._totals.shape == self._geometry_spec.bins_shape
         )
 
-    def is_equal_by_mesh(self, other: "FMesh") -> bool:
-        """Args:
+    def is_equal_by_mesh(self, other: FMesh) -> bool:
+        """Check if the meshes are equivalent by kind and geometry.
 
+        Args:
           other: "FMesh":
 
         Returns:
+            True, if this mesh is equal to other by kind and geometry, otherwise False
         """
         return (
             self.kind == other.kind
             and self._geometry_spec == other._geometry_spec
             and np.array_equal(self.e, other.e)
         )
 
-    def has_better_precision_than(self, other: "FMesh") -> bool:
+    def has_better_precision_than(self, other: FMesh) -> bool:
         """Compare precision achieved for the meshes.
 
         Args:
             other: mesh
 
         Returns:
             True if this mesh is more precise than other one.
@@ -263,16 +272,19 @@
 
         Returns:
             True if point is within the mesh's grid.
         """
         return self._geometry_spec.surrounds_point(x, y, z, local)
 
     def get_spectrum(
-        self, x: ArrayLike, y: ArrayLike, z: ArrayLike
-    ) -> Tuple[ArrayLike, ArrayLike, ArrayLike]:
+        self,
+        x: ArrayLike,
+        y: ArrayLike,
+        z: ArrayLike,
+    ) -> tuple[ArrayLike, ArrayLike, ArrayLike]:
         """Gets energy spectrum at the specified point.
 
         Args:
             x: X, Y and Z coordinate of the point where energy spectrum is
                 required. If point is located outside the mesh, zeros are returned.
             y: ...
             z: ...
@@ -293,20 +305,20 @@
                 result_error *= 0
                 index = 0
             result_data = result_data.take(index, axis=i + 1)
             result_error = result_error.take(index, axis=i + 1)
         return self.e, result_data, result_error
 
     def select_indexes(
-        self, *, x: ArrayLike = None, y: ArrayLike = None, z: ArrayLike = None
-    ) -> Tuple[
-        Union[int, slice, np.ndarray],
-        Union[int, slice, np.ndarray],
-        Union[int, slice, np.ndarray],
-    ]:
+        self,
+        *,
+        x: ArrayLike = None,
+        y: ArrayLike = None,
+        z: ArrayLike = None,
+    ) -> tuple[int | slice | np.ndarray, int | slice | np.ndarray, int | slice | np.ndarray]:
         """Select indexes in spatial bins corresponding to given coordinates.
 
         If coordinate is not specified, then return all the points along this coordinate.
 
         Args:
             x:  (Default value = None)
             y:  (Default value = None)
@@ -314,16 +326,20 @@
 
         Returns:
             tuple of indexes along the coordinates
         """
         return self._geometry_spec.select_indexes(i_values=x, j_values=y, k_values=z)
 
     def get_totals(
-        self, *, x: ArrayLike = None, y: ArrayLike = None, z: ArrayLike = None
-    ) -> Optional[Tuple[np.ndarray, np.ndarray]]:
+        self,
+        *,
+        x: ArrayLike = None,
+        y: ArrayLike = None,
+        z: ArrayLike = None,
+    ) -> tuple[np.ndarray, np.ndarray] | None:
         """Get total values for specified grid points.
 
         If a coordinate is not specified, than all the points along this coordinate.
 
         Args:
             x:  (Default value = None)
             y:  (Default value = None)
@@ -380,15 +396,15 @@
             kwd["origin"] = np.array(self._geometry_spec.origin)
             kwd["axis"] = np.array(self._geometry_spec.axs)
 
         filename.parent.mkdir(parents=True, exist_ok=True)
         np.savez_compressed(str(filename), **kwd)
 
     @classmethod
-    def load_npz(cls, _file: Union[str, Path]) -> "FMesh":
+    def load_npz(cls, _file: str | Path) -> FMesh:
         """Loads Fmesh object from the binary file.
 
         Args:
           _file: npz-file to load from.
 
         Returns:
             The loaded FMesh object.
@@ -397,47 +413,47 @@
             _file = str(_file)
         with np.load(_file) as data:
             meta = data["meta"]
             mark = meta[0]
             assert mark == FMesh.NPZ_MARK, f"Incompatible file format {_file}"
             version = meta[1]
             name, kind = meta[2:4]
-            if 1 <= version:
+            if version >= 1:
                 e = data["E"]
                 x = data["X"]
                 y = data["Y"]
                 z = data["Z"]
                 d = data["data"]
                 r = data["errors"]
-                if 2 < e.size:
+                if e.size > 2:
                     try:
                         totals = data["totals"]
                         totals_err = data["totals_err"]
                     except KeyError:
                         totals = None
                         totals_err = None
                 else:
                     totals = None
                     totals_err = None
                 comment = None
                 origin = None
                 axis = None
-                if 2 <= version:
+                if version >= 2:
                     if "comment" in data:
                         comment = data["comment"]
                         comment = comment.item()
                         assert comment
-                    if 3 <= version:
+                    if version >= 3:
                         if "origin" in data:
                             assert "axis" in data
                             origin = data["origin"]
                             axis = data["axis"]
                             assert origin.size == 3
                             assert axis.size == 3
-                        if 4 <= version:
+                        if version >= 4:
                             pass
                         else:
                             kind = int(kind) + 1
                 if origin is None:
                     geometry_spec = gc.CartesianGeometrySpec(x, y, z)
                 else:
                     geometry_spec = gc.CylinderGeometrySpec(x, y, z, origin=origin, axs=axis)
@@ -448,16 +464,15 @@
                     e,
                     d,
                     r,
                     totals,
                     totals_err,
                     comment=comment,
                 )
-            else:
-                raise FMesh.X("Invalid version for FMesh file %d" % version)
+            raise FMesh.FMeshError("Invalid version for FMesh file %d" % version)
 
     def save2vtk(self, filename: str = None, data_name: str = None) -> str:
         """Saves this fmesh data to vtk file.
 
         Data is saved for every energy bin and, if there are multiple energy bins,
         for total values (sum across energy axis).
 
@@ -476,40 +491,39 @@
         if filename is None:
             filename = str(self.name)
         if data_name is None:
             data_name = str(self.name) + " " + self.kind.name
 
         cell_data = {}
         for i, e in enumerate(self.e[1:]):
-            key = data_name + " E={0:.4e}".format(e)
+            key = data_name + f" E={e:.4e}"
             cell_data[key] = self.data[i, :, :, :]
         if self.has_multiple_energy_bins:
             name = data_name + " total"
             cell_data[name] = np.sum(self.data, axis=0)
         return gridToVTK(filename, self.ibins, self.jbins, self.kbins, cellData=cell_data)
 
     # noinspection PyUnresolvedReferences
     def save_2_mcnp_mesh(self, stream: TextIO) -> None:
         """Saves the mesh in a file in a format similar to mcnp mesh tally textual representation.
 
         Args:
             stream: stream to store the mesh.
         """
 
-        def format_comment(a: "FMesh") -> str:
+        def format_comment(a: FMesh) -> str:
             return "\n" + a.comment if a.comment else ""
 
-        header = f"""
- Mesh Tally Number   {self.name}{format_comment(self)}
- This is a {self.kind.name} mesh tally.
-
- Tally bin boundaries:{self.format_cylinder_origin_and_axis_label()}
-"""[
-            1:-1
-        ]
+        header = dedent(
+            f"""\
+             Mesh Tally Number   {self.name}{format_comment(self)}
+             This is a {self.kind.name} mesh tally.
+
+             Tally bin boundaries:{self.format_cylinder_origin_and_axis_label()}""",
+        )
         e = self.e[1:]
         x = 0.5 * (self.ibins[1:] + self.ibins[:-1])
         y = 0.5 * (self.jbins[1:] + self.jbins[:-1])
         z = 0.5 * (self.kbins[1:] + self.kbins[:-1])
         print(header, file=stream)
         print(
             f"{'R' if self.is_cylinder else 'X'} direction:",
@@ -552,15 +566,15 @@
 
         for ie in range(e.size):
             for ix in range(x.size):
                 for iy in range(y.size):
                     for iz in range(z.size):
                         value = self.data[ie, ix, iy, iz]
                         err = self.errors[ie, ix, iy, iz]
-                        row = " %10.3e%10.3f%10.3f%10.3f %11.5e %11.5e" % (
+                        row = " {:10.3e}{:10.3f}{:10.3f}{:10.3f} {:11.5e} {:11.5e}".format(
                             e[ie],
                             x[ix],
                             y[iy],
                             z[iz],
                             value,
                             err,
                         )
@@ -585,15 +599,15 @@
                         value,
                         err,
                     )
                     print(row, file=stream, end="")
 
             print("\n", file=stream)
 
-    def total_by_energy(self, new_name: int = 0) -> "FMesh":
+    def total_by_energy(self, new_name: int = 0) -> FMesh:
         """Integrate over energy bins.
 
         Args:
             new_name: name for new `FMesh`  (Default value = 0)
 
         Returns:
             The new FMesh object with only one energy bin.
@@ -610,15 +624,15 @@
         xmin=None,
         xmax=None,
         ymin=None,
         ymax=None,
         zmin=None,
         zmax=None,
         new_name=-1,
-    ) -> "FMesh":
+    ) -> FMesh:
         """Select subset of e-voxels within given geometry and energy limits.
 
         Args:
             emin:  limits for new bins
             emax:  (Default value = None)
             xmin:  (Default value = None)
             xmax:  (Default value = None)
@@ -632,15 +646,15 @@
             A new FMesh with reduced bins.
         """
         trim_spec = list(
             rebin.trim_spec_composer(
                 [self.e, self.ibins, self.jbins, self.kbins],
                 [emin, xmin, ymin, zmin],
                 [emax, xmax, ymax, zmax],
-            )
+            ),
         )
         new_bins_list, new_data = rebin.shrink_nd(self.data, iter(trim_spec), assume_sorted=True)
         _, new_errors = rebin.shrink_nd(self.errors, iter(trim_spec), assume_sorted=True)
 
         assert all(np.array_equal(a, b) for a, b in zip(new_bins_list, _))
 
         new_ebins, new_xbins, new_ybins, new_zbins = new_bins_list
@@ -649,19 +663,21 @@
             new_totals_err = None
         else:
             totals_trim_spec = list(
                 rebin.trim_spec_composer(
                     [self.ibins, self.jbins, self.kbins],
                     [xmin, ymin, zmin],
                     [xmax, ymax, zmax],
-                )
+                ),
             )
             _, new_totals = rebin.shrink_nd(self.totals, iter(totals_trim_spec), assume_sorted=True)
             _, new_totals_err = rebin.shrink_nd(
-                self.totals_err, iter(totals_trim_spec), assume_sorted=True
+                self.totals_err,
+                iter(totals_trim_spec),
+                assume_sorted=True,
             )
 
         return FMesh(
             new_name,
             self.kind,
             gc.CartesianGeometrySpec(new_xbins, new_ybins, new_zbins),
             new_ebins,
@@ -674,15 +690,15 @@
     def rebin(
         self,
         new_x: np.ndarray,
         new_y: np.ndarray,
         new_z: np.ndarray,
         new_name=-1,
         extra_process_threshold: int = 1000000,
-    ) -> "FMesh":
+    ) -> FMesh:
         """Extract data for a new spatial grid.
 
         Args:
             new_x: A new binning over X axis.
             new_y: A new binning over Y axis.
             new_z: A new binning over Z axis.
             new_name: A name for the rebinned mesh to be created. (Default value = -1)
@@ -699,23 +715,24 @@
         # To avoid huge memory allocations, iterate over energy with external processes
         pool = ndp.Pool(processes=4)
         data_rebin_spec = list(
             rebin.rebin_spec_composer(
                 [self.ibins, self.jbins, self.kbins],
                 [new_x, new_y, new_z],
                 axes=[0, 1, 2],
-            )
+            ),
         )
 
         def iter_over_e(data):
             for i in range(self.e.size - 1):
                 yield data[i], data_rebin_spec, True
 
         new_data = np.stack(
-            pool.map(_expand_args, iter_over_e(self.data)), axis=0
+            pool.map(_expand_args, iter_over_e(self.data)),
+            axis=0,
         )  # : ignore[PD013]
         t = self.data * self.errors
         new_errors = np.stack(pool.map(_expand_args, iter_over_e(t)), axis=0)  # : ignore[PD013]
         new_errors /= new_data
         if self.totals is None:
             new_totals = None
             new_totals_err = None
@@ -738,15 +755,15 @@
 
     def rebin_single(
         self,
         new_x: np.ndarray,
         new_y: np.ndarray,
         new_z: np.ndarray,
         new_name: int = -1,
-    ) -> "FMesh":
+    ) -> FMesh:
         """Create FMesh object corresponding to this one by fluxes, but over new mesh.
 
         Ags:
             new_x: A new binning over X axis.
             new_y: A new binning over Y axis.
             new_z: A new binning over Z axis.
             new_name: name for the rebinned mesh to be created.
@@ -757,30 +774,30 @@
         assert not self.is_cylinder, "Not implemented for cylinder meshes"
 
         data_rebin_spec = list(
             rebin.rebin_spec_composer(
                 [self.ibins, self.jbins, self.kbins],
                 [new_x, new_y, new_z],
                 axes=[1, 2, 3],
-            )
+            ),
         )
         new_data = rebin.rebin_nd(self.data, iter(data_rebin_spec), assume_sorted=True)
         t = self.data * self.errors
         new_errors = rebin.rebin_nd(t, iter(data_rebin_spec), assume_sorted=True)
         new_errors /= new_data
         if self.totals is None:
             new_totals = None
             new_totals_err = None
         else:
             totals_rebin_spec = list(
                 rebin.rebin_spec_composer(
                     [self.ibins, self.jbins, self.kbins],
                     [new_x, new_y, new_z],
                     axes=[0, 1, 2],
-                )
+                ),
             )
             new_totals = rebin.rebin_nd(self.totals, iter(totals_rebin_spec), assume_sorted=True)
             t = self.totals * self.totals_err
             new_totals_err = rebin.rebin_nd(t, iter(totals_rebin_spec), assume_sorted=True)
             new_totals_err /= new_totals
 
         return FMesh(
@@ -811,29 +828,29 @@
             and self.is_equal_by_mesh(other)
             and np.array_equal(self.data, other.data)
             and np.array_equal(self.errors, other.errors)
             and self.comment == other.comment
         )
         if res and self._totals:
             res = np.all(np.isclose(self.totals, other.totals)) and np.all(
-                np.isclose(self.totals_err, other.totals_err)
+                np.isclose(self.totals_err, other.totals_err),
             )
         return res
 
     def __hash__(self) -> int:
         return hash(
             (
                 self.name,
                 self.kind,
                 self._geometry_spec,
                 self.e,
                 self.data,
                 self.errors,
                 self.comment,
-            )
+            ),
         )
 
     def __repr__(self) -> str:
         msg = (
             "Fmesh({name}, {kind}, {xmin}..{xmax}, {ymin}..{ymax}, {zmin}..{zmax}, {emin}..{emax})"
         )
         (xmin, xmax), (ymin, ymax), (zmin, zmax) = self._geometry_spec.boundaries
@@ -849,15 +866,18 @@
             emin=self.e[0],
             emax=self.e[-1],
         )
 
 
 # noinspection PyTypeChecker,PyProtectedMember
 def merge_tallies(
-    name: int, kind: int, *tally_weight: Tuple[FMesh, float], comment: str = None
+    name: int,
+    kind: int,
+    *tally_weight: tuple[FMesh, float],
+    comment: str = None,
 ) -> FMesh:
     """Makes superposition of tallies with specific weights.
 
     Args:
         name: Name of new fmesh tally.
         kind: Type of new fmesh tally. It can be -1 (or any arbitrary integer).
         tally_weight: List of tally-weight pairs (tuples). tally is FMesh instance. weight
@@ -878,15 +898,16 @@
             geometry_spec = t._geometry_spec
             ebins = t.e
         else:
             result_data += t.data * w
             errors += (t.errors * t.data * w) ** 2
             assert geometry_spec == t._geometry_spec
             assert np.array_equal(
-                ebins.size, t.e.size
+                ebins.size,
+                t.e.size,
             )  # allow merging neutron and photon heating meshes
     nonzero_idx = np.logical_and(result_data > 0.0, errors > 0.0)
     result_error = np.zeros_like(result_data)
     result_error[nonzero_idx] = np.sqrt(errors[nonzero_idx]) / result_data[nonzero_idx]
     return FMesh(
         name,
         kind,
@@ -894,29 +915,29 @@
         ebins,
         result_data,
         result_error,
         comment=comment,
     )
 
 
-def read_meshtal(stream: TextIO, select=None, mesh_file_info=None) -> List[FMesh]:
+def read_meshtal(stream: TextIO, select=None, mesh_file_info=None) -> list[FMesh]:
     """Reads fmesh tallies from a stream.
 
     Args:
         stream: The text stream to read.
         select: Selects the meshes actually to process (Default value = None)
         mesh_file_info: object to collect information from m-file header (Default value = None)
 
     Returns:
         The list of individual fmesh tally.
     """
     next(stream)  # TODO dvp check if we need to store problem time stamp
     next(stream)  # TODO dvp check if we need to store problem title
     line = next(stream)
-    nps = int(float((line.strip().split("=")[1])))
+    nps = int(float(line.strip().split("=")[1]))
     if mesh_file_info is not None:
         mesh_file_info.nps = nps
     return list(iter_meshtal(stream, select))
 
 
 def _iterate_bins(stream, _n, _with_ebins):
     """Parse line with mesh values.
@@ -926,15 +947,15 @@
         _n: number of items
         _with_ebins: are ebins specified
 
     Yields:
         pairs value - error
     """
     value_start, value_end = (41, 53) if _with_ebins else (32, 44)
-    for _i in range(_n):
+    for _ in range(_n):
         _line = next(stream)
         _value = float(_line[value_start:value_end])
         _error = float(_line[value_end:])
         if _value < 0.0:
             _value = _error = 0.0
         yield _value
         yield _error
@@ -985,76 +1006,82 @@
                     part1, part2 = line.split(",")
                     origin = np.fromiter(part1.split()[3:6], dtype=float)
                     axis = np.fromiter(part2.split()[2:5], dtype=float)
                     ibins = np.array(
                         [
                             float(w)
                             for w in _find_words_after(concatv([line], fid), "R", "direction:")
-                        ]
+                        ],
                     )
 
                     jbins = np.array([float(w) for w in _find_words_after(fid, "Z", "direction:")])
 
                     kbins = np.array(
                         [
                             float(w)
                             for w in _find_words_after(fid, "Theta", "direction", "(revolutions):")
-                        ]
+                        ],
                     )
 
                     geometry_spec = gc.CylinderGeometrySpec(
-                        ibins, jbins, kbins, origin=origin, axs=axis
+                        ibins,
+                        jbins,
+                        kbins,
+                        origin=origin,
+                        axs=axis,
                     )
 
                     ebins = np.array(
-                        [float(w) for w in _find_words_after(fid, "Energy", "bin", "boundaries:")]
+                        [float(w) for w in _find_words_after(fid, "Energy", "bin", "boundaries:")],
                     )
                     with_ebins = check_ebins(
-                        fid, ["Energy", "R", "Z", "Th", "Result", "Rel", "Error"]
+                        fid,
+                        ["Energy", "R", "Z", "Th", "Result", "Rel", "Error"],
                     )
                 else:
                     xbins = np.array(
                         [
                             float(w)
                             for w in _find_words_after(concatv([line], fid), "X", "direction:")
-                        ]
+                        ],
                     )
 
                     ybins = np.array([float(w) for w in _find_words_after(fid, "Y", "direction:")])
 
                     zbins = np.array([float(w) for w in _find_words_after(fid, "Z", "direction:")])
 
                     geometry_spec = gc.CartesianGeometrySpec(xbins, ybins, zbins)
 
                     ebins = np.array(
-                        [float(w) for w in _find_words_after(fid, "Energy", "bin", "boundaries:")]
+                        [float(w) for w in _find_words_after(fid, "Energy", "bin", "boundaries:")],
                     )
                     with_ebins = check_ebins(
-                        fid, ["Energy", "X", "Y", "Z", "Result", "Rel", "Error"]
+                        fid,
+                        ["Energy", "X", "Y", "Z", "Result", "Rel", "Error"],
                     )
 
                 spatial_bins_size = geometry_spec.bins_size
                 bins_size = spatial_bins_size * (ebins.size - 1)
 
                 data_items = np.fromiter(_iterate_bins(fid, bins_size, with_ebins), dtype=float)
                 data_items = data_items.reshape(bins_size, 2)
-                shape = (ebins.size - 1,) + geometry_spec.bins_shape
+                shape = (ebins.size - 1, *geometry_spec.bins_shape)
                 data, error = data_items[:, 0].reshape(shape), data_items[:, 1].reshape(shape)
 
                 def _iterate_totals(stream, totals_number):
                     """Reading totals.
 
                     Args:
                         stream: sequence or stream of strings
                         totals_number: number of items to read
 
                     Yields:
                         total values and errors
                     """
-                    for _i in range(totals_number):
+                    for _ in range(totals_number):
                         _line = next(stream).split()
                         # TODO dvp: check for negative values in an MCNP meshtal file
                         assert _line[0] == "Total"
                         for w in _line[4:]:
                             yield float(w)
 
                 if ebins.size > 2:  # Totals are not output if there's only one bin in energy domain
@@ -1081,15 +1108,15 @@
                     yield res
                 else:
                     __LOG.debug("Skipping mesh tally %s", name)
     except EOFError:
         pass
 
 
-def check_ebins(fid: Iterable[str], keys: List[str]) -> bool:
+def check_ebins(fid: Iterable[str], keys: list[str]) -> bool:
     """Check if energy bins present in a mesh tally output values.
 
     If next nonempty line starts with a word keys[0] (i.e. "Energy"), then the energy bins present.
     Also check that the remaining keys correspond to the nonempty line.
 
     Args:
         fid: text rows to scan, including prepending empty rows
@@ -1112,26 +1139,26 @@
     else:
         if keys[1:] != title_line:
             raise ValueError(f"Unexpected values title {title_line}")
         with_ebins = False
     return with_ebins
 
 
-def _next_not_empty_line(f: Iterable[str]) -> Optional[List[str]]:
+def _next_not_empty_line(f: Iterable[str]) -> list[str] | None:
     """Skip empty lines from a string sequence.
 
     Args:
         f: sequence or stream of strings
 
     Returns:
         The first not empty line.
     """
     for line in f:
         words = line.split()
-        if 0 < len(words):
+        if len(words) > 0:
             return words
     return None
 
 
 def _find_words_after(f: TextIO, *keywords: str) -> list[str]:
     """Searches for words that follow keywords.
 
@@ -1151,15 +1178,15 @@
         i = 0  # : ignore[SIM113]
         for w, kw in zip(words, keywords):
             if w != kw:
                 break
             i += 1
         if i >= len(keywords):
             return words[i:]
-    raise EOFError()
+    raise EOFError
 
 
 def m_2_npz(
     stream: TextIO,
     prefix: Path,
     *,
     name_select=lambda _: True,
@@ -1188,15 +1215,15 @@
 
     Returns:
         Total number of files created
     """
     next(stream)  # TODO dvp check if we need to store problem time stamp
     next(stream)  # TODO dvp check if we need to store problem title
     line = next(stream)
-    nps = int(float((line.strip().split("=")[1])))
+    nps = int(float(line.strip().split("=")[1]))
     if mesh_file_info is not None:
         mesh_file_info.nps = nps
     total = 0  # : ignore[SIM113]
     for t in iter_meshtal(stream, name_select=name_select, tally_select=tally_select):
         t.save_2_npz(prefix / (str(t.name) + suffix), check_existing_file_strategy)
         total += 1
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/mesh/geometry_spec.py` & `mckit_meshes-0.1.4/src/mckit_meshes/mesh/geometry_spec.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,24 +24,25 @@
 
     The new callers are to use local_coordinates converter to avoid difficulties.
     For the old callers we will use ZERO_ORIGIN for Geometry Specification being
     used in FMesh.
 """
 from __future__ import annotations
 
-from typing import Final, Iterable, List, Optional, Sequence, TextIO, Tuple, Union, cast
+from typing import Final, Iterable, Sequence, TextIO, cast
 
 import abc
 
 from dataclasses import dataclass, field
 
-import mckit_meshes.utils as ut
-import mckit_meshes.utils.io
 import numpy as np
-import numpy.linalg as linalg
+
+from numpy import linalg
+
+import mckit_meshes.utils.io
 
 from mckit_meshes.utils.cartesian_product import cartesian_product
 
 _2PI: Final[float] = 2.0 * np.pi
 _1_TO_2PI: Final[float] = 1 / _2PI
 __DEG_2_RAD: Final[float] = np.pi / 180.0
 CARTESIAN_BASIS: Final[np.ndarray] = np.eye(3, dtype=np.double)
@@ -87,22 +88,22 @@
         for b in self.bins:
             if not isinstance(b, np.ndarray):
                 raise TypeError(f"Expected numpy array, actual {b[0]}...{b[-1]}")
 
     def __hash__(self) -> int:
         return hash(self.bins)
 
-    def __eq__(self, other: "AbstractGeometrySpecData") -> bool:
+    def __eq__(self, other: AbstractGeometrySpecData) -> bool:
         if not isinstance(other, AbstractGeometrySpecData):
             return False
         a, b = self.bins, other.bins
         return len(a) == len(b) and arrays_equal(zip(a, b))
 
     @property
-    def bins(self) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+    def bins(self) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
         """Pack the fields to tuple.
 
         Returns:
             tuple of origin and bins.
         """
         return self.origin, self.ibins, self.jbins, self.kbins
 
@@ -148,15 +149,15 @@
             indent: indent to insert before lines
         """
         ...
 
     # Generic methods
 
     @property
-    def bins_shape(self) -> Tuple[int, int, int]:
+    def bins_shape(self) -> tuple[int, int, int]:
         """Shape of data corresponding to spatial bins.
 
         Returns:
             Tuple with the data shape.
         """
         return (self.ibins.size - 1), (self.jbins.size - 1), (self.kbins.size - 1)
 
@@ -177,35 +178,35 @@
                 self.ibins[[0, -1]],
                 self.jbins[[0, -1]],
                 self.kbins[[0, -1]],
             ),
         )
 
     @property
-    def boundaries_shape(self) -> Tuple[int, int, int]:
+    def boundaries_shape(self) -> tuple[int, int, int]:
         """Bins (boundaries) shape."""
         return self.ibins.size, self.jbins.size, self.kbins.size
 
     def surrounds_point(self, x: float, y: float, z: float, local: bool = True) -> bool:
         """Check if the point (x,y,z) is within the volume of mesh.
 
         By default, assumes that the point is given in local coordinates.
         """
         if not local:
             x, y, z = self.local_coordinates(np.array([x, y, z], dtype=float))
         (xmin, xmax), (ymin, ymax), (zmin, zmax) = self.boundaries
         return cast(bool, (xmin < x < xmax) and (ymin < y < ymax) and (zmin < z < zmax))
 
     def select_indexes(
-        self, *, i_values=None, j_values=None, k_values=None
-    ) -> Tuple[
-        Union[int, slice, np.ndarray],
-        Union[int, slice, np.ndarray],
-        Union[int, slice, np.ndarray],
-    ]:
+        self,
+        *,
+        i_values=None,
+        j_values=None,
+        k_values=None,
+    ) -> tuple[int | slice | np.ndarray, int | slice | np.ndarray, int | slice | np.ndarray]:
         """Select indices for data corresponding to given spatial values.
 
         Args:
             i_values: indices along i (X or R) dimension
             j_values: ... along j (Y or Z)
             k_values: ... along k (Z or Theta)
 
@@ -214,25 +215,24 @@
         """
         return (
             select_indexes(self.ibins, i_values),
             select_indexes(self.jbins, j_values),
             select_indexes(self.kbins, k_values),
         )
 
-    def print(self, io: TextIO, columns: int = 6) -> None:
+    def print_specification(self, io: TextIO, columns: int = 6) -> None:
         indent = " " * 8
         self.print_geom(io, indent)
         print(indent, "origin=", " ".join(format_floats(self.origin)), sep="", file=io)
         _print_bins(indent, "i", self.ibins, io, columns=columns)
         _print_bins(indent, "j", self.jbins, io, columns=columns)
         _print_bins(indent, "k", self.kbins, io, columns=columns)
 
 
 class CartesianGeometrySpec(AbstractGeometrySpec):
-
     # TODO dvp: add transformation
 
     @property
     def cylinder(self) -> bool:
         return False
 
     @property
@@ -247,48 +247,48 @@
     def z(self) -> np.ndarray:
         return self.kbins
 
     def local_coordinates(self, points: np.ndarray) -> np.ndarray:
         assert points.shape[-1] == 3, "Expected cartesian point array or single point"
         if self.origin is not ZERO_ORIGIN:
             return cast(
-                np.ndarray, points - ZERO_ORIGIN
+                np.ndarray,
+                points - ZERO_ORIGIN,
             )  # TODO dvp: recall what is this subtraction for?
-        else:
-            return points
+        return points
 
     def print_geom(self, io: TextIO, indent: str) -> None:
         pass  # Defaults will do for cartesian mesh
 
     def get_mean_square_distance_weights(self, point):
         ni, nj, nk = self.bins_shape
 
         def calc_sum(bins):
             bins_square = np.square(bins)
             bins_mult = bins[:-1] * bins[1:]
             bins_square = bins_square[:-1] + bins_square[1:] + bins_mult
             return bins_square
 
-        x_square, y_square, z_square = [
+        x_square, y_square, z_square = (
             calc_sum(x - px) for x, px in zip((self.ibins, self.jbins, self.kbins), point)
-        ]
+        )
         w = np.zeros((ni, nj, nk), dtype=float)
         for i in range(ni):
             for j in range(nj):
                 for k in range(nk):
                     w[i, j, k] = x_square[i] + y_square[j] + z_square[k]
         w = (1.0 / 3.0) * w
 
         w = w * (1024.0 / np.max(w))
 
         return w
 
     def calc_cell_centers(self):
         raise NotImplementedError(
-            f"{self.__class__.__name__} has not implemented method calc_cell_centers"
+            f"{self.__class__.__name__} has not implemented method calc_cell_centers",
         )
 
 
 @dataclass(eq=False)
 class CylinderGeometrySpec(AbstractGeometrySpec):
     """Cylinder spec.
 
@@ -299,28 +299,26 @@
 
     axs: np.ndarray = field(default_factory=lambda: DEFAULT_AXIS.copy())
     vec: np.ndarray = field(default_factory=lambda: DEFAULT_VEC.copy())
 
     def __post_init__(self):
         super().__post_init__()
 
-        if self.axs is not DEFAULT_AXIS:
-            if not isinstance(self.axs, np.ndarray):
-                raise TypeError(f"Expected axs as numpy array, actual {self.axs}")
-
-        if self.vec is not DEFAULT_VEC:
-            if not isinstance(self.vec, np.ndarray):
-                raise TypeError(f"Expected vec as numpy array, actual {self.vec}")
+        if self.axs is not DEFAULT_AXIS and not isinstance(self.axs, np.ndarray):
+            raise TypeError(f"Expected axs as numpy array, actual {self.axs}")
+
+        if self.vec is not DEFAULT_VEC and not isinstance(self.vec, np.ndarray):
+            raise TypeError(f"Expected vec as numpy array, actual {self.vec}")
 
         if not (self.theta[0] == 0.0 and self.theta[-1] == 1.0):
             raise ValueError("Theta is expected in rotations only")
 
     @property
     def bins(self):
-        return super().bins + (self.axs, self.vec)
+        return (*super().bins, self.axs, self.vec)
 
     @property
     def cylinder(self) -> bool:
         return True
 
     @property
     def r(self) -> np.ndarray:
@@ -332,23 +330,22 @@
 
     @property
     def theta(self) -> np.ndarray:
         return self.kbins
 
     def local_coordinates(self, points: np.ndarray) -> np.ndarray:
         assert points.shape[-1] == 3, "Expected cartesian point array or single point"
-        assert np.array_equal(self.axs, DEFAULT_AXIS) and (
+        assert np.array_equal(
+            self.axs,
+            DEFAULT_AXIS,
+        ), "Tilted cylinder meshes are not implemented yet"
+        assert (
             np.array_equal(self.vec, DEFAULT_VEC) or self.vec[1] == 0.0  # vec is in xz plane
         ), "Tilted cylinder meshes are not implemented yet"
         # TODO dvp: implement tilted cylinder meshes
-        # ez = self.axs / np.linalg.norm(self.axs)
-        # ey = np.cross(ez, self.vec)
-        # ey /= np.linalg.norm(ey)
-        # ex = np.cross(ey, ez)
-        # ex /= np.linalg.norm(ex)
         local_points: np.ndarray = points - self.origin
         local_points[..., :] = (
             np.sqrt(local_points[..., 0] ** 2 + local_points[..., 1] ** 2),  # r
             local_points[..., 2],  # z, just copy
             np.arctan2(local_points[..., 1], local_points[..., 0])
             * _1_TO_2PI,  # theta in rotations
         )
@@ -381,15 +378,15 @@
         phi = phi * _2PI
         z = self.jbins
         px, py, pz = (
             point - self.origin
         )  # TODO dvp: apply local_coordinates instead of the following
         l1_square = px**2 + py**2
         l1 = np.sqrt(l1_square)  # distance to origin from point projection on z=0 plane
-        assert 0.0 < l1
+        assert l1 > 0.0
         # Terms of integration of L^2 in cylindrical coordinates
         # r^2
         gamma = np.arcsin(py / l1)
         r_square = np.square(r)
         r_square = 0.5 * (r_square[1:] + r_square[:-1])
         r_sum = r[1:] + r[:-1]
         r_mult = r[1:] * r[:-1]
@@ -439,45 +436,46 @@
             return np.array([x, y, z], dtype=float)
 
         cell_centers: np.ndarray = cartesian_product(r_mids, z_mids, t_mids, aggregator=_aggregator)
 
         return cell_centers
 
     # def __hash__(self):
-    #     return hash((super().__hash__(), self.axs, self.vec))
     #
     # def __eq__(self, other):
     #     if not isinstance(other, CylinderGeometrySpec):
-    #         return False
     #     return (
-    #         super().__eq__(other)
     #         and np.array_equal(self.axs, other.axs)
     #         and np.array_equal(self.vec, other.vec)
-    #     )
 
-    def adjust_axs_vec_for_mcnp(self) -> "CylinderGeometrySpec":
+    def adjust_axs_vec_for_mcnp(self) -> CylinderGeometrySpec:
         """Set `axs` and `vec` attributes to the values, which MCNP considers orthogonal.
 
         Assumptions
         -----------
 
         Cylinder mesh is not tilted:
             - `self.vec` is in PY=0 plane
             - `self.axs` is vertical
 
-        Returns
+        Returns:
         -------
         gs:
             new CylinderGeometrySpec with adjusted `axs` and `vec` attributes.
         """
         # TODO dvp: fix for arbitrary axs and vec
         axs = self.origin + DEFAULT_AXIS * self.z[-1]
         vec = self.origin + DEFAULT_VEC * self.r[-1]
         return CylinderGeometrySpec(
-            self.r, self.z, self.theta, origin=self.origin, axs=axs, vec=vec
+            self.r,
+            self.z,
+            self.theta,
+            origin=self.origin,
+            axs=axs,
+            vec=vec,
         )
 
 
 def _print_bins(indent, prefix, _ibins, io, columns: int = 6) -> None:
     intervals, coarse_mesh = compute_intervals_and_coarse_bins(_ibins)
     coarse_mesh = coarse_mesh[1:]  # drop the first value - it's presented with origin
     print(indent, f"{prefix}mesh=", sep="", end="", file=io)
@@ -489,22 +487,22 @@
         max_columns=columns,
     )
     print(indent, f"{prefix}ints=", sep="", end="", file=io)
     mckit_meshes.utils.io.print_n(intervals, io=io, indent=second_indent, max_columns=columns)
 
 
 def select_indexes(
-    a: np.ndarray, x: Optional[Union[float, List[float], np.ndarray]]
-) -> Union[int, slice, np.ndarray]:
+    a: np.ndarray,
+    x: float | list[float] | np.ndarray | None,
+) -> int | slice | np.ndarray:
     """Find indexes for a mesh bin, corresponding given coordinates.
 
     Assumes that `a` is sorted.
 
     Examples:
-
         >>> r = np.arange(5)
         >>> r
         array([0, 1, 2, 3, 4])
 
         For x is None return slice over all `a` indexes.
 
         >>> select_indexes(r, None)
@@ -538,45 +536,44 @@
     Args:
         a:  bin boundaries
         x: one or more coordinates along `a`-boundaries
 
     Returns:
         out: index or indices for each given coordinate
     """
-    assert 1 < a.size, "Parameter a doesn't represent binning"
+    assert a.size > 1, "Parameter a doesn't represent binning"
 
     if x is None:
-        return slice(0, a.size) if 2 < a.size else 0  # squeeze if there's only one bin
+        return slice(0, a.size) if a.size > 2 else 0  # squeeze if there's only one bin
 
     i: np.ndarray = a.searchsorted(x) - 1
 
     if np.isscalar(i):
-        if i < 0:
-            if x == a[0]:
-                return 0
+        if i < 0 and x == a[0]:
+            return 0
     else:
         neg = i < 0
         if np.any(neg):
             eq_to_min = a[0] == x
             i[np.logical_and(neg, eq_to_min)] = 0
 
     return i
 
 
 def format_floats(floats: Iterable[float], _format="{:.6g}") -> Iterable[str]:
     yield from map(_format.format, floats)
 
 
 def compute_intervals_and_coarse_bins(
-    arr: Sequence[float], tolerance: float = 1.0e-4
-) -> Tuple[List[int], Sequence[float]]:
+    arr: Sequence[float],
+    tolerance: float = 1.0e-4,
+) -> tuple[list[int], Sequence[float]]:
     """Compute fine intervals and coarse binning.
 
     Examples:
-
     Find equidistant bins and report as intervals
     >>> arr = np.array([1, 2, 3, 4], dtype=float)
     >>> arr
     array([1., 2., 3., 4.])
     >>> intervals, coarse = compute_intervals_and_coarse_bins(arr)
     >>> intervals
     [3]
@@ -621,12 +618,9 @@
             coarse_bins.append(arr[i - 1])
             count = 1
     fine_intervals.append(count)
     coarse_bins.append(arr[-1])
     return fine_intervals, coarse_bins
 
 
-def arrays_equal(arrays: Iterable[Tuple[np.ndarray, np.ndarray]]) -> bool:
-    for a, b in arrays:
-        if not (a is b or np.array_equal(a, b)):
-            return False
-    return True
+def arrays_equal(arrays: Iterable[tuple[np.ndarray, np.ndarray]]) -> bool:
+    return all(a is b or np.array_equal(a, b) for a, b in arrays)
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/mesh2com.py` & `mckit_meshes-0.1.4/src/mckit_meshes/mesh2com.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sys
 
 
 def mesh2com(xbins, ybins, zbins, out=sys.stdout):
     """Prints content for mcnp com file to plot crossections over mesh.
 
     voxels centers and with normals in x, y and z directions.
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/particle_kind.py` & `mckit_meshes-0.1.4/src/mckit_meshes/particle_kind.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Particle kinds enumeration and methods."""
-
+from __future__ import annotations
 
 from enum import IntEnum
 
 
 class ParticleKind(IntEnum):
     """Particle kinds enumeration and methods."""
 
@@ -31,11 +31,10 @@
             reaction specification for neutron or photon particle
 
         Raises:
             ValueError: if there's no specification for the particle
         """
         if self is self.n:
             return "1 -4"
-        elif self is self.p:
+        if self is self.p:
             return "-5 -6"
-        else:
-            raise ValueError("Heating spec is not defined for " + self.name)
+        raise ValueError("Heating spec is not defined for " + self.name)
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/utils/cartesian_product.py` & `mckit_meshes-0.1.4/src/mckit_meshes/utils/cartesian_product.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Apply function to cartesian product of arrays."""
-from typing import Any, Callable, Dict, Sized
+from __future__ import annotations
+
+from typing import Any, Callable, Sized
 
 from itertools import product
 
 import numpy as np
 
 
 def cartesian_product(
-    *arrays: Sized, aggregator: Callable[[Any, Dict], Any], **kw: Dict[Any, Any]
+    *arrays: Sized,
+    aggregator: Callable[[Any, dict], Any],
+    **kw: dict[Any, Any],
 ) -> np.ndarray:
     """Computes transformations of cartesian product of all the elements in arrays.
 
     Args:
         arrays:  The arrays to product.
         aggregator: Callable to handle an item from product iterator.
             The first parameter of the callable is tuple of current product item.
@@ -20,10 +24,10 @@
 
     Returns:
         ret: Numpy array with dimension of arrays and one more
             additional dimensions for their cartesian product.
     """
     res = np.stack([aggregator(x, **kw) for x in product(*arrays)])
     shape = tuple(map(len, arrays))
-    if 1 < len(res.shape):  # the aggregation result is vector
+    if len(res.shape) > 1:  # the aggregation result is vector
         shape = shape + res.shape[1:]
     return res.reshape(shape)
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/utils/io.py` & `mckit_meshes-0.1.4/src/mckit_meshes/utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import sys
 
 from pathlib import Path
 
 
 def ignore_existing_file_strategy(_: str | Path) -> None:
     """Do nothing if file exists."""
-    pass
 
 
 def raise_error_when_file_exists_strategy(path: str | Path) -> None:
     """Strategy to use when file exists.
 
     Args:
         path: path to check
@@ -41,15 +40,18 @@
     Returns:
         The selected strategy.
     """
     return ignore_existing_file_strategy if override else raise_error_when_file_exists_strategy
 
 
 def print_cols(
-    seq: Iterable[Any], fid: TextIO = sys.stdout, max_columns: int = 6, fmt: str = "{}"
+    seq: Iterable[Any],
+    fid: TextIO = sys.stdout,
+    max_columns: int = 6,
+    fmt: str = "{}",
 ) -> int:
     """Print sequence in max_columns.
 
     Args:
         seq: sequence to print
         fid: output
         max_columns: max max_columns in a line
@@ -68,15 +70,18 @@
         else:
             print(" ", file=fid, end="")
 
     return column
 
 
 def print_n(
-    words: Iterable, io: TextIO = sys.stdout, indent: str = "", max_columns: int = 5
+    words: Iterable,
+    io: TextIO = sys.stdout,
+    indent: str = "",
+    max_columns: int = 5,
 ) -> None:
     """Print sequence in columns with indentation starting from the second row.
 
     If anything was printed, add a newline.
 
     Args:
         words: sequence ot items to print
@@ -92,9 +97,9 @@
         elif column % max_columns == 0:
             to_print = f"\n{indent}{w}"
             column = 1
         else:
             to_print = f" {w}"
             column += 1
         print(to_print, end="", file=io)
-    if 0 < column:
+    if column > 0:
         print(file=io)
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/utils/no_daemon_process.py` & `mckit_meshes-0.1.4/src/mckit_meshes/utils/no_daemon_process.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-"""See:
+"""Some attempt to get better multiprocessing.
+
+See:
 
 https://stackoverflow.com/questions/17223301/python-multiprocessing-is-it-possible-to-have-a-pool-inside-of-a-pool
 https://stackoverflow.com/questions/52948447/error-group-argument-must-be-none-for-now-in-multiprocessing-pool
 https://github.com/nipy/nipype/pull/2754
 """
+from __future__ import annotations
+
+import multiprocessing.pool as pl
 
-import multiprocessing.pool
 
+class Pool(pl.Pool):
+    """Nested Pool."""
 
-class Pool(multiprocessing.pool.Pool):
     # noinspection PyPep8Naming
-    def Process(self, *args, **kwargs):
-        proc = super(Pool, self).Process(*args, **kwargs)
+    def Process(self, *args, **kwargs) -> pl.Pool:  # noqa: N802, ANN003
+        proc = pl.Pool.Process(*args, **kwargs)
 
         class NonDaemonProcess(proc.__class__):
             """Monkey-patch process to ensure it is never daemonized."""
 
             @property
             def daemon(self):
                 return False
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/utils/rebin.py` & `mckit_meshes-0.1.4/src/mckit_meshes/utils/rebin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Functions for rebinning histogram-like distributions."""
 
 # TODO: DVP: implement propagation in result the indexes computed on shrink
 # for reuse in FMesh.shrink for equivalent grids or alike
+from __future__ import annotations
 
-from typing import Iterable, Tuple
+from typing import TYPE_CHECKING, Iterable, Sequence
 
 import collections.abc
 import gc
 import itertools
 import platform
 
 import numpy as np
 
-from numpy import ndarray
+if TYPE_CHECKING:
+    from numpy import ndarray
+    from numpy.typing import ArrayLike
 
 if platform.system() == "Linux":
     from mckit_meshes.utils.no_daemon_process import Pool
 else:
     Pool = None
 
 # TODO
@@ -35,34 +38,37 @@
 __revision__ = "$Id$"
 
 __ZERO = np.array([0.0], dtype=float)
 __EXTERNAL_PROCESS_THRESHOLD = 1000000
 
 
 # noinspection PyTypeChecker
-def is_monotonically_increasing(a: ndarray):
+def is_monotonically_increasing(a: ArrayLike) -> bool:
+    # noinspection PyUnresolvedReferences
     if not a.size:
         return False
     iterator = iter(a)
     prev = next(iterator)
     for val in iterator:
         if prev < val:
             prev = val
         else:
             return False
     return True
 
 
-def set_axis(indices, axis, a_shape):
+# noinspection PyUnresolvedReferences
+def set_axis(indices: ArrayLike, axis: int, a_shape: Sequence[int]) -> ArrayLike:
     shape = [1] * len(a_shape)
     shape[axis] = a_shape[axis]
     return indices.reshape(tuple(shape))
 
 
-def interpolate(x_new, x, y, axis=None):
+# noinspection PyUnresolvedReferences
+def interpolate(x_new: ArrayLike, x: ArrayLike, y: ArrayLike, axis: int = None) -> ArrayLike:
     if y.ndim == 1:
         return np.interp(x_new, x, y)
 
     if axis is None:
         axis = 0
 
     x_new_indices = np.digitize(x_new, x)
@@ -80,37 +86,39 @@
     slice2 = tuple(slice2)
     y_lo = y[slice1]
     y_deltas = y[slice2] - y_lo
     deltas = set_axis(deltas, axis, y_deltas.shape)
     slope = y_deltas / deltas
     new_deltas = x_new - x_lo
     new_deltas = set_axis(new_deltas, axis, slope.shape)
-    y_new = slope * new_deltas + y_lo
-    return y_new
+    return slope * new_deltas + y_lo
 
 
-def rebin_1d(a, bins, new_bins, axis=0, grouped=False, assume_sorted=False):
+# noinspection PyUnresolvedReferences
+def rebin_1d(
+    a: ArrayLike,
+    bins: ArrayLike,
+    new_bins: ArrayLike,
+    axis: int = 0,
+    grouped: bool = False,
+    assume_sorted: bool = False,
+) -> ArrayLike:
     """Transforms 1-D histogram defined as `data` on the limiting points.
 
     define like `bins` to equivalent (see the terms below) histogram defined
     on other limiting points defined as `new_bins`.
 
-    Notes
-    -----
-    The algorithm maintains the equality of integral on intervals defined on
-    new_bins for the original and rebinned distributions.
+    Notes:
+        The algorithm maintains the equality of integral on intervals defined on
+        new_bins for the original and rebinned distributions.
 
-    Parameters
-    ----------
-        a: ndarray
-            The array to rebin
-        bins: ndarray
-            Defines 1-D array representing `a` binning along the given `axis
-        new_bins:  ndarray
-            The new binning required.
+    Args:
+        a: The array to rebin
+        bins: Defines 1-D array representing `a` binning along the given `axis
+        new_bins:  The new binning required.
         axis: int, optional
             An axis along which to rebin array `a`
         grouped: bool, optional
             Defines the approach for rebinning.
 
             - If `True`, then the values in `a` represent the data already
                integrated over bins, like in energy group distributions.
@@ -118,21 +126,23 @@
                energy range in old and new bins.
             - If `False` (default), as for spatial binning - maintain the same
               average value in the same volume in old and new bins.
         assume_sorted: bool, optional
             If True, then skip assertion of bins sorting order,
             by default False - asserts the input_file data
 
-    Returns
-    -------
-        rebinned_data: ndarray
+    Returns:
+        rebinned data
     """
     assert (
-        bins[0] <= new_bins[0] and new_bins[-1] <= bins[-1]
-    ), "Rebinning doesn't provide extrapolation out of the original bins"
+        bins[0] <= new_bins[0]
+    ), "Rebinning doesn't provide extrapolation lower of the original bins"
+    assert (
+        new_bins[-1] <= bins[-1]
+    ), "Rebinning doesn't provide extrapolation upper of the original bins"
     assert (
         bins.size == a.shape[axis] + 1
     ), "The `a` array shape doesn't match the given bins and axis"
     assert assume_sorted or is_monotonically_increasing(bins)
     assert assume_sorted or is_monotonically_increasing(new_bins)
 
     ndim = a.ndim
@@ -167,15 +177,15 @@
         rebinned_data /= new_diff
 
     return rebinned_data
 
 
 def rebin_nd(
     a: ndarray,
-    rebin_spec: Iterable[Tuple[ndarray, ndarray, int, bool]],
+    rebin_spec: Iterable[tuple[ndarray, ndarray, int, bool]],
     assume_sorted: bool = False,
     external_process_threshold: int = __EXTERNAL_PROCESS_THRESHOLD,
 ) -> ndarray:
     """Rebin an array `a` over multidimensional grid.
 
     Args:
         a: An array to rebin.
@@ -185,14 +195,15 @@
             See :py:func:`rebin_1d` for details on the parameters.
         assume_sorted: bool, optional
             If True skip assertion of bins sorting order,
             by default False - asserts the input_file data
         external_process_threshold: int
             If size of `a` is greater than that, then the computation is executed in external process,
             to achieve immediate memory cleanup.
+
     Returns:
         Rebinned data.
     """
     if not isinstance(rebin_spec, collections.abc.Iterator):
         rebin_spec = iter(rebin_spec)
     try:
         bins, new_bins, axis, grouped = next(rebin_spec)
@@ -208,18 +219,23 @@
 
     del recursion_res
     if a.size > external_process_threshold:
         n = gc.collect()
         if n:
             del gc.garbage[:]
 
-    return res
+    return res  # noqa: RET504 - the code above is to be executed
 
 
-def rebin_spec_composer(bins_seq, new_bins_seq, axes=None, grouped_flags=None):
+def rebin_spec_composer(
+    bins_seq,
+    new_bins_seq,
+    axes=None,
+    grouped_flags=None,
+) -> tuple[ArrayLike, ArrayLike, ArrayLike, ArrayLike]:
     """Compose rebin_spec parameter.
 
     See also :py:func:`mckit_meshes.utils.rebin.rebin_nd` with reasonable defaults
     for axes and grouped iterators.
 
     Args:
         bins_seq: sequence of ndarrays
@@ -246,19 +262,24 @@
     elif not grouped_flags:
         grouped_flags = itertools.repeat(False)
     return zip(bins_seq, new_bins_seq, axes, grouped_flags)
 
 
 # @numba.jit
 def shrink_1d(
-    a: np.ndarray, bins: np.ndarray, low=None, high=None, axis=None, assume_sorted=False
-) -> Tuple[np.ndarray, np.ndarray]:
+    a: np.ndarray,
+    bins: np.ndarray,
+    low=None,
+    high=None,
+    axis=None,
+    assume_sorted=False,
+) -> tuple[np.ndarray, np.ndarray]:
     """Select sub-arrays of a `a` and corresponding `bins` for minimal span.
 
-    of bins, which completely covers the range [`low`..`high`]
+    of bins, which completely covers the range [`low`...`high`]
     both sides included.
 
     Args:
         a: ndarray
             An array to shrink.
         bins: ndarray
             Bins corresponding to the grid `a` over the given `axis`.
@@ -276,15 +297,14 @@
 
     Returns:
         new_bins: ndarray
             The shrank bins
         new_data: ndarray
             The shrank grid
     """
-
     if low is None and high is None:
         return bins, a
 
     if axis is None:
         axis = 0
 
     assert a.shape[axis] == bins.size - 1
@@ -297,22 +317,20 @@
         high = bins[-1]
 
     if low == bins[0] and high == bins[-1]:
         return bins, a
 
     if low < bins[0] or bins[-1] < low:
         raise ValueError(
-            "Low shrink edge is beyond the bins range: %g is not in [%g..%g]"
-            % (low, bins[0], bins[-1])
+            f"Low shrink edge is beyond the bins range: {low:g} is not in [{bins[0]:g}..{bins[-1]:g}]",
         )
 
     if high < bins[0] or bins[-1] < high:
         raise ValueError(
-            "High shrink edge is beyond the bins range: %g is not in [%g..%g]"
-            % (high, bins[1], bins[-1])
+            f"High shrink edge is beyond the bins range: {high:g} is not in [{bins[1]:g}..{bins[-1]:g}]",
         )
 
     left_idx, right_idx = np.digitize([low, high], bins) - 1
 
     if left_idx > 0 and bins[left_idx] > low:
         left_idx -= 1
 
@@ -328,68 +346,64 @@
     indices = list(range(left_idx, right_idx + 1))
     new_bins = np.take(bins, indices)
     new_a = np.take(a, indices[:-1], axis=axis)
 
     return new_bins, new_a
 
 
-def shrink_nd(a, trim_spec, assume_sorted=False):
+def shrink_nd(a, trim_spec, assume_sorted=False) -> tuple[ArrayLike, ArrayLike]:
     """Perform multidimensional shrink.
 
     Args:
         a: ndarray
             The grid to shrink.
         trim_spec: sequence of tuples
             Iterates over tuples (bins, low, high, axis)
         assume_sorted: bool, optional
             If True skip assertion of bins sorting order,
             by default False - asserts the input_file data
 
     Returns:
-        new_bins_seq: sequence of ndarrays
-            A sequence with  new bins.
-        recursed_data: ndarray
-            The shrunk grid.
+            A sequence with  new bins,        The shrunk grid.
     """
     if not isinstance(trim_spec, collections.abc.Iterator):
         trim_spec = iter(trim_spec)
     try:
         bins, left, right, axis = next(trim_spec)
     except StopIteration:
         return None, a
     new_bins_seq, recursed_data = shrink_nd(a, trim_spec, assume_sorted)
     top_bins, top_data = shrink_1d(recursed_data, bins, left, right, axis, assume_sorted)
-    if new_bins_seq:
-        new_bins_seq = [top_bins] + new_bins_seq
-    else:
-        new_bins_seq = [top_bins]
+    new_bins_seq = [top_bins, *new_bins_seq] if new_bins_seq else [top_bins]
     return new_bins_seq, top_data
 
 
-def trim_spec_composer(bins_seq, lefts=None, rights=None, axes=None):
+def trim_spec_composer(
+    bins_seq,
+    lefts=None,
+    rights=None,
+    axes=None,
+) -> Iterable[tuple[ArrayLike, float, float, int]]:
     """Helps to compose trim_spec parameter in.
 
-    :py:func:`triniti_ne.rebin.trim_nd` with
+    :func:`triniti_ne.rebin.trim_nd` with
     reasonable defaults for lefts, rights and axes iterators.
 
-    Parameters
-    ----------
-    bins_seq: sequence of ndarrays
-        Iterates over the list of bins associated with a grid to be trimmed.
-    lefts: sequence of floats
-        Iterates over the list of left edges for trimming.
-    rights: sequence of floats
-        Iterates over the list of right edges for trimming.
-    axes: sequence of ints, optional
-        Iterates over the list of corresponding axes.
-        If not provided (default), then iterates over sequence 0..len(bins).
-
-    Returns
-    -------
-    trim_spec: sequence of tuples
+    Args:
+        bins_seq: sequence of ndarrays
+            Iterates over the list of bins associated with a grid to be trimmed.
+        lefts: sequence of floats
+            Iterates over the list of left edges for trimming.
+        rights: sequence of floats
+            Iterates over the list of right edges for trimming.
+        axes: sequence of ints, optional
+            Iterates over the list of corresponding axes.
+            If not provided (default), then iterates over sequence 0..len(bins).
+
+    Returns:
         Iterator over the sequence of tuples (bins, lefts, rights, axis)
     """
     if not lefts:
         lefts = itertools.repeat(None)
     if not rights:
         rights = itertools.repeat(None)
     if not axes:
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/utils/testing.py` & `mckit_meshes-0.1.4/src/mckit_meshes/utils/testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Utilities fof testing."""
+from __future__ import annotations
+
 from typing import cast
 
 import numpy as np
 
 __all__ = ["a"]
 
 
@@ -14,15 +17,14 @@
         args:  sequence of numbers (any type) will be converted to the specified type.
         dtype: A type for the output array
 
     Returns:
         np.ndarray:  The ndarray with the given numbers and type.
 
     Examples:
-
     >>> a(1, 2, 3)
     array([1., 2., 3.])
     >>> a(1, 2, 3, dtype=np.int32)
     array([1, 2, 3], dtype=int32)
     >>> a(0, 1, 2, 3).reshape(2,2)
     array([[0., 1.],
            [2., 3.]])
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/version.py` & `mckit_meshes-0.1.4/src/mckit_meshes/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The meta information on the mckit_meshes package."""
+from __future__ import annotations
 
 from importlib import metadata as _meta
 from importlib.metadata import PackageNotFoundError, version
 
 try:
     __version__ = version(__package__)
 except PackageNotFoundError:  # pragma: no cover
```

### Comparing `mckit_meshes-0.1.3/src/mckit_meshes/wgtmesh.py` & `mckit_meshes-0.1.4/src/mckit_meshes/wgtmesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,62 @@
-from typing import Any, Generator, List, NamedTuple, Optional, TextIO, Tuple, Union
+"""Weight mesh class and functions."""
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Generator, NamedTuple, TextIO, Union
 
 import sys
 
 from dataclasses import dataclass
 from enum import IntEnum
 
+import numpy as np
+
 import mckit_meshes.mesh.geometry_spec as gs
-import mckit_meshes.utils as ut
 import mckit_meshes.utils.io
-import numpy as np
+
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike
 
 GeometrySpec = Union[gs.CartesianGeometrySpec, gs.CylinderGeometrySpec]
 Point = np.ndarray
 
 
-def ensure_float_arrays(*arrays: Any) -> Generator[np.ndarray, None, None]:
-    yield from map(lambda x: np.asarray(x, dtype=float), arrays)
+def ensure_float_arrays(*arrays: ArrayLike) -> Generator[np.ndarray, None, None]:
+    yield from (np.asarray(x, dtype=float) for x in arrays)
 
 
 class Particles(IntEnum):
+    """Particle kind enum."""
+
     neutron = 0
     photon = 1
     n = 0
     p = 1
 
 
-# noinspection GrazieInspection
+# noinspection GrazieInspection,PyUnresolvedReferences
 class WgtMesh:
     """Class to work with MCNP weight window files."""
 
     def __init__(
         self,
         geometry_spec: GeometrySpec,
         energies,
         weights,
     ):
-        self._energies: List[np.ndarray] = list(ensure_float_arrays(*energies))
+        self._energies: list[np.ndarray] = list(ensure_float_arrays(*energies))
         self._geometry_spec = geometry_spec
-        self._weights: List[np.ndarray] = list(ensure_float_arrays(*weights))
+        self._weights: list[np.ndarray] = list(ensure_float_arrays(*weights))
         self.validate()
 
-    def print_mcnp_generator_spec(self, io=None, ref="600 0 50", columns: int = 6):
+    def print_mcnp_generator_spec(self, io=None, ref="600 0 50", columns: int = 6) -> None:
         if io is None:
             io = sys.stdout
         print(f"mesh   ref={ref}", file=io)
-        self._geometry_spec.print(io, columns=columns)
+        self._geometry_spec.print_specification(io, columns=columns)
         print("wwge:n", end=" ", file=io)
         second_indent = " " * 15
         mckit_meshes.utils.io.print_n(
             gs.format_floats(self.energies[0][1:]),
             io=io,
             indent=second_indent,
             max_columns=columns,
@@ -69,82 +77,85 @@
         tally_p_number: int = 24,
         columns: int = 6,
     ) -> None:
         if io is None:
             io = sys.stdout
         print(f"fc{tally_n_number}    === WW generation mesh for neutrons", file=io)
         print(f"fmesh{tally_n_number}:n", file=io)
-        self._geometry_spec.print(io, columns=columns)
+        self._geometry_spec.print_specification(io, columns=columns)
         indent = " " * 8
         print(indent, "emesh=", sep="", end="", file=io)
         second_indent = indent + " " * 6
         mckit_meshes.utils.io.print_n(
             gs.format_floats(self.energies[0][1:]),
             io=io,
             indent=second_indent,
             max_columns=columns,
         )
         if len(self.energies) > 1:
             print(f"fc{tally_p_number}    === WW generation mesh for photons", file=io)
             print(f"fmesh{tally_p_number}:p", file=io)
-            self._geometry_spec.print(io, columns=columns)
+            self._geometry_spec.print_specification(io, columns=columns)
             print(indent, "emesh=", sep="", end="", file=io)
             # TODO dvp: try to use do_print_bins here
             mckit_meshes.utils.io.print_n(
                 gs.format_floats(self.energies[1][1:]),
                 io=io,
                 indent=second_indent,
                 max_columns=columns,
             )
 
-    def validate(self):
+    def validate(self) -> None:
         if len(self.weights) != len(self.energies):
-            raise ValueError(
-                f"Number of energy bins {len(self.energies)} is not equal to number of weight parts {len(self.weights)}"
+            msg = (
+                f"Number of energy bins {len(self.energies)} is not equal "
+                f"to number of weight parts {len(self.weights)}"
             )
+            raise ValueError(msg)
         for part, ebins in enumerate(self.energies):
-            expected_shape = tuple(
-                [
-                    ebins.size - 1,
-                    self.ibins.size - 1,
-                    self.jbins.size - 1,
-                    self.kbins.size - 1,
-                ]
+            # noinspection PyUnresolvedReferences
+            expected_shape = (
+                ebins.size - 1,
+                self.ibins.size - 1,
+                self.jbins.size - 1,
+                self.kbins.size - 1,
             )
             if self.weights[part].shape != expected_shape:
-                raise ValueError(
-                    f"Incompatible number of ebins, voxels and weights: {self.weights[part].shape} != {expected_shape}"
+                msg = (
+                    f"Incompatible number of ebins, voxels and weights: {self.weights[part].shape} "
+                    "!= {expected_shape}"
                 )
+                raise ValueError(msg)
 
     @property
-    def energies(self):
+    def energies(self) -> list[ArrayLike]:
         return self._energies
 
     @property
-    def origin(self):
+    def origin(self) -> ArrayLike:
         return self._geometry_spec.origin
 
     @property
-    def ibins(self):
+    def ibins(self) -> ArrayLike:
         return self._geometry_spec.ibins
 
     @property
-    def jbins(self):
+    def jbins(self) -> ArrayLike:
         return self._geometry_spec.jbins
 
     @property
-    def kbins(self):
+    def kbins(self) -> ArrayLike:
         return self._geometry_spec.kbins
 
     @property
-    def count_voxels(self):
+    def count_voxels(self) -> int:
         return (self.ibins.size - 1) * (self.jbins.size - 1) * (self.kbins.size - 1)
 
     @property
-    def weights(self) -> List[np.ndarray]:
+    def weights(self) -> list[np.ndarray]:
         return self._weights
 
     @property
     def neutron_weights(self) -> np.ndarray:
         return self._weights[0]
 
     @property
@@ -153,107 +164,98 @@
         return self._weights[1]
 
     @property
     def is_cylinder(self) -> bool:
         return self._geometry_spec.cylinder
 
     @property
-    def axs(self) -> Optional[np.ndarray]:
+    def axs(self) -> np.ndarray | None:
         return self._geometry_spec.axs
 
     @property
-    def vec(self) -> Optional[np.ndarray]:
+    def vec(self) -> np.ndarray | None:
         return self._geometry_spec.vec
 
     @property
     def count_parts(self) -> int:
         return len(self.weights)
 
-    def part(self, particle: Particles) -> Tuple[np.ndarray, np.ndarray]:
+    def part(self, particle: Particles) -> tuple[np.ndarray, np.ndarray]:
         return self.energies[particle], self.weights[particle]
 
     def __hash__(self):
         return hash(
             (
                 self._geometry_spec.__hash__(),
                 self.energies,
                 self.weights,
-            )
+            ),
         )
 
     def __eq__(self, other):
         if not self.bins_are_equal(other):
             return False
         for p in range(len(self.weights)):
             if not np.array_equal(self.weights[p], other.weights[p]):
                 return False
         return True
 
-    def bins_are_equal(self, other: "WgtMesh") -> bool:
+    def bins_are_equal(self, other: WgtMesh) -> bool:
         if not isinstance(other, WgtMesh):
-            raise RuntimeError("Invalid class of object to compare: {}", other.__class__)
-        if self._geometry_spec == other._geometry_spec:
+            msg = f"Invalid class of object to compare: {other.__class__}"
+            raise TypeError(msg)
+        if self._geometry_spec == other.geometry_spec:
             le = len(self.energies)
             if le == len(other.energies):
-                for i in range(le):
-                    if not np.array_equal(self.energies[i], other.energies[i]):
-                        return False
-                return True
+                return all(np.array_equal(self.energies[i], other.energies[i]) for i in range(le))
         return False
 
-    def __add__(self, other) -> "WgtMesh":
+    def __add__(self, other) -> WgtMesh:
         assert self.bins_are_equal(other)
         weights = [a + b for a, b in zip(self.weights, other.weights)]
-        res = WgtMesh(
+        return WgtMesh(
             self._geometry_spec,
             self.energies,
             weights,
         )
-        return res
 
-    def __sub__(self, other) -> "WgtMesh":
+    def __sub__(self, other) -> WgtMesh:
         assert self.bins_are_equal(other)
         weights = [a - b for a, b in zip(self.weights, other.weights)]
-        res = WgtMesh(
+        return WgtMesh(
             self._geometry_spec,
             self.energies,
             weights,
         )
-        return res
 
-    def __mul__(self, coeff: float) -> "WgtMesh":
+    def __mul__(self, coeff: float) -> WgtMesh:
         weights = [w * coeff for w in self.weights]
-        res = WgtMesh(
+        return WgtMesh(
             self._geometry_spec,
             self.energies,
             weights,
         )
-        return res
 
-    def __rmul__(self, coeff: float) -> "WgtMesh":
+    def __rmul__(self, coeff: float) -> WgtMesh:
         return self.__mul__(coeff)
 
     # def __repr__(self):
-    #     return f"WgtMesh({tuple(self.origin)}, {self.energies})"
 
     # noinspection SpellCheckingInspection
     def write(self, stream: TextIO) -> None:
         """Writes the mesh to stream.
 
         See WWINP format, MCNP User Manual, Appendix J, Table J.1
 
         Args;
             stream: a stream to write to
         """
         data = []
         _if, _iv, _ni = 1, 1, len(self.energies)
-        if self.is_cylinder:
-            _nr = 16
-        else:
-            _nr = 10
+        _nr = 16 if self.is_cylinder else 10
         data += produce_strings([_if, _iv, _ni, _nr], "{0:10d}")
         # remove the first "\n"
         data = data[1:]
 
         _ne = [x.size - 1 for x in self._energies]
         data += produce_strings(_ne, "{0:10d}")
         _nfx = self.ibins.size - 1
@@ -266,18 +268,20 @@
         _ncy = len(_nfmy)
         _nfmz, _zm = gs.compute_intervals_and_coarse_bins(self.kbins)
         _ncz = len(_nfmz)
         _nwg = 1
         _data = [_nfx, _nfy, _nfz, _x0, _y0, _z0, _ncx, _ncy, _ncz]
         if self.is_cylinder:
             if self.axs is None:
-                raise ValueError("axs is not specified in cylinder mesh")
+                msg = "axs is not specified in cylinder mesh"
+                raise ValueError(msg)
             _xmax, _ymax, _zmax = self.axs
             if self.vec is None:
-                raise ValueError("vec is not specified in cylinder mesh")
+                msg = "vec is not specified in cylinder mesh"
+                raise ValueError(msg)
             _xr, _yr, _zr = self.vec
             _data += [_xmax, _ymax, _zmax, _xr, _yr, _zr]
             _nwg = 2
         _data += [_nwg]
         data += produce_strings(_data, "{0:#13.5g}")
         # Block 2
         _nc = [_ncx, _ncy, _ncz]
@@ -285,32 +289,32 @@
         _r = [_xm, _ym, _zm]
         for i in range(3):
             data1 = [_r[i][0]]
             for j in range(_nc[i]):
                 data1 += [_nfm[i][j], _r[i][j + 1], 1]
             data += produce_strings(data1, "{0:#13.5g}")
         for p in range(_ni):
+            w = self._weights[p]
             data += produce_strings(self.energies[p][1:], "{0:#13.5g}")  # omit the first zero
-            data1 = []
-            # TODO dvp: order of cycling and dimensions are not efficient:
-            #           the index changing faster should be the most inner in cycle.
-            for e in range(_ne[p]):
-                for k in range(_nfz):
-                    for j in range(_nfy):
-                        for i in range(_nfx):
-                            data1.append(self._weights[p][e, i, j, k])
+            data1 = [
+                w[e, i, j, k]
+                for e in range(_ne[p])
+                for k in range(_nfz)
+                for j in range(_nfy)
+                for i in range(_nfx)
+            ]
             data += produce_strings(data1, "{0:#13.5g}")
         stream.write("".join(data))
 
     @dataclass
     class _Reader:
-        data: List[str]
+        data: list[str]
         index: int = 0
 
-        def get(self, items: int) -> List[str]:
+        def get(self, items: int) -> list[str]:
             i = self.index
             self.index += items
             return self.data[i : self.index]
 
         def get_floats(self, items: int) -> Generator[float, None, None]:
             return map(float, self.get(items))
 
@@ -321,15 +325,15 @@
             return map(int, self.get_floats(items))
 
         def skip(self, items: int = 1) -> None:
             self.index += items
 
     # noinspection SpellCheckingInspection
     @classmethod
-    def read(cls, f: TextIO) -> "WgtMesh":
+    def read(cls, f: TextIO) -> WgtMesh:
         """Read an MCNP weights file.
 
         See format description at MCNP User Manual, Version 5 (p.489 or Appendix J, p. J-1)
 
         Args:
             f: Input file in WWINP format
 
@@ -372,57 +376,56 @@
         _z = parse_coordinates(reader.get(delta))
 
         _e = []
         _w = []
 
         for p in range(number_of_particles):
             nep = sizes_of_energy_bins[p]
-            if 0 < nep:
+            if nep > 0:
                 ebins = np.fromiter(reader.get_floats(nep), dtype=float)
                 ebins = np.insert(ebins, 0, 0.0)
                 _e.append(ebins)
                 _wp = np.zeros((nep, _nfx, _nfy, _nfz), dtype=float)
                 _wp_data = np.fromiter(reader.get_floats(_wp.size), dtype=float)
                 for e in range(nep):
                     for k in range(_nfz):
                         for j in range(_nfy):
                             for i in range(_nfx):
                                 cell_index = i + _nfx * (j + _nfy * (k + _nfz * e))
                                 _wp[e, i, j, k] = _wp_data[cell_index]
                 _w.append(_wp)
                 assert np.all(
-                    np.transpose(_wp_data.reshape((nep, _nfz, _nfy, _nfx)), (0, 3, 2, 1)) == _wp
+                    np.transpose(_wp_data.reshape((nep, _nfz, _nfy, _nfx)), (0, 3, 2, 1)) == _wp,
                 )
         geometry_spec = make_geometry_spec([_x0, _y0, _z0], _x, _y, _z, axs=axs, vec=vec)
         return cls(geometry_spec, _e, _w)
 
-    def get_mean_square_distance_weights(self, point):
+    def get_mean_square_distance_weights(self, point) -> WgtMesh:
         w = self._geometry_spec.get_mean_square_distance_weights(point)
         _w = []
         for _e in self.energies:
             le = len(_e)
-            t = w.reshape((1,) + self._geometry_spec.bins_shape)
+            t = w.reshape((1, *self._geometry_spec.bins_shape))
             t = np.repeat(t, le, axis=0)
             _w.append(t)
         return WgtMesh(
             self._geometry_spec,
             self.energies,
             _w,
         )
 
     class MergeSpec(NamedTuple):
-        wm: "WgtMesh"
+        wm: WgtMesh
         nps: int
 
     @classmethod
-    def merge(cls, *merge_specs: Union[MergeSpec, Tuple["WgtMesh", int]]) -> MergeSpec:
+    def merge(cls, *merge_specs: MergeSpec | tuple[WgtMesh, int]) -> MergeSpec:
         r"""Combine weight meshes produced from different runs with weighting factor.
 
         Note:
-
         Importance of a mesh voxel `i` is $1/w_i$ and is proportional to average portion $p_i$ of
         passing particle weight W to a tally for which the weight mesh is computed.
         To obtain combined weight on merging two meshes, we will combine the probabilities using weighting factors and
         use reciprocal of a result as a resulting weight of mesh voxel.
         The weighting factors are usually NPS (Number particles sampled) from a run on which a mesh was produced.
         The combined probability in resulting voxel `i` is:
 
@@ -458,80 +461,81 @@
         if len(merge_specs) > 1:
             second = WgtMesh.merge(*merge_specs[1:])
             merged_weights = []
             assert first.wm.bins_are_equal(second.wm)
             for i, weights in enumerate(first.wm.weights):
                 nps_first, probabilities_first = prepare_probabilities_and_nps(first.nps, weights)
                 nps_second, probabilities_second = prepare_probabilities_and_nps(
-                    second.nps, second.wm.weights[i]
+                    second.nps,
+                    second.wm.weights[i],
                 )
                 nps = np.array(nps_first + nps_second, dtype=float)
                 combined_probabilities = (
                     nps_first * probabilities_first + nps_second * probabilities_second
                 ) * reciprocal(nps)
                 merged_weights.append(reciprocal(combined_probabilities))
             wm = first.wm
             return WgtMesh.MergeSpec(
                 cls(
-                    wm._geometry_spec,
+                    wm.geometry_spec,
                     wm.energies,
                     merged_weights,
                 ),
                 first.nps + second.nps,
             )
-        else:
-            return first
 
-    def reciprocal(self) -> "WgtMesh":
+        return first
+
+    def reciprocal(self) -> WgtMesh:
         """Invert weights values.
 
         To be used for anti-forward method of weight generation.
 
-        Returns
+        Returns:
         -------
         out:
             Reciprocal of this weights
         """
         return WgtMesh(self._geometry_spec, self.energies, list(map(reciprocal, self.weights)))
 
     def normalize(
-        self, normalization_point: Point, normalized_value: float = 1.0, energy_bin=-1
-    ) -> "WgtMesh":
+        self,
+        normalization_point: Point,
+        normalized_value: float = 1.0,
+        energy_bin=-1,
+    ) -> WgtMesh:
         """Scale weights to have value `value` at `normalisation_point`.
 
         All other voxels are scaled proportionally.
 
         Args:
             normalization_point:  Coordinates of point where the weights should equal `value`.
             normalized_value: The value which should be at `normalization_point`
             energy_bin: index of energy bin at which set normalized value, default - the last one.
 
         Returns:
             New normalized weights.
         """
-        gs = self._geometry_spec
+        _gs = self._geometry_spec
         x, y, z = normalization_point
-        ix, iy, iz = gs.select_indexes(i_values=x, j_values=y, k_values=z)
+        ix, iy, iz = _gs.select_indexes(i_values=x, j_values=y, k_values=z)
         new_weights = []
         value_at_normalisation_point = self.weights[0][energy_bin, ix, iy, iz]
         """The value at last energy bin about 20 MeV at neutron weights."""
 
         factor = normalized_value / value_at_normalisation_point
         """Scale all other weights by this value."""
 
-        for i, w in enumerate(self.weights):
+        for w in self.weights:
             # TODO dvp: revise for multiple energy bins, may be add scaling values for each energy bin and particle
-            value_at_normalisation_point = w[
-                energy_bin, ix, iy, iz
-            ]  # the last energy bin about 20 MeV.
             new_weights.append(w * factor)
 
-        return WgtMesh(gs, self.energies, new_weights)
+        return WgtMesh(_gs, self.energies, new_weights)
 
-    def invert(self, normalization_point: Point, normalized_value: float = 1.0) -> "WgtMesh":
+    def invert(self, normalization_point: Point, normalized_value: float = 1.0) -> WgtMesh:
         """Get reciprocal of self weights and normalize to 1 at given point.
 
         Important:
             A caller specifies normalization_point in local coordinates. See :class:`GeometrySpec.local_coordinates`.
 
         Args:
             normalization_point: Point at which output weights should be 1
@@ -539,37 +543,36 @@
 
         Returns:
             WgtMesh: Normalized reciprocal of self weights.
         """
         return self.reciprocal().normalize(normalization_point, normalized_value)
 
     @property
-    def geometry_spec(self):
+    def geometry_spec(self) -> GeometrySpec:
         return self._geometry_spec
 
-    def drop_lower_energies(self, min_energy: float, part: int = 0) -> "WgtMesh":
+    def drop_lower_energies(self, min_energy: float, part: int = 0) -> WgtMesh:
         if len(self.energies) <= part:
-            raise ValueError(f"invalid value for weights object part: {part}")
+            msg = f"invalid value for weights object part: {part}"
+            raise ValueError(msg)
         energies = self.energies[part]
         energies_to_retain = min_energy <= energies
         energies_to_retain[0] = True
         if np.all(energies_to_retain):
             return self
-        else:
-            new_energies = []
-            new_weights = []
-            for i in range(len(self.energies)):
-                if i == part:
-                    new_energies.append(self.energies[i][energies_to_retain])
-                    new_weights.append(self.weights[i][energies_to_retain[1:], :, :, :])
-                else:
-                    new_energies.append(self.energies[i])
-                    new_weights.append(self.weights[i])
-            gs = self._geometry_spec
-            return WgtMesh(gs, new_energies, new_weights)
+        new_energies = []
+        new_weights = []
+        for i in range(len(self.energies)):
+            if i == part:
+                new_energies.append(self.energies[i][energies_to_retain])
+                new_weights.append(self.weights[i][energies_to_retain[1:], :, :, :])
+            else:
+                new_energies.append(self.energies[i])
+                new_weights.append(self.weights[i])
+        return WgtMesh(self._geometry_spec, new_energies, new_weights)
 
 
 def reciprocal(a: np.ndarray, zero_index: np.ndarray = None) -> np.ndarray:
     if a.dtype != float:
         a = np.array(a, dtype=float)
     if zero_index is None:
         zero_index = a == 0.0
@@ -577,15 +580,15 @@
         assert np.array_equal(zero_index, a == 0.0)
     result: np.ndarray = np.reciprocal(a, where=np.logical_not(zero_index))
     #  fix bug in numpy reciprocal: it doesn't pass zero values, the bug doesn't show up on debugging
     result[zero_index] = 0.0
     return result
 
 
-def prepare_probabilities_and_nps(_nps: int, _weights: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+def prepare_probabilities_and_nps(_nps: int, _weights: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
     """Computes intermediate data for merging procedure.
 
     The probabilities are reciprocals to weights.
     Zero weights mean zero probabilities and don't affect the merged result.
 
     Args:
         _nps:
@@ -598,24 +601,24 @@
     nps_array = np.full_like(_weights, _nps, dtype=int)
     zero_index = _weights == 0.0
     probabilities = reciprocal(_weights, zero_index=zero_index)
     nps_array[zero_index] = 0  # voxels with zero weight don't affect weighted sum
     return nps_array, probabilities
 
 
-def produce_strings(stream, format_spec):
+def produce_strings(stream, format_spec) -> list[str]:
     data = []
     for i in range(len(stream)):
         if i % 6 == 0:
             data.append("\n")
         data.append(format_spec.format(stream[i]))
     return data
 
 
-def parse_coordinates(inp: List[str]) -> np.ndarray:
+def parse_coordinates(inp: list[str]) -> np.ndarray:
     def iter_over_coarse_mesh():
         is_first = True
         i = 0
         length = len(inp)
         while i < length:
             coordinate = float(inp[i])
             if is_first:
@@ -651,16 +654,36 @@
             prev_fine_bins = fine_bins
         yield prev_coordinate
 
     return np.fromiter(iter_over_fine_mesh(iter_over_coarse_mesh()), dtype=float)
 
 
 def make_geometry_spec(origin, ibins, jbins, kbins, axs=None, vec=None) -> GeometrySpec:
+    """Make Cartesian or Cylinder geometry specification from with given parameters.
+
+    The parameters are converted to numpy arrays.
+
+    Args:
+        origin: origin point
+        ibins:  X or R bins
+        jbins:  Y or Z bins
+        kbins:  Z or Theta bins
+        axs:    Cylinder mesh axis
+        vec:    Cylinder mesh angle reference vector
+
+    Returns:
+        spec - new geometry specification
+    """
     origin, ibins, jbins, kbins = map(gs.as_float_array, [origin, ibins, jbins, kbins])
     if axs is None:
         geometry_spec = gs.CartesianGeometrySpec(ibins, jbins, kbins, origin=origin)
     else:
         axs, vec = map(gs.as_float_array, [axs, vec])
         geometry_spec = gs.CylinderGeometrySpec(
-            ibins, jbins, kbins, origin=origin, axs=axs, vec=vec
+            ibins,
+            jbins,
+            kbins,
+            origin=origin,
+            axs=axs,
+            vec=vec,
         )
     return geometry_spec
```

### Comparing `mckit_meshes-0.1.3/PKG-INFO` & `mckit_meshes-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: mckit-meshes
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python tools to work with MCNP meshtallies and weight meshes.
 Home-page: https://github.com/MC-kit/mckit-meshes
 License: MIT
 Keywords: mesh,weights,variance reduction
 Author: dvp2015
 Author-email: dmitri_portnov@yahoo.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: click (>=8.0.1)
+Requires-Dist: importlib-resources (>=5.12.0) ; python_version == "3.8"
 Requires-Dist: loguru (>=0.6.0)
-Requires-Dist: numpy (>=1.23.2)
+Requires-Dist: numpy (>=1.24.2)
 Requires-Dist: openpyxl (>=3.0.9)
-Requires-Dist: pandas (>=1.4.1)
+Requires-Dist: pandas (>=2.0.0)
 Requires-Dist: pyevtk (>=1.4.1)
 Requires-Dist: toolz (>=0.11.2)
 Project-URL: Chnagelog, https://github.com/MC-kit/mckit-meshes/releases
 Project-URL: Repository, https://github.com/MC-kit/mckit-meshes
 Description-Content-Type: text/x-rst
 
 ==============================================================================
```

