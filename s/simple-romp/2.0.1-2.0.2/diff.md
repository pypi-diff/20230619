# Comparing `tmp/simple_romp-2.0.1.tar.gz` & `tmp/simple_romp-2.0.2-cp39-cp39-manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_romp-2.0.1.tar", last modified: Mon Jun 19 16:18:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

