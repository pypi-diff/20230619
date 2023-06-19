# Comparing `tmp/cytomine-pims-0.13.6.tar.gz` & `tmp/cytomine-pims-0.13.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytomine-pims-0.13.6.tar", last modified: Tue May 23 07:45:38 2023, max compression
+gzip compressed data, was "cytomine-pims-0.13.7.tar", last modified: Mon Jun 19 11:04:09 2023, max compression
```

## Comparing `cytomine-pims-0.13.6.tar` & `cytomine-pims-0.13.7.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.481255 cytomine-pims-0.13.6/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6657 2023-05-23 07:45:38.481255 cytomine-pims-0.13.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5964 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.465256 cytomine-pims-0.13.6/cytomine_pims.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6657 2023-05-23 07:45:38.000000 cytomine-pims-0.13.6/cytomine_pims.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3258 2023-05-23 07:45:38.000000 cytomine-pims-0.13.6/cytomine_pims.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 07:45:38.000000 cytomine-pims-0.13.6/cytomine_pims.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      544 2023-05-23 07:45:38.000000 cytomine-pims-0.13.6/cytomine_pims.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-23 07:45:38.000000 cytomine-pims-0.13.6/cytomine_pims.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.465256 cytomine-pims-0.13.6/pims/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-05-23 07:45:37.000000 cytomine-pims-0.13.6/pims/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.469256 cytomine-pims-0.13.6/pims/api/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10138 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)     3620 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/colormaps.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2568 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     3378 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/formats.py
--rw-rw-rw-   0 root         (0) root         (0)    13741 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/histograms.py
--rw-rw-rw-   0 root         (0) root         (0)     4252 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/housekeeping.py
--rw-rw-rw-   0 root         (0) root         (0)    25845 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     8603 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/operations.py
--rw-rw-rw-   0 root         (0) root         (0)     8083 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/resized.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/server.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/spectral.py
--rw-rw-rw-   0 root         (0) root         (0)     7411 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/thumb.py
--rw-rw-rw-   0 root         (0) root         (0)    17122 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/tile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.469256 cytomine-pims-0.13.6/pims/api/utils/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/annotation_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     2713 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/cytomine_auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/header.py
--rw-rw-rw-   0 root         (0) root         (0)     6268 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/input_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/mimetype.py
--rw-rw-rw-   0 root         (0) root         (0)    23846 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/models.py
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/output_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     2851 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/parameter.py
--rw-rw-rw-   0 root         (0) root         (0)    10058 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/processing_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     2086 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/range_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     4761 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/utils/response.py
--rw-rw-rw-   0 root         (0) root         (0)     9635 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/api/window.py
--rw-rw-rw-   0 root         (0) root         (0)     5452 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.469256 cytomine-pims-0.13.6/pims/cache/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/cache/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/cache/memory.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/cache/object.py
--rw-rw-rw-   0 root         (0) root         (0)    11634 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/cache/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     2167 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/docs.py
--rw-rw-rw-   0 root         (0) root         (0)     9417 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/fastapi_tweaks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.473255 cytomine-pims-0.13.6/pims/files/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5828 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/files/archive.py
--rw-rw-rw-   0 root         (0) root         (0)    12123 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/files/file.py
--rw-rw-rw-   0 root         (0) root         (0)     3079 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/files/histogram.py
--rw-rw-rw-   0 root         (0) root         (0)    17470 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/files/image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.473255 cytomine-pims-0.13.6/pims/filters/
--rw-rw-rw-   0 root         (0) root         (0)     6374 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/filters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3796 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/filters/global_histogram.py
--rw-rw-rw-   0 root         (0) root         (0)     8819 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/filters/pixel_color_deconvolution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.473255 cytomine-pims-0.13.6/pims/formats/
--rw-rw-rw-   0 root         (0) root         (0)     4345 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.473255 cytomine-pims-0.13.6/pims/formats/common/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3404 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/bmp.py
--rw-rw-rw-   0 root         (0) root         (0)    13688 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/dicom.py
--rw-rw-rw-   0 root         (0) root         (0)     8303 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/imagej.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/jpeg.py
--rw-rw-rw-   0 root         (0) root         (0)     5544 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/jpeg2000.py
--rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/ometiff.py
--rw-rw-rw-   0 root         (0) root         (0)     4928 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/png.py
--rw-rw-rw-   0 root         (0) root         (0)     3648 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/ppm.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/sis.py
--rw-rw-rw-   0 root         (0) root         (0)     5525 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/tiff.py
--rw-rw-rw-   0 root         (0) root         (0)    10568 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/virtual.py
--rw-rw-rw-   0 root         (0) root         (0)     4693 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/common/webp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.473255 cytomine-pims-0.13.6/pims/formats/utils/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9505 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/checker.py
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/convertor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.477255 cytomine-pims-0.13.6/pims/formats/utils/engines/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/engines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2707 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/engines/exiftool.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/engines/omexml.py
--rw-rw-rw-   0 root         (0) root         (0)     7698 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/engines/pil.py
--rw-rw-rw-   0 root         (0) root         (0)     7958 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/engines/tifffile.py
--rw-rw-rw-   0 root         (0) root         (0)     8867 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/engines/vips.py
--rw-rw-rw-   0 root         (0) root         (0)     3405 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     6661 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/histogram.py
--rw-rw-rw-   0 root         (0) root         (0)     3982 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10320 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.477255 cytomine-pims-0.13.6/pims/formats/utils/structures/
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/structures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/structures/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)    13176 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/structures/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     2861 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/structures/planes.py
--rw-rw-rw-   0 root         (0) root         (0)     7924 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/formats/utils/structures/pyramid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.477255 cytomine-pims-0.13.6/pims/importer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 07:45:29.000000 cytomine-pims-0.13.6/pims/importer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2560 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/importer/import_local_images.py
--rw-rw-rw-   0 root         (0) root         (0)    19599 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/importer/importer.py
--rw-rw-rw-   0 root         (0) root         (0)    24279 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/importer/listeners.py
--rw-rw-rw-   0 root         (0) root         (0)     1953 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.477255 cytomine-pims-0.13.6/pims/processing/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)     9001 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/colormaps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.477255 cytomine-pims-0.13.6/pims/processing/histograms/
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/histograms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/histograms/format.py
--rw-rw-rw-   0 root         (0) root         (0)     7616 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/histograms/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    25411 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/image_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5183 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/masks.py
--rw-rw-rw-   0 root         (0) root         (0)    15529 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/pixels.py
--rw-rw-rw-   0 root         (0) root         (0)     6302 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/processing/region.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.477255 cytomine-pims-0.13.6/pims/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4746 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/tasks/queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/tasks/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:38.481255 cytomine-pims-0.13.6/pims/utils/
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/arrays.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/background_task.py
--rw-rw-rw-   0 root         (0) root         (0)     6351 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/color.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)     2554 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/copy.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/dict.py
--rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/dtypes.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/iterables.py
--rw-rw-rw-   0 root         (0) root         (0)     1824 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/math.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/strings.py
--rw-rw-rw-   0 root         (0) root         (0)     2982 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/types.py
--rw-rw-rw-   0 root         (0) root         (0)     2949 2023-05-09 08:02:09.000000 cytomine-pims-0.13.6/pims/utils/vips.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-05-23 07:45:38.481255 cytomine-pims-0.13.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5015 2023-05-23 07:23:23.000000 cytomine-pims-0.13.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.069931 cytomine-pims-0.13.7/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9557 2023-06-19 11:04:09.069931 cytomine-pims-0.13.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     8864 2023-06-09 11:11:39.000000 cytomine-pims-0.13.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.053931 cytomine-pims-0.13.7/cytomine_pims.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9557 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-06-19 11:04:09.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/cytomine_pims.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.053931 cytomine-pims-0.13.7/pims/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-06-19 11:04:08.000000 cytomine-pims-0.13.7/pims/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.057931 cytomine-pims-0.13.7/pims/api/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10138 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3620 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/colormaps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2568 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/formats.py
+-rw-rw-rw-   0 root         (0) root         (0)    13741 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/histograms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4252 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/housekeeping.py
+-rw-rw-rw-   0 root         (0) root         (0)    25845 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     8603 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/operations.py
+-rw-rw-rw-   0 root         (0) root         (0)     8083 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/resized.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/server.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/spectral.py
+-rw-rw-rw-   0 root         (0) root         (0)     7411 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/thumb.py
+-rw-rw-rw-   0 root         (0) root         (0)    17122 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/tile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.057931 cytomine-pims-0.13.7/pims/api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/annotation_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2713 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/cytomine_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     6268 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/input_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/mimetype.py
+-rw-rw-rw-   0 root         (0) root         (0)    23846 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/output_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2851 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10058 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/processing_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/range_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4761 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/utils/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     9635 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/api/window.py
+-rw-rw-rw-   0 root         (0) root         (0)     5452 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.057931 cytomine-pims-0.13.7/pims/cache/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/cache/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/cache/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/cache/object.py
+-rw-rw-rw-   0 root         (0) root         (0)    11634 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/cache/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     2226 2023-06-06 14:49:46.000000 cytomine-pims-0.13.7/pims/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9417 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/fastapi_tweaks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/files/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)    12123 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3079 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/histogram.py
+-rw-rw-rw-   0 root         (0) root         (0)    17470 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/files/image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/filters/
+-rw-rw-rw-   0 root         (0) root         (0)     6374 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/filters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3796 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/filters/global_histogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     8819 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/filters/pixel_color_deconvolution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/formats/
+-rw-rw-rw-   0 root         (0) root         (0)     5552 2023-06-08 09:07:51.000000 cytomine-pims-0.13.7/pims/formats/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/formats/common/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3404 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/bmp.py
+-rw-rw-rw-   0 root         (0) root         (0)    13688 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/dicom.py
+-rw-rw-rw-   0 root         (0) root         (0)     8303 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/imagej.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/jpeg.py
+-rw-rw-rw-   0 root         (0) root         (0)     5544 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/jpeg2000.py
+-rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/ometiff.py
+-rw-rw-rw-   0 root         (0) root         (0)     4928 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/png.py
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/ppm.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/sis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5525 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/tiff.py
+-rw-rw-rw-   0 root         (0) root         (0)    10568 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/virtual.py
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/common/webp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.061931 cytomine-pims-0.13.7/pims/formats/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9505 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/convertor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/formats/utils/engines/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2707 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/exiftool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/omexml.py
+-rw-rw-rw-   0 root         (0) root         (0)     7698 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/pil.py
+-rw-rw-rw-   0 root         (0) root         (0)     7958 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/tifffile.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/engines/vips.py
+-rw-rw-rw-   0 root         (0) root         (0)     3405 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/histogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10320 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/formats/utils/structures/
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13176 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2861 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/planes.py
+-rw-rw-rw-   0 root         (0) root         (0)     7924 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/formats/utils/structures/pyramid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/importer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 11:03:58.000000 cytomine-pims-0.13.7/pims/importer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/importer/import_local_images.py
+-rw-rw-rw-   0 root         (0) root         (0)    19599 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/importer/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)    24279 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/importer/listeners.py
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/processing/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)     9001 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/colormaps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/processing/histograms/
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/histograms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/histograms/format.py
+-rw-rw-rw-   0 root         (0) root         (0)     7616 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/histograms/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    25411 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/image_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     5183 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/masks.py
+-rw-rw-rw-   0 root         (0) root         (0)    15529 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/pixels.py
+-rw-rw-rw-   0 root         (0) root         (0)     6302 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/processing/region.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.065931 cytomine-pims-0.13.7/pims/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4746 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/tasks/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/tasks/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 11:04:09.069931 cytomine-pims-0.13.7/pims/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/arrays.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/background_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/color.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)     2554 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/copy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/dtypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/iterables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/math.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/strings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2982 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-05-09 08:02:09.000000 cytomine-pims-0.13.7/pims/utils/vips.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-19 11:04:09.069931 cytomine-pims-0.13.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5015 2023-05-23 07:23:23.000000 cytomine-pims-0.13.7/setup.py
```

### Comparing `cytomine-pims-0.13.6/LICENSE` & `cytomine-pims-0.13.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/cytomine_pims.egg-info/SOURCES.txt` & `cytomine-pims-0.13.7/cytomine_pims.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/cytomine_pims.egg-info/requires.txt` & `cytomine-pims-0.13.7/cytomine_pims.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/__init__.py` & `cytomine-pims-0.13.7/pims/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/__version__.py` & `cytomine-pims-0.13.7/pims/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 # KEEP ENCODING - so that __version__ can be read even if py2.7 is used.
 
 
 
 __title__ = 'pims'
 __description__ = 'Cytomine Python Image Server'
 __url__ = 'https://doc.uliege.cytomine.org'
