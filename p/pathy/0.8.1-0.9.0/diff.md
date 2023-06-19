# Comparing `tmp/pathy-0.8.1.tar.gz` & `tmp/pathy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathy-0.8.1.tar", last modified: Wed Nov 16 20:26:02 2022, max compression
+gzip compressed data, was "pathy-0.9.0.tar", last modified: Tue Nov 22 19:04:26 2022, max compression
```

## Comparing `pathy-0.8.1.tar` & `pathy-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 20:26:02.137315 pathy-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11345 2022-11-16 20:25:17.000000 pathy-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-11-16 20:25:17.000000 pathy-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15326 2022-11-16 20:26:02.137315 pathy-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14299 2022-11-16 20:25:17.000000 pathy-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 20:26:02.133315 pathy-0.8.1/pathy/
--rw-r--r--   0 runner    (1001) docker     (121)    42897 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 20:26:02.137315 pathy-0.8.1/pathy/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5190 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 20:26:02.137315 pathy-0.8.1/pathy/_tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/fixtures/tar_but_not_gzipped.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (121)     5987 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    10040 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_gcs.py
--rw-r--r--   0 runner    (1001) docker     (121)    22132 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_pathy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_pathy_scandir.py
--rw-r--r--   0 runner    (1001) docker     (121)     7889 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_pure_pathy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/_tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-16 20:25:32.000000 pathy-0.8.1/pathy/about.py
--rw-r--r--   0 runner    (1001) docker     (121)     7853 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/azure.py
--rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6992 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/gcs.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     8476 2022-11-16 20:25:17.000000 pathy-0.8.1/pathy/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 20:26:02.133315 pathy-0.8.1/pathy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15326 2022-11-16 20:26:02.000000 pathy-0.8.1/pathy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-11-16 20:26:02.000000 pathy-0.8.1/pathy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 20:26:02.000000 pathy-0.8.1/pathy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-16 20:26:02.000000 pathy-0.8.1/pathy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-11-16 20:26:02.000000 pathy-0.8.1/pathy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-16 20:26:02.000000 pathy-0.8.1/pathy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-16 20:25:17.000000 pathy-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-11-16 20:26:02.137315 pathy-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-11-16 20:25:17.000000 pathy-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 19:04:26.242911 pathy-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11345 2022-11-22 19:03:29.000000 pathy-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-11-22 19:03:29.000000 pathy-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    15326 2022-11-22 19:04:26.242911 pathy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14299 2022-11-22 19:03:29.000000 pathy-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 19:04:26.242911 pathy-0.9.0/pathy/
+-rw-r--r--   0 runner    (1001) docker     (121)    44507 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 19:04:26.242911 pathy-0.9.0/pathy/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5190 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 19:04:26.242911 pathy-0.9.0/pathy/_tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/fixtures/tar_but_not_gzipped.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6037 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11098 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3241 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22482 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_pathy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_pathy_scandir.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7947 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_pure_pathy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/_tests/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-22 19:03:43.000000 pathy-0.9.0/pathy/about.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7853 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/azure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6992 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     8476 2022-11-22 19:03:29.000000 pathy-0.9.0/pathy/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 19:04:26.242911 pathy-0.9.0/pathy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15326 2022-11-22 19:04:26.000000 pathy-0.9.0/pathy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      746 2022-11-22 19:04:26.000000 pathy-0.9.0/pathy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 19:04:26.000000 pathy-0.9.0/pathy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-22 19:04:26.000000 pathy-0.9.0/pathy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-11-22 19:04:26.000000 pathy-0.9.0/pathy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-22 19:04:26.000000 pathy-0.9.0/pathy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-22 19:03:29.000000 pathy-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-11-22 19:04:26.246911 pathy-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-11-22 19:03:29.000000 pathy-0.9.0/setup.py
```

### Comparing `pathy-0.8.1/LICENSE` & `pathy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/PKG-INFO` & `pathy-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathy
-Version: 0.8.1
+Version: 0.9.0
 Summary: pathlib.Path subclasses for local and cloud bucket storage
 Home-page: https://github.com/justindujardin/pathy
 Author: Justin DuJardin
 Author-email: justin@dujardinconsulting.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pathy-0.8.1/README.md` & `pathy-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/__init__.py` & `pathy-0.9.0/pathy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 StreamableType = IO[Any]
 FluidPath = Union["Pathy", "BasePath"]
 BucketType = TypeVar("BucketType")
 BucketBlobType = TypeVar("BucketBlobType")
 
 _windows_flavour: Any = _WindowsFlavour()  # type:ignore
 _posix_flavour: Any = _PosixFlavour()  # type:ignore
