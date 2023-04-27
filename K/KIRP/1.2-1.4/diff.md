# Comparing `tmp/KIRP-1.2.tar.gz` & `tmp/KIRP-1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KIRP-1.2.tar", last modified: Fri Mar 31 12:04:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