-__version__ = "0.13.6"
+__version__ = "0.13.7"
 __api_version__ = "0.0.0"
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2020-2021 ULiège Cytomine R&D team'
 __author__ = 'Ulysse Rubens'
 __email__ = 'uliege@cytomine.org'
```

### Comparing `cytomine-pims-0.13.6/pims/api/__init__.py` & `cytomine-pims-0.13.7/pims/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/annotation.py` & `cytomine-pims-0.13.7/pims/api/annotation.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/colormaps.py` & `cytomine-pims-0.13.7/pims/api/colormaps.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/exceptions.py` & `cytomine-pims-0.13.7/pims/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/filters.py` & `cytomine-pims-0.13.7/pims/api/filters.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/formats.py` & `cytomine-pims-0.13.7/pims/api/formats.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/histograms.py` & `cytomine-pims-0.13.7/pims/api/histograms.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/housekeeping.py` & `cytomine-pims-0.13.7/pims/api/housekeeping.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/metadata.py` & `cytomine-pims-0.13.7/pims/api/metadata.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/operations.py` & `cytomine-pims-0.13.7/pims/api/operations.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/resized.py` & `cytomine-pims-0.13.7/pims/api/resized.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/server.py` & `cytomine-pims-0.13.7/pims/api/server.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/spectral.py` & `cytomine-pims-0.13.7/pims/api/spectral.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/thumb.py` & `cytomine-pims-0.13.7/pims/api/thumb.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/tile.py` & `cytomine-pims-0.13.7/pims/api/tile.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/__init__.py` & `cytomine-pims-0.13.7/pims/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/annotation_parameter.py` & `cytomine-pims-0.13.7/pims/api/utils/annotation_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/cytomine_auth.py` & `cytomine-pims-0.13.7/pims/api/utils/cytomine_auth.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/header.py` & `cytomine-pims-0.13.7/pims/api/utils/header.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/input_parameter.py` & `cytomine-pims-0.13.7/pims/api/utils/input_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/mimetype.py` & `cytomine-pims-0.13.7/pims/api/utils/mimetype.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/models.py` & `cytomine-pims-0.13.7/pims/api/utils/models.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/output_parameter.py` & `cytomine-pims-0.13.7/pims/api/utils/output_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/parameter.py` & `cytomine-pims-0.13.7/pims/api/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/processing_parameter.py` & `cytomine-pims-0.13.7/pims/api/utils/processing_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/range_parameter.py` & `cytomine-pims-0.13.7/pims/api/utils/range_parameter.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/utils/response.py` & `cytomine-pims-0.13.7/pims/api/utils/response.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/api/window.py` & `cytomine-pims-0.13.7/pims/api/window.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/application.py` & `cytomine-pims-0.13.7/pims/application.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/cache/__init__.py` & `cytomine-pims-0.13.7/pims/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/cache/memory.py` & `cytomine-pims-0.13.7/pims/cache/memory.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/cache/object.py` & `cytomine-pims-0.13.7/pims/cache/object.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/cache/redis.py` & `cytomine-pims-0.13.7/pims/cache/redis.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/config.py` & `cytomine-pims-0.13.7/pims/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 logger = logging.getLogger("pims.app")
 
 
 class ReadableSettings(BaseSettings):
     root: str
     pending_path: str
