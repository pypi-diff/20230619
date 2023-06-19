# Comparing `tmp/mizue-0.2.9.tar.gz` & `tmp/mizue-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizue-0.2.9.tar", last modified: Sun Jun 18 18:09:46 2023, max compression
+gzip compressed data, was "mizue-0.3.0.tar", last modified: Mon Jun 19 13:12:15 2023, max compression
```

## Comparing `mizue-0.2.9.tar` & `mizue-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.998993 mizue-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-18 18:09:26.000000 mizue-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 18:09:45.994994 mizue-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 18:09:26.000000 mizue-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/file/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/file/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/network/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/network/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/network/downloader/data/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/download_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/download_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/downloader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/progress_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/printer/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/printer/grid/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/border_character_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/border_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/cell_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/row_border_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/terminal_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/colorful_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/progress_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/util/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:09:45.998993 mizue-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-18 18:09:45.000000 mizue-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.480823 mizue-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-19 13:11:54.000000 mizue-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-19 13:12:15.480823 mizue-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-19 13:11:54.000000 mizue-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.476822 mizue-0.3.0/mizue/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.476822 mizue-0.3.0/mizue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/file/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.476822 mizue-0.3.0/mizue/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.476822 mizue-0.3.0/mizue/network/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/network/downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.476822 mizue-0.3.0/mizue/network/downloader/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/network/downloader/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/network/downloader/download_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/network/downloader/download_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/network/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/network/downloader/downloader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/network/downloader/progress_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.476822 mizue-0.3.0/mizue/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.480823 mizue-0.3.0/mizue/printer/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/grid/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/grid/border_character_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/grid/border_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/grid/cell_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/grid/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/grid/column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/grid/row_border_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/printer/terminal_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.480823 mizue-0.3.0/mizue/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/progress/colorful_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/progress/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/progress/progress_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/progress/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.480823 mizue-0.3.0/mizue/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/util/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/util/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/util/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-19 13:11:54.000000 mizue-0.3.0/mizue/util/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:15.476822 mizue-0.3.0/mizue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-19 13:12:15.000000 mizue-0.3.0/mizue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-19 13:12:15.000000 mizue-0.3.0/mizue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:12:15.000000 mizue-0.3.0/mizue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:12:15.000000 mizue-0.3.0/mizue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 13:12:15.000000 mizue-0.3.0/mizue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 13:12:15.480823 mizue-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-19 13:12:13.000000 mizue-0.3.0/setup.py
```

### Comparing `mizue-0.2.9/LICENSE` & `mizue-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/PKG-INFO` & `mizue-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.2.9/README.md` & `mizue-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/file/fileutils.py` & `mizue-0.3.0/mizue/file/fileutils.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/network/downloader/data/colors.json` & `mizue-0.3.0/mizue/network/downloader/data/colors.json`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/network/downloader/download_event.py` & `mizue-0.3.0/mizue/network/downloader/download_event.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/network/downloader/downloader.py` & `mizue-0.3.0/mizue/network/downloader/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     ProgressEventArgs
 from .download_metadata import DownloadMetadata
 from .progress_data import ProgressData
 
 
 class Downloader(EventListener):
     def __init__(self):
+        super().__init__()
         self._alive = True
 
         self.output_path = "."
         """The output path for the downloaded files"""
 
         self.retry_count = 5
         """The number of times to retry the download if it fails"""
@@ -131,19 +132,20 @@
     def _get_filename(response: requests.Response) -> str | None:
         content_disposition = response.headers.get('content-disposition')
         if content_disposition:
             filename = content_disposition.split("filename=")[1].split(";")[0].replace("\"", "").strip()
             if filename:
                 return filename
         else:
-            unquoted_filename = urllib.parse.unquote(response.url.split("/")[-1], encoding='utf-8', errors='replace')
-            if unquoted_filename and "?" in unquoted_filename:
-                unquoted_filename = unquoted_filename[:unquoted_filename.rfind("?")]
-            if unquoted_filename:
-                return sanitize_filename(unquoted_filename)
+            unquoted_url = urllib.parse.unquote_plus(response.url, encoding='utf-8', errors='replace')
+            unquoted_url = unquoted_url.replace("?", "_")
+            url_filename = urllib.parse.urlparse(unquoted_url)
+            filename = os.path.basename(url_filename.path)
+            if filename:
+                return sanitize_filename(filename)
         return None
 
     def _get_response(self, url: str) -> requests.Response | None:
         fetching = True
         fetch_try_count = 0
         headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
```

### Comparing `mizue-0.2.9/mizue/network/downloader/downloader_tool.py` & `mizue-0.3.0/mizue/network/downloader/downloader_tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,30 +7,38 @@
 from mizue.file import FileUtils
 from mizue.network.downloader import DownloadStartEvent, ProgressEventArgs, DownloadCompleteEvent, Downloader, \
     DownloadEventType, DownloadFailureEvent
 from mizue.printer import Printer
 from mizue.printer.grid import ColumnSettings, Alignment, Grid, BorderStyle, CellRendererArgs
 from mizue.progress import LabelRendererArgs, \
     InfoSeparatorRendererArgs, InfoTextRendererArgs, ColorfulProgress
