# Comparing `tmp/american_options-0.1.5.tar.gz` & `tmp/american_options-0.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\american_options-0.1.5.tar", last modified: Mon Jun 19 09:13:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