+    checker_resolution_file: str = "checkerResolution.csv"
     default_image_size_safety_mode: str = "SAFE_REJECT"
     default_annotation_origin: str = "LEFT_TOP"
     output_size_limit: int = 10000
     pims_url: str = "http://localhost-ims"
 
     cache_enabled: bool = True
     cache_url: str = "redis://pims-cache:6379"
@@ -58,15 +59,15 @@
     cytomine_private_key: str
 
     task_queue_user: str = "router"
     task_queue_password: str = "router"
 
     class Config:
         env_file = "pims-config.env"
-        env_file_encoding = 'utf-8'
+        env_file_encoding = "utf-8"
 
 
 @lru_cache()
 def get_settings():
-    env_file = os.getenv('CONFIG_FILE', 'pims-config.env')
+    env_file = os.getenv("CONFIG_FILE", "pims-config.env")
     logger.info(f"[green]Loading config from {env_file}")
     return Settings(_env_file=env_file)
```

### Comparing `cytomine-pims-0.13.6/pims/docs.py` & `cytomine-pims-0.13.7/pims/docs.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/fastapi_tweaks.py` & `cytomine-pims-0.13.7/pims/fastapi_tweaks.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/files/__init__.py` & `cytomine-pims-0.13.7/pims/files/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/files/archive.py` & `cytomine-pims-0.13.7/pims/files/archive.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/files/file.py` & `cytomine-pims-0.13.7/pims/files/file.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/files/histogram.py` & `cytomine-pims-0.13.7/pims/files/histogram.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/files/image.py` & `cytomine-pims-0.13.7/pims/files/image.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/filters/__init__.py` & `cytomine-pims-0.13.7/pims/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/filters/global_histogram.py` & `cytomine-pims-0.13.7/pims/filters/global_histogram.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/filters/pixel_color_deconvolution.py` & `cytomine-pims-0.13.7/pims/filters/pixel_color_deconvolution.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/__init__.py` & `cytomine-pims-0.13.7/pims/formats/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,33 +8,68 @@
 #  *
 #  * Unless required by applicable law or agreed to in writing, software
 #  * distributed under the License is distributed on an "AS IS" BASIS,
 #  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  * See the License for the specific language governing permissions and
 #  * limitations under the License.
 
