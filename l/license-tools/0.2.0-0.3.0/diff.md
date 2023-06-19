# Comparing `tmp/license_tools-0.2.0.tar.gz` & `tmp/license_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_tools-0.2.0.tar", last modified: Thu Jun 15 07:57:33 2023, max compression
+gzip compressed data, was "license_tools-0.3.0.tar", last modified: Mon Jun 19 10:45:23 2023, max compression
```

## Comparing `license_tools-0.2.0.tar` & `license_tools-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-15 07:57:33.391027 license_tools-0.2.0/
--rw-r--r--   0 sdostal   (6000) users      (100)    11358 2022-05-16 19:23:11.000000 license_tools-0.2.0/LICENSE.txt
--rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-15 07:57:33.391027 license_tools-0.2.0/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)     1618 2023-06-15 07:55:19.000000 license_tools-0.2.0/README.md
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-15 07:57:33.391027 license_tools-0.2.0/license_tools/
--rw-r--r--   0 sdostal   (6000) users      (100)        0 2021-01-11 15:34:09.000000 license_tools-0.2.0/license_tools/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     2427 2023-06-14 10:37:12.000000 license_tools-0.2.0/license_tools/__main__.py
--rw-r--r--   0 sdostal   (6000) users      (100)    16055 2023-06-15 07:53:43.000000 license_tools-0.2.0/license_tools/scancode_tools.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-15 07:57:33.391027 license_tools-0.2.0/license_tools.egg-info/
--rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)      298 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/SOURCES.txt
--rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/dependency_links.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       68 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/requires.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       14 2023-06-15 07:57:33.000000 license_tools-0.2.0/license_tools.egg-info/top_level.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       38 2023-06-15 07:57:33.391027 license_tools-0.2.0/setup.cfg
--rw-r--r--   0 sdostal   (6000) users      (100)     1423 2023-06-15 07:54:48.000000 license_tools-0.2.0/setup.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-19 10:45:23.917663 license_tools-0.3.0/
+-rw-r--r--   0 sdostal   (6000) users      (100)    11358 2022-05-16 19:23:11.000000 license_tools-0.3.0/LICENSE.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-19 10:45:23.917663 license_tools-0.3.0/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)     1618 2023-06-15 07:55:19.000000 license_tools-0.3.0/README.md
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-19 10:45:23.917663 license_tools-0.3.0/license_tools/
+-rw-r--r--   0 sdostal   (6000) users      (100)        0 2021-01-11 15:34:09.000000 license_tools-0.3.0/license_tools/__init__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)     2569 2023-06-15 12:33:41.000000 license_tools-0.3.0/license_tools/__main__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)    16453 2023-06-19 10:44:27.000000 license_tools-0.3.0/license_tools/scancode_tools.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-06-19 10:45:23.917663 license_tools-0.3.0/license_tools.egg-info/
+-rw-r--r--   0 sdostal   (6000) users      (100)     2397 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)      298 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       68 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/requires.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       14 2023-06-19 10:45:23.000000 license_tools-0.3.0/license_tools.egg-info/top_level.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       38 2023-06-19 10:45:23.917663 license_tools-0.3.0/setup.cfg
+-rw-r--r--   0 sdostal   (6000) users      (100)     1423 2023-06-16 09:52:25.000000 license_tools-0.3.0/setup.py
```

### Comparing `license_tools-0.2.0/LICENSE.txt` & `license_tools-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `license_tools-0.2.0/PKG-INFO` & `license_tools-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license_tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Collection of tools for working with Open Source licenses
 Home-page: https://github.com/stefan6419846/license_tools
 Author: stefan6419846
 License: Apache-2.0
 Keywords: open source,license,package,dependency,licensing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `license_tools-0.2.0/README.md` & `license_tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `license_tools-0.2.0/license_tools/__main__.py` & `license_tools-0.3.0/license_tools/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         description='Run selected license tools. Will determine all license from the given source by default.',
     )
 
     source_group = parser.add_argument_group('Artifact source')
     source_group = source_group.add_mutually_exclusive_group(required=False)
     source_group.add_argument('--directory', action='store', type=str, help='Directory to work on.')
     source_group.add_argument('--file', action='store', type=str, help='File to work on.')
+    source_group.add_argument('--archive', action='store', type=str, help='Archive file to work on.')
     source_group.add_argument('--package', action='store', type=str, help='Package specification to use.')
 
     parser.add_argument(
         '--index-url', action='store', type=str, required=False, default='', help='PyPI index URL to use.'
     )
     parser.add_argument(
         '--jobs', action='store', type=int, required=False, default=4, help='Parallel jobs to use.'
@@ -44,14 +45,15 @@
     )
 
     arguments = parser.parse_args()
 
     scancode_tools.run(
         directory=arguments.directory,
         file_path=arguments.file,
+        archive_path=arguments.archive,
         package_definition=arguments.package,
         index_url=arguments.index_url,
         job_count=arguments.jobs,
         retrieve_copyrights=arguments.retrieve_copyrights,
         retrieve_emails=arguments.retrieve_emails,
         retrieve_file_info=arguments.retrieve_file_info,
         retrieve_urls=arguments.retrieve_urls,
```

