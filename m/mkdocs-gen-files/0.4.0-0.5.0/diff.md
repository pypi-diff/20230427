# Comparing `tmp/mkdocs-gen-files-0.4.0.tar.gz` & `tmp/mkdocs_gen_files-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-gen-files-0.4.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mkdocs-gen-files-0.4.0.tar` & `mkdocs_gen_files-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,18 @@
--rw-r--r--   0        0        0     1083 2021-05-15 15:54:10.002604 mkdocs-gen-files-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     1526 2022-08-21 14:04:18.048188 mkdocs-gen-files-0.4.0/README.md
--rw-r--r--   0        0        0      510 2022-08-16 19:00:51.287702 mkdocs-gen-files-0.4.0/mkdocs_gen_files/__init__.py
--rw-r--r--   0        0        0     1116 2022-08-21 14:04:18.048188 mkdocs-gen-files-0.4.0/mkdocs_gen_files/config_items.py
--rw-r--r--   0        0        0     4433 2022-08-21 14:47:10.165791 mkdocs-gen-files-0.4.0/mkdocs_gen_files/editor.py
--rw-r--r--   0        0        0     2618 2021-05-31 14:52:38.568160 mkdocs-gen-files-0.4.0/mkdocs_gen_files/nav.py
--rw-r--r--   0        0        0     2248 2022-08-21 15:08:34.149827 mkdocs-gen-files-0.4.0/mkdocs_gen_files/plugin.py
--rw-r--r--   0        0        0        0 2022-08-21 14:33:32.896674 mkdocs-gen-files-0.4.0/mkdocs_gen_files/py.typed
--rw-r--r--   0        0        0     1295 2022-08-22 17:39:26.051365 mkdocs-gen-files-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2407 2022-08-22 17:39:28.788077 mkdocs-gen-files-0.4.0/setup.py
--rw-r--r--   0        0        0     2299 2022-08-22 17:39:28.788346 mkdocs-gen-files-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/mkdocs_gen_files/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/mkdocs_gen_files/config_items.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/mkdocs_gen_files/editor.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/mkdocs_gen_files/nav.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/mkdocs_gen_files/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/mkdocs_gen_files/py.typed
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/tests/test_editor.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/tests/test_nav.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/tests/nav/test_nav_basic.yml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/tests/nav/test_nav_chaotic.yml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/tests/nav/test_nav_empty.yml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/tests/nav/test_nav_special_chars.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/tests/nav/test_nav_with_index_item.yml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/README.md
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 mkdocs_gen_files-0.5.0/PKG-INFO
```

### Comparing `mkdocs-gen-files-0.4.0/LICENSE.md` & `mkdocs_gen_files-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-gen-files-0.4.0/README.md` & `mkdocs_gen_files-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # mkdocs-gen-files
 
 **[Plugin][] for [MkDocs][] to programmatically generate documentation pages during the build**
 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-gen-files)](https://pypi.org/project/mkdocs-gen-files/)
 [![GitHub](https://img.shields.io/github/license/oprypin/mkdocs-gen-files)](https://github.com/oprypin/mkdocs-gen-files/blob/master/LICENSE.md)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/oprypin/mkdocs-gen-files/CI)](https://github.com/oprypin/mkdocs-gen-files/actions?query=event%3Apush+branch%3Amaster)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oprypin/mkdocs-gen-files/ci.yml.svg)](https://github.com/oprypin/mkdocs-gen-files/actions?query=event%3Apush+branch%3Amaster)
 
 ```shell
 pip install mkdocs-gen-files
 ```
 
 **Continue to the [documentation site][].**
```

### Comparing `mkdocs-gen-files-0.4.0/mkdocs_gen_files/config_items.py` & `mkdocs_gen_files-0.5.0/mkdocs_gen_files/config_items.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from mkdocs.config.config_options import File, OptionallyRequired, ValidationError
 
 
 class ListOfItems(OptionallyRequired):
     def __init__(self, option_type, default=[], required=False):
         super().__init__(default=None if required else default, required=required)
         self.option_type = option_type
```

### Comparing `mkdocs-gen-files-0.4.0/mkdocs_gen_files/editor.py` & `mkdocs_gen_files-0.5.0/mkdocs_gen_files/editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 import collections
 import os
 import os.path
 import pathlib
 import shutil
-from typing import IO, ClassVar, MutableMapping, Optional
+from typing import IO, ClassVar, MutableMapping
 
 from mkdocs.config import Config, load_config
 from mkdocs.structure.files import File, Files
 
 
 def file_sort_key(f: File):
     parts = pathlib.PurePath(f.src_path).parts
@@ -17,15 +19,15 @@
 
 
 class FilesEditor:
     config: Config
     """The current MkDocs [config](https://www.mkdocs.org/user-guide/plugins/#config)."""
     directory: str
     """The base directory for `open()` ([docs_dir](https://www.mkdocs.org/user-guide/configuration/#docs_dir))."""
-    edit_paths: MutableMapping[str, Optional[str]]
+    edit_paths: MutableMapping[str, str | None]
 
     def open(self, name: str, mode, buffering=-1, encoding=None, *args, **kwargs) -> IO:
         """Open a file under `docs_dir` virtually.
 
         This function, for all intents and purposes, is just an `open()` which pretends that it is
         running under [docs_dir](https://www.mkdocs.org/user-guide/configuration/#docs_dir)
         (*docs/* by default), but write operations don't affect the actual files when running as
@@ -39,14 +41,15 @@
     def _get_file(self, name: str, new: bool = False) -> str:
         new_f = File(
             name,
             src_dir=self.directory,
             dest_dir=self.config["site_dir"],
             use_directory_urls=self.config["use_directory_urls"],
         )
+        new_f.generated_by = "mkdocs-gen-files"  # type: ignore
         normname = pathlib.PurePath(name).as_posix()
 
         if new or normname not in self._files:
             os.makedirs(os.path.dirname(new_f.abs_src_path), exist_ok=True)
             self._files[normname] = new_f
             self.edit_paths.setdefault(normname, None)
             return new_f.abs_src_path
@@ -57,33 +60,33 @@
             self._files[normname] = new_f
             self.edit_paths.setdefault(normname, None)
             shutil.copyfile(f.abs_src_path, new_f.abs_src_path)
             return new_f.abs_src_path
 
         return f.abs_src_path
 
-    def set_edit_path(self, name: str, edit_name: Optional[str]) -> None:
+    def set_edit_path(self, name: str, edit_name: str | None) -> None:
         """Choose a file path to use for the edit URI of this file."""
         self.edit_paths[pathlib.PurePath(name).as_posix()] = edit_name and str(edit_name)
 
-    def __init__(self, files: Files, config: Config, directory: Optional[str] = None):
+    def __init__(self, files: Files, config: Config, directory: str | None = None):
         self._files: MutableMapping[str, File] = collections.ChainMap(
             {}, {pathlib.PurePath(f.src_path).as_posix(): f for f in files}
         )
         self.config = config
         if directory is None:
             directory = config["docs_dir"]
         self.directory = directory
         self.edit_paths = {}
 
-    _current: ClassVar[Optional["FilesEditor"]] = None
-    _default: ClassVar[Optional["FilesEditor"]] = None
+    _current: ClassVar[FilesEditor | None] = None
+    _default: ClassVar[FilesEditor | None] = None
 
     @classmethod
-    def current(cls) -> "FilesEditor":
+    def current(cls) -> FilesEditor:
         """The instance of FilesEditor associated with the currently ongoing MkDocs build.
 
         If used as part of a MkDocs build (*gen-files* plugin), it's an instance using virtual
         files that feed back into the build.
 
         If not, this still tries to load the MkDocs config to find out the *docs_dir*, and then
         actually performs any file writes that happen via `.open()`.
```

### Comparing `mkdocs-gen-files-0.4.0/mkdocs_gen_files/nav.py` & `mkdocs_gen_files-0.5.0/mkdocs_gen_files/nav.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from __future__ import annotations
+
 import dataclasses
 import os
-from typing import Iterable, Mapping, Optional, Tuple, Union
+from typing import Iterable, Mapping
 
 
 class Nav:
     """An object representing MkDocs navigation, consisting of files under nested sequences of
     titles, which are treated like paths.
     """
 
     def __init__(self):
         self._data = {}
 
-    def __setitem__(self, keys: Union[str, Tuple[str, ...]], value: str):
+    def __setitem__(self, keys: str | tuple[str, ...], value: str):
         """Add a link to a file (*value*) into the nav, under the sequence of titles (*keys*).
 
         For example, writing `nav["Foo", "Bar"] = "foo/bar.md"` would mean creating a nav:
         `{"Foo": {"Bar": "foo/bar.md"}}`.
 
         Then, writing `nav["Foo", "Another"] = "test.md"` would merge with the existing sections
         where possible:
@@ -39,29 +41,29 @@
             cur = cur.setdefault(key, {})
         cur[None] = os.fspath(value)
 
     @dataclasses.dataclass
     class Item:
         level: int
         title: str
-        filename: Optional[str]
+        filename: str | None
 
     def items(self) -> Iterable[Item]:
         return self._items(self._data, 0)
 
     @classmethod
     def _items(cls, data: Mapping, level: int) -> Iterable[Item]:
         for key, value in data.items():
             if key is not None:
                 yield cls.Item(level=level, title=key, filename=value.get(None))
                 yield from cls._items(value, level + 1)
 
     _markdown_escape_chars = tuple("!#()*+-[\\]_`{}")
 
-    def build_literate_nav(self, indentation: Union[int, str] = "") -> Iterable[str]:
+    def build_literate_nav(self, indentation: int | str = "") -> Iterable[str]:
         if isinstance(indentation, int):
             indentation = " " * indentation
         for item in self.items():
             line = item.title
             if line.startswith(self._markdown_escape_chars):
                 line = "\\" + line
             if item.filename is not None:
```

### Comparing `mkdocs-gen-files-0.4.0/mkdocs_gen_files/plugin.py` & `mkdocs_gen_files-0.5.0/mkdocs_gen_files/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
+from __future__ import annotations
+
 import logging
 import pathlib
 import runpy
 import tempfile
 import urllib.parse
 
-import mkdocs.utils
 from mkdocs.config import Config
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import Files
 from mkdocs.structure.pages import Page
 
 try:
     from mkdocs.exceptions import PluginError
 except ImportError:
     PluginError = SystemExit  # type: ignore
 
 from .config_items import ListOfFiles
 from .editor import FilesEditor
 
+try:
+    from mkdocs.plugins import event_priority
+except ImportError:
+    event_priority = lambda priority: lambda f: f  # No-op fallback
+
 log = logging.getLogger(f"mkdocs.plugins.{__name__}")
-log.addFilter(mkdocs.utils.warning_filter)
 
 
 class GenFilesPlugin(BasePlugin):
     config_scheme = (("scripts", ListOfFiles(required=True)),)
 
     def on_files(self, files: Files, config: Config) -> Files:
         self._dir = tempfile.TemporaryDirectory(prefix="mkdocs_gen_files_")
@@ -53,14 +58,15 @@
 
                 page.edit_url = path and urllib.parse.urljoin(
                     urllib.parse.urljoin(repo_url, edit_uri), path
                 )
 
         return html
 
+    @event_priority(-100)
     def on_post_build(self, config: Config):
         self._dir.cleanup()
 
         unused_edit_paths = {k: str(v) for k, v in self._edit_paths.items() if v}
         if unused_edit_paths:
             msg = "mkdocs_gen_files: These set_edit_path invocations went unused (the files don't exist): %r"
             log.warning(msg, unused_edit_paths)
```

### Comparing `mkdocs-gen-files-0.4.0/PKG-INFO` & `mkdocs_gen_files-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 Metadata-Version: 2.1
 Name: mkdocs-gen-files
-Version: 0.4.0
+Version: 0.5.0
 Summary: MkDocs plugin to programmatically generate documentation pages during the build
-Home-page: https://github.com/oprypin/mkdocs-gen-files
-License: MIT
+Project-URL: Documentation, https://oprypin.github.io/mkdocs-gen-files/
+Project-URL: Source, https://github.com/oprypin/mkdocs-gen-files
+Project-URL: Issues, https://github.com/oprypin/mkdocs-gen-files/issues
+Project-URL: History, https://github.com/oprypin/mkdocs-gen-files/releases
+Author-email: Oleh Prypin <oleh@pryp.in>
+License-Expression: MIT
+License-File: LICENSE.md
 Keywords: mkdocs,mkdocs-plugin
-Author: Oleh Prypin
-Author-email: oleh@pryp.in
-Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: mkdocs (>=1.0.3,<2.0.0)
-Project-URL: Repository, https://github.com/oprypin/mkdocs-gen-files
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Requires-Dist: mkdocs>=1.0.3
 Description-Content-Type: text/markdown
 
 # mkdocs-gen-files
 
 **[Plugin][] for [MkDocs][] to programmatically generate documentation pages during the build**
 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-gen-files)](https://pypi.org/project/mkdocs-gen-files/)
 [![GitHub](https://img.shields.io/github/license/oprypin/mkdocs-gen-files)](https://github.com/oprypin/mkdocs-gen-files/blob/master/LICENSE.md)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/oprypin/mkdocs-gen-files/CI)](https://github.com/oprypin/mkdocs-gen-files/actions?query=event%3Apush+branch%3Amaster)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oprypin/mkdocs-gen-files/ci.yml.svg)](https://github.com/oprypin/mkdocs-gen-files/actions?query=event%3Apush+branch%3Amaster)
 
 ```shell
 pip install mkdocs-gen-files
 ```
 
 **Continue to the [documentation site][].**
 
@@ -56,8 +68,7 @@
 with mkdocs_gen_files.open("foo.md", "w") as f:
     print("Hello, world!", file=f)
 ```
 
 This added a programmatically generated page to our site. That is, the document doesn't actually appear in our source files, it only *virtually* becomes part of the site to be built by MkDocs.
 
 **Continue to the [documentation site][].**
-
```