+from functools import partial
 import logging
 from importlib import import_module
 from inspect import isabstract, isclass
 from pkgutil import iter_modules
+
 from types import ModuleType
 from typing import Dict, List, Type, Union
+from pims.config import get_settings
+import csv
+import os
 
 from importlib_metadata import EntryPoint, entry_points  # noqa
 
 from pims.formats.utils.abstract import AbstractFormat
 
-FORMAT_PLUGIN_PREFIX = 'pims_format_'
+FORMAT_PLUGIN_PREFIX = "pims_format_"
 NON_PLUGINS_MODULES = ["pims.formats.utils"]
 PLUGIN_GROUP = "pims.formats"
 
 logger = logging.getLogger("pims.app")
 logger.info("[green bold]Formats initialization...")
 
 
+def custom_sort_key(item, dictionary):
+    return dictionary.get(item, dictionary.get(getattr(item, "module", None), 0))
+
+
+def reorder_plugins(
+    plugin_list, csv_path, name_column="name", resolution_order_column="resolution_order"
+):
+    plugin_resolution_orders = {}
+
+    for _, name, _ in iter_modules(__path__, prefix="pims.formats."):
+        if name not in NON_PLUGINS_MODULES:
+            plugin_resolution_orders[name] = 0
+
+    with open(csv_path, "r") as file:
+        reader = csv.DictReader(file)
+
+        for row in reader:
+            plugin_name = row[name_column]
+            resolution_order = int(row[resolution_order_column])
+
+            if plugin_name is not None and resolution_order is not None:
+                plugin_resolution_orders[plugin_name] = resolution_order
+                
+    sorted_plugin_list = sorted(
+        plugin_list, key=partial(custom_sort_key, dictionary=plugin_resolution_orders)
+    )
+
+    return sorted_plugin_list
+
+
 def _discover_format_plugins() -> List[Union[str, EntryPoint]]:
     """
     Discover format plugins in the Python env.
     Plugins are:
     * modules in `pims.formats`.
     * modules starting with `FORMAT_PLUGIN_PREFIX`.
     * packages having an entrypoint in group `PLUGIN_GROUP`.
@@ -45,24 +80,28 @@
     Returns
     -------
     plugins
         The list of plugin module names or entry points
     """
 
     plugins = [
-        name for _, name, _ in iter_modules(__path__, prefix="pims.formats.")
+        name
+        for _, name, _ in iter_modules(__path__, prefix="pims.formats.")
         if name not in NON_PLUGINS_MODULES
     ]
     plugins += [
-        name for _, name, _ in iter_modules()
-        if name.startswith(FORMAT_PLUGIN_PREFIX)
+        name for _, name, _ in iter_modules() if name.startswith(FORMAT_PLUGIN_PREFIX)
     ]
     plugins += entry_points(group=PLUGIN_GROUP)
 
     plugin_names = [p.module if type(p) is EntryPoint else p for p in plugins]