### Comparing `license_tools-0.2.0/license_tools/scancode_tools.py` & `license_tools-0.3.0/license_tools/scancode_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -241,14 +241,80 @@
             self.urls = Urls(**api.get_urls(path_str))
         if self.retrieve_licenses:
             self.licenses = Licenses(**api.get_licenses(path_str))
         if self.retrieve_file_info:
             self.file_info = FileInfo(**api.get_file_info(path_str))
 
 
+class RetrievalFlags:
+    """
+    Data retrieval flags to get shorter parameter lists.
+    """
+
+    COPYRIGHTS = 1
+    EMAILS = 2
+    FILE_INFO = 4
+    URLS = 8
+    LDD_DATA = 16
+
+    @classmethod
+    def to_int(
+            cls,
+            retrieve_copyrights: bool = False,
+            retrieve_emails: bool = False,
+            retrieve_file_info: bool = False,
+            retrieve_urls: bool = False,
+            retrieve_ldd_data: bool = False,
+    ) -> int:
+        """
+        Convert the given boolean parameter values to a single integer flag value.
+
+        :param retrieve_copyrights: Whether to retrieve copyright information.
+        :param retrieve_emails: Whether to retrieve e-mails.
+        :param retrieve_file_info: Whether to retrieve file-specific information.
+        :param retrieve_urls: Whether to retrieve URLs.
+        :param retrieve_ldd_data: Whether to retrieve linking data for shared objects.
+        :return: The flags derived from the given parameters.
+        """
+        return (
+            cls.COPYRIGHTS * retrieve_copyrights +
+            cls.EMAILS * retrieve_emails +
+            cls.FILE_INFO * retrieve_file_info +
+            cls.URLS * retrieve_urls +
+            cls.LDD_DATA * retrieve_ldd_data
+        )
+
+    @classmethod
+    def is_set(cls, flags: int, flag: int) -> bool:
+        """
+        Check if the given flag is set.
+
+        :param flags: The flags to check inside.
+        :param flag: The flag value to check for.
+        :return: The check result.
+        """
+        return bool(flags & flag)
+
+    @classmethod
+    def to_kwargs(cls, flags: int) -> dict[str, bool]:
+        """
+        Convert the given flags to keyword arguments.
+
+        :param flags: The flags to convert.
+        :return: The associated keyword arguments.
+        """
+        return dict(
+            retrieve_copyrights=cls.is_set(flags=flags, flag=cls.COPYRIGHTS),
+            retrieve_emails=cls.is_set(flags=flags, flag=cls.EMAILS),
+            retrieve_file_info=cls.is_set(flags=flags, flag=cls.FILE_INFO),
+            retrieve_urls=cls.is_set(flags=flags, flag=cls.URLS),
+            retrieve_ldd_data=cls.is_set(flags=flags, flag=cls.LDD_DATA),
+        )
+
+
 def check_shared_objects(path: Path) -> str | None:
     """
     Check which other shared objects a shared object links to.
 
     :param path: The file path to analyze.
     :return: The analysis results if the path points to a shared object, `None` otherwise.
     """