+_drive_letters = [(f"{chr(ord('a') + i)}:") for i in range(26)]  # lower case with :
 
 
 @dataclass
 class ClientError(BaseException):
     message: str
     code: Optional[int]
 
@@ -87,15 +88,15 @@
     raw: Optional[Blob]
 
     def __init__(
         self,
         name: str,
         is_dir: bool = False,
         size: int = -1,
-        last_modified: int = -1,
+        last_modified: Optional[int] = None,
         raw: Optional[Blob] = None,
     ):
         self.name = name
         self.raw = raw
         self._is_dir = is_dir
         self._stat = BlobStat(name=name, size=size, last_modified=last_modified)
 
@@ -220,15 +221,21 @@
 
     def owner(self, path: "Pathy") -> Optional[str]:
         blob: Optional[Blob] = self.get_blob(path)
         return blob.owner if blob is not None else None
 
     def resolve(self, path: "Pathy", strict: bool = False) -> "Pathy":
         path_parts = str(path).replace(path.drive, "")
-        return Pathy(f"{path.drive}{os.path.abspath(path_parts)}")
+        resolved = f"{path.drive}{os.path.abspath(path_parts)}"
+        # On Windows the abspath normalization that happens replaces
+        # / with \\ so we have to revert it here to preserve the
+        # expected resolved path.
+        if path.drive.lower() not in _drive_letters:
+            resolved = resolved.replace("\\", "/")
+        return Pathy(resolved)
 
     def mkdir(self, path: "Pathy", mode: int = 0) -> None:
         bucket: Optional[Bucket] = self.lookup_bucket(path)
         if bucket is None or not bucket.exists():
             self.create_bucket(path)
 
 
