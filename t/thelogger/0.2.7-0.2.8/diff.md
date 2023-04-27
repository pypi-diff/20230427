# Comparing `tmp/thelogger-0.2.7.tar.gz` & `tmp/thelogger-0.2.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\thelogger-0.2.7.tar", last modified: Tue Feb 28 14:52:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

