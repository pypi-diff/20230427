# Comparing `tmp/pythonabm-0.3.1.tar.gz` & `tmp/pythonabm-0.3.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonabm-0.3.1.tar", last modified: Fri Apr  8 00:20:38 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

