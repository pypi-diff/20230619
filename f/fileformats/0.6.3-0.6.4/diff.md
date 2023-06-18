# Comparing `tmp/fileformats-0.6.3.tar.gz` & `tmp/fileformats-0.6.4.tar.gz`

## Comparing `fileformats-0.6.3.tar` & `fileformats-0.6.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/archive/__init__.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/archive/converters.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/_version.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/converter.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/datatype.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/field.py
--rw-r--r--   0        0        0    32098 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/fileset.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/mark.py
--rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/mixin.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/utils.py
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/document/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/base.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/converters.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/vector.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/tests/test_image_converters.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/serialization/converters.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.3/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.3/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.3/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.3/README.rst
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/archive/converters.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/archive/tests/test_archive_converters.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/converter.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/datatype.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/field.py
+-rw-r--r--   0        0        0    37604 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/mark.py
+-rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/mixin.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/utils.py
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/base.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/converters.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/vector.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/tests/test_image_converters.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/misc/medical.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/serialization/converters.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/serialization/tests/test_serialization_converters.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/text/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.4/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.4/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.4/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.4/README.rst
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.4/PKG-INFO
```

### Comparing `fileformats-0.6.3/fileformats/archive/__init__.py` & `fileformats-0.6.4/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/archive/converters.py` & `fileformats-0.6.4/fileformats/archive/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/archive/tests/test_archive_converters.py` & `fileformats-0.6.4/fileformats/archive/tests/test_archive_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/audio/__init__.py` & `fileformats-0.6.4/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/converter.py` & `fileformats-0.6.4/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/datatype.py` & `fileformats-0.6.4/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/field.py` & `fileformats-0.6.4/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/fileset.py` & `fileformats-0.6.4/fileformats/core/fileset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 import os
 from copy import copy
 import struct
-from enum import Enum
+from enum import Enum, IntEnum
 from warnings import warn
+from collections import Counter
 import traceback
 import typing as ty
 import importlib
 import shutil
 from operator import itemgetter
 import itertools
 import functools
@@ -17,14 +18,15 @@
 import attrs
 from .utils import (
     classproperty,
     fspaths_converter,
     to_mime_format_name,
     STANDARD_NAMESPACES,
     describe_task,
+    splitext,
 )
 from .converter import SubtypeVar
 from .exceptions import (
     FileFormatsError,
     FormatMismatchError,
     FormatConversionError,
 )
@@ -74,60 +76,23 @@
 
     # Store converters registered by @converter decorator that convert to FileSet
     # NB: each class will have its own version of this dictionary
     converters = {}
 
     is_fileset = True
 
-    class CopyMode(Enum):
-        """Designates the desired behaviour of the FileSet.copy() method"""
-
-        dont_copy = 0b0001  # simply leave the files where they are (i.e. don't copy)
-        symlink = 0b0010  # symlink the file into the destination directory
-        hardlink = 0b0100  # hardlink the file into the destination directory
-        copy = (
-            0b1000  # duplicate (actually copy) the file into the destination directory
-        )
-
-        link = 0b0110  # use either linking method (preferring symbolic)
-        link_or_copy = 0b1110  # use either linking method or copy (preferring symbolic, hardlink and then copy)
-        symlink_or_copy = 0b1010
-        hardlink_or_copy = 0b1100
-
-        # Masks
-        all = 0b1111  # use any method (preferring dont_copy)
-        no_supported = 0b0000  # none of the requested methods are supported
-
-        # rarely used combinations
-        dont_copy_or_symlink = 0b0011
-        dont_copy_or_hardlink = 0b0101
-        dont_copy_or_link = 0b0111
-        dont_copy_or_symlink_or_copy = 0b1011
-        dont_copy_or_hardlink_or_copy = 0b1101
-
-        def __xor__(self, other):
-            return type(self)(self.value ^ other.value)
-
-        def __and__(self, other):
-            return type(self)(self.value & other.value)
-
-        def __or__(self, other):
-            return type(self)(self.value | other.value)
-
-        def __sub__(self, other):
-            return type(self)((self.value & (self.value ^ other.value)))
-
-        def __bool__(self):
-            return bool(self.value)
-
     def __hash__(self):
         return hash(sorted(self.fspaths))
 
     def __repr__(self):
