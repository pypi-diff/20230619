# Comparing `tmp/bidfx-api-1.0.0.tar.gz` & `tmp/bidfx_api-1.1.0-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bidfx-api-1.0.0.tar", last modified: Wed Mar 11 17:38:36 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

