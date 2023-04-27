# Comparing `tmp/rich-9.8.2.tar.gz` & `tmp/rich-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich-9.8.2.tar", last modified: Fri Jan 15 10:08:04 2021, max compression
+gzip compressed data, was "rich-9.9.0.tar", last modified: Sat Jan 23 15:43:09 2021, max compression
```

## Comparing `rich-9.8.2.tar` & `rich-9.9.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0     1053 2020-01-24 13:59:03.998541 rich-9.8.2/LICENSE
--rw-r--r--   0        0        0    15351 2021-01-09 20:38:57.332285 rich-9.8.2/README.md
--rw-r--r--   0        0        0     1337 2021-01-15 10:07:53.399936 rich-9.8.2/pyproject.toml
--rw-r--r--   0        0        0     3954 2021-01-11 21:16:14.970935 rich-9.8.2/rich/__init__.py
--rw-r--r--   0        0        0     7199 2020-12-18 15:34:31.166977 rich-9.8.2/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-06-09 21:31:38.948386 rich-9.8.2/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-06-09 22:25:04.834263 rich-9.8.2/rich/_emoji_codes.py
--rw-r--r--   0        0        0      462 2021-01-05 17:28:01.831941 rich-9.8.2/rich/_emoji_replace.py
--rw-r--r--   0        0        0     8399 2021-01-13 16:59:49.670786 rich-9.8.2/rich/_inspect.py
--rw-r--r--   0        0        0     2607 2020-12-11 15:15:43.912219 rich-9.8.2/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2021-01-07 21:28:10.706134 rich-9.8.2/rich/_loop.py
--rw-r--r--   0        0        0     1185 2020-06-21 11:32:35.980180 rich-9.8.2/rich/_lru_cache.py
--rw-r--r--   0        0        0     6808 2020-08-05 09:09:12.004145 rich-9.8.2/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-08-28 11:51:20.729571 rich-9.8.2/rich/_pick.py
--rw-r--r--   0        0        0     2285 2020-09-12 13:30:35.534784 rich-9.8.2/rich/_ratio.py
--rw-r--r--   0        0        0    26521 2020-12-11 15:15:49.785731 rich-9.8.2/rich/_spinners.py
--rw-r--r--   0        0        0      351 2019-11-24 14:46:58.448301 rich-9.8.2/rich/_stack.py
--rw-r--r--   0        0        0     2000 2020-10-12 15:57:19.913343 rich-9.8.2/rich/_windows.py
--rw-r--r--   0        0        0     1804 2020-07-03 18:27:02.615856 rich-9.8.2/rich/_wrap.py
--rw-r--r--   0        0        0      878 2021-01-10 12:35:52.850658 rich-9.8.2/rich/abc.py
--rw-r--r--   0        0        0     7350 2021-01-11 21:16:14.971250 rich-9.8.2/rich/align.py
--rw-r--r--   0        0        0     6663 2021-01-11 11:08:08.719159 rich-9.8.2/rich/ansi.py
--rw-r--r--   0        0        0     3150 2020-12-11 15:15:43.913989 rich-9.8.2/rich/bar.py
--rw-r--r--   0        0        0     8910 2021-01-04 15:26:55.320533 rich-9.8.2/rich/box.py
--rw-r--r--   0        0        0     3660 2020-08-29 15:29:10.069455 rich-9.8.2/rich/cells.py
--rw-r--r--   0        0        0    17094 2021-01-09 15:38:20.580108 rich-9.8.2/rich/color.py
--rw-r--r--   0        0        0     1054 2020-09-25 12:10:56.450457 rich-9.8.2/rich/color_triplet.py
--rw-r--r--   0        0        0     7104 2020-12-11 15:15:49.787469 rich-9.8.2/rich/columns.py
--rw-r--r--   0        0        0    60796 2021-01-11 21:41:18.566736 rich-9.8.2/rich/console.py
--rw-r--r--   0        0        0     1261 2020-10-23 15:44:06.158139 rich-9.8.2/rich/constrain.py
--rw-r--r--   0        0        0     5285 2020-12-30 14:56:17.500247 rich-9.8.2/rich/containers.py
--rw-r--r--   0        0        0     1298 2020-08-28 11:51:20.929811 rich-9.8.2/rich/control.py
--rw-r--r--   0        0        0     6385 2021-01-09 15:32:13.516324 rich-9.8.2/rich/default_styles.py
--rw-r--r--   0        0        0      159 2020-12-12 12:02:59.728991 rich-9.8.2/rich/diagnose.py
--rw-r--r--   0        0        0     1962 2020-09-16 15:30:21.104796 rich-9.8.2/rich/emoji.py
--rw-r--r--   0        0        0      493 2020-03-14 21:59:04.157954 rich-9.8.2/rich/errors.py
--rw-r--r--   0        0        0     1657 2020-12-18 15:34:31.169096 rich-9.8.2/rich/file_proxy.py
--rw-r--r--   0        0        0     1884 2020-06-21 11:32:35.988808 rich-9.8.2/rich/filesize.py
--rw-r--r--   0        0        0     4343 2021-01-08 21:59:36.405771 rich-9.8.2/rich/highlighter.py
--rw-r--r--   0        0        0     2369 2020-12-11 15:15:43.917109 rich-9.8.2/rich/jupyter.py
--rw-r--r--   0        0        0    13707 2021-01-15 10:07:53.400903 rich-9.8.2/rich/live.py
--rw-r--r--   0        0        0     2563 2020-12-02 22:14:56.136173 rich-9.8.2/rich/live_render.py
--rw-r--r--   0        0        0     9896 2020-12-30 15:29:21.556058 rich-9.8.2/rich/logging.py
--rw-r--r--   0        0        0    20301 2021-01-11 21:16:14.973877 rich-9.8.2/rich/markdown.py
--rw-r--r--   0        0        0     5598 2021-01-08 20:19:05.815192 rich-9.8.2/rich/markup.py
--rw-r--r--   0        0        0     5213 2020-10-18 11:07:41.415689 rich-9.8.2/rich/measure.py
--rw-r--r--   0        0        0     4419 2020-10-03 10:33:06.488124 rich-9.8.2/rich/padding.py
--rw-r--r--   0        0        0      759 2020-10-16 13:53:51.312360 rich-9.8.2/rich/pager.py
--rw-r--r--   0        0        0     3250 2020-12-28 18:12:38.808843 rich-9.8.2/rich/palette.py
--rw-r--r--   0        0        0     6866 2021-01-11 21:16:14.974208 rich-9.8.2/rich/panel.py
--rw-r--r--   0        0        0    20445 2020-12-30 14:31:37.203734 rich-9.8.2/rich/pretty.py
--rw-r--r--   0        0        0    38568 2021-01-08 13:36:47.401284 rich-9.8.2/rich/progress.py
--rw-r--r--   0        0        0     7699 2021-01-11 21:16:14.974519 rich-9.8.2/rich/progress_bar.py
--rw-r--r--   0        0        0    11218 2021-01-13 16:22:28.302307 rich-9.8.2/rich/prompt.py
--rw-r--r--   0        0        0      243 2020-12-02 22:14:56.142923 rich-9.8.2/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-03-31 13:22:05.771554 rich-9.8.2/rich/py.typed
--rw-r--r--   0        0        0     4183 2020-12-30 20:11:51.435741 rich-9.8.2/rich/rule.py
--rw-r--r--   0        0        0     2769 2020-12-11 15:15:43.925216 rich-9.8.2/rich/scope.py
--rw-r--r--   0        0        0    12873 2021-01-09 16:24:07.205060 rich-9.8.2/rich/segment.py
--rw-r--r--   0        0        0     2834 2020-12-11 15:15:49.793226 rich-9.8.2/rich/spinner.py
--rw-r--r--   0        0        0     4314 2020-12-11 15:15:49.793731 rich-9.8.2/rich/status.py
--rw-r--r--   0        0        0    23334 2021-01-09 16:24:07.206285 rich-9.8.2/rich/style.py
--rw-r--r--   0        0        0     1211 2020-12-17 19:58:35.673087 rich-9.8.2/rich/styled.py
--rw-r--r--   0        0        0    22656 2021-01-13 16:59:49.675262 rich-9.8.2/rich/syntax.py
--rw-r--r--   0        0        0    32939 2021-01-07 16:55:10.406227 rich-9.8.2/rich/table.py
--rw-r--r--   0        0        0     2287 2020-09-25 12:10:56.457482 rich-9.8.2/rich/tabulate.py
--rw-r--r--   0        0        0     1056 2020-05-28 15:37:57.306675 rich-9.8.2/rich/terminal_theme.py
--rw-r--r--   0        0        0    38155 2020-12-30 14:44:43.480791 rich-9.8.2/rich/text.py
--rw-r--r--   0        0        0     3593 2020-10-03 13:26:15.704704 rich-9.8.2/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-09 17:00:57.617294 rich-9.8.2/rich/themes.py
--rw-r--r--   0        0        0    19566 2021-01-11 21:16:14.976858 rich-9.8.2/rich/traceback.py
--rw-r--r--   0        0        0     8473 2021-01-11 21:16:14.977374 rich-9.8.2/rich/tree.py
--rw-r--r--   0        0        0    16750 2021-01-15 10:08:05.142390 rich-9.8.2/setup.py
--rw-r--r--   0        0        0    16713 2021-01-15 10:08:05.143141 rich-9.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1053 2020-01-24 13:59:03.998541 rich-9.9.0/LICENSE
+-rw-r--r--   0        0        0    15351 2021-01-20 17:36:00.267444 rich-9.9.0/README.md
+-rw-r--r--   0        0        0     1337 2021-01-23 15:42:46.809446 rich-9.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4008 2021-01-23 15:42:46.811189 rich-9.9.0/rich/__init__.py
+-rw-r--r--   0        0        0     7199 2021-01-20 17:36:00.348072 rich-9.9.0/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-06-09 21:31:38.948386 rich-9.9.0/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-06-09 22:25:04.834263 rich-9.9.0/rich/_emoji_codes.py
+-rw-r--r--   0        0        0      462 2021-01-05 17:28:01.831941 rich-9.9.0/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     8399 2021-01-20 17:36:00.348671 rich-9.9.0/rich/_inspect.py
+-rw-r--r--   0        0        0     2607 2021-01-20 17:36:00.348924 rich-9.9.0/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2021-01-07 21:28:10.706134 rich-9.9.0/rich/_loop.py
+-rw-r--r--   0        0        0     1185 2020-06-21 11:32:35.980180 rich-9.9.0/rich/_lru_cache.py
+-rw-r--r--   0        0        0     7063 2021-01-22 10:36:13.365237 rich-9.9.0/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2021-01-20 17:36:00.349322 rich-9.9.0/rich/_pick.py
+-rw-r--r--   0        0        0     2285 2021-01-20 17:36:00.349541 rich-9.9.0/rich/_ratio.py
+-rw-r--r--   0        0        0    26521 2021-01-20 17:36:00.349732 rich-9.9.0/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2019-11-24 14:46:58.448301 rich-9.9.0/rich/_stack.py
+-rw-r--r--   0        0        0      324 2021-01-23 15:42:46.812081 rich-9.9.0/rich/_timer.py
+-rw-r--r--   0        0        0     2000 2021-01-20 17:36:00.349997 rich-9.9.0/rich/_windows.py
+-rw-r--r--   0        0        0     1804 2020-07-03 18:27:02.615856 rich-9.9.0/rich/_wrap.py
+-rw-r--r--   0        0        0      878 2021-01-20 17:36:00.350115 rich-9.9.0/rich/abc.py
+-rw-r--r--   0        0        0     7350 2021-01-20 17:36:00.350787 rich-9.9.0/rich/align.py
+-rw-r--r--   0        0        0     6663 2021-01-20 17:36:00.350979 rich-9.9.0/rich/ansi.py
+-rw-r--r--   0        0        0     3150 2021-01-20 17:36:00.351234 rich-9.9.0/rich/bar.py
+-rw-r--r--   0        0        0     8910 2021-01-20 17:36:00.351499 rich-9.9.0/rich/box.py
+-rw-r--r--   0        0        0     3660 2021-01-20 17:36:00.351785 rich-9.9.0/rich/cells.py
+-rw-r--r--   0        0        0    17176 2021-01-22 10:36:13.365833 rich-9.9.0/rich/color.py
+-rw-r--r--   0        0        0     1054 2021-01-20 17:36:00.352401 rich-9.9.0/rich/color_triplet.py
+-rw-r--r--   0        0        0     7104 2021-01-20 17:36:00.352648 rich-9.9.0/rich/columns.py
+-rw-r--r--   0        0        0    60906 2021-01-23 15:42:46.812776 rich-9.9.0/rich/console.py
+-rw-r--r--   0        0        0     1261 2021-01-20 17:36:00.355315 rich-9.9.0/rich/constrain.py
+-rw-r--r--   0        0        0     5285 2021-01-20 17:36:00.355584 rich-9.9.0/rich/containers.py
+-rw-r--r--   0        0        0     1298 2021-01-20 17:36:00.355823 rich-9.9.0/rich/control.py
+-rw-r--r--   0        0        0     6385 2021-01-20 17:36:00.356061 rich-9.9.0/rich/default_styles.py
+-rw-r--r--   0        0        0      159 2021-01-20 17:36:00.356192 rich-9.9.0/rich/diagnose.py
+-rw-r--r--   0        0        0     1962 2021-01-20 17:36:00.356429 rich-9.9.0/rich/emoji.py
+-rw-r--r--   0        0        0      493 2020-03-14 21:59:04.157954 rich-9.9.0/rich/errors.py
+-rw-r--r--   0        0        0     1657 2021-01-20 17:36:00.356597 rich-9.9.0/rich/file_proxy.py
+-rw-r--r--   0        0        0     1884 2020-06-21 11:32:35.988808 rich-9.9.0/rich/filesize.py
+-rw-r--r--   0        0        0     4350 2021-01-22 10:36:13.366467 rich-9.9.0/rich/highlighter.py
+-rw-r--r--   0        0        0     2369 2021-01-20 17:36:00.357054 rich-9.9.0/rich/jupyter.py
+-rw-r--r--   0        0        0    13707 2021-01-20 17:36:00.357642 rich-9.9.0/rich/live.py
+-rw-r--r--   0        0        0     2563 2021-01-20 17:36:00.357966 rich-9.9.0/rich/live_render.py
+-rw-r--r--   0        0        0     9896 2021-01-20 17:36:00.358272 rich-9.9.0/rich/logging.py
+-rw-r--r--   0        0        0    20301 2021-01-20 17:36:00.359084 rich-9.9.0/rich/markdown.py
+-rw-r--r--   0        0        0     5598 2021-01-20 17:36:00.359823 rich-9.9.0/rich/markup.py
+-rw-r--r--   0        0        0     5213 2021-01-20 17:36:00.360128 rich-9.9.0/rich/measure.py
+-rw-r--r--   0        0        0     4419 2021-01-20 17:36:00.360431 rich-9.9.0/rich/padding.py
+-rw-r--r--   0        0        0      759 2021-01-20 17:36:00.360612 rich-9.9.0/rich/pager.py
+-rw-r--r--   0        0        0     3288 2021-01-22 10:36:13.367109 rich-9.9.0/rich/palette.py
+-rw-r--r--   0        0        0     6866 2021-01-20 17:36:00.361714 rich-9.9.0/rich/panel.py
+-rw-r--r--   0        0        0    20445 2021-01-20 17:36:00.362203 rich-9.9.0/rich/pretty.py
+-rw-r--r--   0        0        0    38568 2021-01-20 17:36:00.362826 rich-9.9.0/rich/progress.py
+-rw-r--r--   0        0        0     7699 2021-01-20 17:36:00.363489 rich-9.9.0/rich/progress_bar.py
+-rw-r--r--   0        0        0    11218 2021-01-20 17:36:00.364209 rich-9.9.0/rich/prompt.py
+-rw-r--r--   0        0        0      243 2021-01-20 17:36:00.364567 rich-9.9.0/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-03-31 13:22:05.771554 rich-9.9.0/rich/py.typed
+-rw-r--r--   0        0        0     4183 2021-01-20 17:36:00.364912 rich-9.9.0/rich/rule.py
+-rw-r--r--   0        0        0     2769 2021-01-20 17:36:00.365126 rich-9.9.0/rich/scope.py
+-rw-r--r--   0        0        0    13518 2021-01-22 10:36:13.367721 rich-9.9.0/rich/segment.py
+-rw-r--r--   0        0        0     2834 2021-01-20 17:36:00.365914 rich-9.9.0/rich/spinner.py
+-rw-r--r--   0        0        0     4314 2021-01-20 17:36:00.366439 rich-9.9.0/rich/status.py
+-rw-r--r--   0        0        0    23334 2021-01-20 17:36:00.367383 rich-9.9.0/rich/style.py
+-rw-r--r--   0        0        0     1211 2021-01-20 17:36:00.367819 rich-9.9.0/rich/styled.py
+-rw-r--r--   0        0        0    24671 2021-01-23 15:42:46.813182 rich-9.9.0/rich/syntax.py
+-rw-r--r--   0        0        0    32912 2021-01-23 15:42:46.814016 rich-9.9.0/rich/table.py
+-rw-r--r--   0        0        0     2287 2021-01-20 17:36:00.369519 rich-9.9.0/rich/tabulate.py
+-rw-r--r--   0        0        0     1439 2021-01-22 10:36:13.368132 rich-9.9.0/rich/terminal_theme.py
+-rw-r--r--   0        0        0    38008 2021-01-23 15:42:46.814617 rich-9.9.0/rich/text.py
+-rw-r--r--   0        0        0     3593 2021-01-20 17:36:00.370224 rich-9.9.0/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-09 17:00:57.617294 rich-9.9.0/rich/themes.py
+-rw-r--r--   0        0        0    19978 2021-01-23 15:42:46.815151 rich-9.9.0/rich/traceback.py
+-rw-r--r--   0        0        0     8699 2021-01-22 10:36:13.368693 rich-9.9.0/rich/tree.py
+-rw-r--r--   0        0        0    16750 2021-01-23 15:43:10.115419 rich-9.9.0/setup.py
+-rw-r--r--   0        0        0    16713 2021-01-23 15:43:10.116643 rich-9.9.0/PKG-INFO
```

### Comparing `rich-9.8.2/LICENSE` & `rich-9.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/README.md` & `rich-9.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/pyproject.toml` & `rich-9.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "rich"
 homepage = "https://github.com/willmcgugan/rich"
 documentation = "https://rich.readthedocs.io/en/latest/"
