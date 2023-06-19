# Comparing `tmp/fileformats-0.6.4.tar.gz` & `tmp/fileformats-0.6.5.tar.gz`

## Comparing `fileformats-0.6.4.tar` & `fileformats-0.6.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/archive/__init__.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/archive/converters.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/_version.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/converter.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/datatype.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/field.py
--rw-r--r--   0        0        0    37604 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/fileset.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/mark.py
--rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/mixin.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/utils.py
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/document/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/base.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/converters.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/vector.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/tests/test_image_converters.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/serialization/converters.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.4/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.4/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.4/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.4/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.4/README.rst
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/archive/converters.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/archive/tests/test_archive_converters.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/converter.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/datatype.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/field.py
+-rw-r--r--   0        0        0    42571 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/mark.py
+-rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/mixin.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/utils.py
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/base.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/converters.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/vector.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/tests/test_image_converters.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/misc/medical.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/serialization/converters.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/serialization/tests/test_serialization_converters.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/text/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.5/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.5/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.5/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.5/README.rst
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.5/PKG-INFO
```

### Comparing `fileformats-0.6.4/fileformats/archive/__init__.py` & `fileformats-0.6.5/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/archive/converters.py` & `fileformats-0.6.5/fileformats/archive/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/archive/tests/test_archive_converters.py` & `fileformats-0.6.5/fileformats/archive/tests/test_archive_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/audio/__init__.py` & `fileformats-0.6.5/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/converter.py` & `fileformats-0.6.5/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/datatype.py` & `fileformats-0.6.5/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/field.py` & `fileformats-0.6.5/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/fileset.py` & `fileformats-0.6.5/fileformats/core/fileset.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import attrs
 from .utils import (
     classproperty,
     fspaths_converter,
     to_mime_format_name,
     STANDARD_NAMESPACES,
     describe_task,
-    splitext,
 )
 from .converter import SubtypeVar
 from .exceptions import (
     FileFormatsError,
     FormatMismatchError,
     FormatConversionError,
 )
@@ -198,14 +197,30 @@
                     if isinstance(p, os.PathLike):
                         paths.append(Path(p))
             for path in paths:
                 if path in self.fspaths:
                     required.add(path)
         return required
 
+    def nested_filesets(self) -> ty.List[FileSet]:
+        """Returns all nested filesets that are required for the format
+
+        Returns
+        ------
+        fileset : list[FileSet]
+            a fileset that is nested within the broader fileset
+        """
+        nested = []
+        for prop_name in sorted(self.required_properties()):
+            prop = getattr(self, prop_name)
+            if isinstance(prop, FileSet):
+                nested.append(prop)
+                nested.extend(prop.nested_filesets())
+        return nested
+
     def trim_paths(self):
         """Trims paths in fspaths to only those that are "required" by the format class
         i.e. returned by a required property"""
         self.fspaths = fspaths_converter(self.required_paths())
         return self
 
     @classmethod