@@ -270,16 +277,14 @@
         few characters. In a website you would see a scheme of "http" or "https".
 
         Consider a few examples:
 
         ```python
         assert Pathy("gs://foo/bar").scheme == "gs"
         assert Pathy("file:///tmp/foo/bar").scheme == "file"
-        assert Pathy("/dev/null").scheme == ""
-
         """
         # If there is no drive, return nothing
         if self.drive == "":
             return ""
         # This is an assumption of mine. I think it's fine, but let's
         # cause an error if it's not the case.
         assert self.drive[-1] == ":", "drive should end with :"
@@ -312,14 +317,17 @@
         if not self.is_absolute():
             raise ValueError("relative paths are unsupported")
 
     @classmethod
     def _format_parsed_parts(cls, drv: str, root: str, parts: List[str]) -> str:
         # Bucket path "gs://foo/bar"
         join_fn: Callable[[List[str]], str] = cls._flavour.join  # type:ignore
+        # If the scheme is file: and it's Windows, use \\ slashes to join
+        if drv.lower() == "file:" and os.name == "nt":
+            join_fn = "\\".join
         res: str
         if drv and root:
             res = f"{drv}//{root}/" + join_fn(parts[2:])
         # Absolute path
         elif drv or root:
             res = drv + root + join_fn(parts[1:])
         else:
@@ -344,31 +352,52 @@
         )  # type:ignore
         for blob in blobs:
             stat = blob.stat()
             yield BlobStat(
                 name=str(blob.name), size=stat.size, last_modified=stat.last_modified
             )
 
+    def iterdir(self: Any) -> Generator["BasePath", None, None]:
+        """Iterate over the blobs found in the given bucket or blob prefix path."""
+        client: BucketClient = get_client(getattr(self, "scheme", "file"))
+        blobs: "ScanDirFS" = cast(
+            ScanDirFS, client.scandir(self, prefix=getattr(self, "prefix", None))
+        )  # type:ignore
+        for blob in blobs:
+            yield self / blob.name
+
 
 class BucketsAccessor:
     """Path access for python < 3.11"""
 
     def scandir(self, target: Any) -> "PathyScanDir":
         client: BucketClientFS = get_client(getattr(target, "scheme", "file"))
         return client.scandir(target, prefix=getattr(target, "prefix", None))
 
 
-class Pathy(Path, PurePathy):
+class Pathy(PurePathy, BasePath):
     """Subclass of `pathlib.Path` that works with bucket APIs."""
 
     __slots__ = ()
     _accessor: BucketsAccessor = BucketsAccessor()
     _NOT_SUPPORTED_MESSAGE = "{method} is an unsupported bucket operation"
+    _UNSUPPORTED_PATH = (
+        "absolute file paths must be initialized using Pathy.fluid(path)"
+    )
     _client: Optional[BucketClient]
 
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(**kwargs)
+        # Error when initializing paths without using Pathy.fluid if the
+        # path is an absolute system path (windows/unix)
+        root = str(self)[0]  # "/tmp/path"
+        drv = str(self)[:2].lower()  # C:\\tmp\\path
+        if root == "/" or drv in _drive_letters:
+            raise ValueError(Pathy._UNSUPPORTED_PATH)
+
     def client(self, path: "Pathy") -> BucketClient:
         return get_client(path.scheme)
 
     def __truediv__(  # type: ignore[override]
         self, key: Union[str, Path, "Pathy", PurePathy]
     ) -> "Pathy":
         return super().__truediv__(key)  # type:ignore
@@ -395,18 +424,21 @@
         fluid_path: FluidPath = Pathy.fluid("gs://my_bucket/foo.txt")
         # Narrow the type to a specific class
         assert isinstance(fluid_path, Pathy), "must be Pathy"
         # Use a member specific to that class
         assert fluid_path.prefix == "foo.txt/"
         ```
         """
-        from_path: FluidPath = Pathy(path_candidate)
-        if from_path.root in ["/", ""]:
-            from_path = BasePath(path_candidate)
-        return from_path
+        try:
+            result = Pathy(path_candidate)
+            if result.root != "":
+                return result
+        except ValueError:
+            pass
+        return BasePath(path_candidate)
 
     @classmethod
     def from_bucket(cls, bucket_name: str, scheme: str = "gs") -> "Pathy":
         """Initialize a Pathy from a bucket name. This helper adds a trailing slash and
         the appropriate prefix.
 
         ```python
@@ -477,19 +509,15 @@
         """List blob names with stat information under the given path.
 
         This is considerably faster than using iterdir if you also need
         the stat information for the enumerated blobs.
 
         Yields BlobStat objects for each found blob.
         """
-        blobs: "PathyScanDir" = self.client(self).scandir(
-            self, prefix=self.prefix
-        )  # type:ignore
-        for blob in blobs:
-            yield blob._stat
+        yield from super().ls()
 
     def stat(  # type: ignore[override]
         self: "Pathy", *, follow_symlinks: bool = True
     ) -> BlobStat:
         """Returns information about this bucket path."""
         self._absolute_path_validation()
         if not self.key:
@@ -542,27 +570,25 @@
         try:
             return bool(self.stat())
         except (ClientError, FileNotFoundError):
             return False
 
     def iterdir(self: "Pathy") -> Generator["Pathy", None, None]:
         """Iterate over the blobs found in the given bucket or blob prefix path."""
-        self._absolute_path_validation()
-        for blob in self.ls():
-            yield self / blob.name
+        yield from cast(Generator["Pathy", None, None], super().iterdir())
 
     def glob(self: "Pathy", pattern: str) -> Generator["Pathy", None, None]:
         """Perform a glob match relative to this Pathy instance, yielding all matched
         blobs."""
-        yield from super().glob(pattern)  # type:ignore
+        yield from cast(Generator["Pathy", None, None], super().glob(pattern))
 
     def rglob(self: "Pathy", pattern: str) -> Generator["Pathy", None, None]:
         """Perform a recursive glob match relative to this Pathy instance, yielding
         all matched blobs. Imagine adding "**/" before a call to glob."""
-        yield from super().rglob(pattern)  # type:ignore
+        yield from cast(Generator["Pathy", None, None], super().rglob(pattern))
 
     def open(  # type:ignore
         self: "Pathy",
         mode: str = "r",
         buffering: int = DEFAULT_BUFFER_SIZE,
         encoding: Optional[str] = None,
         errors: Optional[str] = None,
@@ -622,16 +648,14 @@
 
         If path is a blob prefix, it will replace all the blobs with the same prefix
         to match the target prefix."""
         self._absolute_path_validation()
         self_type = type(self)
         result = target if isinstance(target, self_type) else self_type(target)
         result._absolute_path_validation()  # type:ignore
-        # super().rename(result)
-        # return result
 
         client: BucketClient = self.client(self)
         bucket: Bucket = client.get_bucket(self)
         target_bucket: Bucket = client.get_bucket(result)
 
         # Single file
         if not self.is_dir():
@@ -879,16 +903,17 @@
             return None
         stat = native_blob.stat()
         # path.owner() raises KeyError if the owner's UID isn't known
         #
         # https://docs.python.org/3/library/pathlib.html#pathlib.Path.owner
         owner: Optional[str]
         try:
-            owner = native_blob.owner()
-        except KeyError:
+            # path.owner() raises NotImplementedError on windows
+            owner = native_blob.owner()  # type:ignore
+        except (KeyError, NotImplementedError):
             owner = None
         return BlobFS(
             bucket=self,
             owner=owner,
             name=blob_name,
             raw=native_blob,
             size=stat.st_size,
@@ -937,14 +962,18 @@
     def is_dir(self, path: Pathy) -> bool:
         return self.full_path(path).is_dir()
 
     def rmdir(self, path: Pathy) -> None:
         full_path = self.full_path(path)
         return shutil.rmtree(str(full_path))
 
+    def mkdir(self, path: "Pathy", mode: int = 0) -> None:
+        full_path = self.full_path(path)
+        os.makedirs(full_path, exist_ok=True)
+
     def open(
         self,
         path: Pathy,
         *,
         mode: str = "r",
         buffering: int = DEFAULT_BUFFER_SIZE,
         encoding: Optional[str] = None,
@@ -1061,15 +1090,15 @@
 
 
 class ScanDirFS(PathyScanDir):
     _client: BucketClientFS
 
     def scandir(self) -> Generator[BucketEntry, None, None]:
         scan_path = self._client.root / self._path.root
-        if isinstance(self._path, BasePath):
+        if isinstance(self._path, BasePath) and not isinstance(self._path, Pathy):
             scan_path = (
                 self._client.root / self._path.root
                 if not self._path.is_absolute()
                 else self._path
             )
         if self._prefix is not None:
             scan_path = scan_path / self._prefix
```

