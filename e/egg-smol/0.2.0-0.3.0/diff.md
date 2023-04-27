# Comparing `tmp/egg_smol-0.2.0.tar.gz` & `tmp/egg_smol-0.3.0-cp37-cp37m-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