@@ -726,14 +741,111 @@
         """
         cls = type(self)
         yield f"{cls.__module__}.{cls.__name__}:".encode()
         for key, chunk_iter in self.byte_chunks():
             yield (",'" + key + "'=").encode()
             yield from chunk_iter
 
+    class ExtensionDecomposition(IntEnum):
+        """What to consider the file extension to be for paths without an explicitly
+        defined extension
+
+        Options
+        -------
+        none
+            assume it doesn't have a file extension
+        single
+            assume that anything after the last '.' is the extension, e.g. the extension
+            of "file.nii.gz" would be ".gz"
+        multiple
+            assume that anything after the first '.' is the extension, e.g. the extension
+            of "file.nii.gz" would be "nii.gz"
+        """
+
+        none = 0
+        single = 1
+        multiple = 2
+
+        def __str__(self):
+            return self.name
+
+    def decomposed_fspaths(
+        self,
+        required_only: bool = True,
+        decomposition_mode: ExtensionDecomposition = ExtensionDecomposition.single,
+    ) -> ty.List[ty.Tuple[Path, str, str]]:
+        """Decompose paths into parent directory, filename stem, and extension
+
+        Parameters
+        ----------
+        required_only : bool, optional
+            only include required paths, by default True
+        assume_implicit_ext : FileSet.ExtensionDecomposition, optional
+            how to interpret paths without an explicitly defined extension (i.e. by
+            either the extension of the FileSet or nested filesets), by default single
+
+        Returns
+        -------
+        decomposed_fspath : list[tuple[Path, str, str]]
+            a tuple consisting of the parent directory, file-stem and extension
+        """
+        from ..generic import File
+
+        decomposed_fspaths = []
+        implicit = set(
+            self.required_paths()
+            if required_only and self.required_paths()
+            else self.fspaths
+        )
+        nested = self.nested_filesets()
+        for fileset in [self] + nested:
+            if isinstance(fileset, File):
+                decomposed = (fileset.fspath.parent, fileset.stem, fileset.actual_ext)
+                if fileset.fspath in implicit:
+                    decomposed_fspaths.append(decomposed)
+                    implicit.remove(fileset.fspath)
+                elif decomposed not in decomposed_fspaths:
+                    previous_fileset = next(
+                        f for f in nested if f.fspath == fileset.fspath
+                    )
+                    previous = (
+                        previous_fileset.fspath.parent,
+                        previous_fileset.stem,
+                        previous_fileset.actual_ext,
+                    )
+                    warn(
+                        f"The '{fileset.fspath}' path within {self} into has been decomposed as "
+                        f"{previous} as it was interpreted as a {type(previous_fileset)} "
+                        f"file, whereas it is also interpreted as a {type(fileset)}, in "
+                        f"which case it could be alternatively decomposed into {decomposed}"
+                    )
+        for fspath in implicit:
+            decomposed_fspaths.append(
+                self.decompose_fspath(fspath, mode=decomposition_mode)
+            )
+        return decomposed_fspaths
+
+    @classmethod
+    def decompose_fspath(
+        cls, fspath: Path, mode: ExtensionDecomposition = ExtensionDecomposition.single
+    ) -> ty.Tuple[Path, str, str]:
+        """Decompose an arbitrary file-system path into parent dir, stem and extension
+        given the assumption on what constitutes an extension"""
+        if mode == cls.ExtensionDecomposition.multiple:
+            ext = "".join(fspath.suffixes)
+            stem = fspath.name[: -len(ext)]
+        elif mode == cls.ExtensionDecomposition.single:
+            stem = fspath.stem
+            ext = fspath.suffix
+        else:
+            assert mode == cls.ExtensionDecomposition.none
+            stem = fspath
+            ext = ""
+        return fspath.parent, stem, ext
+
     class CopyMode(Enum):
         """Designates the desired behaviour of the FileSet.copy() method with regards to
         symbolic, hard or full copies
 
         Basic options (in order of preference)
         --------------------------------------
         leave
@@ -840,20 +952,20 @@
             return self.name
 
     def copy(
         self,
         dest_dir: Path,
         mode: ty.Union[CopyMode, str] = CopyMode.copy,
         collation: ty.Union[CopyCollation, str] = CopyCollation.any,
-        stem: ty.Optional[str] = None,
+        new_stem: ty.Optional[str] = None,
         trim: bool = True,
         make_dirs: bool = False,
         overwrite: bool = False,
-        multi_splitext: bool = True,
         supported_modes: CopyMode = CopyMode.any,
+        extension_decomposition: ExtensionDecomposition = ExtensionDecomposition.single,
     ):
         """Copies the file-set to a new directory, optionally renaming the files
         to have consistent name-stems.
 
         Parameters
         ----------
         dest_dir : str
@@ -861,66 +973,76 @@
         mode : FileSet.CopyMode or str, optional
             designates whether to perform an actual copy or whether a link (symbolic or
             hard) is okay, 'duplicate' by default. See FielSet.CopyMode for details
         collation : FileSet.CopyCollation or str, optional
             how to treat relative paths within the fileset, i.e. whether to move them
             to a single directory, rename them to the same file-stem or maintain
             relative directory structure. See FileSet.CopyCollation for details
-        stem: str, optional
+        new_stem: str, optional
             the file name excluding file extensions, to give the files/dirs in the parent
             directory, by default the original file name is used
         trim : bool, optional
             Only copy the paths in the file-set that are "required" by the format,
             true by default
         make_dirs : bool, optional
             Make the parent destination and all missing ancestors if they are missing,
             false by default
         overwrite : bool, optional
             whether to overwrite existing files/directories if present
-        multi_splitext : bool, optional
-            whether to consider file extensions to start from the first '.' (True) or the
-            last (False), by default True
         supported_modes : CopyMode, optional
             supported modes for the copy operation. Used to mask out the requested
             copy mode
+        extension_decomposition : FileSet.ExtensionDecomposition, optional
+            whether to consider file extensions to start from the first '.' (multiple) or the
+            last (single) or be empty (none), when the extension of a fspath in the
+            FileSet isn't explicitly defined by the FileSet class. Only relevant when
+            collation mode is set to "adjacent". By default True
         """
         mode = self.CopyMode[mode] if isinstance(mode, str) else mode
         selected_mode = mode & supported_modes
