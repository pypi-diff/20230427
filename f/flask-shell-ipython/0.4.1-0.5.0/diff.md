# Comparing `tmp/flask-shell-ipython-0.4.1.tar.gz` & `tmp/flask_shell_ipython-0.5.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-shell-ipython-0.4.1.tar", last modified: Mon May  6 07:57:37 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