+from mizue.util import EventListener
 
 
 @dataclass
 class _DownloadReport:
     filename: str
     filesize: int
     url: str
 
 
-class DownloaderTool:
+class DownloaderTool(EventListener):
     def __init__(self):
+        super().__init__()
         self._file_color_scheme = {}
         self._report_data: list[_DownloadReport] = []
         self._bulk_download_size = 0
         self._downloaded_count = 0
         self._total_download_count = 0
+        self._success_count = 0  # For bulk downloads
+        self._failure_count = 0  # For bulk downloads
+
+        self.display_report = True
+        """Whether to display the download report after the download is complete"""
+
         self.progress: ColorfulProgress | None = None
         self._load_color_scheme()
 
     def download(self, url: str, output_path: str):
         """
         Download a file to a specified directory
         :param url: The URL to download
@@ -48,15 +56,17 @@
         except KeyboardInterrupt:
             downloader.close()
             self.progress.stop()
             Printer.warning(f"{os.linesep}Keyboard interrupt detected. Cleaning up...")
             if len(filepath) > 0:
                 os.remove(filepath[0])
             self._report_data.append(_DownloadReport(url, 0, url))
-        self._print_report()
+        
+        if self.display_report:
+            self._print_report()
 
     def download_bulk(self, urls: list[str] | list[tuple[str, str]], output_path: str | None = None, parallel: int = 4):
         """
         Download a list of files to a specified directory or a list of [url, output_path] tuples.
 
         If the urls parameter is a list of [url, output_path] tuples, every url will be downloaded to its corresponding
         output_path.
