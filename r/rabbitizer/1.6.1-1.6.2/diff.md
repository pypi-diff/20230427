# Comparing `tmp/rabbitizer-1.6.1.tar.gz` & `tmp/rabbitizer-1.6.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitizer-1.6.1.tar", last modified: Tue Apr 18 04:16:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

