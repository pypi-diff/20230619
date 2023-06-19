# Comparing `tmp/pyscal3-3.0.0.dev6.tar.gz` & `tmp/pyscal3-3.0.1-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal3-3.0.0.dev6.tar", last modified: Fri Jun 16 11:30:28 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

