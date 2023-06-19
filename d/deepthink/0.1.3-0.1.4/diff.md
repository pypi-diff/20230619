# Comparing `tmp/deepthink-0.1.3.tar.gz` & `tmp/deepthink-0.1.4-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepthink-0.1.3.tar", last modified: Sun Jan 22 19:45:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

