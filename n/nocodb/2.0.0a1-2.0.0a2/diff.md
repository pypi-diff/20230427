# Comparing `tmp/nocodb-2.0.0a1.tar.gz` & `tmp/nocodb-2.0.0a2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nocodb-2.0.0a1.tar", last modified: Fri Mar  3 23:42:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