-version = "9.8.2"
+version = "9.9.0"
 description = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
 authors = ["Will McGugan <willmcgugan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",    
     "Environment :: Console", 
@@ -36,12 +36,12 @@
 [tool.poetry.extras]
 jupyter = ["ipywidgets"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.1"
 black = "^20.8b1"
 mypy = "^0.790"
-pytest-cov = "^2.10.1"
+pytest-cov = "^2.11.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rich-9.8.2/rich/__init__.py` & `rich-9.9.0/rich/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Rich text and beautiful formatting in the terminal."""
 
+import os
 from typing import Any, IO, Optional, TYPE_CHECKING
 
 __all__ = ["get_console", "reconfigure", "print", "inspect"]
 
 if TYPE_CHECKING:
     from .console import Console
 
 # Global console used by alternative print
 _console: Optional["Console"] = None
 
+_IMPORT_CWD = os.path.abspath(os.getcwd())
+
 
 def get_console() -> "Console":
     """Get a global :class:`~rich.console.Console` instance. This function is used when Rich requires a Console,
     and hasn't been explicitly given one.
 
     Returns:
         Console: A console instance.
```

### Comparing `rich-9.8.2/rich/__main__.py` & `rich-9.9.0/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_cell_widths.py` & `rich-9.9.0/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_emoji_codes.py` & `rich-9.9.0/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_inspect.py` & `rich-9.9.0/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_log_render.py` & `rich-9.9.0/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_loop.py` & `rich-9.9.0/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_lru_cache.py` & `rich-9.9.0/rich/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_palettes.py` & `rich-9.9.0/rich/_palettes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 from .palette import Palette
 
 
-# The standard ansi colors
+# Taken from https://en.wikipedia.org/wiki/ANSI_escape_code (Windows 10 column)
 WINDOWS_PALETTE = Palette(
     [
-        (0, 0, 0),
-        (128, 0, 0),
-        (0, 128, 0),
-        (128, 128, 0),
-        (0, 0, 128),
-        (128, 0, 128),
-        (0, 128, 128),
-        (192, 192, 192),
+        (12, 12, 12),
+        (197, 15, 31),
+        (19, 161, 14),
+        (193, 156, 0),
+        (0, 55, 218),
+        (136, 23, 152),
+        (58, 150, 221),
+        (204, 204, 204),
+        (118, 118, 118),
+        (231, 72, 86),
+        (22, 198, 12),
+        (249, 241, 165),
+        (59, 120, 255),
+        (180, 0, 158),
+        (97, 214, 214),
+        (242, 242, 242),
     ]
 )
 
 # # The standard ansi colors (including bright variants)
 STANDARD_PALETTE = Palette(
     [
         (0, 0, 0),
```

### Comparing `rich-9.8.2/rich/_ratio.py` & `rich-9.9.0/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_spinners.py` & `rich-9.9.0/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_windows.py` & `rich-9.9.0/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/_wrap.py` & `rich-9.9.0/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/abc.py` & `rich-9.9.0/rich/abc.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/align.py` & `rich-9.9.0/rich/align.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/ansi.py` & `rich-9.9.0/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/bar.py` & `rich-9.9.0/rich/bar.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/box.py` & `rich-9.9.0/rich/box.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/cells.py` & `rich-9.9.0/rich/cells.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/color.py` & `rich-9.9.0/rich/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,19 @@
     """The type of the color."""
     number: Optional[int] = None
     """The color number, if a standard color, or None."""
     triplet: Optional[ColorTriplet] = None
     """A triplet of color components, if an RGB color."""
 
     def __repr__(self) -> str:
-        return f"<color {self.name!r} ({self.type.name.lower()})>"
+        return (
+            f"<color {self.name!r} ({self.type.name.lower()})>"
+            if self.number is None
+            else f"<color {self.name!r} {self.number} ({self.type.name.lower()})>"
+        )
 
     def __rich__(self) -> "Text":
         """Dispays the actual color if Rich printed."""
         from .text import Text
         from .style import Style
 
         return Text.assemble(
@@ -322,15 +326,15 @@
             assert self.number is not None
             return EIGHT_BIT_PALETTE[self.number]
         elif self.type == ColorType.STANDARD:
             assert self.number is not None
             return theme.ansi_colors[self.number]
         elif self.type == ColorType.WINDOWS:
             assert self.number is not None
-            return STANDARD_PALETTE[self.number]
+            return WINDOWS_PALETTE[self.number]
         else:  # self.type == ColorType.DEFAULT:
             assert self.number is None
             return theme.foreground_color if foreground else theme.background_color
 
     @classmethod
     def from_ansi(cls, number: int) -> "Color":
         """Create a Color number from it's 8-bit ansi number.
@@ -441,15 +445,16 @@
         _type = self.type
         if _type == ColorType.DEFAULT:
             return ("39" if foreground else "49",)
 
         elif _type == ColorType.WINDOWS:
             number = self.number
             assert number is not None
-            return (str(30 + number if foreground else 40 + number),)
+            fore, back = (30, 40) if number < 8 else (82, 92)
+            return (str(fore + number if foreground else back + number),)
 
         elif _type == ColorType.STANDARD:
             number = self.number
             assert number is not None
             fore, back = (30, 40) if number < 8 else (82, 92)
             return (str(fore + number if foreground else back + number),)
 
@@ -503,18 +508,16 @@
 
         elif system == ColorSystem.WINDOWS:
             if self.system == ColorSystem.TRUECOLOR:
                 assert self.triplet is not None
                 triplet = self.triplet
             else:  # self.system == ColorSystem.EIGHT_BIT
                 assert self.number is not None
-                if self.number < 8:
+                if self.number < 16:
                     return Color(self.name, ColorType.WINDOWS, number=self.number)
-                elif self.number < 16:
-                    return Color(self.name, ColorType.WINDOWS, number=self.number - 8)
                 triplet = ColorTriplet(*EIGHT_BIT_PALETTE[self.number])
 
             color_number = WINDOWS_PALETTE.match(triplet)
             return Color(self.name, ColorType.WINDOWS, number=color_number)
 
         return self
```

### Comparing `rich-9.8.2/rich/color_triplet.py` & `rich-9.9.0/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/columns.py` & `rich-9.9.0/rich/columns.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/console.py` & `rich-9.9.0/rich/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,14 +399,15 @@
         theme (Theme, optional): An optional style theme object, or ``None`` for default theme.
         stderr (bool, optional): Use stderr rather than stdout if ``file `` is not specified. Defaults to False.
         file (IO, optional): A file object where the console should write to. Defaults to stdout.
         width (int, optional): The width of the terminal. Leave as default to auto-detect width.
         height (int, optional): The height of the terminal. Leave as default to auto-detect height.
         style (StyleType, optional): Style to apply to all output, or None for no style. Defaults to None.
         no_color (Optional[bool], optional): Enabled no color mode, or None to auto detect. Defaults to None.
+        tab_size (int, optional): Number of spaces used to replace a tab character. Defaults to 8.
         record (bool, optional): Boolean to enable recording of terminal output,
             required to call :meth:`export_html` and :meth:`export_text`. Defaults to False.
         markup (bool, optional): Boolean to enable :ref:`console_markup`. Defaults to True.
         emoji (bool, optional): Enable emoji code. Defaults to True.
         highlight (bool, optional): Enable automatic highlighting. Defaults to True.
         log_time (bool, optional): Boolean to enable logging of time by :meth:`log` methods. Defaults to True.
         log_path (bool, optional): Boolean to enable the logging of the caller by :meth:`log`. Defaults to True.
@@ -802,14 +803,15 @@
             home (bool, optional): Also move the cursor to 'home' position. Defaults to True.
         """
         self.control("\033[2J\033[H" if home else "\033[2J")
 
     def status(
         self,
         status: RenderableType,
+        *,
         spinner: str = "dots",
         spinner_style: str = "status.spinner",
         speed: float = 1.0,
         refresh_per_second: float = 12.5,
     ) -> "Status":
         """Display a status and spinner.
```

### Comparing `rich-9.8.2/rich/constrain.py` & `rich-9.9.0/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/containers.py` & `rich-9.9.0/rich/containers.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/control.py` & `rich-9.9.0/rich/control.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/default_styles.py` & `rich-9.9.0/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/emoji.py` & `rich-9.9.0/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/file_proxy.py` & `rich-9.9.0/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/filesize.py` & `rich-9.9.0/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/highlighter.py` & `rich-9.9.0/rich/highlighter.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 class ReprHighlighter(RegexHighlighter):
     """Highlights the text typically produced from ``__repr__`` methods."""
 
     base_style = "repr."
     highlights = [
         r"(?P<tag_start>\<)(?P<tag_name>[\w\-\.\:]*)(?P<tag_contents>.*?)(?P<tag_end>\>)",
-        r"(?P<attrib_name>\w+?)=(?P<attrib_value>\"?[\w_]+\"?)?",
+        r"(?P<attrib_name>[\w_]{1,50})=(?P<attrib_value>\"?[\w_]+\"?)?",
         _combine_regex(
             r"(?P<ipv4>[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3})",
             r"(?P<ipv6>([A-Fa-f0-9]{1,4}::?){1,7}[A-Fa-f0-9]{1,4})",
             r"(?P<eui64>(?:[0-9A-Fa-f]{1,2}-){7}[0-9A-Fa-f]{1,2}|(?:[0-9A-Fa-f]{1,2}:){7}[0-9A-Fa-f]{1,2}|(?:[0-9A-Fa-f]{4}\.){3}[0-9A-Fa-f]{4})",
             r"(?P<eui48>(?:[0-9A-Fa-f]{1,2}-){5}[0-9A-Fa-f]{1,2}|(?:[0-9A-Fa-f]{1,2}:){5}[0-9A-Fa-f]{1,2}|(?:[0-9A-Fa-f]{4}\.){2}[0-9A-Fa-f]{4})",
             r"(?P<brace>[\{\[\(\)\]\}])",
             r"(?P<bool_true>True)|(?P<bool_false>False)|(?P<none>None)",
```

### Comparing `rich-9.8.2/rich/jupyter.py` & `rich-9.9.0/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/live.py` & `rich-9.9.0/rich/live.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/live_render.py` & `rich-9.9.0/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/logging.py` & `rich-9.9.0/rich/logging.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/markdown.py` & `rich-9.9.0/rich/markdown.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/markup.py` & `rich-9.9.0/rich/markup.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/measure.py` & `rich-9.9.0/rich/measure.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/padding.py` & `rich-9.9.0/rich/padding.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/pager.py` & `rich-9.9.0/rich/pager.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/palette.py` & `rich-9.9.0/rich/palette.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,20 @@
             color (Tuple[int, int, int]): RGB components in range 0 > 255.
 
         Returns:
             int: Index of closes matching color.
         """
         red1, green1, blue1 = color
         _sqrt = sqrt
+        get_color = self._colors.__getitem__
 
         def get_color_distance(index: int) -> float:
             """Get the distance to a color."""
-            red2, green2, blue2 = self._colors[index]
-            red_mean = int((red1 + red2) / 2)
+            red2, green2, blue2 = get_color(index)
+            red_mean = (red1 + red2) // 2
             red = red1 - red2
             green = green1 - green2
             blue = blue1 - blue2
             return _sqrt(
                 (((512 + red_mean) * red * red) >> 8)
                 + 4 * green * green
                 + (((767 - red_mean) * blue * blue) >> 8)
```

### Comparing `rich-9.8.2/rich/panel.py` & `rich-9.9.0/rich/panel.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/pretty.py` & `rich-9.9.0/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/progress.py` & `rich-9.9.0/rich/progress.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/progress_bar.py` & `rich-9.9.0/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/prompt.py` & `rich-9.9.0/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/rule.py` & `rich-9.9.0/rich/rule.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/scope.py` & `rich-9.9.0/rich/scope.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/segment.py` & `rich-9.9.0/rich/segment.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,32 +65,49 @@
     @classmethod
     def line(cls, is_control: bool = False) -> "Segment":
         """Make a new line segment."""
         return cls("\n", is_control=is_control)
 
     @classmethod
     def apply_style(
-        cls, segments: Iterable["Segment"], style: Style = None
+        cls,
+        segments: Iterable["Segment"],
+        style: Style = None,
+        post_style: Style = None,
     ) -> Iterable["Segment"]:
-        """Apply a style to an iterable of segments.
+        """Apply style(s) to an iterable of segments.
+
+        Returns an iterable of segments where the style is replaced by ``style + segment.style + post_style``.
 
         Args:
             segments (Iterable[Segment]): Segments to process.
-            style (Style, optional): A style to apply. Defaults to None.
+            style (Style, optional): Base style. Defaults to None.
+            post_style (Style, optional): Style to apply on top of segment style. Defaults to None.
 
         Returns:
             Iterable[Segments]: A new iterable of segments (possibly the same iterable).
         """
-        if style is None:
-            return segments
-        apply = style.__add__
-        return (
-            cls(text, None if is_control else apply(style), is_control)
-            for text, style, is_control in segments
-        )
+        if style is not None:
+            apply = style.__add__
+            segments = (
+                cls(text, None if is_control else apply(_style), is_control)
+                for text, _style, is_control in segments
+            )
+        if post_style is not None:
+            segments = (
+                cls(
+                    text,
+                    None
+                    if is_control
+                    else (_style + post_style if _style else post_style),
+                    is_control,
+                )
+                for text, _style, is_control in segments
+            )
+        return segments
 
     @classmethod
     def filter_control(
         cls, segments: Iterable["Segment"], is_control=False
     ) -> Iterable["Segment"]:
         """Filter segments by ``is_control`` attribute.
```

### Comparing `rich-9.8.2/rich/spinner.py` & `rich-9.9.0/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/status.py` & `rich-9.9.0/rich/status.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/style.py` & `rich-9.9.0/rich/style.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/styled.py` & `rich-9.9.0/rich/styled.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/syntax.py` & `rich-9.9.0/rich/syntax.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
 import platform
 import textwrap
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Optional, Set, Tuple, Type, Union
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, Type, Union
 
 from pygments.lexers import get_lexer_by_name, guess_lexer_for_filename
 from pygments.style import Style as PygmentsStyle
 from pygments.styles import get_style_by_name
 from pygments.token import (
     Comment,
     Error,
@@ -343,45 +343,84 @@
 
         Returns:
             Optional[Color]: Color from theme, or None for no color.
         """
         style = self._theme.get_style_for_token(token_type)
         return style.color
 
-    def highlight(self, code: str) -> Text:
+    def highlight(self, code: str, line_range: Tuple[int, int] = None) -> Text:
         """Highlight code and return a Text instance.
 
         Args:
-            code (str). Code to highlight.
+            code (str): Code to highlight.
+            line_range(Tuple[int, int], optional): Optional line range to highlight.
 
         Returns:
-            Text: A text instance containing syntax highlight.
+            Text: A text instance containing highlighted syntax.
         """
 
         base_style = self._get_base_style()
         justify: JustifyMethod = (
             "default" if base_style.transparent_background else "left"
         )
 
         text = Text(
             justify=justify,
             style=base_style,
             tab_size=self.tab_size,
             no_wrap=not self.word_wrap,
         )
+        _get_theme_style = self._theme.get_style_for_token
         try:
             lexer = get_lexer_by_name(self.lexer_name)
         except ClassNotFound:
             text.append(code)
         else:
-            _get_theme_style = self._theme.get_style_for_token
-            text.append_tokens(
-                (token, _get_theme_style(token_type))
-                for token_type, token in lexer.get_tokens(code)
-            )
+            if line_range:
+                # More complicated path to only stylize a portion of the code
+                # This speeds up further operations as there are less spans to process
+                line_start, line_end = line_range
+
+                def line_tokenize() -> Iterable[Tuple[Any, str]]:
+                    """Split tokens to one per line."""
+                    for token_type, token in lexer.get_tokens(code):
+                        while token:
+                            line_token, new_line, token = token.partition("\n")
+                            yield token_type, line_token + new_line
+
+                def tokens_to_spans() -> Iterable[Tuple[str, Optional[Style]]]:
+                    """Convert tokens to spans."""
+                    tokens = iter(line_tokenize())
+                    line_no = 0
+                    _line_start = line_start - 1
+
+                    # Skip over tokens until line start
+                    while line_no < _line_start:
+                        _token_type, token = next(tokens)
+                        yield (token, None)
+                        if token.endswith("\n"):
+                            line_no += 1
+                    # Generate spans until line end
+                    for token_type, token in tokens:
+                        yield (token, _get_theme_style(token_type))
+                        if token.endswith("\n"):
+                            line_no += 1
+                            if line_no >= line_end:
+                                break
+                    # Exhaust tokens
+                    for token_type, token in tokens:
+                        yield (token, None)
+
+                text.append_tokens(tokens_to_spans())
+
+            else:
+                text.append_tokens(
+                    (token, _get_theme_style(token_type))
+                    for token_type, token in lexer.get_tokens(code)
+                )
             if self.background_color is not None:
                 text.stylize(f"on {self.background_color}")
         return text
 
     def _get_line_numbers_color(self, blend: float = 0.3) -> Color:
         background_color = self._theme.get_background_style().bgcolor
         if background_color is None or background_color.is_system_defined:
@@ -430,52 +469,60 @@
             width = self.code_width + self._numbers_column_width
             return Measurement(self._numbers_column_width, width)
         return Measurement(self._numbers_column_width, max_width)
 
     def __rich_console__(
         self, console: Console, options: ConsoleOptions
     ) -> RenderResult:
+
         transparent_background = self._get_base_style().transparent_background
         code_width = (
             (options.max_width - self._numbers_column_width - 1)
             if self.code_width is None
             else self.code_width
         )
+
+        line_offset = 0
+        if self.line_range:
+            start_line, end_line = self.line_range
+            line_offset = max(0, start_line - 1)
+
         code = textwrap.dedent(self.code) if self.dedent else self.code
         code = code.expandtabs(self.tab_size)
-        text = self.highlight(code)
+        text = self.highlight(code, self.line_range)
         text.remove_suffix("\n")
-        text.expand_tabs(self.tab_size)
 
         (
             background_style,
             number_style,
             highlight_number_style,
         ) = self._get_number_styles(console)
 
-        if self.indent_guides and not options.ascii_only:
-            style = (
-                self._get_base_style()
-                + self._theme.get_style_for_token(Comment)
-                + Style(dim=True)
-            )
-            text = text.with_indent_guides(self.tab_size, style=style)
-
         if not self.line_numbers:
             # Simple case of just rendering text
             yield from console.render(text, options=options.update(width=code_width))
             return
 
         lines = text.split("\n")
-        line_offset = 0
         if self.line_range:
-            start_line, end_line = self.line_range
-            line_offset = max(0, start_line - 1)
             lines = lines[line_offset:end_line]
 
+        if self.indent_guides and not options.ascii_only:
+            style = (
+                self._get_base_style()
+                + self._theme.get_style_for_token(Comment)
+                + Style(dim=True)
+            )
+            lines = (
+                Text("\n")
+                .join(lines)
+                .with_indent_guides(self.tab_size, style=style)
+                .split("\n")
+            )
+
         numbers_column_width = self._numbers_column_width
         render_options = options.update(width=code_width)
 
         highlight_line = self.highlight_lines.__contains__
         _Segment = Segment
         padding = _Segment(" " * numbers_column_width + " ", background_style)
         new_line = _Segment("\n")
```

### Comparing `rich-9.8.2/rich/table.py` & `rich-9.9.0/rich/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,22 +163,14 @@
         title_justify: "JustifyMethod" = "center",
         caption_justify: "JustifyMethod" = "center",
         highlight: bool = False,
     ) -> None:
 
         self.columns: List[Column] = []
         self.rows: List[Row] = []
-        append_column = self.columns.append
-        for index, header in enumerate(headers):
-            if isinstance(header, str):
-                append_column(Column(_index=index, header=header))
-            else:
-                header._index = index
-                append_column(header)
-
         self.title = title
         self.caption = caption
         self.width = width
         self.min_width = min_width
         self.box = box
         self.safe_box = safe_box
         self._padding = Padding.unpack(padding)
@@ -196,14 +188,21 @@
         self.border_style = border_style
         self.title_style = title_style
         self.caption_style = caption_style
         self.title_justify = title_justify
         self.caption_justify = caption_justify
         self.highlight = highlight
         self.row_styles = list(row_styles or [])
+        append_column = self.columns.append
+        for header in headers:
+            if isinstance(header, str):
+                self.add_column(header=header)
+            else:
+                header._index = len(self.columns)
+                append_column(header)
 
     @classmethod
     def grid(
         cls,
         padding: PaddingDimensions = 0,
         collapse_padding: bool = True,
         pad_edge: bool = False,
```

### Comparing `rich-9.8.2/rich/tabulate.py` & `rich-9.9.0/rich/tabulate.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/text.py` & `rich-9.9.0/rich/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+import re
 from functools import partial, reduce
-from io import UnsupportedOperation
 from math import gcd
-import re
-from operator import itemgetter
+from operator import attrgetter, itemgetter
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
@@ -26,20 +25,15 @@
 from .control import strip_control_codes
 from .jupyter import JupyterMixin
 from .measure import Measurement
 from .segment import Segment
 from .style import Style, StyleType
 
 if TYPE_CHECKING:  # pragma: no cover
-    from .console import (
-        Console,
-        ConsoleOptions,
-        JustifyMethod,
-        OverflowMethod,
-    )
+    from .console import Console, ConsoleOptions, JustifyMethod, OverflowMethod
 
 DEFAULT_JUSTIFY: "JustifyMethod" = "default"
 DEFAULT_OVERFLOW: "OverflowMethod" = "fold"
 
 
 _re_whitespace = re.compile(r"\s+$")
 
@@ -831,30 +825,31 @@
         self._spans.extend(
             _Span(start + text_length, end + text_length, style)
             for start, end, style in text._spans
         )
         self._length += len(text)
         return self
 
-    def append_tokens(self, tokens: Iterable[Tuple[str, StyleType]]):
+    def append_tokens(self, tokens: Iterable[Tuple[str, Optional[StyleType]]]):
         """Append iterable of str and style. Style may be a Style instance or a str style definition.
 
         Args:
-            pairs (Iterable[Tuple[str, StyleType]]): An iterable of tuples containing str content and style.
+            pairs (Iterable[Tuple[str, Optional[StyleType]]]): An iterable of tuples containing str content and style.
 
         Returns:
             Text: Returns self for chaining.
         """
         append_text = self._text.append
         append_span = self._spans.append
         _Span = Span
         offset = len(self)
         for content, style in tokens:
             append_text(content)
-            append_span(_Span(offset, offset + len(content), style))
+            if style is not None:
+                append_span(_Span(offset, offset + len(content), style))
             offset += len(content)
         self._length = offset
         return self
 
     def copy_styles(self, text: "Text") -> None:
         """Copy styles from another Text instance.
 
@@ -883,90 +878,85 @@
         assert separator, "separator must not be empty"
 
         text = self.plain
         if separator not in text:
             return Lines([self.copy()])
         if not allow_blank and text.endswith(separator):
             text = text[: -len(separator)]
-        offsets: List[int] = []
-        append = offsets.append
-        offset = 0
-        while True:
-            try:
-                offset = text.index(separator, offset) + len(separator)
-            except ValueError:
-                break
-            append(offset)
+        offsets = [
+            match.start() + 1 for match in re.finditer(re.escape(separator), text)
+        ]
         lines = self.divide(offsets)
         if not include_separator:
             separator_length = len(separator)
             for line in lines:
                 if line.plain.endswith(separator):
                     line.right_crop(separator_length)
+
         return lines
 
     def divide(self, offsets: Iterable[int]) -> Lines:
         """Divide text in to a number of lines at given offsets.
 
         Args:
             offsets (Iterable[int]): Offsets used to divide text.
 
         Returns:
             Lines: New RichText instances between offsets.
         """
-
         if not offsets:
-            line = self.copy()
-            return Lines([line])
+            return Lines([self.copy()])
 
         text = self.plain
         text_length = len(text)
         divide_offsets = [0, *offsets, text_length]
         line_ranges = list(zip(divide_offsets, divide_offsets[1:]))
-        average_line_length = -(-text_length // len(line_ranges))
 
+        style = self.style
+        justify = self.justify
+        overflow = self.overflow
+        _Text = Text
         new_lines = Lines(
-            Text(
+            _Text(
                 text[start:end],
-                style=self.style,
-                justify=self.justify,
-                overflow=self.overflow,
+                style=style,
+                justify=justify,
+                overflow=overflow,
             )
             for start, end in line_ranges
         )
-        line_ranges = [
-            (offset, offset + len(line))
-            for offset, line in zip(divide_offsets, new_lines)
-        ]
-        for span in self._spans:
-            line_index = (span.start // average_line_length) % len(line_ranges)
+        if not self._spans:
+            return new_lines
+        order = {span: span_index for span_index, span in enumerate(self._spans)}
+        span_stack = sorted(self._spans, key=attrgetter("start"), reverse=True)
 
-            line_start, line_end = line_ranges[line_index]
-            if span.start < line_start:
-                while True:
-                    line_index -= 1
-                    line_start, line_end = line_ranges[line_index]
-                    if span.start >= line_start:
-                        break
-            elif span.start > line_end:
-                while True:
-                    line_index += 1
-                    line_start, line_end = line_ranges[line_index]
-                    if span.start <= line_end:
-                        break
-
-            while True:
-                span, new_span = span.split(line_end)
-                if span:
-                    new_lines[line_index]._spans.append(span.move(-line_start))
-                if new_span is None:
-                    break
-                span = new_span
-                line_index = (line_index + 1) % len(line_ranges)
-                line_start, line_end = line_ranges[line_index]
+        pop = span_stack.pop
+        push = span_stack.append
+        _Span = Span
+        get_order = order.__getitem__
+
+        for line, (start, end) in zip(new_lines, line_ranges):
+            if not span_stack:
+                break
+            append_span = line._spans.append
+            position = len(span_stack) - 1
+            while span_stack[position].start < end:
+                span = pop(position)
+                add_span, remaining_span = span.split(end)
+                if remaining_span:
+                    push(remaining_span)
+                    order[remaining_span] = order[span]
+                span_start, span_end, span_style = add_span
+                line_span = _Span(span_start - start, span_end - start, span_style)
+                order[line_span] = order[span]
+                append_span(line_span)
+                position -= 1
+                if position < 0 or not span_stack:
+                    break  # pragma: no cover
+            line._spans.sort(key=get_order)
 
         return new_lines
 
     def right_crop(self, amount: int = 1) -> None:
         """Remove a number of characters from the end of the text."""
         self.plain = self.plain[:-amount]
```

### Comparing `rich-9.8.2/rich/theme.py` & `rich-9.9.0/rich/theme.py`

 * *Files identical despite different names*

### Comparing `rich-9.8.2/rich/traceback.py` & `rich-9.9.0/rich/traceback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 from __future__ import absolute_import
 
-import os.path
+import os
 import platform
 import sys
 from dataclasses import dataclass, field
-from textwrap import indent
 from traceback import walk_tb
 from types import TracebackType
 from typing import Callable, Dict, Iterable, List, Optional, Type
 
 from pygments.lexers import guess_lexer_for_filename
-from pygments.token import (
-    Comment,
-    Keyword,
-    Name,
-    Number,
-    Operator,
-    String,
-    Token,
-    Text as TextToken,
-)
+from pygments.token import Comment, Keyword, Name, Number, Operator, String
+from pygments.token import Text as TextToken
+from pygments.token import Token
 
 from . import pretty
 from ._loop import loop_first, loop_last
 from .columns import Columns
 from .console import (
     Console,
     ConsoleOptions,
@@ -150,14 +142,16 @@
         show_locals (bool, optional): Enable display of local variables. Defaults to False.
         indent_guides (bool, optional): Enable indent guides in code and locals. Defaults to True.
         locals_max_length (int, optional): Maximum length of containers before abbreviating, or None for no abbreviation.
             Defaults to 10.
         locals_max_string (int, optional): Maximum length of string before truncating, or None to disable. Defaults to 80.
     """
 
+    LEXERS = {".py": "python", ".pxd": "cython", ".pyx": "cython", ".pxi": "pyrex"}
+
     def __init__(
         self,
         trace: Trace = None,
         width: Optional[int] = 100,
         extra_lines: int = 3,
         theme: Optional[str] = None,
         word_wrap: bool = False,
@@ -258,14 +252,16 @@
         Returns:
             Trace: A Trace instance which you can use to construct a `Traceback`.
         """
 
         stacks: List[Stack] = []
         is_cause = False
 
+        from rich import _IMPORT_CWD
+
         while True:
             stack = Stack(
                 exc_type=str(exc_type.__name__),
                 exc_value=str(exc_value),
                 is_cause=is_cause,
             )
 
@@ -280,17 +276,18 @@
 
             stacks.append(stack)
             append = stack.frames.append
 
             for frame_summary, line_no in walk_tb(traceback):
                 filename = frame_summary.f_code.co_filename
                 if filename and not filename.startswith("<"):
-                    filename = os.path.abspath(filename) if filename else "?"
+                    if not os.path.isabs(filename):
+                        filename = os.path.join(_IMPORT_CWD, filename)
                 frame = Frame(
-                    filename=filename,
+                    filename=filename or "?",
                     lineno=line_no,
                     name=frame_summary.f_code.co_name,
                     locals={
                         key: pretty.traverse(
                             value,
                             max_length=locals_max_length,
                             max_string=locals_max_string,
@@ -422,14 +419,22 @@
         syntax_error_text.stylize("bold underline", offset, offset + 1)
         syntax_error_text += Text.from_markup(
             "\n" + " " * offset + "[traceback.offset]▲[/]",
             style="pygments.text",
         )
         yield syntax_error_text
 
+    @classmethod
+    def _guess_lexer(cls, filename: str, code: str) -> str:
+        ext = os.path.splitext(filename)[-1]
+        lexer_name = (
+            cls.LEXERS.get(ext) or guess_lexer_for_filename(filename, code).name
+        )
+        return lexer_name
+
     @render_group()
     def _render_stack(self, stack: Stack) -> RenderResult:
         path_highlighter = PathHighlighter()
         theme = self.theme
         code_cache: Dict[str, str] = {}
 
         def read_code(filename: str) -> str:
@@ -473,29 +478,29 @@
                 yield ""
             yield text
             if frame.filename.startswith("<"):
                 yield from render_locals(frame)
                 continue
             try:
                 code = read_code(frame.filename)
-                lexer = guess_lexer_for_filename(frame.filename, code)
-                lexer_name = lexer.name
+                lexer_name = self._guess_lexer(frame.filename, code)
                 syntax = Syntax(
                     code,
                     lexer_name,
                     theme=theme,
                     line_numbers=True,
                     line_range=(
                         frame.lineno - self.extra_lines,
                         frame.lineno + self.extra_lines,
                     ),
                     highlight_lines={frame.lineno},
                     word_wrap=self.word_wrap,
                     code_width=88,
                     indent_guides=self.indent_guides,
+                    dedent=False,
                 )
                 yield ""
             except Exception as error:
                 yield Text.assemble(
                     (f"{error.__class__.__name__}: {error}", "traceback.error"),
                 )
             else:
```

### Comparing `rich-9.8.2/rich/tree.py` & `rich-9.9.0/rich/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,22 +91,23 @@
 
         def make_guide(index: int, style: Style) -> Segment:
             """Make a Segment for a level of the guide lines."""
             if options.ascii_only:
                 line = ASCII_GUIDES[index]
             else:
                 guide = 1 if style.bold else (2 if style.underline2 else 0)
-                line = TREE_GUIDES[guide][index]
+                line = TREE_GUIDES[0 if options.legacy_windows else guide][index]
             return _Segment(line, style)
 
         levels: List[Segment] = [make_guide(CONTINUE, guide_style)]
         push(iter(loop_last([self])))
 
         guide_style_stack = StyleStack(get_style(self.guide_style))
         style_stack = StyleStack(get_style(self.style))
+        remove_guide_styles = Style(bold=False, underline2=False)
 
         while stack:
             stack_node = pop()
             try:
                 last, node = next(stack_node)
             except StopIteration:
                 levels.pop()
@@ -129,15 +130,19 @@
                     width=options.max_width
                     - sum(level.cell_length for level in prefix),
                     highlight=self.highlight,
                 ),
             )
             for first, line in loop_first(renderable_lines):
                 if prefix:
-                    yield from _Segment.apply_style(prefix, style.background_style)
+                    yield from _Segment.apply_style(
+                        prefix,
+                        style.background_style,
+                        post_style=remove_guide_styles,
+                    )
                 yield from line
                 yield new_line
                 if first and prefix:
                     prefix[-1] = make_guide(
                         SPACE if last else CONTINUE, prefix[-1].style or null_style
                     )
```

### Comparing `rich-9.8.2/setup.py` & `rich-9.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.7,<0.9'],
  'jupyter': ['ipywidgets>=7.5.1,<8.0.0']}
 
 setup_kwargs = {
     'name': 'rich',
-    'version': '9.8.2',
+    'version': '9.9.0',
     'description': 'Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal',
     'long_description': '# Rich\n\n[![PyPI version](https://badge.fury.io/py/rich.svg)](https://badge.fury.io/py/rich)\n[![codecov](https://codecov.io/gh/willmcgugan/rich/branch/master/graph/badge.svg)](https://codecov.io/gh/willmcgugan/rich)\n[![Rich blog](https://img.shields.io/badge/blog-rich%20news-yellowgreen)](https://www.willmcgugan.com/tag/rich/)\n[![Twitter Follow](https://img.shields.io/twitter/follow/willmcgugan.svg?style=social)](https://twitter.com/willmcgugan)\n\n[中文 readme](https://github.com/willmcgugan/rich/blob/master/README.cn.md) • [lengua española readme](https://github.com/willmcgugan/rich/blob/master/README.es.md)\n\nRich is a Python library for _rich_ text and beautiful formatting in the terminal.\n\nThe [Rich API](https://rich.readthedocs.io/en/latest/) makes it easy to add color and style to terminal output. Rich can also render pretty tables, progress bars, markdown, syntax highlighted source code, tracebacks, and more — out of the box.\n\n![Features](https://github.com/willmcgugan/rich/raw/master/imgs/features.png)\n\nFor a video introduction to Rich see [calmcode.io](https://calmcode.io/rich/introduction.html) by [@fishnets88](https://twitter.com/fishnets88).\n\nSee what [people are saying about Rich](https://www.willmcgugan.com/blog/pages/post/rich-tweets/).\n\n## Compatibility\n\nRich works with Linux, OSX, and Windows. True color / emoji works with new Windows Terminal, classic terminal is limited to 8 colors. Rich requires Python 3.6.1 or later.\n\nRich works with [Jupyter notebooks](https://jupyter.org/) with no additional configuration required.\n\n## Installing\n\nInstall with `pip` or your favorite PyPi package manager.\n\n```\npip install rich\n```\n\nRun the following to test Rich output on your terminal:\n\n```\npython -m rich\n```\n\n## Rich print function\n\nTo effortlessly add rich output to your application, you can import the [rich print](https://rich.readthedocs.io/en/latest/introduction.html#quick-start) method, which has the same signature as the builtin Python function. Try this:\n\n```python\nfrom rich import print\n\nprint("Hello, [bold magenta]World[/bold magenta]!", ":vampire:", locals())\n```\n\n![Hello World](https://github.com/willmcgugan/rich/raw/master/imgs/print.png)\n\n## Rich REPL\n\nRich can be installed in the Python REPL, so that any data structures will be pretty printed and highlighted.\n\n```python\n>>> from rich import pretty\n>>> pretty.install()\n```\n\n![REPL](https://github.com/willmcgugan/rich/raw/master/imgs/repl.png)\n\n## Rich Inspect\n\nRich has an [inspect](https://rich.readthedocs.io/en/latest/reference/init.html?highlight=inspect#rich.inspect) function which can produce a report on any Python object, such as class, instance, or builtin.\n\n```python\n>>> from rich import inspect\n>>> inspect(str, methods=True)\n```\n\n## Using the Console\n\nFor more control over rich terminal content, import and construct a [Console](https://rich.readthedocs.io/en/latest/reference/console.html#rich.console.Console) object.\n\n```python\nfrom rich.console import Console\n\nconsole = Console()\n```\n\nThe Console object has a `print` method which has an intentionally similar interface to the builtin `print` function. Here\'s an example of use:\n\n```python\nconsole.print("Hello", "World!")\n```\n\nAs you might expect, this will print `"Hello World!"` to the terminal. Note that unlike the builtin `print` function, Rich will word-wrap your text to fit within the terminal width.\n\nThere are a few ways of adding color and style to your output. You can set a style for the entire output by adding a `style` keyword argument. Here\'s an example:\n\n```python\nconsole.print("Hello", "World!", style="bold red")\n```\n\nThe output will be something like the following:\n\n![Hello World](https://github.com/willmcgugan/rich/raw/master/imgs/hello_world.png)\n\nThat\'s fine for styling a line of text at a time. For more finely grained styling, Rich renders a special markup which is similar in syntax to [bbcode](https://en.wikipedia.org/wiki/BBCode). Here\'s an example:\n\n```python\nconsole.print("Where there is a [bold cyan]Will[/bold cyan] there [u]is[/u] a [i]way[/i].")\n```\n\n![Console Markup](https://github.com/willmcgugan/rich/raw/master/imgs/where_there_is_a_will.png)\n\n### Console logging\n\nThe Console object has a `log()` method which has a similar interface to `print()`, but also renders a column for the current time and the file and line which made the call. By default Rich will do syntax highlighting for Python structures and for repr strings. If you log a collection (i.e. a dict or a list) Rich will pretty print it so that it fits in the available space. Here\'s an example of some of these features.\n\n```python\nfrom rich.console import Console\nconsole = Console()\n\ntest_data = [\n    {"jsonrpc": "2.0", "method": "sum", "params": [None, 1, 2, 4, False, True], "id": "1",},\n    {"jsonrpc": "2.0", "method": "notify_hello", "params": [7]},\n    {"jsonrpc": "2.0", "method": "subtract", "params": [42, 23], "id": "2"},\n]\n\ndef test_log():\n    enabled = False\n    context = {\n        "foo": "bar",\n    }\n    movies = ["Deadpool", "Rise of the Skywalker"]\n    console.log("Hello from", console, "!")\n    console.log(test_data, log_locals=True)\n\n\ntest_log()\n```\n\nThe above produces the following output:\n\n![Log](https://github.com/willmcgugan/rich/raw/master/imgs/log.png)\n\nNote the `log_locals` argument, which outputs a table containing the local variables where the log method was called.\n\nThe log method could be used for logging to the terminal for long running applications such as servers, but is also a very nice debugging aid.\n\n### Logging Handler\n\nYou can also use the builtin [Handler class](https://rich.readthedocs.io/en/latest/logging.html) to format and colorize output from Python\'s logging module. Here\'s an example of the output:\n\n![Logging](https://github.com/willmcgugan/rich/raw/master/imgs/logging.png)\n\n## Emoji\n\nTo insert an emoji in to console output place the name between two colons. Here\'s an example:\n\n```python\n>>> console.print(":smiley: :vampire: :pile_of_poo: :thumbs_up: :raccoon:")\n😃 🧛 💩 👍 🦝\n```\n\nPlease use this feature wisely.\n\n## Tables\n\nRich can render flexible [tables](https://rich.readthedocs.io/en/latest/tables.html) with unicode box characters. There is a large variety of formatting options for borders, styles, cell alignment etc.\n\n![table movie](https://github.com/willmcgugan/rich/raw/master/imgs/table_movie.gif)\n\nThe animation above was generated with [table_movie.py](https://github.com/willmcgugan/rich/blob/master/examples/table_movie.py) in the examples directory.\n\nHere\'s a simpler table example:\n\n```python\nfrom rich.console import Console\nfrom rich.table import Table\n\nconsole = Console()\n\ntable = Table(show_header=True, header_style="bold magenta")\ntable.add_column("Date", style="dim", width=12)\ntable.add_column("Title")\ntable.add_column("Production Budget", justify="right")\ntable.add_column("Box Office", justify="right")\ntable.add_row(\n    "Dev 20, 2019", "Star Wars: The Rise of Skywalker", "$275,000,000", "$375,126,118"\n)\ntable.add_row(\n    "May 25, 2018",\n    "[red]Solo[/red]: A Star Wars Story",\n    "$275,000,000",\n    "$393,151,347",\n)\ntable.add_row(\n    "Dec 15, 2017",\n    "Star Wars Ep. VIII: The Last Jedi",\n    "$262,000,000",\n    "[bold]$1,332,539,889[/bold]",\n)\n\nconsole.print(table)\n```\n\nThis produces the following output:\n\n![table](https://github.com/willmcgugan/rich/raw/master/imgs/table.png)\n\nNote that console markup is rendered in the same way as `print()` and `log()`. In fact, anything that is renderable by Rich may be included in the headers / rows (even other tables).\n\nThe `Table` class is smart enough to resize columns to fit the available width of the terminal, wrapping text as required. Here\'s the same example, with the terminal made smaller than the table above:\n\n![table2](https://github.com/willmcgugan/rich/raw/master/imgs/table2.png)\n\n## Progress Bars\n\nRich can render multiple flicker-free [progress](https://rich.readthedocs.io/en/latest/progress.html) bars to track long-running tasks.\n\nFor basic usage, wrap any sequence in the `track` function and iterate over the result. Here\'s an example:\n\n```python\nfrom rich.progress import track\n\nfor step in track(range(100)):\n    do_step(step)\n```\n\nIt\'s not much harder to add multiple progress bars. Here\'s an example taken from the docs:\n\n![progress](https://github.com/willmcgugan/rich/raw/master/imgs/progress.gif)\n\nThe columns may be configured to show any details you want. Built-in columns include percentage complete, file size, file speed, and time remaining. Here\'s another example showing a download in progress:\n\n![progress](https://github.com/willmcgugan/rich/raw/master/imgs/downloader.gif)\n\nTo try this out yourself, see [examples/downloader.py](https://github.com/willmcgugan/rich/blob/master/examples/downloader.py) which can download multiple URLs simultaneously while displaying progress.\n\n## Status\n\nFor situations where it is hard to calculate progress, you can use the [status](https://rich.readthedocs.io/en/latest/reference/console.html#rich.console.Console.status) method which will display a \'spinner\' animation and message. The animation won\'t prevent you from using the console as normal. Here\'s an example:\n\n```python\nfrom time import sleep\nfrom rich.console import Console\n\nconsole = Console()\ntasks = [f"task {n}" for n in range(1, 11)]\n\nwith console.status("[bold green]Working on tasks...") as status:\n    while tasks:\n        task = tasks.pop(0)\n        sleep(1)\n        console.log(f"{task} complete")\n```\n\nThis generates the following output in the terminal.\n\n![status](https://github.com/willmcgugan/rich/raw/master/imgs/status.gif)\n\nThe spinner animations were borrowed from [cli-spinners](https://www.npmjs.com/package/cli-spinners). You can select a spinner by specifying the `spinner` parameter. Run the following command to see the available values:\n\n```\npython -m rich.spinner\n```\n\nThe above command generate the following output in the terminal:\n\n![spinners](https://github.com/willmcgugan/rich/raw/master/imgs/spinners.gif)\n\n## Tree\n\nRich can render a [tree](https://rich.readthedocs.io/en/latest/tree.html) with guide lines. A tree is ideal for displaying a file structure, or any other hierarchical data.\n\nThe labels of the tree can be simple text or anything else Rich can render. Run the following for a demonstration:\n\n```\npython -m rich.tree\n```\n\nThis generates the following output:\n\n![markdown](https://github.com/willmcgugan/rich/raw/master/imgs/tree.png)\n\nSee the [tree.py](https://github.com/willmcgugan/rich/blob/master/examples/tree.py) example for a script that displays a tree view of any directory, similar to the linux `tree` command.\n\n## Columns\n\nRich can render content in neat [columns](https://rich.readthedocs.io/en/latest/columns.html) with equal or optimal width. Here\'s a very basic clone of the (MacOS / Linux) `ls` command which displays a directory listing in columns:\n\n```python\nimport os\nimport sys\n\nfrom rich import print\nfrom rich.columns import Columns\n\ndirectory = os.listdir(sys.argv[1])\nprint(Columns(directory))\n```\n\nThe following screenshot is the output from the [columns example](https://github.com/willmcgugan/rich/blob/master/examples/columns.py) which displays data pulled from an API in columns:\n\n![columns](https://github.com/willmcgugan/rich/raw/master/imgs/columns.png)\n\n## Markdown\n\nRich can render [markdown](https://rich.readthedocs.io/en/latest/markdown.html) and does a reasonable job of translating the formatting to the terminal.\n\nTo render markdown import the `Markdown` class and construct it with a string containing markdown code. Then print it to the console. Here\'s an example:\n\n```python\nfrom rich.console import Console\nfrom rich.markdown import Markdown\n\nconsole = Console()\nwith open("README.md") as readme:\n    markdown = Markdown(readme.read())\nconsole.print(markdown)\n```\n\nThis will produce output something like the following:\n\n![markdown](https://github.com/willmcgugan/rich/raw/master/imgs/markdown.png)\n\n## Syntax Highlighting\n\nRich uses the [pygments](https://pygments.org/) library to implement [syntax highlighting](https://rich.readthedocs.io/en/latest/syntax.html). Usage is similar to rendering markdown; construct a `Syntax` object and print it to the console. Here\'s an example:\n\n```python\nfrom rich.console import Console\nfrom rich.syntax import Syntax\n\nmy_code = \'\'\'\ndef iter_first_last(values: Iterable[T]) -> Iterable[Tuple[bool, bool, T]]:\n    """Iterate and generate a tuple with a flag for first and last value."""\n    iter_values = iter(values)\n    try:\n        previous_value = next(iter_values)\n    except StopIteration:\n        return\n    first = True\n    for value in iter_values:\n        yield first, False, previous_value\n        first = False\n        previous_value = value\n    yield first, True, previous_value\n\'\'\'\nsyntax = Syntax(my_code, "python", theme="monokai", line_numbers=True)\nconsole = Console()\nconsole.print(syntax)\n```\n\nThis will produce the following output:\n\n![syntax](https://github.com/willmcgugan/rich/raw/master/imgs/syntax.png)\n\n## Tracebacks\n\nRich can render [beautiful tracebacks](https://rich.readthedocs.io/en/latest/traceback.html) which are easier to read and show more code than standard Python tracebacks. You can set Rich as the default traceback handler so all uncaught exceptions will be rendered by Rich.\n\nHere\'s what it looks like on OSX (similar on Linux):\n\n![traceback](https://github.com/willmcgugan/rich/raw/master/imgs/traceback.png)\n\n## Project using Rich\n\nHere are a few projects using Rich:\n\n- [BrancoLab/BrainRender](https://github.com/BrancoLab/BrainRender)\n  a python package for the visualization of three dimensional neuro-anatomical data\n- [Ciphey/Ciphey](https://github.com/Ciphey/Ciphey)\n  Automated decryption tool\n- [emeryberger/scalene](https://github.com/emeryberger/scalene)\n  a high-performance, high-precision CPU and memory profiler for Python\n- [hedythedev/StarCli](https://github.com/hedythedev/starcli)\n  Browse GitHub trending projects from your command line\n- [intel/cve-bin-tool](https://github.com/intel/cve-bin-tool)\n  This tool scans for a number of common, vulnerable components (openssl, libpng, libxml2, expat and a few others) to let you know if your system includes common libraries with known vulnerabilities.\n- [nf-core/tools](https://github.com/nf-core/tools)\n  Python package with helper tools for the nf-core community.\n- [cansarigol/pdbr](https://github.com/cansarigol/pdbr)\n  pdb + Rich library for enhanced debugging\n- [plant99/felicette](https://github.com/plant99/felicette)\n  Satellite imagery for dummies.\n- [seleniumbase/SeleniumBase](https://github.com/seleniumbase/SeleniumBase)\n  Automate & test 10x faster with Selenium & pytest. Batteries included.\n- [smacke/ffsubsync](https://github.com/smacke/ffsubsync)\n  Automagically synchronize subtitles with video.\n- [tryolabs/norfair](https://github.com/tryolabs/norfair)\n  Lightweight Python library for adding real-time 2D object tracking to any detector.\n- [ansible/ansible-lint](https://github.com/ansible/ansible-lint) Ansible-lint checks playbooks for practices and behaviour that could potentially be improved\n- [ansible-community/molecule](https://github.com/ansible-community/molecule) Ansible Molecule testing framework\n- +[Many more](https://github.com/willmcgugan/rich/network/dependents)!\n',
     'author': 'Will McGugan',
     'author_email': 'willmcgugan@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/willmcgugan/rich',
```

### Comparing `rich-9.8.2/PKG-INFO` & `rich-9.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich
-Version: 9.8.2
+Version: 9.9.0
 Summary: Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal
 Home-page: https://github.com/willmcgugan/rich
 License: MIT
 Author: Will McGugan
 Author-email: willmcgugan@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

