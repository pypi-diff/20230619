# Comparing `tmp/simple_romp-1.0.9.tar.gz` & `tmp/simple_romp-2.0.0-py3.9-macosx-11.1-arm64.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_romp-1.0.9.tar", last modified: Mon Jun 19 13:45:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

