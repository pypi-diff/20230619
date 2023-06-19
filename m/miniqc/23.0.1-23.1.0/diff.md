# Comparing `tmp/miniqc-23.0.1.tar.gz` & `tmp/miniqc-23.1.0.tar.gz`

## Comparing `miniqc-23.0.1.tar` & `miniqc-23.1.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 miniqc-23.0.1/CHANGELOG.rst
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 miniqc-23.0.1/Dockerfile
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 miniqc-23.0.1/.github/workflows/docker.yml
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 miniqc-23.0.1/.github/workflows/hatch.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 miniqc-23.0.1/.maint/local_gitignore
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 miniqc-23.0.1/.maint/make_gitignore
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/__init__.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/__main__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/_version.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/_version.pyi
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/nifti.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/py.typed
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 miniqc-23.0.1/miniqc/types.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/__init__.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/conftest.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/test_miniqc.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/test_nifti.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/dataset_description.json
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/sub-01/anat/sub-01_acq-dangling_T2w.nii.gz -> does-not-exist
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/sub-01/anat/sub-01_acq-good_T1w.nii.gz
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/sub-01/anat/sub-01_acq-nii2_T1w.nii.gz
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 miniqc-23.0.1/tests/data/bids_dataset/sub-01/anat/sub-01_acq-truncated_T2w.nii.gz
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 miniqc-23.0.1/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 miniqc-23.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 miniqc-23.0.1/README.md
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 miniqc-23.0.1/pyproject.toml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 miniqc-23.0.1/PKG-INFO
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 miniqc-23.1.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 miniqc-23.1.0/Dockerfile
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 miniqc-23.1.0/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 miniqc-23.1.0/.github/workflows/hatch.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 miniqc-23.1.0/.maint/local_gitignore
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 miniqc-23.1.0/.maint/make_gitignore
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 miniqc-23.1.0/changelog.d/20230618_155723_effigies_check_individual_files.rst
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 miniqc-23.1.0/changelog.d/20230618_162534_effigies_alpine.rst
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 miniqc-23.1.0/changelog.d/20230618_201200_effigies_consolidate.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 miniqc-23.1.0/miniqc/__init__.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 miniqc-23.1.0/miniqc/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 miniqc-23.1.0/miniqc/_version.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 miniqc-23.1.0/miniqc/_version.pyi
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 miniqc-23.1.0/miniqc/nifti.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miniqc-23.1.0/miniqc/py.typed
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 miniqc-23.1.0/miniqc/types.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 miniqc-23.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 miniqc-23.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 miniqc-23.1.0/tests/test_miniqc.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 miniqc-23.1.0/tests/test_nifti.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 miniqc-23.1.0/tests/data/bids_dataset/dataset_description.json
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 miniqc-23.1.0/tests/data/bids_dataset/sub-01/anat/sub-01_acq-dangling_T2w.nii.gz -> does-not-exist
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 miniqc-23.1.0/tests/data/bids_dataset/sub-01/anat/sub-01_acq-good_T1w.nii.gz
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 miniqc-23.1.0/tests/data/bids_dataset/sub-01/anat/sub-01_acq-nii2_T1w.nii.gz
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 miniqc-23.1.0/tests/data/bids_dataset/sub-01/anat/sub-01_acq-truncated_T2w.nii.gz
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 miniqc-23.1.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 miniqc-23.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 miniqc-23.1.0/README.md
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 miniqc-23.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 miniqc-23.1.0/PKG-INFO
```

### Comparing `miniqc-23.0.1/.github/workflows/docker.yml` & `miniqc-23.1.0/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `miniqc-23.0.1/.maint/make_gitignore` & `miniqc-23.1.0/.maint/make_gitignore`

 * *Files identical despite different names*

### Comparing `miniqc-23.0.1/miniqc/__main__.py` & `miniqc-23.1.0/miniqc/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import json
 import os
 import re
+import posixpath
 import typing as ty
 from enum import Enum
