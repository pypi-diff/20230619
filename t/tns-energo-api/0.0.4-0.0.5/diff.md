# Comparing `tmp/tns-energo-api-0.0.4.tar.gz` & `tmp/tns_energo_api-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tns-energo-api-0.0.4.tar", last modified: Fri Sep 24 14:25:36 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