@@ -257,177 +323,134 @@
     output = subprocess.check_output(['ldd', path], stderr=subprocess.PIPE)
     return output.decode('UTF-8')
 
 
 def run_on_file(
         path: Path,
         short_path: str,
-        retrieve_copyrights: bool = False,
-        retrieve_emails: bool = False,
-        retrieve_file_info: bool = False,
-        retrieve_urls: bool = False,
-        retrieve_ldd_data: bool = False,
+        retrieval_flags: int = 0,
 ) -> FileResults:
     """
     Run the analysis on the given file.
 
     :param path: The file path to analyze.
     :param short_path: The short path to use for display.
-    :param retrieve_copyrights: Whether to retrieve copyright information.
-    :param retrieve_emails: Whether to retrieve e-mails.
-    :param retrieve_file_info: Whether to retrieve file-specific information.
-    :param retrieve_urls: Whether to retrieve URLs.
-    :param retrieve_ldd_data: Whether to retrieve linking data for shared objects.
+    :param retrieval_flags: Values to retrieve.
     :return: The requested results.
     """
+    retrieval_kwargs = RetrievalFlags.to_kwargs(flags=retrieval_flags)
+
     # This data is not yet part of the dataclasses above, as it is a custom analysis.
-    if retrieve_ldd_data:
+    if retrieval_kwargs.pop('retrieve_ldd_data'):
         results = check_shared_objects(path=path)
         if results:
             print(short_path + '\n' + results)
 
     # Register this here as each parallel process has its own directory.
     atexit.register(cleanup, scancode_config.scancode_temp_dir)
 
     return FileResults(
         path=path,
         short_path=short_path,
-        retrieve_copyrights=retrieve_copyrights,
-        retrieve_emails=retrieve_emails,
-        retrieve_file_info=retrieve_file_info,
-        retrieve_urls=retrieve_urls,
         retrieve_licenses=True,
+        **retrieval_kwargs
     )
 
 
 def run_on_directory(
         directory: str,
         job_count: int = 4,
-        retrieve_copyrights: bool = False,
-        retrieve_emails: bool = False,
-        retrieve_file_info: bool = False,
-        retrieve_urls: bool = False,
-        retrieve_ldd_data: bool = False,
+        retrieval_flags: int = 0,
 ) -> Generator[FileResults, None, None]:
     """
     Run the analysis on the given directory.
 
     :param path: The directory to analyze.
     :param job_count: The number of parallel jobs to use.
-    :param retrieve_copyrights: Whether to retrieve copyright information.
-    :param retrieve_emails: Whether to retrieve e-mails.
-    :param retrieve_file_info: Whether to retrieve file-specific information.
-    :param retrieve_urls: Whether to retrieve URLs.
-    :param retrieve_ldd_data: Whether to retrieve linking data for shared objects.
+    :param retrieval_flags: Values to retrieve.
     :return: The requested results per file.
     """
     common_prefix_length = len(directory) + int(not directory.endswith("/"))
 
     def get_paths() -> tuple[Path, str]:
         for path in sorted(Path(directory).rglob("*"), key=str):
             if path.is_dir():
                 continue
             distribution_path = str(path)[common_prefix_length:]
             yield path, distribution_path
 
     results = Parallel(n_jobs=job_count)(
         delayed(run_on_file)(
-            path,
-            short_path,
-            retrieve_copyrights,
-            retrieve_emails,
-            retrieve_file_info,
-            retrieve_urls,
-            retrieve_ldd_data,
+            path=path,
+            short_path=short_path,
+            retrieval_flags=retrieval_flags,
         ) for path, short_path in get_paths()
     )
     yield from results
 
 
 def run_on_package_archive_file(
         archive_path: Path,
         job_count: int = 4,
-        retrieve_copyrights: bool = False,
-        retrieve_emails: bool = False,
-        retrieve_file_info: bool = False,
-        retrieve_urls: bool = False,
-        retrieve_ldd_data: bool = False,
+        retrieval_flags: int = 0,
 ) -> Generator[FileResults, None, None]:
     """
     Run the analysis on the given package archive file.
 
     :param path: The package archive path to analyze.
     :param job_count: The number of parallel jobs to use.
-    :param retrieve_copyrights: Whether to retrieve copyright information.
-    :param retrieve_emails: Whether to retrieve e-mails.
-    :param retrieve_file_info: Whether to retrieve file-specific information.
-    :param retrieve_urls: Whether to retrieve URLs.
-    :param retrieve_ldd_data: Whether to retrieve linking data for shared objects.
+    :param retrieval_flags: Values to retrieve.
     :return: The requested results.
     """
     with TemporaryDirectory() as working_directory:
         if archive_path.suffix == ".whl":
             # `shutil.unpack_archive` cannot handle wheel files.
             with zipfile.ZipFile(archive_path, "r") as zip_file:
                 zip_file.extractall(working_directory)
         else:
             shutil.unpack_archive(archive_path, working_directory)
         yield from run_on_directory(
             directory=working_directory,
             job_count=job_count,
-            retrieve_copyrights=retrieve_copyrights,
-            retrieve_emails=retrieve_emails,
-            retrieve_file_info=retrieve_file_info,
-            retrieve_urls=retrieve_urls,
+            retrieval_flags=retrieval_flags,
         )
 
 
 def run_on_downloaded_package_file(
         package_definition: str,
         index_url: str | None = None,
         job_count: int = 4,
-        retrieve_copyrights: bool = False,
-        retrieve_emails: bool = False,
-        retrieve_file_info: bool = False,
-        retrieve_urls: bool = False,
-        retrieve_ldd_data: bool = False,
+        retrieval_flags: int = 0,
 ) -> Generator[FileResults, None, None]:
     """
     Run the analysis for the given package definition.
 
     :param package_definition: The package definition to get the files for.
     :param index_url: The PyPI index URL to use. Uses the default one from the `.pypirc` file if unset.
     :param job_count: The number of parallel jobs to use.
-    :param retrieve_copyrights: Whether to retrieve copyright information.
-    :param retrieve_emails: Whether to retrieve e-mails.
-    :param retrieve_file_info: Whether to retrieve file-specific information.
-    :param retrieve_urls: Whether to retrieve URLs.
-    :param retrieve_ldd_data: Whether to retrieve linking data for shared objects.
+    :param retrieval_flags: Values to retrieve.
     :return: The requested results.
     """
     with TemporaryDirectory() as download_directory:
         command = [
             "pip",
             "download",
             "--no-deps",
             package_definition,
             "--dest",
             download_directory,
         ]
         if index_url:
             command += ["--index-url", index_url]