-        collation = (
-            self.CopyCollation[collation] if isinstance(collation, str) else collation
-        )
-        if len(self.fspaths) > 1:
-            if collation >= self.CopyCollation.siblings:
-                if not all(p.parent == self.parent for p in self.fspaths):
-                    selected_mode -= self.CopyMode.leave
-                duplicate_names = [
-                    n for n, c in Counter(p.name for p in self.fspaths).items() if c > 1
-                ]
-                if duplicate_names:
-                    raise FileFormatsError(
-                        f"Cannot copy {self} to {dest_dir} with collation mode "
-                        f'"{collation}", as there are duplicate filenames, {duplicate_names}, '
-                        f"in file paths: " + "\n".join(str(p) for p in self.fspaths)
-                    )
-            if collation == self.CopyCollation.adjacent:
-                exts = [splitext(p, multi=multi_splitext)[1] for p in self.fspaths]
-                duplicate_exts = [n for n, c in Counter(exts).items() if c > 1]
-                if duplicate_exts:
-                    raise FileFormatsError(
-                        f"Cannot copy {self} to {dest_dir} with collation mode "
-                        f'"{collation}", as there are duplicate extensions, {duplicate_exts}, '
-                        f"in file paths: " + "\n".join(str(p) for p in self.fspaths)
-                    )
+        if len(self.fspaths) == 1:
+            # If there is only one path to copy, then collation isn't meaningful
+            collation = self.CopyCollation.any
+        else:
+            collation = (
+                self.CopyCollation[collation]
+                if isinstance(collation, str)
+                else collation
+            )
+        if collation >= self.CopyCollation.siblings:
+            if not all(p.parent == self.parent for p in self.fspaths):
+                selected_mode -= self.CopyMode.leave
+            duplicate_names = [
+                n for n, c in Counter(p.name for p in self.fspaths).items() if c > 1
+            ]
+            if duplicate_names:
+                raise FileFormatsError(
+                    f"Cannot copy {self} to {dest_dir} with collation mode "
+                    f'"{collation}", as there are duplicate filenames, {duplicate_names}, '
+                    f"in file paths: " + "\n".join(str(p) for p in self.fspaths)
+                )
         if not selected_mode:
             raise FileFormatsError(
                 f"Cannot copy {self} using {mode} mode as it is not supported by "
                 f"the {supported_modes} given the collation specification, {collation}"
             )
         if selected_mode & self.CopyMode.leave:
-            return self
+            return self  # Don't need to do anything
+        if collation == self.CopyCollation.adjacent:
+            decomposed_fspaths = self.decomposed_fspaths(
+                required_only=trim, decomposition_mode=extension_decomposition
+            )
+            exts = [d[-1] for d in decomposed_fspaths]
+            duplicate_exts = [n for n, c in Counter(exts).items() if c > 1]
+            if duplicate_exts:
+                raise FileFormatsError(
+                    f"Cannot copy {self} to {dest_dir} with collation mode "
+                    f'"{collation}", as there are duplicate extensions, {duplicate_exts}, '
+                    f"in file paths: " + "\n".join(str(p) for p in self.fspaths)
+                )
         dest_dir = Path(dest_dir)  # ensure a Path not a string
         if make_dirs:
             dest_dir.mkdir(parents=True, exist_ok=True)
         if selected_mode & self.CopyMode.symlink:
             copy_dir = copy_file = os.symlink
         elif selected_mode & self.CopyMode.hardlink:
             copy_file = os.link
@@ -945,30 +1067,29 @@
             fspaths_to_copy = self.fspaths
         if not fspaths_to_copy:
             raise FileFormatsError(
                 f"Cannot copy {self} because none of the fspaths in the file-set are "
                 "required. Set trim=False to copy all file-paths"
             )
         if collation == self.CopyCollation.adjacent:
