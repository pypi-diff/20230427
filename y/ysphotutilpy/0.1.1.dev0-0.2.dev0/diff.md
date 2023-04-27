# Comparing `tmp/ysphotutilpy-0.1.1.dev0.tar.gz` & `tmp/ysphotutilpy-0.2.dev0-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ysphotutilpy-0.1.1.dev0.tar", last modified: Thu Apr 27 10:46:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