@@ -92,14 +102,17 @@
         """
 
         self.progress = ColorfulProgress(start=0, end=len(urls), value=0)
         self._configure_progress()
         self.progress.start()
         self._downloaded_count = 0
         self._total_download_count = len(urls)
+        self._report_data = []
+        self._success_count = 0
+        self._failure_count = 0
         download_dict = {}
 
         with concurrent.futures.ThreadPoolExecutor(max_workers=parallel) as executor:
             try:
                 responses: list[concurrent.futures.Future] = []
                 downloader = Downloader()
                 downloader.add_event(DownloadEventType.PROGRESS,
@@ -116,15 +129,16 @@
                 executor.shutdown(wait=True)
             except KeyboardInterrupt:
                 downloader.close()
                 self.progress.stop()
                 Printer.warning(f"{os.linesep}Keyboard interrupt detected. Cleaning up...")
                 executor.shutdown(wait=False, cancel_futures=True)
         self.progress.stop()
-        self._print_report()
+        if self.display_report:
+            self._print_report()
 
     def _configure_progress(self):
         self.progress.info_separator_renderer = self._info_separator_renderer
         self.progress.info_text_renderer = self._info_text_renderer
         self.progress.label_renderer = self._label_renderer
         self.progress.label = "Downloading: "
 
@@ -137,70 +151,85 @@
         size_text = FileUtils.get_readable_file_size(sum(download_dict.values()))
         return f'{file_progress_text} ⟪{size_text}⟫'
 
     @staticmethod
     def _info_separator_renderer(args: InfoSeparatorRendererArgs):
         return ColorfulProgress.get_basic_colored_text(" | ", args.percentage)
 
-    @staticmethod
-    def _info_text_renderer(args: InfoTextRendererArgs):
-        # return Printer.format_hex(args.text, '#FFCC75')
-        return DownloaderTool._get_basic_colored_text(args.text, args.percentage)
+    def _info_text_renderer(self, args: InfoTextRendererArgs):
+        info_text = DownloaderTool._get_basic_colored_text(args.text, args.percentage)
+        separator = ColorfulProgress.get_basic_colored_text(" | ", args.percentage)
+        successful_text = Printer.format_hex(f'{self._success_count}', '#0EB33B')
+        failed_text = Printer.format_hex(f'{self._failure_count}', '#FF0000')
+        status_text = str.format("{}{}{}{}{}",
+                                 ColorfulProgress.get_basic_colored_text("⟪", args.percentage),
+                                 successful_text,
+                                 ColorfulProgress.get_basic_colored_text("/", args.percentage),
+                                 failed_text,
+                                 ColorfulProgress.get_basic_colored_text("⟫", args.percentage))
+        full_info_text = str.format("{}{}{}", info_text, separator, status_text)
+        return full_info_text
 
     @staticmethod
     def _label_renderer(args: LabelRendererArgs):
         if args.percentage < 100:
             return Printer.format_hex(args.label, '#FFCC75')
         return Printer.format_hex('Downloaded: ', '#0EB33B')
 
     def _load_color_scheme(self):
         file_path = os.path.join(os.path.dirname(__file__), "data", "colors.json")
         with open(file_path, "r") as f:
             self._file_color_scheme = json.load(f)
 
     def _on_bulk_download_complete(self, event: DownloadCompleteEvent):
         self._report_data.append(_DownloadReport(event.filename, event.filesize, event.url))
+        self._success_count += 1
 
     def _on_bulk_download_failed(self, event: DownloadFailureEvent):
         self._report_data.append(_DownloadReport("", 0, event.url))
+        self._failure_count += 1
 
     def _on_bulk_download_progress(self, event: ProgressEventArgs, download_dict: dict):
         download_dict[event.url] = event.downloaded
         self.progress.info_text = self._get_bulk_progress_info(download_dict)
 
     def _on_download_complete(self, event: DownloadCompleteEvent):
         self.progress.update_value(event.filesize)
         downloaded_info = FileUtils.get_readable_file_size(event.filesize)
         filesize_info = FileUtils.get_readable_file_size(event.filesize)
         info = f'[{downloaded_info}/{filesize_info}]'
         self.progress.info_text = info
         time.sleep(0.5)
         self.progress.stop()
         self._report_data.append(_DownloadReport(event.filename, event.filesize, event.url))
+        self._fire_event(DownloadEventType.COMPLETED, event)
 
     def _on_download_failure(self, event: DownloadFailureEvent):
         if isinstance(event.exception, KeyboardInterrupt):
             Printer.warning("Download has been cancelled by user.")
             print(os.linesep)
         if self.progress:
             self.progress.terminate()
         self._report_data.append(_DownloadReport("", 0, event.url))
+        self._fire_event(DownloadEventType.FAILED, event)
 
     def _on_download_progress(self, event: ProgressEventArgs):
         self.progress.update_value(event.downloaded)
         downloaded_info = FileUtils.get_readable_file_size(event.downloaded)
         filesize_info = FileUtils.get_readable_file_size(event.filesize)
         info = f'[{downloaded_info}/{filesize_info}]'
         self.progress.info_text = info
+        self._fire_event(DownloadEventType.PROGRESS, event)
 
     def _on_download_start(self, event: DownloadStartEvent, filepath: list[str]):
         self.progress = ColorfulProgress(start=0, end=event.filesize, value=0)
         self._configure_progress()
         self.progress.start()
         filepath.append(event.filepath)
+        self._fire_event(DownloadEventType.STARTED, event)
 
     def _print_report(self):
         success_data = [report for report in self._report_data if report.filesize > 0]
         failed_data = [report for report in self._report_data if report.filesize == 0]
         row_index = 1
         success_grid_data = []
         for report in success_data:
```

### Comparing `mizue-0.2.9/mizue/printer/grid/border_character_codes.py` & `mizue-0.3.0/mizue/printer/grid/border_character_codes.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/printer/grid/column.py` & `mizue-0.3.0/mizue/printer/grid/column.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/printer/grid/grid.py` & `mizue-0.3.0/mizue/printer/grid/grid.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/printer/printer.py` & `mizue-0.3.0/mizue/printer/printer.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/progress/colorful_progress.py` & `mizue-0.3.0/mizue/progress/colorful_progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/progress/progress.py` & `mizue-0.3.0/mizue/progress/progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/progress/progress_renderer_args.py` & `mizue-0.3.0/mizue/progress/progress_renderer_args.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/progress/spinner.py` & `mizue-0.3.0/mizue/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/util/event_listener.py` & `mizue-0.3.0/mizue/util/event_listener.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from abc import ABC
 
 
 class EventListener(ABC):
     """Abstract class for event listeners"""
-    _event_id_counter: int = 0
-    _events: dict[str, list[callable]] = {}
-    _event_id_map: dict[int, [str, callable]] = {}
+    def __init__(self):
+        self._event_id_counter: int = 0
+        self._events: dict[str, list[callable]] = {}
+        self._event_id_map: dict[int, [str, callable]] = {}
 
     def add_event(self, event: str, callback: callable) -> int:
         """Add a callback to an event"""
         if event not in self._events:
             self._events[event] = []
 
         event_id = self._event_id_counter
         self._event_id_counter += 1
         self._event_id_map[event_id] = [event, callback]
         self._events[event].append(callback)
         return event_id
 
-    def remove_event(self, event_id) -> None:
+    def remove_event(self, event_id: int) -> None:
         """Remove a callback from an event"""
         if event_id in self._event_id_map:
             event, callback = self._event_id_map[event_id]
             self._events[event].remove(callback)
             del self._event_id_map[event_id]
 
     def _fire_event(self, event: str, *args, **kwargs) -> None:
```

### Comparing `mizue-0.2.9/mizue/util/signal_handler.py` & `mizue-0.3.0/mizue/util/signal_handler.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue/util/utility.py` & `mizue-0.3.0/mizue/util/utility.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/mizue.egg-info/PKG-INFO` & `mizue-0.3.0/mizue.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.2.9/mizue.egg-info/SOURCES.txt` & `mizue-0.3.0/mizue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizue-0.2.9/setup.py` & `mizue-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="mizue",
-    version="0.2.9",
+    version="0.3.0",
     description="A Python package for various utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hoshilily",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