-        subprocess.check_output(command, stderr=subprocess.PIPE)
+        subprocess.check_output(command)
         name = list(Path(download_directory).glob("*"))[0]
         yield from run_on_package_archive_file(
             archive_path=name.resolve(),
             job_count=job_count,
-            retrieve_copyrights=retrieve_copyrights,
-            retrieve_emails=retrieve_emails,
-            retrieve_file_info=retrieve_file_info,
-            retrieve_urls=retrieve_urls,
+            retrieval_flags=retrieval_flags,
         )
 
 
 def _check_that_exactly_one_value_is_set(values: list[Path | str | None]) -> bool:
     """
     Check that exactly one value does not evaluate to `False`.
     """
@@ -441,79 +464,91 @@
     """
     fileutils.delete(directory)
 
 
 def run(
         directory: Path | str | None = None,
         file_path: Path | str | None = None,
+        archive_path: Path | str | None = None,
         package_definition: str | None = None,
         index_url: str | None = None,
         job_count: int = 4,
         retrieve_copyrights: bool = False,
         retrieve_emails: bool = False,
         retrieve_file_info: bool = False,
         retrieve_urls: bool = False,
         retrieve_ldd_data: bool = False,
 ) -> FileResults:
     """
     Run the analysis for the given input definition.
 