+from itertools import chain
 from pathlib import Path
 
 import nibabel as nb
 import typer
 from typing_extensions import TypeAlias
 
 from . import nifti
 from .types import CheckList, FailedCheck
 
 # Add to this list as file types are added
-SupportedType: TypeAlias = ty.Union[nb.Nifti1Image,]
+SupportedType: TypeAlias = ty.Union[
+    nb.Nifti1Image,
+]
 
 # Regex patterns paired with checklists to verify on file
 # To avoid multiple reads, only the first matching check is applied to each
 # file
 CHECKS: list[tuple[re.Pattern[str], CheckList[SupportedType]]] = [
     (re.compile(r'\.nii(\.gz)?$'), nifti.CHECKS),
 ]
@@ -40,39 +44,52 @@
     allow_dangling_links: bool = typer.Option(
         False,
         '--allow-dangling-links',
         '-l',
         help='Ignore symlinks with missing targets',
     ),
 ) -> None:
-    errors = []
-    for root, dirs, files in os.walk(bids_dir):
-        dirs[:] = [d for d in dirs if not d[0] == '.']
-        root_path = Path(root)
-        for file in files:
-            for pattern, checklist in CHECKS:
-                if re.search(pattern, file):
-                    path = root_path / file
-                    try:
-                        fileobj = checklist.loader(path)
-                        for check in checklist.checks:
-                            result, message = check(fileobj)
-                            if not result:
-                                raise FailedCheck(message or check.__doc__)
-                    except Exception as e:
-                        if not allow_dangling_links or not isinstance(
-                            e, FileNotFoundError
-                        ):
-                            errors.append(
-                                (
-                                    str(path.relative_to(bids_dir)),
-                                    type(e).__name__,
-                                    str(e),
-                                )
-                            )
-                    break
+
+    # Allow to be used on individual files
+    if not bids_dir.is_dir():
+        errors = check_file(bids_dir)
+    else:
+        errors = []
+        for root, dirs, files in os.walk(bids_dir):
+            dirs[:] = [d for d in dirs if not d[0] == '.']
+            root_path = Path(root)
+            errors.extend(
+                chain.from_iterable(check_file(root_path / file, bids_dir) for file in files)
+            )
+
+    if allow_dangling_links:
+        errors = [err for err in errors if err[1] != 'FileNotFoundError']
     print(json.dumps(errors, indent=2))
     raise typer.Exit(code=len(errors) > 0)
 
 
+def unix_format(pathlike: os.PathLike) -> str:
+    """Format any pathlike in POSIX style (forward-slashes)."""
+    return posixpath.join(*Path(pathlike).parts)
+
+
+def check_file(
+    path: Path,
+    bids_dir: ty.Optional[Path] = None,
+) -> list[tuple[str, str, str]]:
+    for pattern, checklist in CHECKS:
+        if pattern.search(path.name):
+            try:
+                fileobj = checklist.loader(path)
+                for check in checklist.checks:
+                    result, message = check(fileobj)
+                    if not result:
+                        raise FailedCheck(message or check.__doc__)
+            except Exception as e:
+                if bids_dir is not None:
+                    path = path.relative_to(bids_dir)
+                return [(unix_format(path), type(e).__name__, str(e))]
+    return []
+
+
 if __name__ == '__main__':
     app()
```

### Comparing `miniqc-23.0.1/miniqc/nifti.py` & `miniqc-23.1.0/miniqc/nifti.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     dataobj: nb.arrayproxy.ArrayProxy = img.dataobj  # type: ignore
 
     expected: int = dataobj.offset + dataobj.dtype.itemsize * prod(dataobj.shape)
 
     with dataobj._get_fileobj() as fobj:
         # Seek beyond end returns end position
         actual: int = fobj.seek(expected + 1)
