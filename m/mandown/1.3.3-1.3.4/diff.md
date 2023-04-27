# Comparing `tmp/mandown-1.3.3.tar.gz` & `tmp/mandown-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mandown-1.3.3.tar", max compression
+gzip compressed data, was "mandown-1.3.4.tar", max compression
```

## Comparing `mandown-1.3.3.tar` & `mandown-1.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    34520 2023-01-19 04:32:59.935926 mandown-1.3.3/LICENSE
--rw-r--r--   0        0        0     3819 2023-02-26 21:02:31.227352 mandown-1.3.3/README.md
--rw-r--r--   0        0        0      523 2023-01-24 02:20:51.102114 mandown-1.3.3/mandown/__init__.py
--rw-r--r--   0        0        0    11017 2023-03-17 14:44:13.814737 mandown-1.3.3/mandown/api.py
--rw-r--r--   0        0        0     1700 2022-12-31 01:43:12.048313 mandown-1.3.3/mandown/base.py
--rw-r--r--   0        0        0    15625 2023-02-17 04:19:10.504220 mandown-1.3.3/mandown/cli.py
--rw-r--r--   0        0        0     2564 2023-01-19 03:47:14.110630 mandown-1.3.3/mandown/comic.py
--rw-r--r--   0        0        0     5207 2023-01-29 00:06:55.288571 mandown-1.3.3/mandown/io.py
--rw-r--r--   0        0        0     5102 2023-01-29 00:07:27.899107 mandown-1.3.3/mandown/processor/__init__.py
--rw-r--r--   0        0        0     4109 2022-12-31 00:17:08.710330 mandown-1.3.3/mandown/processor/ops.py
--rw-r--r--   0        0        0     1603 2022-12-31 00:17:08.710330 mandown-1.3.3/mandown/processor/profiles.py
--rw-r--r--   0        0        0     1069 2022-12-28 04:11:26.754516 mandown-1.3.3/mandown/sources/__init__.py
--rw-r--r--   0        0        0     2017 2022-12-23 01:36:28.689150 mandown-1.3.3/mandown/sources/base_source.py
--rw-r--r--   0        0        0     4938 2023-01-29 00:08:10.853514 mandown-1.3.3/mandown/sources/source_mangadex.py
--rw-r--r--   0        0        0     2561 2022-10-06 18:48:03.141061 mandown-1.3.3/mandown/sources/source_mangakakalot.py
--rw-r--r--   0        0        0     2697 2023-03-16 22:50:42.471198 mandown-1.3.3/mandown/sources/source_manganato.py
--rw-r--r--   0        0        0     3744 2022-10-06 18:48:03.142061 mandown-1.3.3/mandown/sources/source_mangasee.py
--rw-r--r--   0        0        0     3617 2023-03-16 22:46:08.667522 mandown-1.3.3/mandown/sources/source_readcomiconline.py
--rw-r--r--   0        0        0     4116 2023-03-28 15:47:14.408606 mandown-1.3.3/mandown/sources/source_webtoons.py
--rw-r--r--   0        0        0     4597 2022-10-06 18:48:03.142061 mandown-1.3.3/mandown/ui/form.ui
--rw-r--r--   0        0        0     7214 2022-10-06 18:48:03.143061 mandown-1.3.3/mandown/ui/mainwin.py
--rw-r--r--   0        0        0       38 2022-10-06 18:48:03.143061 mandown-1.3.3/mandown/ui/mandown-qt.pyproject
--rw-r--r--   0        0        0     7049 2022-10-06 18:48:03.143061 mandown-1.3.3/mandown/ui/ui.py
--rw-r--r--   0        0        0     1384 2023-03-28 15:47:23.515423 mandown-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     5046 1970-01-01 00:00:00.000000 mandown-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-01-19 04:32:59.935926 mandown-1.3.4/LICENSE
+-rw-r--r--   0        0        0     3819 2023-02-26 21:02:31.227352 mandown-1.3.4/README.md
+-rw-r--r--   0        0        0      523 2023-04-27 21:56:31.915371 mandown-1.3.4/mandown/__init__.py
+-rw-r--r--   0        0        0    11018 2023-04-09 22:54:34.442921 mandown-1.3.4/mandown/api.py
+-rw-r--r--   0        0        0     1700 2022-12-31 01:43:12.048313 mandown-1.3.4/mandown/base.py
+-rw-r--r--   0        0        0    15780 2023-04-09 22:50:30.475038 mandown-1.3.4/mandown/cli.py
+-rw-r--r--   0        0        0     2564 2023-01-19 03:47:14.110630 mandown-1.3.4/mandown/comic.py
+-rw-r--r--   0        0        0     5549 2023-04-09 23:00:40.166019 mandown-1.3.4/mandown/io.py
+-rw-r--r--   0        0        0     5102 2023-01-29 00:07:27.899107 mandown-1.3.4/mandown/processor/__init__.py
+-rw-r--r--   0        0        0     4109 2022-12-31 00:17:08.710330 mandown-1.3.4/mandown/processor/ops.py
+-rw-r--r--   0        0        0     1603 2022-12-31 00:17:08.710330 mandown-1.3.4/mandown/processor/profiles.py
+-rw-r--r--   0        0        0     1428 2023-04-09 22:52:14.729134 mandown-1.3.4/mandown/sources/__init__.py
+-rw-r--r--   0        0        0     2017 2022-12-23 01:36:28.689150 mandown-1.3.4/mandown/sources/base_source.py
+-rw-r--r--   0        0        0     4938 2023-01-29 00:08:10.853514 mandown-1.3.4/mandown/sources/source_mangadex.py
+-rw-r--r--   0        0        0     2561 2022-10-06 18:48:03.141061 mandown-1.3.4/mandown/sources/source_mangakakalot.py
+-rw-r--r--   0        0        0     2697 2023-03-16 22:50:42.471198 mandown-1.3.4/mandown/sources/source_manganato.py
+-rw-r--r--   0        0        0     3744 2022-10-06 18:48:03.142061 mandown-1.3.4/mandown/sources/source_mangasee.py
+-rw-r--r--   0        0        0     3617 2023-03-16 22:46:08.667522 mandown-1.3.4/mandown/sources/source_readcomiconline.py
+-rw-r--r--   0        0        0     4116 2023-03-28 15:47:14.408606 mandown-1.3.4/mandown/sources/source_webtoons.py
+-rw-r--r--   0        0        0     4597 2022-10-06 18:48:03.142061 mandown-1.3.4/mandown/ui/form.ui
+-rw-r--r--   0        0        0     7214 2022-10-06 18:48:03.143061 mandown-1.3.4/mandown/ui/mainwin.py
+-rw-r--r--   0        0        0       38 2022-10-06 18:48:03.143061 mandown-1.3.4/mandown/ui/mandown-qt.pyproject
+-rw-r--r--   0        0        0     7049 2022-10-06 18:48:03.143061 mandown-1.3.4/mandown/ui/ui.py
+-rw-r--r--   0        0        0     1406 2023-04-27 21:56:20.091790 mandown-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5046 1970-01-01 00:00:00.000000 mandown-1.3.4/PKG-INFO
```

### Comparing `mandown-1.3.3/LICENSE` & `mandown-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/README.md` & `mandown-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/__init__.py` & `mandown-1.3.4/mandown/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     ProcessConfig,
     ProcessOps,
     ProcessOptionMismatchError,
     Processor,
 )
 from .processor.profiles import SupportedProfiles, all_profiles
 