-            if stem is None:
-                try:
-                    # Attempt to get the stem of the primary path
-                    stem = self.stem
-                except AttributeError:
-                    # If there isn't a primary path, ick the stem of the first of the sorted
-                    # paths
-                    stem = splitext(sorted(self.fspaths)[0], multi=multi_splitext)[0]
-        elif stem is not None:
+            if new_stem is None:
+                new_stem = sorted(decomposed_fspaths)[0][1]
+            # Warning we redefine fspaths_to_copy as list of tuples not Paths
+            fspaths_to_copy = decomposed_fspaths
+        elif new_stem is not None:
             raise FileFormatsError(
-                f"'stem' ({stem}) provided to FileSet.copy() method when collation is "
+                f"'stem' ({new_stem}) provided to FileSet.copy() method when collation is "
                 f"not set to 'adjacent' ({collation})"
             )
         for fspath in fspaths_to_copy:
             if collation == self.CopyCollation.adjacent:
-                new_path = dest_dir / (stem + splitext(fspath, multi=multi_splitext)[1])
+                # fspath is a path decomposed into parent, stem, ext instead of a Path
+                parent_dir, old_stem, ext = fspath
+                fspath = parent_dir / (old_stem + ext)  # reconstruct into a Path
+                new_path = dest_dir / (new_stem + ext)
             elif collation == self.CopyCollation.siblings:
                 new_path = dest_dir / fspath.name
             else:
                 assert collation == self.CopyCollation.any
                 new_path = dest_dir / fspath.relative_to(self.parent)
                 new_path.parent.mkdir(parents=True, exist_ok=True)
             if new_path.exists():
```

### Comparing `fileformats-0.6.4/fileformats/core/mark.py` & `fileformats-0.6.5/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/mixin.py` & `fileformats-0.6.5/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/utils.py` & `fileformats-0.6.5/fileformats/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,42 +45,14 @@
     return matches
 
 
 def from_mime(mime_str: str):
     return fileformats.core.DataType.from_mime(mime_str)
 
 