-        return f"{type(self).__name__}('" + "', '".join(self.fspaths) + "')"
+        return (
+            f"{type(self).__name__}('"
+            + "', '".join(str(p) for p in self.fspaths)
+            + "')"
+        )
 
     def __attrs_post_init__(self):
         # Check required properties don't raise errors
         for prop_name in self.required_properties():
             getattr(self, prop_name)
         # Loop through all attributes and find methods marked by CHECK_ANNOTATION
         for check in self.checks():
@@ -158,14 +123,24 @@
 
     @property
     def metadata(self):
         if self._metadata is None and hasattr(self, "load_metadata"):
             self._metadata = self.load_metadata()
         return self._metadata
 
+    @property
+    def parent(self) -> Path:
+        "A common parent directory for all the top-level paths in the file-set"
+        return Path(os.path.commonpath(p.parent for p in self.fspaths))
+
+    @property
+    def relative_fspaths(self) -> ty.Iterator[Path]:
+        "Paths for all top-level paths in the file-set relative to the common parent directory"
+        return (p.relative_to(self.parent) for p in self.fspaths)
+
     @classproperty
     def mime_type(cls):
         """Generates a MIME type (IANA) identifier from a format class. If an official
         IANA MIME type doesn't exist it will create one in the in the MIME style, e.g.
 
             fileformats.text.Plain to "text/plain"
 
@@ -251,118 +226,14 @@
             try:
                 klass_attr.__annotations__[CHECK_ANNOTATION]
             except (AttributeError, KeyError):
                 pass
             else:
                 yield attr_name
 
-    def copy(
-        self,
-        dest_dir: Path,
-        stem: ty.Optional[str] = None,
-        mode: ty.Union[CopyMode, str] = CopyMode.copy,
-        trim: bool = True,
-        make_dirs: bool = False,
-        overwrite: bool = False,
-        supported_modes: CopyMode = CopyMode.all,
-    ):
-        """Copies the file-set to a new directory, optionally renaming the files
-        to have consistent name-stems.
-
-        Parameters
-        ----------
-        dest_dir : str
-            Path to the parent directory to save the file-set
-        stem: str, optional
-            the file name excluding file extensions, to give the files/dirs in the parent
-            directory, by default the original file name is used
-        mode : CopyMode or str, optional
-            designates whether to perform an actual copy or whether a link (symbolic or
-            hard) is okay, 'duplicate' by default.
-        trim : bool, optional
-            Only copy the paths in the file-set that are "required" by the format,
-            true by default
-        make_dirs : bool, optional
-            Make the parent destination and all missing ancestors if they are missing,
-            false by default
-        overwrite : bool, optional
-            whether to overwrite existing files/directories if present
-        supported_modes : CopyMode, optional
-            supported modes for the copy operation. Used to mask out the requested
-            copy mode
-        """
-        mode = self.CopyMode[mode] if isinstance(mode, str) else mode
-        selected_mode = mode & supported_modes
-        if not selected_mode:
-            raise FileFormatsError(
-                f"Cannot copy {self} using {mode} mode as it is not supported "
-                f"({supported_modes})"
-            )
-        if selected_mode & self.CopyMode.dont_copy:
-            return self
-        dest_dir = Path(dest_dir)  # ensure a Path not a string
-        if make_dirs:
-            dest_dir.mkdir(parents=True, exist_ok=True)
-        if selected_mode & self.CopyMode.symlink:
-            copy_dir = copy_file = os.symlink
-        elif selected_mode & self.CopyMode.hardlink:
-            copy_file = os.link
-
-            def hardlink_dir(src: Path, dest: Path):
-                for dpath, _, fpaths in os.walk(src):
-                    dpath = Path(dpath)
-                    relpath = dpath.relative_to(src)
-                    (dest / relpath).mkdir()
-                    for fpath in fpaths:
-                        os.link(dpath / fpath, dest / relpath / fpath)
-
-            copy_dir = hardlink_dir
-        else:
-            assert selected_mode & self.CopyMode.copy
-            copy_dir = shutil.copytree
-            copy_file = shutil.copyfile
-        new_paths = []
-        if trim and self.required_paths():
-            fspaths_to_copy = self.required_paths()
-        else:
-            fspaths_to_copy = self.fspaths
-        if not fspaths_to_copy:
-            raise FileFormatsError(
-                f"Cannot copy {self} because none of the fspaths in the file-set are "
-                "required. Set trim=False to copy all file-paths"
-            )
-        for fspath in fspaths_to_copy:
-            if stem:
-                new_fname = stem + "".join(fspath.suffixes)
-            else:
-                new_fname = fspath.name
-            new_path = dest_dir / new_fname
-            if new_path.exists():
-                if overwrite:
-                    if fspath.is_dir():
-                        shutil.rmtree(new_path)
-                    else:
-                        os.unlink(new_path)
-                else:
-                    raise FileFormatsError(
-                        f"Destination path '{str(new_path)}' exists, set "
-                        "'overwrite' to overwrite it"
-                    )
-            if fspath.is_dir():
-                copy_dir(fspath, new_path)
-            else:
-                copy_file(fspath, new_path)
-            new_paths.append(new_path)
-        return type(self)(new_paths)
-
-    def copy_to(self, *args, **kwargs):
-        """For b/w compatibility (temporary message)"""
-        warn("'FileSet.copy_to()' has been deprecated, please use copy() instead")
-        return self.copy(*args, **kwargs)
-
     def select_by_ext(
         self, fileformat: ty.Optional[type] = None, allow_none: bool = False
     ) -> Path:
         """Selects a single path from a set of file-system paths based on the file
         extension
 
         Parameters
