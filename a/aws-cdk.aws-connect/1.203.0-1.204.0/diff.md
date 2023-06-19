# Comparing `tmp/aws-cdk.aws-connect-1.203.0.tar.gz` & `tmp/aws_cdk.aws_connect-1.204.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src637092372/src/packages/@aws-cdk/aws-connect/dist/python/aws-cdk.aws-connect-1.203.0.tar", last modified: Wed May 31 18:47:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