-def splitext(fspath: Path, multi=False):
-    """splits an extension from the file stem, taking into consideration multi-part
-    extensions such as ".nii.gz".
-
-    Parameters
-    ----------
-    fspath : Path
-        the file-system path to split the extension from
-    multi : bool, optional
-        whether to support multi-part extensions such as ".nii.gz". Note this means that
-        it will match sections of file names with "."s in them, by default False
-
-    Returns
-    -------
-    str
-        file stem
-    str
-        file extension
-    """
-    if multi:
-        ext = "".join(fspath.suffixes)
-        stem = fspath.name[: -len(ext)]
-    else:
-        stem = fspath.stem
-        ext = fspath.suffix
-    return stem, ext
-
-
 def subpackages():
     """Iterates over all subpackages within the fileformats namespace
 
     Yields
     ------
     module
         all modules within the package
```

### Comparing `fileformats-0.6.4/fileformats/core/tests/test_classifiers.py` & `fileformats-0.6.5/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/tests/test_converter.py` & `fileformats-0.6.5/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/tests/test_detection.py` & `fileformats-0.6.5/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/tests/test_general.py` & `fileformats-0.6.5/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/tests/test_mime.py` & `fileformats-0.6.5/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/tests/test_mixin.py` & `fileformats-0.6.5/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/core/tests/test_utils.py` & `fileformats-0.6.5/fileformats/core/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 import os.path
 import random
 import shutil
 import time
 import pytest
-from fileformats.core import FileSet
+from fileformats.core import FileSet, mark
 from fileformats.generic import File, Directory, FsObject
 from fileformats.core.mixin import WithSeparateHeader
 from fileformats.core.utils import (
     find_matching,
     MissingExtendedDependency,
 )
 from fileformats.core.exceptions import MissingExtendedDepenciesError, FileFormatsError
@@ -114,15 +114,14 @@
         for c, o in zip(sorted(cpy.fspaths), sorted(fsobject.fspaths))
         if o.is_file()
     )
     assert cpy.hash() == fsobject.hash()
 
 
 def test_copy_collation_same_name(work_dir: Path, dest_dir: Path):
-
     a = work_dir / "a" / "file.txt"
     b = work_dir / "b" / "file.txt"
     c = work_dir / "c" / "d" / "file.txt"
     fspaths = (a, b, c)
 
     for x in fspaths:
         x.parent.mkdir(parents=True)
@@ -137,15 +136,14 @@
         fileset.copy(dest_dir=dest_dir, collation="siblings")
     cpy = fileset.copy(dest_dir=dest_dir, collation="any")
     assert sorted(cpy.relative_fspaths) == sorted(fileset.relative_fspaths)
     assert cpy.parent == dest_dir
 
 
 def test_copy_collation_same_ext(work_dir: Path, dest_dir: Path):
-
     a = work_dir / "a" / "filea.txt"
     b = work_dir / "b" / "fileb.txt"
     c = work_dir / "c" / "d" / "filec.txt"
     fspaths = (a, b, c)
 
     for x in fspaths:
         x.parent.mkdir(parents=True)
@@ -162,15 +160,14 @@
     assert sorted(p.name for p in cpy.fspaths) == sorted(
         p.name for p in fileset.fspaths
     )
     assert all(p.parent == dest_dir for p in cpy.fspaths)
 
 
 def test_copy_collation_diff_ext(work_dir: Path, dest_dir: Path):
-
     a = work_dir / "a" / "filea.x"
     b = work_dir / "b" / "fileb.y"
     c = work_dir / "c" / "d" / "filec.z"
     fspaths = (a, b, c)
 
     for x in fspaths:
         x.parent.mkdir(parents=True)
@@ -180,40 +177,38 @@
 
     cpy = fileset.copy(dest_dir=dest_dir, collation="adjacent")
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert all(p.stem == "filea" for p in cpy.fspaths)
 
 
 def test_copy_collation_stem(work_dir: Path, dest_dir: Path):
-
     a = work_dir / "a" / "filea.x"
     b = work_dir / "b" / "fileb.y"
     c = work_dir / "c" / "d" / "filec.z"
     fspaths = (a, b, c)
 
     for x in fspaths:
         x.parent.mkdir(parents=True)
         Path.touch(x)
 
     fileset = FileSet(fspaths)
 
-    cpy = fileset.copy(dest_dir=dest_dir, collation="adjacent", stem="newfile")
+    cpy = fileset.copy(dest_dir=dest_dir, collation="adjacent", new_stem="newfile")
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert all(p.stem == "newfile" for p in cpy.fspaths)
 
 
 def test_copy_collation_with_stem_not_adjacent(foo_file: Foo, dest_dir):
     with pytest.raises(
         FileFormatsError, match="when collation is not set to 'adjacent'"
     ):
-        foo_file.copy(dest_dir, collation="any", stem="new")
+        foo_file.copy(dest_dir, collation="any", new_stem="new")
 
 
 def test_copy_collation_leave_diff_dir(work_dir: Path, dest_dir: Path):
-
     a = work_dir / "a" / "file.x"
     b = work_dir / "b" / "file.y"
     c = work_dir / "c" / "file.z"
     fspaths = (a, b, c)
 
     for x in fspaths:
         x.parent.mkdir(parents=True)
@@ -232,19 +227,65 @@
         match="using leave mode as it is not supported by the any given the collation specification",
     ):
         fileset.copy(dest_dir=dest_dir, mode="leave", collation="adjacent")
 
 
 def test_copy_ext(work_dir):
     assert (
-        File.copy_ext(work_dir / "x.foo.bar", work_dir / "y") == work_dir / "y.foo.bar"
+        File.copy_ext(
+            work_dir / "x.foo.bar",
+            work_dir / "y",
+            decomposition_mode=FileSet.ExtensionDecomposition.none,
+        )
+        == work_dir / "y"
+    )
+    assert (
+        File.copy_ext(
+            work_dir / "x.foo.bar",
+            work_dir / "y",
+            decomposition_mode=FileSet.ExtensionDecomposition.single,
+        )
+        == work_dir / "y.bar"
+    )
+    assert (
+        File.copy_ext(
+            work_dir / "x.foo.bar",
+            work_dir / "y",
+            decomposition_mode=FileSet.ExtensionDecomposition.multiple,
+        )
+        == work_dir / "y.foo.bar"
     )
     assert Bar.copy_ext(work_dir / "x.foo.bar", work_dir / "y") == work_dir / "y.bar"
 
 
+def test_decompose_fspaths(work_dir):
+    class FooBar(File):
+        ext = ".foo.bar"
+
+    class DoubleBar(FileSet):
+        @mark.required
+        @property
+        def bar(self):
+            return Bar(self.select_by_ext(Bar))
+
+        @mark.required
+        @property
+        def foo_bar(self):
+            return FooBar(self.select_by_ext(FooBar))
+
+    fspath = work_dir / "file.foo.bar"
+    Path.touch(fspath)
+    double_bar = DoubleBar(fspath)
+
+    with pytest.warns(match="whereas it is also interpreted as a"):
+        decomposed = double_bar.decomposed_fspaths()
+
+    assert decomposed == [(work_dir, "file.foo", ".bar")]
+
+
 def test_format_detection(work_dir):
     text_file = work_dir / "text.txt"
 
     with open(text_file, "w") as f:
         f.write("sample text")
 
     detected = find_matching(text_file, standard_only=True)
```

### Comparing `fileformats-0.6.4/fileformats/document/__init__.py` & `fileformats-0.6.5/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/field/__init__.py` & `fileformats-0.6.5/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/field/tests/test_fields.py` & `fileformats-0.6.5/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.6.5/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/generic/__init__.py` & `fileformats-0.6.5/fileformats/generic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 import attrs
 from fileformats.core.fileset import FileSet
 from fileformats.core.exceptions import FormatMismatchError, FileFormatsError
 from fileformats.core import mark
-from fileformats.core.utils import splitext, classproperty
+from fileformats.core.utils import classproperty
 from fileformats.core.mixin import WithClassifiers
 
 
 @attrs.define
 class FsObject(FileSet, os.PathLike):
     "Generic file-system object, can be either a file or a directory"
 
@@ -60,36 +60,48 @@
                 raise FormatMismatchError(
                     f'Path that matches extension of "{type(self)}", {fspath}, is not a '
                     "file in {repr(self)}" + msg
                 )
         return fspath
 
     @classmethod
-    def copy_ext(cls, old_path: Path, new_path: Path):
+    def copy_ext(
+        cls,
+        old_path: Path,
+        new_path: Path,
+        decomposition_mode=FileSet.ExtensionDecomposition.none,
+    ):
         """Copy extension from the old path to the new path, ensuring that all
         of the extension is used (e.g. 'my.gz' instead of 'gz')
 
         Parameters
         ----------
         old_path: Path or str
             The path from which to copy the extension from
         new_path: Path or str
             The path to append the extension to