-__version__ = (1, 3, 0)
+__version__ = (1, 3, 4)
 __version_str__ = ".".join(map(str, __version__))
```

### Comparing `mandown-1.3.3/mandown/api.py` & `mandown-1.3.4/mandown/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # pylint: disable=invalid-name
+
 import shutil
 from enum import Enum
 from pathlib import Path
 from typing import Iterator
 
 import comicon
```

### Comparing `mandown-1.3.3/mandown/base.py` & `mandown-1.3.4/mandown/base.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/cli.py` & `mandown-1.3.4/mandown/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,36 +381,38 @@
 
     size_profile = cast(SupportedProfiles | None, size_profile)
 
     # get and save metadata
     comic = cli_query(url)
 
     typer.echo(
-        f"Found item from source {sources.get_class_for(url).name}",
+        f'Found comic "{comic.metadata.title}" from source {sources.get_class_for(url).name}',
     )
 
     # get processing range
     start_chapter = start or 1
     end_chapter = end or len(comic.chapters)
 
     # zero-index
     start_chapter -= 1
 
     comic.set_chapter_range(start=start_chapter, end=end_chapter)
 
     # download
-    typer.echo("Downloading...")
+    typer.echo(f"Downloading {end_chapter - start_chapter} chapter(s)...")
     with typer.progressbar(
         api.download_progress(comic, dest, threads=maxthreads),
         length=len(comic.chapters),
     ) as progress:
         for title in progress:
             progress.label = title