-    return CheckResult(
-        (actual == expected, f'Expected {expected} bytes; found {actual}')
-    )
+    return CheckResult((actual == expected, f'Expected {expected} bytes; found {actual}'))
 
 
 CHECKS = CheckList(
     loader=load,
     checks=[
         fullsize,
     ],
```

### Comparing `miniqc-23.0.1/tests/conftest.py` & `miniqc-23.1.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,13 @@
 @pytest.fixture(scope='session')
 def good_nifti(example_dataset: Path) -> Path:
     return example_dataset / 'sub-01' / 'anat' / 'sub-01_acq-good_T1w.nii.gz'
 
 
 @pytest.fixture(scope='session')
 def truncated_nifti(example_dataset: Path) -> Path:
-    return (
-        example_dataset / 'sub-01' / 'anat' / 'sub-01_acq-truncated_T2w.nii.gz'
-    )
+    return example_dataset / 'sub-01' / 'anat' / 'sub-01_acq-truncated_T2w.nii.gz'
 
 
 @pytest.fixture(scope='session')
 def good_nifti2(example_dataset: Path) -> Path:
     return example_dataset / 'sub-01' / 'anat' / 'sub-01_acq-nii2_T1w.nii.gz'
```

### Comparing `miniqc-23.0.1/tests/test_miniqc.py` & `miniqc-23.1.0/tests/test_miniqc.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,7 +24,33 @@
         'sub-01/anat/sub-01_acq-truncated_T2w.nii.gz',
         'FailedCheck',
         'Expected 477 bytes; found 352',
     ] in errors
 
     if not allow_dangling:
         assert any([err[1] == 'FileNotFoundError' for err in errors])
+
+
+@pytest.mark.parametrize(
+    'file, allow_dangling, exit_code',
+    (
+        ('sub-01_acq-good_T1w.nii.gz', False, 0),
+        ('sub-01_acq-truncated_T2w.nii.gz', False, 1),
+        ('sub-01_acq-dangling_T2w.nii.gz', False, 1),
+        ('sub-01_acq-dangling_T2w.nii.gz', True, 0),
+    ),
+)
+def test_single_file(
+    example_dataset: Path,
+    file: str,
+    allow_dangling: bool,
+    exit_code: bool,
+) -> None:
+    args = ['-l', str(example_dataset / 'sub-01' / 'anat' / file)]
+    if not allow_dangling:
+        args = args[1:]
+
+    result = runner.invoke(app, args)
+
+    assert result.exit_code == exit_code
+    errors: list[list[str]] = json.loads(result.stdout)
+    assert len(errors) == exit_code
```

### Comparing `miniqc-23.0.1/tests/test_nifti.py` & `miniqc-23.1.0/tests/test_nifti.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,17 +21,15 @@
     # Images that are missing or lacking a NIfTI header will fail
     with pytest.raises(FileNotFoundError):
         load(example_dataset / 'does_not_exist.nii')
     with pytest.raises(nb.filebasedimages.ImageFileError):
         load(example_dataset / 'dataset_description.json')
 
 
-def test_fullsize(
-    good_nifti: Path, truncated_nifti: Path, good_nifti2: Path
-) -> None:
+def test_fullsize(good_nifti: Path, truncated_nifti: Path, good_nifti2: Path) -> None:
     # fullsize returns results if load succeeds
     good, message = fullsize(load(good_nifti))
     assert good
     good, message = fullsize(load(truncated_nifti))
     assert not good
     good, message = fullsize(load(good_nifti2))
     assert good
