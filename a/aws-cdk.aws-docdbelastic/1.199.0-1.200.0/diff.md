# Comparing `tmp/aws-cdk.aws-docdbelastic-1.199.0.tar.gz` & `tmp/aws_cdk.aws_docdbelastic-1.200.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src015969006/src/packages/@aws-cdk/aws-docdbelastic/dist/python/aws-cdk.aws-docdbelastic-1.199.0.tar", last modified: Thu Apr 20 17:20:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
