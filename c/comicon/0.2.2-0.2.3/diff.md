# Comparing `tmp/comicon-0.2.2.tar.gz` & `tmp/comicon-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicon-0.2.2.tar", max compression
+gzip compressed data, was "comicon-0.2.3.tar", max compression
```

## Comparing `comicon-0.2.2.tar` & `comicon-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    34520 2023-01-19 01:21:43.343731 comicon-0.2.2/LICENSE
--rw-r--r--   0        0        0     1493 2023-01-24 02:59:24.432940 comicon-0.2.2/README.md
--rw-r--r--   0        0        0      348 2023-01-19 03:38:16.600950 comicon-0.2.2/comicon/__init__.py
--rw-r--r--   0        0        0      585 2023-01-19 03:20:26.070654 comicon-0.2.2/comicon/api.py
--rw-r--r--   0        0        0     1034 2023-02-14 03:05:01.345420 comicon-0.2.2/comicon/base.py
--rw-r--r--   0        0        0     3548 2023-01-19 14:48:26.457554 comicon-0.2.2/comicon/cirtools.py
--rw-r--r--   0        0        0        0 2023-02-14 02:58:14.098947 comicon-0.2.2/comicon/common/__init__.py
--rw-r--r--   0        0        0      409 2023-02-14 03:09:59.308920 comicon-0.2.2/comicon/common/cbz.py
--rw-r--r--   0        0        0        0 2023-02-14 02:58:23.310865 comicon-0.2.2/comicon/common/cir.py
--rw-r--r--   0        0        0        0 2023-02-14 02:58:16.479925 comicon-0.2.2/comicon/common/epub.py
--rw-r--r--   0        0        0        0 2023-02-14 02:58:27.834825 comicon-0.2.2/comicon/common/pdf.py
--rw-r--r--   0        0        0      810 2023-01-19 14:44:56.400117 comicon-0.2.2/comicon/errors.py
--rw-r--r--   0        0        0     1890 2023-03-10 05:20:48.406102 comicon-0.2.2/comicon/inputs/__init__.py
--rw-r--r--   0        0        0     4605 2023-01-19 03:30:58.971799 comicon-0.2.2/comicon/inputs/cbz.py
--rw-r--r--   0        0        0      631 2023-01-18 18:36:38.546802 comicon-0.2.2/comicon/inputs/cir.py
--rw-r--r--   0        0        0     5888 2023-02-11 18:50:43.896715 comicon-0.2.2/comicon/inputs/epub.py
--rw-r--r--   0        0        0     2810 2023-01-19 03:30:58.621800 comicon-0.2.2/comicon/inputs/pdf.py
--rw-r--r--   0        0        0     1873 2023-03-10 05:20:48.406102 comicon-0.2.2/comicon/outputs/__init__.py
--rw-r--r--   0        0        0     1845 2023-01-19 03:01:28.528083 comicon-0.2.2/comicon/outputs/cbz.py
--rw-r--r--   0        0        0      657 2023-01-18 19:12:20.005904 comicon-0.2.2/comicon/outputs/cir.py
--rw-r--r--   0        0        0     3117 2023-01-19 03:30:47.666814 comicon-0.2.2/comicon/outputs/epub.py
--rw-r--r--   0        0        0     1891 2023-02-11 18:47:57.091972 comicon-0.2.2/comicon/outputs/pdf.py
--rw-r--r--   0        0        0      718 2023-03-10 05:20:48.408102 comicon-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 comicon-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-01-19 01:21:43.343731 comicon-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1493 2023-01-24 02:59:24.432940 comicon-0.2.3/README.md
+-rw-r--r--   0        0        0      348 2023-01-19 03:38:16.600950 comicon-0.2.3/comicon/__init__.py
+-rw-r--r--   0        0        0      585 2023-01-19 03:20:26.070654 comicon-0.2.3/comicon/api.py
+-rw-r--r--   0        0        0     1034 2023-02-14 03:05:01.345420 comicon-0.2.3/comicon/base.py
+-rw-r--r--   0        0        0     3548 2023-04-09 23:32:40.814526 comicon-0.2.3/comicon/cirtools.py
+-rw-r--r--   0        0        0        0 2023-02-14 02:58:14.098947 comicon-0.2.3/comicon/common/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-09 23:34:20.162767 comicon-0.2.3/comicon/common/cbz.py
+-rw-r--r--   0        0        0        0 2023-02-14 02:58:23.310865 comicon-0.2.3/comicon/common/cir.py
+-rw-r--r--   0        0        0        0 2023-02-14 02:58:16.479925 comicon-0.2.3/comicon/common/epub.py
+-rw-r--r--   0        0        0        0 2023-02-14 02:58:27.834825 comicon-0.2.3/comicon/common/pdf.py
+-rw-r--r--   0        0        0      810 2023-01-19 14:44:56.400117 comicon-0.2.3/comicon/errors.py
+-rw-r--r--   0        0        0     1890 2023-03-10 05:20:48.406102 comicon-0.2.3/comicon/inputs/__init__.py
+-rw-r--r--   0        0        0     4605 2023-04-27 21:51:31.834322 comicon-0.2.3/comicon/inputs/cbz.py
+-rw-r--r--   0        0        0      631 2023-01-18 18:36:38.546802 comicon-0.2.3/comicon/inputs/cir.py
+-rw-r--r--   0        0        0     5888 2023-02-11 18:50:43.896715 comicon-0.2.3/comicon/inputs/epub.py
+-rw-r--r--   0        0        0     2810 2023-01-19 03:30:58.621800 comicon-0.2.3/comicon/inputs/pdf.py
+-rw-r--r--   0        0        0     1873 2023-03-10 05:20:48.406102 comicon-0.2.3/comicon/outputs/__init__.py
+-rw-r--r--   0        0        0     1845 2023-01-19 03:01:28.528083 comicon-0.2.3/comicon/outputs/cbz.py
+-rw-r--r--   0        0        0      657 2023-01-18 19:12:20.005904 comicon-0.2.3/comicon/outputs/cir.py
+-rw-r--r--   0        0        0     3117 2023-01-19 03:30:47.666814 comicon-0.2.3/comicon/outputs/epub.py
+-rw-r--r--   0        0        0     1891 2023-02-11 18:47:57.091972 comicon-0.2.3/comicon/outputs/pdf.py
+-rw-r--r--   0        0        0      964 2023-04-27 21:52:58.311564 comicon-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 comicon-0.2.3/PKG-INFO
```

### Comparing `comicon-0.2.2/LICENSE` & `comicon-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/README.md` & `comicon-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/api.py` & `comicon-0.2.3/comicon/api.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/base.py` & `comicon-0.2.3/comicon/base.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/cirtools.py` & `comicon-0.2.3/comicon/cirtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,19 +83,19 @@
 
     # check that all chapter folders contain at least one image
     for chapter_folder in chapter_folders:
         images = sorted(f for f in chapter_folder.iterdir() if f.is_file())
         if not images:
             raise EmptyChapterError(f"{chapter_folder} is empty")
         for image in images:
-            if not image.suffix.lower() in ALLOWED_COVER_EXTENSIONS:
+            if image.suffix.lower() not in ALLOWED_COVER_EXTENSIONS:
                 raise BadImageError(f"{image} is not an image")
 
     # check that the cover image exists
     if comic.metadata.cover_path_rel:
         cover_path = path / f"{comic.metadata.cover_path_rel}"
         if not cover_path.is_file():
             raise FileNotFoundError(
                 f"{cover_path} does not exist but is declared in {data_file}"
             )
-        if not cover_path.suffix.lower() in ALLOWED_COVER_EXTENSIONS:
+        if cover_path.suffix.lower() not in ALLOWED_COVER_EXTENSIONS:
             raise BadImageError(f"{cover_path} is not an accepted image")
```

### Comparing `comicon-0.2.2/comicon/errors.py` & `comicon-0.2.3/comicon/errors.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/inputs/__init__.py` & `comicon-0.2.3/comicon/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/inputs/cbz.py` & `comicon-0.2.3/comicon/inputs/cbz.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,8 @@
             for image_path in image_paths:
                 with z.open(str(image_path)) as file:
                     data = file.read()
 
                 new_path = dest / "chapter-1" / image_path.name
                 with open(new_path, "wb") as file:
                     file.write(data)
-                    yield str(filename)
+                    yield str(new_path)
```

### Comparing `comicon-0.2.2/comicon/inputs/cir.py` & `comicon-0.2.3/comicon/inputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/inputs/epub.py` & `comicon-0.2.3/comicon/inputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/inputs/pdf.py` & `comicon-0.2.3/comicon/inputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/outputs/__init__.py` & `comicon-0.2.3/comicon/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/outputs/cbz.py` & `comicon-0.2.3/comicon/outputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/outputs/cir.py` & `comicon-0.2.3/comicon/outputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/outputs/epub.py` & `comicon-0.2.3/comicon/outputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/comicon/outputs/pdf.py` & `comicon-0.2.3/comicon/outputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-0.2.2/pyproject.toml` & `comicon-0.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "comicon"
-version = "0.2.2"
+version = "0.2.3"
 description = "A simple comic conversion library between CBZ/EPUB/PDF"
 authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 repository = "https://github.com/potatoeggy/comicon"
 documentation = "https://github.com/potatoeggy/comicon"
 keywords = ["converter", "comic", "cbz", "epub", "pdf"]
@@ -19,9 +19,21 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-split_on_trailing_comma = true
+[tool.ruff]
+select = ["B", "C", "E", "F", "W"]
+ignore = ["B905"]
+exclude = ["mandown/ui/*", "build/*"]
+target-version = "py310"
+line-length = 100
+
+[tool.ruff.mccabe]
+max-complexity = 18
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+"mandown/cli.py" = ["B008"]
+"tests/*" = ["E501"]
```

### Comparing `comicon-0.2.2/PKG-INFO` & `comicon-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicon
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple comic conversion library between CBZ/EPUB/PDF
 Home-page: https://github.com/potatoeggy/comicon
 License: AGPL-3.0-only
 Keywords: converter,comic,cbz,epub,pdf
 Author: Daniel Chen
 Author-email: danielchen04@hotmail.ca
 Requires-Python: >=3.10
```