+
+    if os.path.isfile(get_settings().checker_resolution_file):
+        plugins = reorder_plugins(plugins, get_settings().checker_resolution_file)
+
     logger.info(
         f"[green bold]Format plugins: found {len(plugins)} plugin(s)[/] "
         f"[yellow]({', '.join(plugin_names)})"
     )
     return plugins
 
 
@@ -81,30 +120,32 @@
         The format classes
     """
     formats = list()
     for _, name, _ in iter_modules(mod.__path__):
         submodule_name = f"{mod.__name__}.{name}"
         try:
             for var in vars(import_module(submodule_name)).values():
-                if isclass(var) and \
-                        issubclass(var, AbstractFormat) and \
-                        not isabstract(var) and \
-                        'Abstract' not in var.__name__:
+                if (
+                    isclass(var)
+                    and issubclass(var, AbstractFormat)
+                    and not isabstract(var)
+                    and "Abstract" not in var.__name__
+                ):
                     format = var
                     formats.append(format)
                     format.init()
 
                     logger.info(
                         f"[green] * [yellow]{format.get_identifier()} "
                         f"- {format.get_name()}[/] imported."
                     )
         except ImportError as e:
             logger.error(
-                f"{submodule_name} submodule cannot be checked for "
-                f"formats !", exc_info=e
+                f"{submodule_name} submodule cannot be checked for " f"formats !",
+                exc_info=e,
             )
     return formats
 
 
 def _get_all_formats() -> List[Type[AbstractFormat]]:
     """
     Find all Format classes in modules specified in FORMAT_PLUGINS.
