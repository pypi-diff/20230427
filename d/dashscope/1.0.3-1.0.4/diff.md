# Comparing `tmp/dashscope-1.0.3.tar.gz` & `tmp/dashscope-1.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dashscope-1.0.3.tar", last modified: Mon Apr 10 14:28:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