@@ -832,16 +703,16 @@
             crypto_obj = crypto()
             for bytes_str in bytes_iter:
                 crypto_obj.update(bytes_str)
             file_hashes[str(path)] = crypto_obj.hexdigest()
         return file_hashes
 
     def __bytes_repr__(
-        self, cache: dict
-    ) -> ty.Iterable[bytes]:  # pylint: disable=unused-argument
+        self, cache: dict  # pylint: disable=unused-argument
+    ) -> ty.Iterable[bytes]:
         """Provided for compatibility with Pydra's hashing function, return the contents
         of all the files in the file-set in chunks
 
         Parameters
         ----------
         cache : dict
             an object passed around by Pydra's hashing function to store cached versions
@@ -855,10 +726,274 @@
         """
         cls = type(self)
         yield f"{cls.__module__}.{cls.__name__}:".encode()
         for key, chunk_iter in self.byte_chunks():
             yield (",'" + key + "'=").encode()
             yield from chunk_iter
 
+    class CopyMode(Enum):
+        """Designates the desired behaviour of the FileSet.copy() method with regards to
+        symbolic, hard or full copies
+
+        Basic options (in order of preference)
+        --------------------------------------
+        leave
+            simply leave the files where they are (i.e. do nothing)
+        symlink
+            symlink the files into the destination directory
+        hardlink
+            hardlink the files into the destination directory
+        copy
+            duplicate (actually copy) the files into the destination directory
+
+        Common combinations
+        -------------------
+        link
+            use either linking method (preferring symbolic)
+        link_or_copy
+            use either link method or copy (preferring sym, hard, then copy)
+        symlink_or_copy
+            "  symbolic "   "         "
+        hardlink_or_copy
+            "  hard "   "         "
+
+        Masks
+        -----
+        any
+            use any method (preferring leave)
+        none
+            none of the requested methods are supported (i.e. after masking with the
+            supported options mask)
+        """
+
+        # Bases
+
+        leave = 0b0001
+        symlink = 0b0010
+        hardlink = 0b0100
+        copy = 0b1000
+
+        # Common combinations
+
+        link = 0b0110
+        link_or_copy = 0b1110
+        symlink_or_copy = 0b1010
+        hardlink_or_copy = 0b1100
+
+        # Masks
+
+        any = 0b1111
+        none = 0b0000
+
+        # All other combinations (typically the result of bit-masking)
+
+        leave_or_symlink = 0b0011
+        leave_or_hardlink = 0b0101
+        leave_or_link = 0b0111
+        leave_or_symlink_or_copy = 0b1011
+        leave_or_hardlink_or_copy = 0b1101
+
+        def __xor__(self, other):
+            return type(self)(self.value ^ other.value)
+
+        def __and__(self, other):
+            return type(self)(self.value & other.value)
+
+        def __or__(self, other):
+            return type(self)(self.value | other.value)
+
+        def __sub__(self, other):
+            return type(self)((self.value & (self.value ^ other.value)))
+
+        def __bool__(self):
+            return bool(self.value)
+
+        def __str__(self):
+            return self.name
+
+    class CopyCollation(IntEnum):
+        """Designates the desired "collation" behaviour of the FileSet.copy() method
+
+        Bases
+        -----
+        separated
+            If mode == leave, paths can exist in separate directories in the
+            file-system. For other copy modes, the relative directory structure between
+            the "copied" paths (incl. links) in the set will be maintained within the
+            destination directory. This guarantees there won't be name clashes between
+            copied paths.
+        siblings
+            copied paths are guaranteed to be "copied" to the root of the destination
+            directory, i.e be siblings. However, this requires that the file/dir name
+            in fspaths are unique.
+        adjacent
+            copied paths are guaranteed to have the same name-stem and only differ in
+            file-extensions. Requires that the file-set only includes files/dirs with
+            unique suffixes (NB: suffixes are considered to be everything after the first
+            '.' in the filename).
+        """
+
+        any = 0
+        siblings = 1
+        adjacent = 2
+
+        def __str__(self):
+            return self.name
+
+    def copy(
+        self,
+        dest_dir: Path,
+        mode: ty.Union[CopyMode, str] = CopyMode.copy,
+        collation: ty.Union[CopyCollation, str] = CopyCollation.any,
+        stem: ty.Optional[str] = None,
+        trim: bool = True,
+        make_dirs: bool = False,
+        overwrite: bool = False,
+        multi_splitext: bool = True,
+        supported_modes: CopyMode = CopyMode.any,
+    ):
+        """Copies the file-set to a new directory, optionally renaming the files
+        to have consistent name-stems.
+
+        Parameters
+        ----------
+        dest_dir : str
+            Path to the parent directory to save the file-set
+        mode : FileSet.CopyMode or str, optional
+            designates whether to perform an actual copy or whether a link (symbolic or
+            hard) is okay, 'duplicate' by default. See FielSet.CopyMode for details
+        collation : FileSet.CopyCollation or str, optional
+            how to treat relative paths within the fileset, i.e. whether to move them
+            to a single directory, rename them to the same file-stem or maintain
+            relative directory structure. See FileSet.CopyCollation for details
+        stem: str, optional
+            the file name excluding file extensions, to give the files/dirs in the parent
+            directory, by default the original file name is used
+        trim : bool, optional
+            Only copy the paths in the file-set that are "required" by the format,
+            true by default
+        make_dirs : bool, optional
+            Make the parent destination and all missing ancestors if they are missing,
+            false by default
+        overwrite : bool, optional
+            whether to overwrite existing files/directories if present
+        multi_splitext : bool, optional
+            whether to consider file extensions to start from the first '.' (True) or the
+            last (False), by default True
+        supported_modes : CopyMode, optional
+            supported modes for the copy operation. Used to mask out the requested
+            copy mode
+        """
+        mode = self.CopyMode[mode] if isinstance(mode, str) else mode
+        selected_mode = mode & supported_modes
+        collation = (
+            self.CopyCollation[collation] if isinstance(collation, str) else collation
+        )
+        if len(self.fspaths) > 1:
+            if collation >= self.CopyCollation.siblings:
+                if not all(p.parent == self.parent for p in self.fspaths):
+                    selected_mode -= self.CopyMode.leave
+                duplicate_names = [
+                    n for n, c in Counter(p.name for p in self.fspaths).items() if c > 1
+                ]
+                if duplicate_names:
+                    raise FileFormatsError(
+                        f"Cannot copy {self} to {dest_dir} with collation mode "
+                        f'"{collation}", as there are duplicate filenames, {duplicate_names}, '
+                        f"in file paths: " + "\n".join(str(p) for p in self.fspaths)
+                    )
+            if collation == self.CopyCollation.adjacent:
+                exts = [splitext(p, multi=multi_splitext)[1] for p in self.fspaths]
+                duplicate_exts = [n for n, c in Counter(exts).items() if c > 1]
+                if duplicate_exts:
+                    raise FileFormatsError(
+                        f"Cannot copy {self} to {dest_dir} with collation mode "
+                        f'"{collation}", as there are duplicate extensions, {duplicate_exts}, '
+                        f"in file paths: " + "\n".join(str(p) for p in self.fspaths)
+                    )
+        if not selected_mode:
+            raise FileFormatsError(
+                f"Cannot copy {self} using {mode} mode as it is not supported by "
+                f"the {supported_modes} given the collation specification, {collation}"
+            )
+        if selected_mode & self.CopyMode.leave:
+            return self
+        dest_dir = Path(dest_dir)  # ensure a Path not a string
+        if make_dirs:
+            dest_dir.mkdir(parents=True, exist_ok=True)
+        if selected_mode & self.CopyMode.symlink:
+            copy_dir = copy_file = os.symlink
+        elif selected_mode & self.CopyMode.hardlink:
+            copy_file = os.link
+
+            def hardlink_dir(src: Path, dest: Path):
+                for dpath, _, fpaths in os.walk(src):
+                    dpath = Path(dpath)
+                    relpath = dpath.relative_to(src)
+                    (dest / relpath).mkdir()
+                    for fpath in fpaths:
+                        os.link(dpath / fpath, dest / relpath / fpath)
+
+            copy_dir = hardlink_dir
+        else:
+            assert selected_mode & self.CopyMode.copy
+            copy_dir = shutil.copytree
+            copy_file = shutil.copyfile
+        new_paths = []
+        if trim and self.required_paths():
+            fspaths_to_copy = self.required_paths()
+        else:
+            fspaths_to_copy = self.fspaths
+        if not fspaths_to_copy:
+            raise FileFormatsError(
+                f"Cannot copy {self} because none of the fspaths in the file-set are "
+                "required. Set trim=False to copy all file-paths"
+            )
+        if collation == self.CopyCollation.adjacent:
+            if stem is None:
+                try:
+                    # Attempt to get the stem of the primary path
+                    stem = self.stem
+                except AttributeError:
+                    # If there isn't a primary path, ick the stem of the first of the sorted
+                    # paths
+                    stem = splitext(sorted(self.fspaths)[0], multi=multi_splitext)[0]
+        elif stem is not None:
+            raise FileFormatsError(
+                f"'stem' ({stem}) provided to FileSet.copy() method when collation is "
+                f"not set to 'adjacent' ({collation})"
+            )
+        for fspath in fspaths_to_copy:
+            if collation == self.CopyCollation.adjacent:
+                new_path = dest_dir / (stem + splitext(fspath, multi=multi_splitext)[1])
+            elif collation == self.CopyCollation.siblings:
+                new_path = dest_dir / fspath.name
+            else:
+                assert collation == self.CopyCollation.any
+                new_path = dest_dir / fspath.relative_to(self.parent)
+                new_path.parent.mkdir(parents=True, exist_ok=True)
+            if new_path.exists():
+                if overwrite:
+                    if fspath.is_dir():
+                        shutil.rmtree(new_path)
+                    else:
+                        os.unlink(new_path)
+                else:
+                    raise FileFormatsError(
+                        f"Destination path '{str(new_path)}' exists, set "
+                        "'overwrite' to overwrite it"
+                    )
+            if fspath.is_dir():
+                copy_dir(fspath, new_path)
+            else:
+                copy_file(fspath, new_path)
+            new_paths.append(new_path)
+        return type(self)(new_paths)
+
+    def copy_to(self, *args, **kwargs):
+        """For b/w compatibility (temporary message)"""
+        warn("'FileSet.copy_to()' has been deprecated, please use copy() instead")
+        return self.copy(*args, **kwargs)
+
     _all_formats = None
     _formats_by_iana_mime = None
     _formats_by_name = None
