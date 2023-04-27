# Comparing `tmp/geovisio_cli-0.0.4.tar.gz` & `tmp/geovisio_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.0.4.tar", last modified: Fri Apr 14 11:24:02 2023, max compression
+gzip compressed data, was "geovisio_cli-0.0.5.tar", last modified: Thu Apr 27 14:19:43 2023, max compression
```

## Comparing `geovisio_cli-0.0.4.tar` & `geovisio_cli-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/.gitignore
--rw-r--r--   0        0        0     1732 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/.gitlab-ci.yml
--rw-r--r--   0        0        0     1527 2023-04-14 11:18:33.201654 geovisio_cli-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/LICENSE
--rw-r--r--   0        0        0      551 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/Makefile
--rw-r--r--   0        0        0     4632 2023-04-14 07:21:46.587626 geovisio_cli-0.0.4/README.md
--rw-r--r--   0        0        0     2320 2023-04-14 07:21:46.587626 geovisio_cli-0.0.4/USAGE.md
--rw-r--r--   0        0        0       53 2023-04-14 11:18:33.205654 geovisio_cli-0.0.4/geovisio_cli/__init__.py
--rw-r--r--   0        0        0     1972 2023-04-14 11:12:54.559203 geovisio_cli-0.0.4/geovisio_cli/auth.py
--rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.0.4/geovisio_cli/exception.py
--rw-r--r--   0        0        0     3621 2023-04-14 07:21:46.587626 geovisio_cli-0.0.4/geovisio_cli/main.py
--rw-r--r--   0        0        0      173 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/geovisio_cli/model.py
--rw-r--r--   0        0        0    13940 2023-04-14 11:12:54.559203 geovisio_cli-0.0.4/geovisio_cli/sequence.py
--rw-r--r--   0        0        0      896 2023-03-14 16:32:00.535627 geovisio_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/integration/__init__.py
--rw-r--r--   0        0        0      865 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/integration/conftest.py
--rw-r--r--   0        0        0      671 2023-03-14 16:32:00.535627 geovisio_cli-0.0.4/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      319 2023-04-07 07:41:38.712978 geovisio_cli-0.0.4/tests/integration/test_status.py
--rw-r--r--   0        0        0     4914 2023-04-14 11:12:54.559203 geovisio_cli-0.0.4/tests/integration/test_upload.py
--rw-r--r--   0        0        0      528 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/tests/test_process.py
--rw-r--r--   0        0        0      813 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/tests/test_sequence.py
--rw-r--r--   0        0        0     5491 1970-01-01 00:00:00.000000 geovisio_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1732 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1714 2023-04-27 14:14:42.006482 geovisio_cli-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/LICENSE
+-rw-r--r--   0        0        0      551 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/Makefile
+-rw-r--r--   0        0        0     7328 2023-04-27 14:14:42.006482 geovisio_cli-0.0.5/README.md
+-rw-r--r--   0        0        0     2320 2023-04-14 07:21:46.587626 geovisio_cli-0.0.5/USAGE.md
+-rw-r--r--   0        0        0       53 2023-04-27 14:14:42.006482 geovisio_cli-0.0.5/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0     1972 2023-04-14 11:12:54.559203 geovisio_cli-0.0.5/geovisio_cli/auth.py
+-rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.0.5/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     3621 2023-04-14 07:21:46.587626 geovisio_cli-0.0.5/geovisio_cli/main.py
+-rw-r--r--   0        0        0      173 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/geovisio_cli/model.py
+-rw-r--r--   0        0        0    14418 2023-04-24 11:28:19.596669 geovisio_cli-0.0.5/geovisio_cli/sequence.py
+-rw-r--r--   0        0        0      896 2023-03-14 16:32:00.535627 geovisio_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.0.5/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/integration/__init__.py
+-rw-r--r--   0        0        0      865 2023-03-14 15:26:20.141986 geovisio_cli-0.0.5/tests/integration/conftest.py
+-rw-r--r--   0        0        0      671 2023-03-14 16:32:00.535627 geovisio_cli-0.0.5/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      319 2023-04-07 07:41:38.712978 geovisio_cli-0.0.5/tests/integration/test_status.py
+-rw-r--r--   0        0        0     4914 2023-04-14 11:12:54.559203 geovisio_cli-0.0.5/tests/integration/test_upload.py
+-rw-r--r--   0        0        0      528 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/tests/test_process.py
+-rw-r--r--   0        0        0      813 2023-03-24 13:15:13.689899 geovisio_cli-0.0.5/tests/test_sequence.py
+-rw-r--r--   0        0        0     8187 1970-01-01 00:00:00.000000 geovisio_cli-0.0.5/PKG-INFO
```

### Comparing `geovisio_cli-0.0.4/.gitlab-ci.yml` & `geovisio_cli-0.0.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/CHANGELOG.md` & `geovisio_cli-0.0.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+
+## [0.0.5] - 2023-04-27
+
+### Fixed
+- Add a timeout to avoid `requests` module to hang forever if API is not responding
+
+
 ## [0.0.4] - 2023-04-14
 
 ### Changed
 - Changed the `--path` option of the `geovisio upload` command to a positional argument since it seems more ergonomic. So now `geovisio upload --api-url <some_url> --path <some dir>` is replaced by `geovisio upload --api-url <some_url> <some dir>` (or `geovisio upload <some dir> --api-url <some_url>` since the parameters order is not relevant)
 - Improve some error messages
 
 ## [0.0.3] - 2023-04-12
