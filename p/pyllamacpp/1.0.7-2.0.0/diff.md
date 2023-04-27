# Comparing `tmp/pyllamacpp-1.0.7.tar.gz` & `tmp/pyllamacpp-2.0.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllamacpp-1.0.7.tar", last modified: Sun Apr 23 02:06:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