@@ -116,16 +157,15 @@
     """
     formats = list()
     for plugin in FORMAT_PLUGINS:
         entrypoint_plugin = type(plugin) is EntryPoint
 
         module_name = plugin.module if entrypoint_plugin else plugin
         logger.info(
-            f"[green bold]Importing formats from "
-            f"[yellow]{module_name}[/] plugin..."
+            f"[green bold]Importing formats from " f"[yellow]{module_name}[/] plugin..."
         )
 
         if entrypoint_plugin:
             module = plugin.load()
         else:
             module = import_module(module_name)
         formats.extend(_find_formats_in_module(module))
@@ -133,11 +173,8 @@
     return formats
 
 
 FormatsByExt = Dict[str, Type[AbstractFormat]]
 
 
 FORMAT_PLUGINS: List[Union[str, EntryPoint]] = _discover_format_plugins()
-FORMATS: FormatsByExt = {
-    f.get_identifier(): f
-    for f in _get_all_formats()
-}
+FORMATS: FormatsByExt = {f.get_identifier(): f for f in _get_all_formats()}
```

### Comparing `cytomine-pims-0.13.6/pims/formats/common/__init__.py` & `cytomine-pims-0.13.7/pims/formats/common/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/bmp.py` & `cytomine-pims-0.13.7/pims/formats/common/bmp.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/dicom.py` & `cytomine-pims-0.13.7/pims/formats/common/dicom.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/imagej.py` & `cytomine-pims-0.13.7/pims/formats/common/imagej.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/jpeg.py` & `cytomine-pims-0.13.7/pims/formats/common/jpeg.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/jpeg2000.py` & `cytomine-pims-0.13.7/pims/formats/common/jpeg2000.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/ometiff.py` & `cytomine-pims-0.13.7/pims/formats/common/ometiff.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/png.py` & `cytomine-pims-0.13.7/pims/formats/common/png.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/ppm.py` & `cytomine-pims-0.13.7/pims/formats/common/ppm.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/sis.py` & `cytomine-pims-0.13.7/pims/formats/common/sis.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/tiff.py` & `cytomine-pims-0.13.7/pims/formats/common/tiff.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/virtual.py` & `cytomine-pims-0.13.7/pims/formats/common/virtual.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/common/webp.py` & `cytomine-pims-0.13.7/pims/formats/common/webp.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/__init__.py` & `cytomine-pims-0.13.7/pims/formats/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/abstract.py` & `cytomine-pims-0.13.7/pims/formats/utils/abstract.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/checker.py` & `cytomine-pims-0.13.7/pims/formats/utils/checker.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/convertor.py` & `cytomine-pims-0.13.7/pims/formats/utils/convertor.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/engines/__init__.py` & `cytomine-pims-0.13.7/pims/formats/utils/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/engines/exiftool.py` & `cytomine-pims-0.13.7/pims/formats/utils/engines/exiftool.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/engines/omexml.py` & `cytomine-pims-0.13.7/pims/formats/utils/engines/omexml.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/engines/pil.py` & `cytomine-pims-0.13.7/pims/formats/utils/engines/pil.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/engines/tifffile.py` & `cytomine-pims-0.13.7/pims/formats/utils/engines/tifffile.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/engines/vips.py` & `cytomine-pims-0.13.7/pims/formats/utils/engines/vips.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/factories.py` & `cytomine-pims-0.13.7/pims/formats/utils/factories.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/histogram.py` & `cytomine-pims-0.13.7/pims/formats/utils/histogram.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/parser.py` & `cytomine-pims-0.13.7/pims/formats/utils/parser.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/reader.py` & `cytomine-pims-0.13.7/pims/formats/utils/reader.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/structures/__init__.py` & `cytomine-pims-0.13.7/pims/formats/utils/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/structures/annotations.py` & `cytomine-pims-0.13.7/pims/formats/utils/structures/annotations.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/structures/metadata.py` & `cytomine-pims-0.13.7/pims/formats/utils/structures/metadata.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/structures/planes.py` & `cytomine-pims-0.13.7/pims/formats/utils/structures/planes.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/formats/utils/structures/pyramid.py` & `cytomine-pims-0.13.7/pims/formats/utils/structures/pyramid.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/importer/import_local_images.py` & `cytomine-pims-0.13.7/pims/importer/import_local_images.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/importer/importer.py` & `cytomine-pims-0.13.7/pims/importer/importer.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/importer/listeners.py` & `cytomine-pims-0.13.7/pims/importer/listeners.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/logger.py` & `cytomine-pims-0.13.7/pims/logger.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/main.py` & `cytomine-pims-0.13.7/pims/main.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/__init__.py` & `cytomine-pims-0.13.7/pims/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/adapters.py` & `cytomine-pims-0.13.7/pims/processing/adapters.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/annotations.py` & `cytomine-pims-0.13.7/pims/processing/annotations.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/colormaps.py` & `cytomine-pims-0.13.7/pims/processing/colormaps.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/histograms/__init__.py` & `cytomine-pims-0.13.7/pims/processing/histograms/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/histograms/format.py` & `cytomine-pims-0.13.7/pims/processing/histograms/format.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/histograms/utils.py` & `cytomine-pims-0.13.7/pims/processing/histograms/utils.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/image_response.py` & `cytomine-pims-0.13.7/pims/processing/image_response.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/masks.py` & `cytomine-pims-0.13.7/pims/processing/masks.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/pixels.py` & `cytomine-pims-0.13.7/pims/processing/pixels.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/processing/region.py` & `cytomine-pims-0.13.7/pims/processing/region.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/tasks/__init__.py` & `cytomine-pims-0.13.7/pims/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/tasks/queue.py` & `cytomine-pims-0.13.7/pims/tasks/queue.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/tasks/worker.py` & `cytomine-pims-0.13.7/pims/tasks/worker.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/__init__.py` & `cytomine-pims-0.13.7/pims/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/arrays.py` & `cytomine-pims-0.13.7/pims/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/background_task.py` & `cytomine-pims-0.13.7/pims/utils/background_task.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/color.py` & `cytomine-pims-0.13.7/pims/utils/color.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/concurrency.py` & `cytomine-pims-0.13.7/pims/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/copy.py` & `cytomine-pims-0.13.7/pims/utils/copy.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/dict.py` & `cytomine-pims-0.13.7/pims/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/dtypes.py` & `cytomine-pims-0.13.7/pims/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/iterables.py` & `cytomine-pims-0.13.7/pims/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/math.py` & `cytomine-pims-0.13.7/pims/utils/math.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/strings.py` & `cytomine-pims-0.13.7/pims/utils/strings.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/types.py` & `cytomine-pims-0.13.7/pims/utils/types.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/pims/utils/vips.py` & `cytomine-pims-0.13.7/pims/utils/vips.py`

 * *Files identical despite different names*

### Comparing `cytomine-pims-0.13.6/setup.py` & `cytomine-pims-0.13.7/setup.py`

 * *Files identical despite different names*