-    The `directory`, `file_path` and `package_definition` parameters are mutually exclusive,
+    The `directory`, `file_path`, `archive_path` and `package_definition` parameters are mutually exclusive,
     but exactly one has to be set.
 
     :param directory: The directory to run on.
     :param file_path: The file to run on.
+    :param archive_path: The package archive to run on.
     :param package_definition: The package definition to run for.
     :param index_url: The PyPI index URL to use. Uses the default one from the `.pypirc` file if unset.
     :param job_count: The number of parallel jobs to use.
     :param retrieve_copyrights: Whether to retrieve copyright information.
     :param retrieve_emails: Whether to retrieve e-mails.
     :param retrieve_file_info: Whether to retrieve file-specific information.
     :param retrieve_urls: Whether to retrieve URLs.
     :param retrieve_ldd_data: Whether to retrieve linking data for shared objects.
     :return: The requested results.
     """
     # Remove the temporary directory of the main thread.
     atexit.register(cleanup, scancode_config.scancode_temp_dir)
 
-    assert _check_that_exactly_one_value_is_set([directory, file_path, package_definition]), 'Exactly one source is required.'
+    assert _check_that_exactly_one_value_is_set(
+        [directory, file_path, archive_path, package_definition]
+    ), 'Exactly one source is required.'
 
     license_counts = defaultdict(int)
-    kwargs = dict(
+    retrieval_flags = RetrievalFlags.to_int(
         retrieve_copyrights=retrieve_copyrights,
         retrieve_emails=retrieve_emails,
         retrieve_file_info=retrieve_file_info,
         retrieve_urls=retrieve_urls,
         retrieve_ldd_data=retrieve_ldd_data,
-        job_count=job_count,
     )
 
     # Run the analysis itself.
     if package_definition:
         results = list(
             run_on_downloaded_package_file(
                 package_definition=package_definition,
                 index_url=index_url,
-                **kwargs
+                retrieval_flags=retrieval_flags,
+                job_count=job_count,
             )
         )
     elif directory:
         results = list(
             run_on_directory(
                 directory=directory,
-                **kwargs
+                retrieval_flags=retrieval_flags,
+                job_count=job_count,
+            )
+        )
+    elif archive_path:
+        results = list(
+            run_on_package_archive_file(
+                archive_path=Path(archive_path),
+                retrieval_flags=retrieval_flags,
+                job_count=job_count,
             )
         )
     elif file_path:
-        kwargs.pop('job_count')
         results = [
             run_on_file(
-                path=file_path,
+                path=Path(file_path),
                 short_path=file_path,
-                **kwargs
+                retrieval_flags=retrieval_flags,
             )
         ]
 
     # Display the file-level results.
     for result in results:
         scores = result.licenses.get_scores_of_detected_license_expression_spdx()
         print(
```

### Comparing `license_tools-0.2.0/license_tools.egg-info/PKG-INFO` & `license_tools-0.3.0/license_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Collection of tools for working with Open Source licenses
 Home-page: https://github.com/stefan6419846/license_tools
 Author: stefan6419846
 License: Apache-2.0
 Keywords: open source,license,package,dependency,licensing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `license_tools-0.2.0/setup.py` & `license_tools-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ROOT_DIRECTORY = Path(__file__).parent.resolve()
 
 
 setuptools.setup(
     name='license_tools',
     description='Collection of tools for working with Open Source licenses',
-    version='0.2.0',
+    version='0.3.0',
     license='Apache-2.0',
     long_description=Path(ROOT_DIRECTORY / 'README.md').read_text(encoding='UTF-8'),
     long_description_content_type='text/markdown',
     author='stefan6419846',
     url='https://github.com/stefan6419846/license_tools',
     packages=setuptools.find_packages(),
     include_package_data=True,
```