@@ -28,12 +35,13 @@
 
 ## [0.0.1] - 2023-03-14
 
 ### Added
 - Basic scripts for uploading pictures to a GeoVisio API
 
 
-[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.0.2...main
+[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.0.5...main
+[0.0.5]: https://gitlab.com/geovisio/cli/-/compare/0.0.4...0.0.5
 [0.0.4]: https://gitlab.com/geovisio/cli/-/compare/0.0.3...0.0.4
 [0.0.3]: https://gitlab.com/geovisio/cli/-/compare/0.0.2...0.0.3
 [0.0.2]: https://gitlab.com/geovisio/cli/-/compare/0.0.1...0.0.2
 [0.0.1]: https://gitlab.com/PanierAvide/geovisio/-/commits/0.0.1
```

### Comparing `geovisio_cli-0.0.4/CODE_OF_CONDUCT.md` & `geovisio_cli-0.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/LICENSE` & `geovisio_cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/Makefile` & `geovisio_cli-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/USAGE.md` & `geovisio_cli-0.0.5/USAGE.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/geovisio_cli/auth.py` & `geovisio_cli-0.0.5/geovisio_cli/auth.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/geovisio_cli/main.py` & `geovisio_cli-0.0.5/geovisio_cli/main.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/geovisio_cli/sequence.py` & `geovisio_cli-0.0.5/geovisio_cli/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path, PurePath
 from dataclasses import dataclass, field
-from typing import List, Optional
+from typing import List, Optional, Union
 import requests
 from rich import print
 from rich.table import Table
 from rich.markup import escape
 from rich.progress import (
     Progress,
     SpinnerColumn,
@@ -18,14 +18,16 @@
 from rich.live import Live
 from geovisio_cli.exception import CliException, raise_for_status
 from geovisio_cli.auth import login
 from geovisio_cli.model import Geovisio
 from time import sleep
 from datetime import timedelta
 
+REQUESTS_TIMEOUT = 5
+
 
 @dataclass
 class Picture:
     path: str
 
 
 @dataclass
@@ -34,15 +36,15 @@
     pictures: List[Picture] = field(default_factory=lambda: [])
 
 
 @dataclass
 class UploadError:
     position: int
     picture_path: str
-    error: str
+    error: Union[str, dict]
     status_code: int
 
 
 @dataclass
 class UploadedPicture:
     path: str
     location: str
@@ -119,18 +121,22 @@
     print(f'📂 Publishing "{sequence.title}"')
 
     data = {}
     if sequence.title:
         data["title"] = sequence.title
 
     with requests.session() as s:
-        seq = s.post(f"{geovisio.url}/api/collections", data=data)
+        seq = s.post(
+            f"{geovisio.url}/api/collections", data=data, timeout=REQUESTS_TIMEOUT
+        )
         if seq.status_code == 401:
             login(s, geovisio)
-            seq = s.post(f"{geovisio.url}/api/collections", data=data)
+            seq = s.post(
+                f"{geovisio.url}/api/collections", data=data, timeout=REQUESTS_TIMEOUT
+            )
         raise_for_status(seq, "Impossible to query geovisio")
 
         seq_location = seq.headers["Location"]
         print(f"✅ Created collection {seq_location}")
         report = UploadReport(location=seq_location)
 
         uploading_progress = Progress(
@@ -170,14 +176,15 @@
                 picture_response = s.post(
                     f"{seq_location}/items",
                     files={"picture": open(p.path, "rb")},
                     data={
                         "position": i,
                         "isBlurred": "true" if alreadyBlurred else "false",
                     },
+                    timeout=REQUESTS_TIMEOUT,
                 )
                 if picture_response.status_code >= 400:
                     body = (
                         picture_response.json()
                         if picture_response.headers.get("Content-Type")
                         == "application/json"
                         else picture_response.text
@@ -211,15 +218,17 @@
         else:
             print(
                 f"🎉 [bold green]{len(report.uploaded_pictures)}[/bold green] pictures uploaded"
             )
         if report.errors:
             print(f"[bold red]{len(report.errors)}[/bold red] pictures not uploaded:")
             for e in report.errors:
-                msg = escape(e.error.replace("\n", "\\n"))
+                msg: Union[str, dict] = e.error
+                if isinstance(e.error, str):
+                    msg = escape(e.error.replace("\n", "\\n"))
                 print(f" - {e.picture_path} (status [bold]{e.status_code}[/]): {msg}")
 
         if wait:
             wait_for_sequence(seq_location)
         else:
             print(f"Note: You can follow the picture processing with the command:")
             from rich.syntax import Syntax
@@ -274,16 +283,21 @@
 
     return s
 
 
 def _test_geovisio_url(geovisio: str):
     full_url = f"{geovisio}/api/collections"
     try:
-        r = requests.get(full_url)
-    except requests.ConnectionError as e:
+        r = requests.get(full_url, timeout=REQUESTS_TIMEOUT)
+    except (
+        requests.Timeout,
+        requests.ConnectionError,
+        requests.ConnectTimeout,
+        requests.TooManyRedirects,
+    ) as e:
         raise CliException(
             f"""The API is not reachable. Please check error and used URL below, and retry later if the URL is correct.
 
 [bold]Used URL:[/bold] {full_url}
 [bold]Error:[/bold]
 {e}"""
         )
@@ -313,29 +327,29 @@
 [bold]Used URL:[/bold] {full_url}
 [bold]Error[/bold] (code [cyan]{r.status_code}[/cyan]):
 {r.text}"""
         )
 
 
 def status(sequence_location: str) -> SequenceStatus:
-    s = requests.get(f"{sequence_location}/geovisio_status")
+    s = requests.get(f"{sequence_location}/geovisio_status", timeout=REQUESTS_TIMEOUT)
     if s.status_code == 404:
         raise CliException(f"Sequence {sequence_location} not found")
     if s.status_code >= 400:
         raise CliException(
             f"Impossible to get sequence {sequence_location} status: {s.text}"
         )
     r = s.json()
     return SequenceStatus(
         pictures=[PictureStatus(id=p["id"], status=p["status"]) for p in r["items"]]
     )
 
 
 def info(sequence_location: str) -> GeovisioSequence:
-    s = requests.get(sequence_location)
+    s = requests.get(sequence_location, timeout=REQUESTS_TIMEOUT)
     if s.status_code == 404:
         raise CliException(f"Sequence {sequence_location} not found")
     if s.status_code >= 400:
         raise CliException(
             f"Impossible to get sequence {sequence_location} status: {s.text}"
         )
     r = s.json()
```

### Comparing `geovisio_cli-0.0.4/pyproject.toml` & `geovisio_cli-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/tests/fixtures/e1.jpg` & `geovisio_cli-0.0.5/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/tests/fixtures/e2.jpg` & `geovisio_cli-0.0.5/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/tests/fixtures/e3.jpg` & `geovisio_cli-0.0.5/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/tests/integration/conftest.py` & `geovisio_cli-0.0.5/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/tests/integration/docker-compose-geovisio.yml` & `geovisio_cli-0.0.5/tests/integration/docker-compose-geovisio.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/tests/integration/test_upload.py` & `geovisio_cli-0.0.5/tests/integration/test_upload.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/tests/test_process.py` & `geovisio_cli-0.0.5/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/tests/test_sequence.py` & `geovisio_cli-0.0.5/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.4/PKG-INFO` & `geovisio_cli-0.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-Metadata-Version: 2.1
-Name: geovisio_cli
-Version: 0.0.4
-Summary: Geovio client cli tool
-Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: requests ~= 2.28.0
-Requires-Dist: typer ~= 0.7.0
-Requires-Dist: rich[all] ~= 13.3.0
-Requires-Dist: flit ~= 3.8.0 ; extra == "build"
-Requires-Dist: black ~= 22.8.0 ; extra == "dev"
-Requires-Dist: mypy ~= 1.0.0 ; extra == "dev"
-Requires-Dist: types-requests ~= 2.28.0 ; extra == "dev"
-Requires-Dist: pytest ~= 7.2.0 ; extra == "dev"
-Requires-Dist: testcontainers-compose ~= 0.0.1rc1 ; extra == "dev"
-Requires-Dist: pytest-datafiles ~= 2.0.1 ; extra == "dev"
-Requires-Dist: typer-cli ~= 0.0.13 ; extra == "dev"
-Project-URL: Home, https://gitlab.com/geovisio/cli
-Provides-Extra: build
-Provides-Extra: dev
+# ![GeoVisio](https://gitlab.com/geovisio/api/-/raw/develop/images/logo_full.png)
 
-# [GeoVisio](https://gitlab.com/geovisio/api) Command Line Interface (cli)
+__GeoVisio__ is a complete solution for storing and __serving your own 📍📷 geolocated pictures__ (like [StreetView](https://www.google.com/streetview/) / [Mapillary](https://mapillary.com/)).
 
-![GeoVisio logo](https://gitlab.com/geovisio/api/-/raw/develop/images/logo_full.png)
+➡️ __Give it a try__ at [panoramax.ign.fr](https://panoramax.ign.fr/) or [geovisio.fr](https://geovisio.fr/viewer) !
 
-Command Line Interface tool to interact with a [Geovisio](https://gitlab.com/geovisio/api) instance.
+## 📦 Components
 
-[[_TOC_]]
+GeoVisio is __modular__ and made of several components, each of them standardized and ♻️ replaceable.
 
+![GeoVisio architecture](https://gitlab.com/geovisio/api/-/raw/develop/images/big_picture.png)
+
+All of them are 📖 __open-source__ and available online:
+
+|                               🌐 Server                                 |                      💻 Client                       |
+|:-----------------------------------------------------------------------:|:----------------------------------------------------:|
+|                 [API](https://gitlab.com/geovisio/api)                  |    [Website](https://gitlab.com/geovisio/website)    |
+|            [Blur API](https://gitlab.com/geovisio/blurring)             | [Web viewer](https://gitlab.com/geovisio/web-viewer) |
+| [GeoPic Tag Reader](https://gitlab.com/geovisio/geo-picture-tag-reader) |   [Command line](https://gitlab.com/geovisio/cli)    |
+
+
+# ⌨️ GeoVisio Command-line scripts
+
+This repository only contains __command-line interface (CLI)__.
 
 ## Features
 
 This tool allows you to:
 
 - Upload a sequence of pictures on a GeoVisio API
 
-It is under __heavy development__, new features will appear in a near future 😉
+It is under __development__, new features will appear in a near future 😉
 
 
 ## Install
 
 GeoVisio CLI can be installed using two methods:
 
 - From [PyPI](https://pypi.org/project/geovisio_cli/), the Python central package repository
@@ -180,12 +174,41 @@
 
 Note that before opening a pull requests, you may want to check formatting and tests of your changes:
 
 ```bash
 make ci
 ```
 
+### Make a release
+
+```bash
+git checkout main
+git pull
+
+make docs ci
+vim CHANGELOG.md							# Edit version + links at bottom
+vim geovisio_cli/__init__.py	# Edit version
+
+git add *
+git commit -m "Release x.x.x"
+git tag -a x.x.x -m "Release x.x.x"
+git push origin main --tags
+```
+
+
+## 🤗 Special thanks
+
+![Sponsors](https://gitlab.com/geovisio/api/-/raw/develop/images/sponsors.png)
+
+GeoVisio was made possible thanks to a group of ✨ __amazing__ people ✨ :
+
+- __[GéoVélo](https://geovelo.fr/)__ team, for 💶 funding initial development and for 🔍 testing/improving software
+- __[Carto Cité](https://cartocite.fr/)__ team (in particular Antoine Riche), for 💶 funding improvements on viewer (map browser, flat pictures support)
+- __[La Fabrique des Géocommuns (IGN)](https://www.ign.fr/institut/la-fabrique-des-geocommuns-incubateur-de-communs-lign)__ for offering long-term support and funding the [Panoramax](https://panoramax.fr/) initiative and core team (Camille Salou, Mathilde Ferrey, Christian Quest, Antoine Desbordes, Jean Andreani, Adrien Pavie)
+- Many _many_ __wonderful people__ who worked on various parts of GeoVisio or core dependencies we use : 🧙 Stéphane Péneau, 🎚 Albin Calais & Cyrille Giquello, 📷 [Damien Sorel](https://www.strangeplanet.fr/), Pascal Rhod, Nick Whitelegg...
+- __[Adrien Pavie](https://pavie.info/)__, for ⚙️ initial development of GeoVisio
+- And you all ✨ __GeoVisio users__ for making this project useful !
 
-## License
 
-Copyright (c) GeoVisio team 2022-2023, [released under MIT license](./LICENSE).
+## ⚖️ License
 
+Copyright (c) GeoVisio team 2022-2023, [released under MIT license](https://gitlab.com/geovisio/cli/-/blob/main/LICENSE).
```