### Comparing `pathy-0.8.1/pathy/_tests/__init__.py` & `pathy-0.9.0/pathy/_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/_tests/conftest.py` & `pathy-0.9.0/pathy/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/_tests/fixtures/tar_but_not_gzipped.tar.gz` & `pathy-0.9.0/pathy/_tests/fixtures/tar_but_not_gzipped.tar.gz`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/_tests/test_azure.py` & `pathy-0.9.0/pathy/_tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/_tests/test_base.py` & `pathy-0.9.0/pathy/_tests/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,73 +35,73 @@
 
 def test_base_home() -> None:
     with pytest.raises(NotImplementedError):
         Pathy.home()
 
 
 def test_base_expanduser() -> None:
-    path = Pathy("/fake-bucket/fake-key")
+    path = Pathy("gs://fake-bucket/fake-key")
     with pytest.raises(NotImplementedError):
         path.expanduser()
 
 
 def test_base_chmod() -> None:
-    path = Pathy("/fake-bucket/fake-key")
+    path = Pathy("gs://fake-bucket/fake-key")
     with pytest.raises(NotImplementedError):
         path.chmod(0o666)
 
 
 def test_base_lchmod() -> None:
-    path = Pathy("/fake-bucket/fake-key")
+    path = Pathy("gs://fake-bucket/fake-key")
     with pytest.raises(NotImplementedError):
         path.lchmod(0o666)
 
 
 def test_base_group() -> None:
-    path = Pathy("/fake-bucket/fake-key")
+    path = Pathy("gs://fake-bucket/fake-key")
     with pytest.raises(NotImplementedError):
         path.group()
 
 
 def test_base_is_mount() -> None:
-    assert not Pathy("/fake-bucket/fake-key").is_mount()
+    assert not Pathy("gs://fake-bucket/fake-key").is_mount()
 
 
 def test_base_is_symlink() -> None:
-    assert not Pathy("/fake-bucket/fake-key").is_symlink()
+    assert not Pathy("gs://fake-bucket/fake-key").is_symlink()
 
 
 def test_base_is_socket() -> None:
-    assert not Pathy("/fake-bucket/fake-key").is_socket()
+    assert not Pathy("gs://fake-bucket/fake-key").is_socket()
 
 
 def test_base_is_fifo() -> None:
-    assert not Pathy("/fake-bucket/fake-key").is_fifo()
+    assert not Pathy("gs://fake-bucket/fake-key").is_fifo()
 
 
 def test_base_is_block_device() -> None:
-    path = Pathy("/fake-bucket/fake-key")
+    path = Pathy("gs://fake-bucket/fake-key")
     with pytest.raises(NotImplementedError):
         path.is_block_device()
 
 
 def test_base_is_char_device() -> None:
-    path = Pathy("/fake-bucket/fake-key")
+    path = Pathy("gs://fake-bucket/fake-key")
     with pytest.raises(NotImplementedError):
         path.is_char_device()
 
 
 def test_base_lstat() -> None:
-    path = Pathy("/fake-bucket/fake-key")
+    path = Pathy("gs://fake-bucket/fake-key")
     with pytest.raises(NotImplementedError):
         path.lstat()
 
 
 def test_base_symlink_to() -> None:
-    path = Pathy("/fake-bucket/fake-key")
+    path = Pathy("gs://fake-bucket/fake-key")
     with pytest.raises(NotImplementedError):
         path.symlink_to("file_name")
 
 
 def test_pathy_mro() -> None:
     assert PurePathy in Pathy.mro()
     assert Path in Pathy.mro()
@@ -208,9 +208,9 @@
     assert entry.is_file() is True
     entry.inode()
     assert "BucketEntry" in repr(entry)
     assert "last_modified" in repr(entry)
     assert "size" in repr(entry)
     stat = entry.stat()
     assert isinstance(stat, BlobStat)
-    assert stat.last_modified == -1
+    assert stat.last_modified is None
     assert stat.size == -1
```

### Comparing `pathy-0.8.1/pathy/_tests/test_cli.py` & `pathy-0.9.0/pathy/_tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+import shutil
 import tempfile
 
 import pytest
 from typer.testing import CliRunner
 
 from pathy import Pathy
 from pathy.cli import app
@@ -258,7 +259,38 @@
     assert str(root / "folder") in result.output
 
     result = runner.invoke(app, ["ls", "-l", str(root)])
     assert result.exit_code == 0
     assert one in result.output
     assert two in result.output
     assert str(root / "folder") in result.output
+
+
+def test_cli_ls_diff_years_modified() -> None:
+    import os
+
+    root = Pathy.fluid(tempfile.mkdtemp()) / ENV_ID / "ls_diff_year"
+    root.mkdir(parents=True, exist_ok=True)
+
+    # Create one file right now
+    new_path = root / "new_file.txt"
+    new_path.write_text("new")
+
+    # Create another and set its modified time to one year before now
+    old_path = root / "old_file.txt"
+    old_path.write_text("old")
+    old_stat = old_path.stat()
+    assert isinstance(old_stat, os.stat_result), "expect local file"
+    one_year = 31556926  # seconds
+    os.utime(
+        str(old_path), (old_stat.st_atime - one_year, old_stat.st_mtime - one_year)
+    )
+    new_old_stat = old_path.stat()
+    assert isinstance(new_old_stat, os.stat_result), "expect local file"
+    assert int(old_stat.st_mtime) == int(new_old_stat.st_mtime + one_year)
+
+    result = runner.invoke(app, ["ls", "-l", str(root)])
+    assert result.exit_code == 0
+    assert str(old_path) in result.output
+    assert str(new_path) in result.output
+
+    shutil.rmtree(str(root))
```

### Comparing `pathy-0.8.1/pathy/_tests/test_clients.py` & `pathy-0.9.0/pathy/_tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/_tests/test_file.py` & `pathy-0.9.0/pathy/_tests/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,26 @@
 
 @pytest.mark.parametrize("adapter", FS_ADAPTER)
 def test_file_bucket_client_fs_open(with_adapter: str) -> None:
     client: BucketClientFS = get_client("gs")
     blob = Pathy("gs://foo/bar")
     with pytest.raises(ClientError):
         client.open(blob)
-    blob.mkdir()
+    blob.parent.mkdir(parents=True, exist_ok=True)
     blob.touch()
     assert client.open(blob) is not None
 
 
 @pytest.mark.parametrize("adapter", FS_ADAPTER)
 def test_file_bucket_client_fs_make_uri(with_adapter: str) -> None:
     client: BucketClientFS = get_client("gs")
     blob = Pathy("gs://foo/bar")
     actual = client.make_uri(blob)
-    expected = f"file://{client.root}/foo/bar"
+    sep = client.root._flavour.sep  # type:ignore
+    expected = f"file://{client.root}{sep}foo{sep}bar"
     assert actual == expected
 
     # Invalid root
     other = Pathy("")
     with pytest.raises(ValueError):
         client.make_uri(other)