+        decomposition_mode : FileSet.ExtensionDecomposition, optional
+            if the file doesn't have an explicit extension, how to interpret "." within
+            the filename
 
         Returns
         -------
         Path
             The new path with the copied extension
         """
         if not cls.matching_exts([old_path], [cls.ext]):
             raise FormatMismatchError(
                 f"Extension of old path ('{str(old_path)}') does not match that "
                 f"of file, '{cls.ext}'"
             )
-        suffix = cls.ext if cls.ext else splitext(old_path, multi=True)[-1]
+        suffix = (
+            cls.ext
+            if cls.ext
+            else cls.decompose_fspath(old_path, mode=decomposition_mode)[-1]
+        )
         return Path(new_path).with_suffix(suffix)
 
     @property
     def contents(self):
         return self.read_contents()
 
     def read_contents(self, size=None, offset=0):
@@ -119,15 +131,19 @@
                 "checked at initialisation"
             )
         # Return the longest matching extension, useful for optional extensions
         return sorted(matching, key=len)[-1]
 
     @property
     def stem(self):
-        return self.fspath.name[: -len(self.actual_ext)]
+        if self.actual_ext:
+            stem = self.fspath.name[: -len(self.actual_ext)]
+        else:
+            stem = self.fspath
+        return stem
 
 
 @attrs.define
 class Directory(FsObject):
     """Base directory to be overridden by subtypes that represent directories but don't
     want to inherit content type "qualifers" (i.e. most of them)"""
 
@@ -236,12 +252,11 @@
     # WithClassifiers-required class attrs
     classifiers_attr_name = "content_types"
     allowed_classifiers = (FileSet,)
     generically_qualifies = True
 
 
 class SetOf(WithClassifiers, TypedSet):
-
     # WithClassifiers-required class attrs
     classifiers_attr_name = "content_types"
     allowed_classifiers = (FileSet,)
     generically_qualifies = True
```

### Comparing `fileformats-0.6.4/fileformats/image/converters.py` & `fileformats-0.6.5/fileformats/image/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/image/raster.py` & `fileformats-0.6.5/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/image/tests/test_image_converters.py` & `fileformats-0.6.5/fileformats/image/tests/test_image_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/image/tests/test_image_raster.py` & `fileformats-0.6.5/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/serialization/__init__.py` & `fileformats-0.6.5/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/serialization/converters.py` & `fileformats-0.6.5/fileformats/serialization/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/serialization/tests/test_serialization_converters.py` & `fileformats-0.6.5/fileformats/serialization/tests/test_serialization_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/fileformats/text/__init__.py` & `fileformats-0.6.5/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/LICENSE` & `fileformats-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/README.rst` & `fileformats-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/pyproject.toml` & `fileformats-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.4/PKG-INFO` & `fileformats-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.6.4
+Version: 0.6.5
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