+
+    full_dest_folder = dest.absolute() / comic.metadata.title
     typer.secho(
-        f"Successfully downloaded {end_chapter - start_chapter} chapters.",
+        f"Successfully downloaded {end_chapter - start_chapter} chapter(s) to {full_dest_folder}.",
         fg=typer.colors.GREEN,
     )
 
     # process
     if processing_options:
         try:
             config = ProcessConfig(
```

### Comparing `mandown-1.3.3/mandown/comic.py` & `mandown-1.3.4/mandown/comic.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/io.py` & `mandown-1.3.4/mandown/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     Raises ValueError if the folder does not exist.
 
     :param `urls`: A list of URLs to download.
     :param `dest_folder`: The path to download files into.
     :param `filestems`: Specify the name of each downloaded file instead of the default.
     :param `headers`: Request headers
     :param `threads`: The number of processes to open
-    :returns An iterator that yields `None` for each downloaded file.
+    :returns An Iterator that yields `None` for each downloaded file.
     """
     dest_folder = Path(dest_folder)
 
     # attempt to create
     dest_folder.mkdir(exist_ok=True)
 
     # args to async_download
@@ -103,18 +103,20 @@
         BaseMetadata(**data["metadata"]),
         [BaseChapter(**c) for c in data["chapters"]],
     )
 
 
 def parse_comic(path: Path | str, donor_comic: BaseComic | None = None) -> BaseComic:
     """
-    Parse and return an incomplete comic (without most metadata)
+    Attempt to construct a Mandown comic from a folder from the filesystem (without most metadata).
+    This function is non-destructive and does not modify the filesystem. If you want to save the
+    comic, call `save_comic` on the returned `BaseComic`.
 
     :param `path`: A folder containing images
-    :param `donor_comic`: A comic to fill unfilled metadata from
+    :param `donor_comic`: A comic to fill metadata from
     :returns A `BaseComic` with metadata and chapter data of that folder
     """
     path = Path(path)
 
     title = path.stem
     authors: list[str] = []
     url = ""
@@ -136,15 +138,16 @@
             local.url = remote.url
 
     return BaseComic(metadata, chapters)
 
 
 def save_comic(comic: BaseComic, path: Path | str) -> None:
     """
-    Save an `md-metadata.json` from `comic` into `path`.
+    Save an `md-metadata.json` from `comic` into `path`. If `path` does not exist, it will
+    be created. THIS FUNCTION IS DESTRUCTIVE AND WILL OVERWRITE ANY EXISTING `md-metadata.json`.
 
     :param `comic`: A comic to save
     :param `path`: A folder to save `md-metadata.json` into
     """
     path = Path(path)
     path.mkdir(exist_ok=True)
 
@@ -153,15 +156,15 @@
     with open(json_path, "w", encoding="utf-8") as file:
         json.dump(comic.asdict(), file)
 
 
 def discover_local_images(path: Path | str) -> dict[str, list[Path]]:
     """
     Given a comic path, return a dictionary of slugs: images.
-    Basically a slightly modified version of os.walk.
+    Basically a slightly modified version of os.walk. Only recurses one level deep.
 
     :param `path`: A folder containing images
     :returns A dictionary of {slugs: images}
     """
     path = Path(path)
 
     return {
```

### Comparing `mandown-1.3.3/mandown/processor/__init__.py` & `mandown-1.3.4/mandown/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/processor/ops.py` & `mandown-1.3.4/mandown/processor/ops.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/processor/profiles.py` & `mandown-1.3.4/mandown/processor/profiles.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/sources/base_source.py` & `mandown-1.3.4/mandown/sources/base_source.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/sources/source_mangadex.py` & `mandown-1.3.4/mandown/sources/source_mangadex.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/sources/source_mangakakalot.py` & `mandown-1.3.4/mandown/sources/source_mangakakalot.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/sources/source_manganato.py` & `mandown-1.3.4/mandown/sources/source_manganato.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/sources/source_mangasee.py` & `mandown-1.3.4/mandown/sources/source_mangasee.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/sources/source_readcomiconline.py` & `mandown-1.3.4/mandown/sources/source_readcomiconline.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/sources/source_webtoons.py` & `mandown-1.3.4/mandown/sources/source_webtoons.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/ui/form.ui` & `mandown-1.3.4/mandown/ui/form.ui`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/ui/mainwin.py` & `mandown-1.3.4/mandown/ui/mainwin.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/mandown/ui/ui.py` & `mandown-1.3.4/mandown/ui/ui.py`

 * *Files identical despite different names*

### Comparing `mandown-1.3.3/pyproject.toml` & `mandown-1.3.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mandown"
-version = "1.3.3"
+version = "1.3.4"
 description = "Comic/manga/webtoon downloader and CBZ/EPUB/PDF converter"
 authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/potatoeggy/mandown"
 documentation = "https://github.com/potatoeggy/mandown"
 keywords = ["manga", "comic", "downloader", "download", "webtoons", "webtoon"]
@@ -21,26 +21,27 @@
 requests = "^2.27.0"
 lxml = "^4.7.1"
 Pillow = "^9.0.1"
 python-slugify = "^6.1.2"
 PySide6 = {version = "^6.4.0", optional = true}
 natsort = "^8.1.0"
 filetype = "^1.1.0"
-comicon = "^0.2.2"
+comicon = "^0.2.3"
 
 [tool.poetry.dev-dependencies]
 types-requests = "^2.26.3"
 types-lxml = "^2022.4.10"
 pytest = "^7.2.0"
 
 [tool.poetry.extras]
 gui = ["PySide6"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = ["B", "C", "E", "F", "W"]
```

### Comparing `mandown-1.3.3/PKG-INFO` & `mandown-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mandown
-Version: 1.3.3
+Version: 1.3.4
 Summary: Comic/manga/webtoon downloader and CBZ/EPUB/PDF converter
 Home-page: https://github.com/potatoeggy/mandown
 License: AGPL-3.0-only
 Keywords: manga,comic,downloader,download,webtoons,webtoon
 Author: Daniel Chen
 Author-email: danielchen04@hotmail.ca
 Requires-Python: >=3.10,<3.12
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
 Requires-Dist: Pillow (>=9.0.1,<10.0.0)
 Requires-Dist: PySide6 (>=6.4.0,<7.0.0) ; extra == "gui"
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
-Requires-Dist: comicon (>=0.2.2,<0.3.0)
+Requires-Dist: comicon (>=0.2.3,<0.3.0)
 Requires-Dist: feedparser (>=6.0.8,<7.0.0)
 Requires-Dist: filetype (>=1.1.0,<2.0.0)
 Requires-Dist: lxml (>=4.7.1,<5.0.0)
 Requires-Dist: natsort (>=8.1.0,<9.0.0)
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
 Requires-Dist: requests (>=2.27.0,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
```