```

### Comparing `pathy-0.8.1/pathy/_tests/test_gcs.py` & `pathy-0.9.0/pathy/_tests/test_gcs.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/_tests/test_pathy.py` & `pathy-0.9.0/pathy/_tests/test_pathy.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,22 +25,32 @@
 
 @pytest.mark.parametrize("adapter", TEST_ADAPTERS)
 def test_pathy_is_path_instance(with_adapter: str) -> None:
     blob = Pathy(f"{with_adapter}://fake/blob")
     assert isinstance(blob, Path)
 
 
+def test_pathy_error_invalid_scheme_paths() -> None:
+    # Initializing a path with an absolute system path warns
+    with pytest.raises(ValueError):
+        Pathy("c:\\temp\\other\\file.txt")
+    with pytest.raises(ValueError):
+        Pathy("/tmp/other/file.txt")
+
+
 @pytest.mark.parametrize("adapter", TEST_ADAPTERS)
 def test_pathy_fluid(with_adapter: str, bucket: str) -> None:
     path: FluidPath = Pathy.fluid(f"{with_adapter}://{bucket}/{ENV_ID}/fake-key")
     assert isinstance(path, Pathy)
     path = Pathy.fluid("foo/bar.txt")
     assert isinstance(path, BasePath)
     path = Pathy.fluid("/dev/null")
     assert isinstance(path, BasePath)
+    path = Pathy.fluid("C:\\Windows\\Path")
+    assert isinstance(path, BasePath)
 
 
 @pytest.mark.parametrize("adapter", TEST_ADAPTERS)
 def test_pathy_path_to_local(with_adapter: str, bucket: str) -> None:
     root: Pathy = Pathy(f"{with_adapter}://{bucket}/{ENV_ID}/to_local")
     foo_blob: Pathy = root / "foo"
     foo_blob.write_text("---")
```

### Comparing `pathy-0.8.1/pathy/_tests/test_pathy_scandir.py` & `pathy-0.9.0/pathy/_tests/test_pathy_scandir.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/_tests/test_pure_pathy.py` & `pathy-0.9.0/pathy/_tests/test_pure_pathy.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 
 def test_pure_pathy_scheme_extraction() -> None:
     assert PurePathy("gs://var/tests/fake").scheme == "gs"
     assert PurePathy("s3://var/tests/fake").scheme == "s3"
     assert PurePathy("file://var/tests/fake").scheme == "file"
     assert PurePathy("/var/tests/fake").scheme == ""
+    assert PurePathy("C:\\pathy\\subfolder").scheme == ""
 
 
 @pytest.mark.skipif(sys.version_info < (3, 6), reason="requires python3.6 or higher")
 def test_pure_pathy_fspath() -> None:
     assert os.fspath(PurePathy("/var/tests/fake")) == "/var/tests/fake"
```

### Comparing `pathy-0.8.1/pathy/_tests/test_s3.py` & `pathy-0.9.0/pathy/_tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/azure.py` & `pathy-0.9.0/pathy/azure.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/cli.py` & `pathy-0.9.0/pathy/cli.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/gcs.py` & `pathy-0.9.0/pathy/gcs.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy/s3.py` & `pathy-0.9.0/pathy/s3.py`

 * *Files identical despite different names*

### Comparing `pathy-0.8.1/pathy.egg-info/PKG-INFO` & `pathy-0.9.0/pathy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathy
-Version: 0.8.1
+Version: 0.9.0
 Summary: pathlib.Path subclasses for local and cloud bucket storage
 Home-page: https://github.com/justindujardin/pathy
 Author: Justin DuJardin
 Author-email: justin@dujardinconsulting.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pathy-0.8.1/pathy.egg-info/SOURCES.txt` & `pathy-0.9.0/pathy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 pathy/_tests/test_clients.py
 pathy/_tests/test_file.py
 pathy/_tests/test_gcs.py
 pathy/_tests/test_pathy.py
 pathy/_tests/test_pathy_scandir.py
 pathy/_tests/test_pure_pathy.py
 pathy/_tests/test_s3.py
+pathy/_tests/test_windows.py
 pathy/_tests/fixtures/tar_but_not_gzipped.tar.gz
```

### Comparing `pathy-0.8.1/setup.py` & `pathy-0.9.0/setup.py`

 * *Files identical despite different names*