```

### Comparing `fileformats-0.6.3/fileformats/core/mark.py` & `fileformats-0.6.4/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/mixin.py` & `fileformats-0.6.4/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/utils.py` & `fileformats-0.6.4/fileformats/core/utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/tests/test_classifiers.py` & `fileformats-0.6.4/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/tests/test_converter.py` & `fileformats-0.6.4/fileformats/core/tests/test_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import attrs
 import pytest
+from pydra.engine.specs import File
 from fileformats.testing import Foo, Bar, Baz, Qux
 from fileformats.core import mark
 from fileformats.core.exceptions import FormatConversionError
 from conftest import write_test_file
 
 try:
     import pydra.mark
@@ -38,15 +39,15 @@
 def FooQuxConverter():
     from pydra.engine import specs
     from pydra import ShellCommandTask
 
     input_fields = [
         (
             "in_file",
-            specs.File,
+            File,
             {
                 "help_string": "the input file",
                 "argstr": "",
             },
         ),
         (
             "out_file",
@@ -63,15 +64,15 @@
     FooQux_input_spec = specs.SpecInfo(
         name="Input", fields=input_fields, bases=(specs.ShellSpec,)
     )
 
     output_fields = [
         (
             "out_file",
-            specs.File,
+            File,
             {
                 "help_string": "output file",
             },
         ),
     ]
     FooQux_output_spec = specs.SpecInfo(
         name="Output", fields=output_fields, bases=(specs.ShellOutSpec,)
```

### Comparing `fileformats-0.6.3/fileformats/core/tests/test_detection.py` & `fileformats-0.6.4/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/tests/test_general.py` & `fileformats-0.6.4/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/tests/test_mime.py` & `fileformats-0.6.4/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/tests/test_mixin.py` & `fileformats-0.6.4/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/core/tests/test_utils.py` & `fileformats-0.6.4/fileformats/core/tests/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from pathlib import Path
 import os.path
 import random
 import shutil
 import time
 import pytest
+from fileformats.core import FileSet
 from fileformats.generic import File, Directory, FsObject
 from fileformats.core.mixin import WithSeparateHeader
 from fileformats.core.utils import (
     find_matching,
     MissingExtendedDependency,
 )
-from fileformats.core.exceptions import MissingExtendedDepenciesError
+from fileformats.core.exceptions import MissingExtendedDepenciesError, FileFormatsError
 import fileformats.text
 import fileformats.numeric
 from conftest import write_test_file
 
 
 class Bar(File):
     ext = ".bar"
@@ -112,18 +113,129 @@
         os.path.samefile(c, o)
         for c, o in zip(sorted(cpy.fspaths), sorted(fsobject.fspaths))
         if o.is_file()
     )
     assert cpy.hash() == fsobject.hash()
 
 
-def test_copy_with_rename(foo_file, dest_dir):
-    cpy = foo_file.copy(dest_dir, stem="new")
-    assert cpy.fspath.name == "new.foo"
-    assert cpy.header.fspath.name == "new.bar"
+def test_copy_collation_same_name(work_dir: Path, dest_dir: Path):
+
+    a = work_dir / "a" / "file.txt"
+    b = work_dir / "b" / "file.txt"
+    c = work_dir / "c" / "d" / "file.txt"
+    fspaths = (a, b, c)
+
+    for x in fspaths:
+        x.parent.mkdir(parents=True)
+        Path.touch(x)
+
+    fileset = FileSet(fspaths)
+
+    with pytest.raises(
+        FileFormatsError,
+        match="as there are duplicate filenames",
+    ):
+        fileset.copy(dest_dir=dest_dir, collation="siblings")
+    cpy = fileset.copy(dest_dir=dest_dir, collation="any")
+    assert sorted(cpy.relative_fspaths) == sorted(fileset.relative_fspaths)
+    assert cpy.parent == dest_dir
+
+
+def test_copy_collation_same_ext(work_dir: Path, dest_dir: Path):
+
+    a = work_dir / "a" / "filea.txt"
+    b = work_dir / "b" / "fileb.txt"
+    c = work_dir / "c" / "d" / "filec.txt"
+    fspaths = (a, b, c)
+
+    for x in fspaths:
+        x.parent.mkdir(parents=True)
+        Path.touch(x)
+
+    fileset = FileSet(fspaths)
+
+    with pytest.raises(
+        FileFormatsError,
+        match="as there are duplicate extensions",
+    ):
+        fileset.copy(dest_dir=dest_dir, collation="adjacent")
+    cpy = fileset.copy(dest_dir=dest_dir, collation="siblings")
+    assert sorted(p.name for p in cpy.fspaths) == sorted(
+        p.name for p in fileset.fspaths
+    )
+    assert all(p.parent == dest_dir for p in cpy.fspaths)
+
+
+def test_copy_collation_diff_ext(work_dir: Path, dest_dir: Path):
+
+    a = work_dir / "a" / "filea.x"
+    b = work_dir / "b" / "fileb.y"
+    c = work_dir / "c" / "d" / "filec.z"
+    fspaths = (a, b, c)
+
+    for x in fspaths:
+        x.parent.mkdir(parents=True)
+        Path.touch(x)
+
+    fileset = FileSet(fspaths)
+
+    cpy = fileset.copy(dest_dir=dest_dir, collation="adjacent")
+    assert all(p.parent == dest_dir for p in cpy.fspaths)
+    assert all(p.stem == "filea" for p in cpy.fspaths)
+
+
+def test_copy_collation_stem(work_dir: Path, dest_dir: Path):
+
+    a = work_dir / "a" / "filea.x"
+    b = work_dir / "b" / "fileb.y"
+    c = work_dir / "c" / "d" / "filec.z"
+    fspaths = (a, b, c)
+
+    for x in fspaths:
+        x.parent.mkdir(parents=True)
+        Path.touch(x)
+
+    fileset = FileSet(fspaths)
+
+    cpy = fileset.copy(dest_dir=dest_dir, collation="adjacent", stem="newfile")
+    assert all(p.parent == dest_dir for p in cpy.fspaths)
+    assert all(p.stem == "newfile" for p in cpy.fspaths)
+
+
+def test_copy_collation_with_stem_not_adjacent(foo_file: Foo, dest_dir):
+    with pytest.raises(
+        FileFormatsError, match="when collation is not set to 'adjacent'"
+    ):
+        foo_file.copy(dest_dir, collation="any", stem="new")
+
+
+def test_copy_collation_leave_diff_dir(work_dir: Path, dest_dir: Path):
+
+    a = work_dir / "a" / "file.x"
+    b = work_dir / "b" / "file.y"
+    c = work_dir / "c" / "file.z"
+    fspaths = (a, b, c)
+
+    for x in fspaths:
+        x.parent.mkdir(parents=True)
+        Path.touch(x)
+
+    fileset = FileSet(fspaths)
+
+    with pytest.raises(
+        FileFormatsError,
+        match="using leave mode as it is not supported by the any given the collation specification",
+    ):
+        fileset.copy(dest_dir=dest_dir, mode="leave", collation="siblings")
+
+    with pytest.raises(
+        FileFormatsError,
+        match="using leave mode as it is not supported by the any given the collation specification",
+    ):
+        fileset.copy(dest_dir=dest_dir, mode="leave", collation="adjacent")
 
 
 def test_copy_ext(work_dir):
     assert (
         File.copy_ext(work_dir / "x.foo.bar", work_dir / "y") == work_dir / "y.foo.bar"
     )
     assert Bar.copy_ext(work_dir / "x.foo.bar", work_dir / "y") == work_dir / "y.bar"
```

### Comparing `fileformats-0.6.3/fileformats/document/__init__.py` & `fileformats-0.6.4/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/field/__init__.py` & `fileformats-0.6.4/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/field/tests/test_fields.py` & `fileformats-0.6.4/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.6.4/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/generic/__init__.py` & `fileformats-0.6.4/fileformats/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/image/converters.py` & `fileformats-0.6.4/fileformats/image/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/image/raster.py` & `fileformats-0.6.4/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/image/tests/test_image_converters.py` & `fileformats-0.6.4/fileformats/image/tests/test_image_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/image/tests/test_image_raster.py` & `fileformats-0.6.4/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/serialization/__init__.py` & `fileformats-0.6.4/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/serialization/converters.py` & `fileformats-0.6.4/fileformats/serialization/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/serialization/tests/test_serialization_converters.py` & `fileformats-0.6.4/fileformats/serialization/tests/test_serialization_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/fileformats/text/__init__.py` & `fileformats-0.6.4/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/LICENSE` & `fileformats-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/README.rst` & `fileformats-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/pyproject.toml` & `fileformats-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.3/PKG-INFO` & `fileformats-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.6.3
+Version: 0.6.4
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