```

### Comparing `miniqc-23.0.1/.gitignore` & `miniqc-23.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `miniqc-23.0.1/LICENSE.txt` & `miniqc-23.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniqc-23.0.1/README.md` & `miniqc-23.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # miniQC
 
 [![PyPI - Version](https://img.shields.io/pypi/v/miniqc.svg)](https://pypi.org/project/miniqc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/miniqc.svg)](https://pypi.org/project/miniqc)
+[![GHCR - Available Tags](https://ghcr-badge.egpl.dev/OpenNeuroOrg/miniqc/tags?trim=major&label=ghcr.io&ignore=unstable,latest)](https://github.com/OpenNeuroOrg/miniqc/pkgs/container/miniqc)
 
 -----
 
 miniQC is a BIDS App for performing minimal quality control beyond validation.
 Its goal is to rapidly detect data corruption, as opposed to dataset coherence
 or image quality.
 
@@ -50,14 +51,27 @@
     "sub-01/anat/sub-01_acq-dangling_T2w.nii.gz",
     "FileNotFoundError",
     "[Errno 2] No such file or directory: 'tests/data/bids_dataset/sub-01/anat/sub-01_acq-dangling_T2w.nii.gz'"
   ]
 ]
 ```
 
+Single file usage is also permitted:
+
+```console
+$ miniqc tests/data/bids_dataset/sub-01/anat/sub-01_acq-truncated_T2w.nii.gz
+[
+  [
+    "/git/miniqc/tests/data/bids_dataset/sub-01/anat/sub-01_acq-truncated_T2w.nii.gz",
+    "FailedCheck",
+    "Expected 477 bytes; found 352"
+  ]
+]
+```
+
 ### Outputs
 
 The output of this tool is a JSON array of arrays, each of length 3.
 Each sub-array contains the failed file (relative to dataset root),
 the type of error, and a message with more detail.
 
 ## Testing
```

### Comparing `miniqc-23.0.1/pyproject.toml` & `miniqc-23.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 license = "MIT"
 keywords = []
 authors = [
   { name = "Chris Markiewicz", email = "markiewicz@stanford.edu" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
+  "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "nibabel",
@@ -77,7 +78,10 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.blue]
+line-length = 100
```

### Comparing `miniqc-23.0.1/PKG-INFO` & `miniqc-23.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: miniqc
-Version: 23.0.1
+Version: 23.1.0
 Summary: A BIDS app for performing minimal QC beyond validation
 Project-URL: Documentation, https://github.com/effigies/miniqc#readme
 Project-URL: Issues, https://github.com/effigies/miniqc/issues
 Project-URL: Source, https://github.com/effigies/miniqc
 Author-email: Chris Markiewicz <markiewicz@stanford.edu>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: nibabel
 Requires-Dist: typer
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # miniQC
 
 [![PyPI - Version](https://img.shields.io/pypi/v/miniqc.svg)](https://pypi.org/project/miniqc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/miniqc.svg)](https://pypi.org/project/miniqc)
+[![GHCR - Available Tags](https://ghcr-badge.egpl.dev/OpenNeuroOrg/miniqc/tags?trim=major&label=ghcr.io&ignore=unstable,latest)](https://github.com/OpenNeuroOrg/miniqc/pkgs/container/miniqc)
 
 -----
 
 miniQC is a BIDS App for performing minimal quality control beyond validation.
 Its goal is to rapidly detect data corruption, as opposed to dataset coherence
 or image quality.
 
@@ -71,14 +73,27 @@
     "sub-01/anat/sub-01_acq-dangling_T2w.nii.gz",
     "FileNotFoundError",
     "[Errno 2] No such file or directory: 'tests/data/bids_dataset/sub-01/anat/sub-01_acq-dangling_T2w.nii.gz'"
   ]
 ]
 ```
 
+Single file usage is also permitted:
+
+```console
+$ miniqc tests/data/bids_dataset/sub-01/anat/sub-01_acq-truncated_T2w.nii.gz
+[
+  [
+    "/git/miniqc/tests/data/bids_dataset/sub-01/anat/sub-01_acq-truncated_T2w.nii.gz",
+    "FailedCheck",
+    "Expected 477 bytes; found 352"
+  ]
+]
+```
+
 ### Outputs
 
 The output of this tool is a JSON array of arrays, each of length 3.
 Each sub-array contains the failed file (relative to dataset root),
 the type of error, and a message with more detail.
 
 ## Testing
```

