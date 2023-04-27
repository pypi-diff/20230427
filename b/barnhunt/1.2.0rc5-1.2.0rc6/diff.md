# Comparing `tmp/barnhunt-1.2.0rc5.tar.gz` & `tmp/barnhunt-1.2.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barnhunt-1.2.0rc5.tar", last modified: Mon Mar  6 03:20:28 2023, max compression
+gzip compressed data, was "barnhunt-1.2.0rc6.tar", last modified: Thu Apr 27 17:34:20 2023, max compression
```

## Comparing `barnhunt-1.2.0rc5.tar` & `barnhunt-1.2.0rc6.tar`

### file list

```diff
@@ -1,68 +1,53 @@
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.613256 barnhunt-1.2.0rc5/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    13437 2023-03-06 02:16:08.000000 barnhunt-1.2.0rc5/CHANGES.md
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)    32528 2022-08-20 01:47:19.000000 barnhunt-1.2.0rc5/LICENSE
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      321 2022-08-31 17:57:49.000000 barnhunt-1.2.0rc5/MANIFEST.in
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    17352 2023-03-06 03:20:28.613256 barnhunt-1.2.0rc5/PKG-INFO
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3179 2022-10-04 16:12:45.000000 barnhunt-1.2.0rc5/README.md
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.609256 barnhunt-1.2.0rc5/barnhunt/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)        0 2022-08-24 01:23:13.000000 barnhunt-1.2.0rc5/barnhunt/__init__.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       61 2022-08-24 01:24:12.000000 barnhunt-1.2.0rc5/barnhunt/__main__.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      449 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/barnhunt/_compat.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    13899 2022-10-19 04:43:42.000000 barnhunt-1.2.0rc5/barnhunt/cli.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     8946 2023-03-06 01:54:33.000000 barnhunt-1.2.0rc5/barnhunt/coursemaps.py
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.609256 barnhunt-1.2.0rc5/barnhunt/inkscape/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)        0 2017-11-16 05:03:25.000000 barnhunt-1.2.0rc5/barnhunt/inkscape/__init__.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3022 2023-03-05 18:12:18.000000 barnhunt-1.2.0rc5/barnhunt/inkscape/css.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    11435 2023-03-05 18:07:56.000000 barnhunt-1.2.0rc5/barnhunt/inkscape/runner.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    11204 2023-03-06 00:41:46.000000 barnhunt-1.2.0rc5/barnhunt/inkscape/svg.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     2565 2022-10-19 04:41:36.000000 barnhunt-1.2.0rc5/barnhunt/inkscape/utils.py
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.609256 barnhunt-1.2.0rc5/barnhunt/installer/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     8378 2022-10-16 22:55:25.000000 barnhunt-1.2.0rc5/barnhunt/installer/__init__.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     2101 2022-10-16 22:55:25.000000 barnhunt-1.2.0rc5/barnhunt/installer/github.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     4612 2022-10-19 01:28:28.000000 barnhunt-1.2.0rc5/barnhunt/installer/metadata.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     4717 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/barnhunt/layerinfo.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     4252 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/barnhunt/pager.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3865 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/barnhunt/pdfutil.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     7769 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/barnhunt/templating.py
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.609256 barnhunt-1.2.0rc5/barnhunt.egg-info/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    17352 2023-03-06 03:20:28.000000 barnhunt-1.2.0rc5/barnhunt.egg-info/PKG-INFO
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1363 2023-03-06 03:20:28.000000 barnhunt-1.2.0rc5/barnhunt.egg-info/SOURCES.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)        1 2023-03-06 03:20:28.000000 barnhunt-1.2.0rc5/barnhunt.egg-info/dependency_links.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       47 2023-03-06 03:20:28.000000 barnhunt-1.2.0rc5/barnhunt.egg-info/entry_points.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      214 2023-03-06 03:20:28.000000 barnhunt-1.2.0rc5/barnhunt.egg-info/requires.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)        9 2023-03-06 03:20:28.000000 barnhunt-1.2.0rc5/barnhunt.egg-info/top_level.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3123 2022-10-15 02:05:11.000000 barnhunt-1.2.0rc5/pyproject.toml
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       38 2023-03-06 03:20:28.613256 barnhunt-1.2.0rc5/setup.cfg
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.609256 barnhunt-1.2.0rc5/stubs/
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.609256 barnhunt-1.2.0rc5/stubs/pexpect/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       35 2022-08-24 22:18:46.000000 barnhunt-1.2.0rc5/stubs/pexpect/__init__.pyi
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      205 2022-08-24 22:18:46.000000 barnhunt-1.2.0rc5/stubs/pexpect/exceptions.pyi
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1774 2022-08-24 22:18:46.000000 barnhunt-1.2.0rc5/stubs/pexpect/popen_spawn.pyi
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     5501 2022-08-24 22:18:46.000000 barnhunt-1.2.0rc5/stubs/pexpect/spawnbase.pyi
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.613256 barnhunt-1.2.0rc5/tests/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1033 2022-10-16 15:23:21.000000 barnhunt-1.2.0rc5/tests/conftest.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     4089 2019-02-20 22:35:05.000000 barnhunt-1.2.0rc5/tests/drawing.svg
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.613256 barnhunt-1.2.0rc5/tests/inkscape/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      558 2022-08-24 22:18:46.000000 barnhunt-1.2.0rc5/tests/inkscape/dummy_inkscape.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     2221 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/tests/inkscape/test_css.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     7259 2023-03-06 02:14:38.000000 barnhunt-1.2.0rc5/tests/inkscape/test_runner.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1899 2023-01-10 05:32:03.000000 barnhunt-1.2.0rc5/tests/inkscape/test_shell_mode_integration.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    10830 2023-03-06 00:41:46.000000 barnhunt-1.2.0rc5/tests/inkscape/test_svg.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     4259 2023-01-10 01:28:36.000000 barnhunt-1.2.0rc5/tests/inkscape/test_utils.py
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-03-06 03:20:28.613256 barnhunt-1.2.0rc5/tests/installer/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      887 2022-10-16 22:55:25.000000 barnhunt-1.2.0rc5/tests/installer/ratelimit.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      627 2022-10-16 22:55:25.000000 barnhunt-1.2.0rc5/tests/installer/test_github.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)    11880 2023-01-10 01:17:59.000000 barnhunt-1.2.0rc5/tests/installer/test_installer.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3457 2022-10-19 01:30:27.000000 barnhunt-1.2.0rc5/tests/installer/test_metadata.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     4052 2019-02-20 22:35:05.000000 barnhunt-1.2.0rc5/tests/test1.pdf
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     4098 2019-02-20 22:35:05.000000 barnhunt-1.2.0rc5/tests/test2.pdf
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     5511 2022-10-16 22:55:25.000000 barnhunt-1.2.0rc5/tests/test_cli.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     8719 2023-03-06 00:41:46.000000 barnhunt-1.2.0rc5/tests/test_coursemaps.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3318 2022-08-31 17:57:49.000000 barnhunt-1.2.0rc5/tests/test_functional.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     5833 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/tests/test_layerinfo.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      350 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/tests/test_main.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3616 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/tests/test_pager.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     3998 2023-03-05 18:08:01.000000 barnhunt-1.2.0rc5/tests/test_pdfutil.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     9120 2022-08-25 01:22:56.000000 barnhunt-1.2.0rc5/tests/test_templating.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     2780 2023-03-06 00:41:46.000000 barnhunt-1.2.0rc5/tests/testlib.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     2105 2023-03-06 02:00:50.000000 barnhunt-1.2.0rc5/tox.ini
+-rw-r--r--   0        0        0    14281 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/CHANGES.md
+-rw-r--r--   0        0        0    32528 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/LICENSE
+-rw-r--r--   0        0        0     3179 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/README.md
+-rw-r--r--   0        0        0       61 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/__main__.py
+-rw-r--r--   0        0        0      360 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/_compat.py
+-rw-r--r--   0        0        0       22 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/_version.py
+-rw-r--r--   0        0        0    15274 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/cli.py
+-rw-r--r--   0        0        0     8946 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/coursemaps.py
+-rw-r--r--   0        0        0        0 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/__init__.py
+-rw-r--r--   0        0        0     3022 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/css.py
+-rw-r--r--   0        0        0    11435 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/runner.py
+-rw-r--r--   0        0        0    11100 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/svg.py
+-rw-r--r--   0        0        0     2565 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/inkscape/utils.py
+-rw-r--r--   0        0        0     8378 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/installer/__init__.py
+-rw-r--r--   0        0        0     2101 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/installer/github.py
+-rw-r--r--   0        0        0     4612 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/installer/metadata.py
+-rw-r--r--   0        0        0     4717 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/layerinfo.py
+-rw-r--r--   0        0        0     4252 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/pager.py
+-rw-r--r--   0        0        0     3843 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/pdfutil.py
+-rw-r--r--   0        0        0     7769 2023-04-27 17:34:10.339351 barnhunt-1.2.0rc6/barnhunt/templating.py
+-rw-r--r--   0        0        0     3882 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/pdm_build.py
+-rw-r--r--   0        0        0    10037 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/pyoxidizer/pyoxidizer.bzl
+-rw-r--r--   0        0        0    21401 2023-04-27 17:34:20.579693 barnhunt-1.2.0rc6/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/stubs/pexpect/__init__.pyi
+-rw-r--r--   0        0        0      205 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/stubs/pexpect/exceptions.pyi
+-rw-r--r--   0        0        0     1774 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/stubs/pexpect/popen_spawn.pyi
+-rw-r--r--   0        0        0     5501 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/stubs/pexpect/spawnbase.pyi
+-rw-r--r--   0        0        0     1033 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/conftest.py
+-rw-r--r--   0        0        0     4089 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/drawing.svg
+-rw-r--r--   0        0        0      558 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/dummy_inkscape.py
+-rw-r--r--   0        0        0     2221 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_css.py
+-rw-r--r--   0        0        0     7259 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_runner.py
+-rw-r--r--   0        0        0     1899 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_shell_mode_integration.py
+-rw-r--r--   0        0        0    10830 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_svg.py
+-rw-r--r--   0        0        0     4259 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/inkscape/test_utils.py
+-rw-r--r--   0        0        0      887 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/installer/ratelimit.py
+-rw-r--r--   0        0        0      627 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/installer/test_github.py
+-rw-r--r--   0        0        0    11880 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/installer/test_installer.py
+-rw-r--r--   0        0        0     3457 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/installer/test_metadata.py
+-rw-r--r--   0        0        0     4052 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test1.pdf
+-rw-r--r--   0        0        0     4098 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test2.pdf
+-rw-r--r--   0        0        0     6922 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_cli.py
+-rw-r--r--   0        0        0     8719 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_coursemaps.py
+-rw-r--r--   0        0        0     3366 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_functional.py
+-rw-r--r--   0        0        0     5833 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_layerinfo.py
+-rw-r--r--   0        0        0      350 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_main.py
+-rw-r--r--   0        0        0     3616 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_pager.py
+-rw-r--r--   0        0        0     3998 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_pdfutil.py
+-rw-r--r--   0        0        0     9120 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/test_templating.py
+-rw-r--r--   0        0        0     2780 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tests/testlib.py
+-rw-r--r--   0        0        0     1544 2023-04-27 17:34:10.343351 barnhunt-1.2.0rc6/tox.ini
+-rw-r--r--   0        0        0    18572 1970-01-01 00:00:00.000000 barnhunt-1.2.0rc6/PKG-INFO
```

### Comparing `barnhunt-1.2.0rc5/CHANGES.md` & `barnhunt-1.2.0rc6/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 ## Changes
 
+### Release 1.2.0rc6 (2023-04-27)
+
+- Build an Windows executable and installer using [PyOxidizer].  The
+  .msi installer should be downloadable from the
+  [Releases](https://github.com/barnhunt/barnhunt/releases) page.
+
+- Added a `--dump-loaded-modules` option which causes `barnhunt` to
+  write a list of all loaded modules the current working directory.
+  (This is a development tool, not generally useful to most users.)
+
+- Hardwire the distribution version into `barnhunt.__version__` rather
+  than deducing it via `importlib.metadata`.  This allows us to monkey
+  with the version we report from the PyOxidizer-built Windows
+  executable so that it indicates the MSI build version as well as
+  the distribution version.
+
+- Convert package from setuptools to PDM.
+
+[PyOxidizer]: https://pyoxidizer.readthedocs.io/en/stable/pyoxidizer.html
+
 ### Release 1.2.0rc5 (2023-03-05)
 
 #### Bugs Fixed
 
 - When there was a visible “clone” (`<svg:use>` element) that
   referenced a source on a hidden layer were being pruned from the SVG
   before conversion to PDF.  (When exporting an SVG, hidden layers are
```

### Comparing `barnhunt-1.2.0rc5/LICENSE` & `barnhunt-1.2.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/PKG-INFO` & `barnhunt-1.2.0rc6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 Metadata-Version: 2.1
 Name: barnhunt
-Version: 1.2.0rc5
+Version: 1.2.0rc6
 Summary: Helpers for drawing Barn Hunt course maps using Inkscape
-Author-email: Jeff Dairiki <dairiki@dairiki.org>
+Keywords: barn hunt inkscape course maps
+Author-Email: Jeff Dairiki <dairiki@dairiki.org>
 License: GPL-3.0-only
-Project-URL: Homepage, https://github.com/barnhunt/barnhunt
-Keywords: barn hunt,inkscape,course maps
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
+Project-URL: Homepage, https://github.com/barnhunt/barnhunt
 Requires-Python: >=3.7
+Requires-Dist: atomicwrites~=1.4
+Requires-Dist: click~=8.1
+Requires-Dist: jinja2~=3.1
+Requires-Dist: lxml~=4.9
+Requires-Dist: marshmallow~=3.19
+Requires-Dist: marshmallow-dataclass~=8.5.13
+Requires-Dist: packaging~=23.1
+Requires-Dist: pexpect~=4.8
+Requires-Dist: pikepdf~=6.2
+Requires-Dist: requests~=2.29
+Requires-Dist: tinycss2~=1.2
+Requires-Dist: typing-extensions~=4.5; python_version < "3.10"
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Barn Hunt Map Helper
 
 [![Tests](https://github.com/barnhunt/barnhunt/actions/workflows/tests.yml/badge.svg)](https://github.com/barnhunt/barnhunt/actions/workflows/tests.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/barnhunt.svg)](https://pypi.org/project/barnhunt/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/barnhunt.svg)](https://pypi.org/project/barnhunt/)
 [![Inkscape Versions](https://img.shields.io/badge/Inkscape-0.9x%E2%80%931.2-blue.svg?logo=inkscape)](https://inkscape.org/)
@@ -113,14 +124,34 @@
 [pipx]: https://pypa.github.io/pipx/ (The pipx home page)
 [pip]: https://pip.pypa.io/en/stable/ (Documentation for pip)
 [pikepdf]: https://pikepdf.readthedocs.io/en/latest/installation.html
 (The Installation section of the pikepdf documentation)
 
 ## Changes
 
+### Release 1.2.0rc6 (2023-04-27)
+
+- Build an Windows executable and installer using [PyOxidizer].  The
+  .msi installer should be downloadable from the
+  [Releases](https://github.com/barnhunt/barnhunt/releases) page.
+
+- Added a `--dump-loaded-modules` option which causes `barnhunt` to
+  write a list of all loaded modules the current working directory.
+  (This is a development tool, not generally useful to most users.)
+
+- Hardwire the distribution version into `barnhunt.__version__` rather
+  than deducing it via `importlib.metadata`.  This allows us to monkey
+  with the version we report from the PyOxidizer-built Windows
+  executable so that it indicates the MSI build version as well as
+  the distribution version.
+
+- Convert package from setuptools to PDM.
+
+[PyOxidizer]: https://pyoxidizer.readthedocs.io/en/stable/pyoxidizer.html
+
 ### Release 1.2.0rc5 (2023-03-05)
 
 #### Bugs Fixed
 
 - When there was a visible “clone” (`<svg:use>` element) that
   referenced a source on a hidden layer were being pruned from the SVG
   before conversion to PDF.  (When exporting an SVG, hidden layers are
```

### Comparing `barnhunt-1.2.0rc5/README.md` & `barnhunt-1.2.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/cli.py` & `barnhunt-1.2.0rc6/barnhunt/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import atexit
+import datetime
 import logging
 import os
 import random
 import sys
 from collections import defaultdict
 from contextlib import ExitStack
 from functools import partial
@@ -17,14 +19,15 @@
 from typing import Iterable
 from typing import Sequence
 from typing import TypeVar
 
 import click
 from atomicwrites import atomic_write
 
+import barnhunt
 from .coursemaps import Coursemap
 from .coursemaps import iter_coursemaps
 from .inkscape.runner import inkscape_runner
 from .inkscape.utils import get_user_data_directory
 from .installer import DEFAULT_REQUIREMENTS
 from .installer import InkexRequirement
 from .installer import Installer
@@ -36,28 +39,52 @@
 _U = TypeVar("_U")
 
 log = logging.getLogger("")
 
 POSITIVE_INT = click.IntRange(1, None)
 
 
+def _dump_loaded_modules() -> None:
+    utcnow = datetime.datetime.utcnow()
+    dump_file = f"barnhunt-modules.{os.getpid()}"
+    with open(dump_file, "w") as fp:
+        print(f"# Modules loaded by barnhunt {barnhunt.__version__}", file=fp)
+        print(f"# {utcnow.isoformat(timespec='seconds')}Z", file=fp)
+        print(f"# Command: {' '.join(sys.argv[1:])}", file=fp)
+        for name in sorted(sys.modules):
+            print(name, file=fp)
+    log.warning("Dumped loaded modules to %r", dump_file)
+
+
 @click.group()
 @click.option("-v", "--verbose", count=True)
-@click.version_option()
-def main(verbose: int) -> None:
+@click.option(
+    "--dump-loaded-modules/--no-dump-loaded-modules",
+    envvar="BARNHUNT_DUMP_LOADED_MODULES",
+    default=False,
+    help=(
+        "Write a list of loaded modules to barnhunt-modes.<pid> after "
+        "command completion. (This can also be controlled by setting "
+        "the $BARNHUNT_DUMP_LOADED_MODULES environment variable.)"
+    ),
+)
+@click.version_option(version=barnhunt.__version__)
+def barnhunt_cli(verbose: int, dump_loaded_modules: bool) -> None:
     """Utilities for creating Barn Hunt course maps."""
     log_level = logging.WARNING
     if verbose:  # pragma: NO COVER
         log_level = logging.DEBUG if verbose > 1 else logging.INFO
     logging.basicConfig(
         level=log_level, format="(%(levelname)1.1s) [%(threadName)s] %(message)s"
     )
+    if dump_loaded_modules:
+        atexit.register(_dump_loaded_modules)  # pragma: no cover
 
 
-@main.command()
+@barnhunt_cli.command()
 @click.argument(
     "svgfiles",
     type=click.Path(exists=True, dir_okay=False, writable=True),
     nargs=-1,
     required=True,
 )
 @click.option(
@@ -125,15 +152,15 @@
 def default_shell_mode() -> bool:
     """Whether to use Inkscape's shell-mode by default."""
     if sys.platform == "darwin":
         return False  # ShellModeRunner current borked
     return True
 
 
-@main.command()
+@barnhunt_cli.command()
 @click.argument("svgfiles", type=click.File("rb"), nargs=-1, required=True)
 @click.option(
     "--output-directory",
     "-o",
     type=click.Path(file_okay=False),
     default="pdfs",
     help="""
@@ -210,15 +237,15 @@
                 for coursemap in coursemaps:
                     log.info("Reading %s", coursemap.description)
 
             concat_pdfs(temp_fns, output_fn)
             log.warning("Wrote %d pages to %r", len(temp_fns), os.fspath(output_fn))
 
 
-@main.command("rats")
+@barnhunt_cli.command("rats")
 @click.option(
     "-n",
     "--number-of-rows",
     type=POSITIVE_INT,
     metavar="<n>",
     help="Number of rows of rat numbers to generate.  (Default: 5).",
     default=5,
@@ -229,15 +256,15 @@
     Prints rows of five random numbers in the range [1, 5].
     """
     for _ in range(number_of_rows):
         rats = tuple(random.randint(1, 5) for n in range(5))
         print("%d %d %d %d %d" % rats)
 
 
-@main.command()
+@barnhunt_cli.command()
 @click.option(
     "-n",
     "--number-of-rows",
     type=POSITIVE_INT,
     default=1000,
     metavar="<n>",
     help="Number of coordinates to generate. "
@@ -306,15 +333,15 @@
         )
     input_path = input_paths.pop()
     output_path = input_path.with_name(input_path.stem + "-2up" + input_path.suffix)
     click.echo(f"Writing output to {output_path!s}")
     return output_path
 
 
-@main.command(name="2up")
+@barnhunt_cli.command(name="2up")
 @click.argument("pdffiles", type=click.File("rb"), nargs=-1, required=True)
 @click.option(
     "-o",
     "--output-file",
     type=click.File("wb", atomic=True),
     default=default_2up_output_file,
     help="Output file name. " "(Default input filename with '-2up' appended to stem.)",
@@ -374,15 +401,15 @@
 ) -> str:
     if ctx.default_map is None:
         ctx.default_map = {}
     ctx.default_map["target"] = partial(get_user_data_directory, inkscape_command)
     return inkscape_command
 
 
-@main.command()
+@barnhunt_cli.command()
 @click.argument(
     "requirements",
     type=InkexRequirementType(),
     nargs=-1,
 )
 @click.option(
     "--upgrade/--no-upgrade", "-U", help="Upgrade to the newest available versions."
@@ -415,15 +442,15 @@
     """Install extensions and/or symbol sets."""
     installer = Installer(target, dry_run=dry_run, github_token=github_token)
     log.warning("installing to '%s'", target)
     for requirement in requirements or DEFAULT_REQUIREMENTS:
         installer.install(requirement, pre_flag=pre, upgrade=upgrade)
 
 
-@main.command()
+@barnhunt_cli.command()
 @click.argument(
     "requirements",
     type=InkexRequirementType(allow_specifiers=False),
     nargs=-1,
 )
 @click.option("-n", "--dry-run/--no-dry-run", help="Just show what would be done.")
 @target_option
@@ -437,7 +464,14 @@
     dry_run: bool,
     requirements: Sequence[InkexRequirement],
 ) -> None:
     """Uninstall extensions and/or symbol sets."""
     installer = Installer(target, dry_run=dry_run)
     for requirement in requirements or DEFAULT_REQUIREMENTS:
         installer.uninstall(requirement)
+
+
+def main(args: Sequence[str] | None = None) -> None:
+    prog_name = None  # by default let click figure out program name
+    if sys.argv[0] == "-c":
+        prog_name = "barnhunt"  # pragma: no cover
+    barnhunt_cli(args, prog_name=prog_name)
```

### Comparing `barnhunt-1.2.0rc5/barnhunt/coursemaps.py` & `barnhunt-1.2.0rc6/barnhunt/coursemaps.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/inkscape/css.py` & `barnhunt-1.2.0rc6/barnhunt/inkscape/css.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/inkscape/runner.py` & `barnhunt-1.2.0rc6/barnhunt/inkscape/runner.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/inkscape/svg.py` & `barnhunt-1.2.0rc6/barnhunt/inkscape/svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 import copy
 import dataclasses
 import math
 import random
 from collections import deque
 from functools import lru_cache
 from itertools import islice
-from typing import cast
 from typing import Collection
 from typing import Iterable
 from typing import Iterator
-from typing import List
 from typing import Mapping
 from typing import NamedTuple
 from typing import NewType
 from typing import overload
 from typing import TYPE_CHECKING
 
 from lxml import etree
@@ -39,15 +37,15 @@
 NSMAP = {
     "svg": "http://www.w3.org/2000/svg",
     "inkscape": "http://www.inkscape.org/namespaces/inkscape",
     "xlink": "http://www.w3.org/1999/xlink",
     "bh": "http://dairiki.org/barnhunt/inkscape-extensions",
 }
 
-etree.register_namespace("bh", NSMAP["bh"])  # type: ignore[attr-defined]
+etree.register_namespace("bh", NSMAP["bh"])
 
 
 def _qname(tag: str) -> str:
     prefix, sep, localname = tag.rpartition(":")
     assert sep
     return f"{{{NSMAP[prefix]}}}{localname}"
 
@@ -90,15 +88,15 @@
 
     """
     nodes = elem.findall("./" + LAYER_XP)
     while nodes:
         elem = LayerElement(nodes.pop())
         children = elem.findall("./" + LAYER_XP)
         children.reverse()
-        yield elem, cast(List[LayerElement], children)
+        yield elem, children
         nodes.extend(reversed(children))
 
 
 def is_layer(elem: Element) -> TypeGuard[LayerElement]:
     """Is elem an Inkscape layer element?"""
     return elem.tag == SVG_G_TAG and elem.get(INKSCAPE_GROUPMODE) == "layer"
```

### Comparing `barnhunt-1.2.0rc5/barnhunt/inkscape/utils.py` & `barnhunt-1.2.0rc6/barnhunt/inkscape/utils.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/installer/__init__.py` & `barnhunt-1.2.0rc6/barnhunt/installer/__init__.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/installer/github.py` & `barnhunt-1.2.0rc6/barnhunt/installer/github.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/installer/metadata.py` & `barnhunt-1.2.0rc6/barnhunt/installer/metadata.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/layerinfo.py` & `barnhunt-1.2.0rc6/barnhunt/layerinfo.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/pager.py` & `barnhunt-1.2.0rc6/barnhunt/pager.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/barnhunt/pdfutil.py` & `barnhunt-1.2.0rc6/barnhunt/pdfutil.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Iterable
 from typing import Sequence
 
 from pikepdf import ObjectStreamMode
 from pikepdf import Pdf
 from pikepdf import Rectangle
 
-from ._compat import metadata
+import barnhunt
 
 
 def concat_pdfs(in_fns: Sequence[str | Path], out_fn: str | Path) -> None:
     """Concatenate named PDF files to a single output file."""
     if len(in_fns) == 0:
         raise ValueError("No PDFs to concatenate")
     Path(out_fn).parent.mkdir(parents=True, exist_ok=True)
@@ -80,15 +80,15 @@
             src_meta = src.open_metadata()
             if src_meta:
                 meta.update(src_meta)
             else:
                 meta.load_from_docinfo(src.docinfo)
 
         date = iso_date(now_)
-        meta["pdf:Producer"] = f"barnhunt {metadata.version('barnhunt')}"
+        meta["pdf:Producer"] = f"barnhunt {barnhunt.__version__}"
         meta["xmp:MetadataDate"] = date
         meta.setdefault("xmp:ModifyDate", date)
 
 
 def iso_date(secs: float | None = None) -> str:
     """Format date and time to ISO-8601 format.
```

### Comparing `barnhunt-1.2.0rc5/barnhunt/templating.py` & `barnhunt-1.2.0rc6/barnhunt/templating.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/stubs/pexpect/popen_spawn.pyi` & `barnhunt-1.2.0rc6/stubs/pexpect/popen_spawn.pyi`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/stubs/pexpect/spawnbase.pyi` & `barnhunt-1.2.0rc6/stubs/pexpect/spawnbase.pyi`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/conftest.py` & `barnhunt-1.2.0rc6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/drawing.svg` & `barnhunt-1.2.0rc6/tests/drawing.svg`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/inkscape/dummy_inkscape.py` & `barnhunt-1.2.0rc6/tests/inkscape/dummy_inkscape.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/inkscape/test_css.py` & `barnhunt-1.2.0rc6/tests/inkscape/test_css.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/inkscape/test_runner.py` & `barnhunt-1.2.0rc6/tests/inkscape/test_runner.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/inkscape/test_shell_mode_integration.py` & `barnhunt-1.2.0rc6/tests/inkscape/test_shell_mode_integration.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/inkscape/test_svg.py` & `barnhunt-1.2.0rc6/tests/inkscape/test_svg.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/inkscape/test_utils.py` & `barnhunt-1.2.0rc6/tests/inkscape/test_utils.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/installer/ratelimit.py` & `barnhunt-1.2.0rc6/tests/installer/ratelimit.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/installer/test_github.py` & `barnhunt-1.2.0rc6/tests/installer/test_github.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/installer/test_installer.py` & `barnhunt-1.2.0rc6/tests/installer/test_installer.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/installer/test_metadata.py` & `barnhunt-1.2.0rc6/tests/installer/test_metadata.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/test1.pdf` & `barnhunt-1.2.0rc6/tests/test1.pdf`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/test2.pdf` & `barnhunt-1.2.0rc6/tests/test2.pdf`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/test_coursemaps.py` & `barnhunt-1.2.0rc6/tests/test_coursemaps.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/test_functional.py` & `barnhunt-1.2.0rc6/tests/test_functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 
 import pytest
 from click.testing import CliRunner
 from lxml import etree
 from pdfminer.high_level import extract_text
 
-from barnhunt.cli import main
+from barnhunt.cli import barnhunt_cli
 
 
 def test_random_seed(tmp_drawing_svg: Path, caplog: pytest.LogCaptureFixture) -> None:
     caplog.set_level(logging.INFO)
     svgfile = tmp_drawing_svg.__fspath__()
 
     def get_random_seed() -> int:
@@ -27,15 +27,15 @@
         return int(value)
 
     def run_it(*args: str) -> None:
         cmd = ["random-seed"]
         cmd.extend(args)
         cmd.append(svgfile)
         runner = CliRunner()
-        result = runner.invoke(main, cmd)
+        result = runner.invoke(barnhunt_cli, cmd)
         assert result.exit_code == 0
 
     # Set seed in SVG file without pre-existing seed
     run_it()
     random_seed = get_random_seed()
     assert isinstance(random_seed, int)
 
@@ -60,15 +60,15 @@
     caplog.set_level(logging.INFO)
     here = os.path.dirname(__file__)
     drawing_svg = os.path.join(here, "drawing.svg")
     cmd = ["pdfs", "-o", os.fspath(tmp_path), drawing_svg]
     if processes is not None:
         cmd[1:1] = ["-p", processes]
     runner = CliRunner()
-    result = runner.invoke(main, cmd)
+    result = runner.invoke(barnhunt_cli, cmd)
     assert result.exit_code == 0
     expected_pdfs = {
         "novice.pdf",
         "Master_1/Blind_1.pdf",
     }
     outputs = {
         Path(dirpath).joinpath(fn)
@@ -79,33 +79,33 @@
 
     # Check that template was expanded
     assert "Novice 1" in extract_text(tmp_path / "novice.pdf", page_numbers=[0])
 
 
 def test_rats() -> None:
     runner = CliRunner()
-    result = runner.invoke(main, ["rats"])
+    result = runner.invoke(barnhunt_cli, ["rats"])
     assert result.exit_code == 0
     assert re.sub(r"[1-5]", "X", result.output) == ("X X X X X\n" * 5)
 
 
 def test_coords() -> None:
     runner = CliRunner()
-    result = runner.invoke(main, ["coords", "-n", "50"])
+    result = runner.invoke(barnhunt_cli, ["coords", "-n", "50"])
     assert result.exit_code == 0
     lines = result.output.rstrip().split("\n")
     pairs = [list(map(int, line.split(","))) for line in lines if line]
     assert len(pairs) == 50
     for x, y in pairs:
         assert 0 <= x <= 25
         assert 0 <= y <= 30
 
 
 def test_2up(tmp_path: Path, test1_pdf: Path) -> None:
     outfile = tmp_path / "output.pdf"
     runner = CliRunner()
     result = runner.invoke(
-        main,
+        barnhunt_cli,
         ["2up", "-o", os.fspath(outfile), os.fspath(test1_pdf)],
     )
     assert result.exit_code == 0
     assert outfile.exists()
```

### Comparing `barnhunt-1.2.0rc5/tests/test_layerinfo.py` & `barnhunt-1.2.0rc6/tests/test_layerinfo.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/test_pager.py` & `barnhunt-1.2.0rc6/tests/test_pager.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/test_pdfutil.py` & `barnhunt-1.2.0rc6/tests/test_pdfutil.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/test_templating.py` & `barnhunt-1.2.0rc6/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tests/testlib.py` & `barnhunt-1.2.0rc6/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `barnhunt-1.2.0rc5/tox.ini` & `barnhunt-1.2.0rc6/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -48,54 +48,32 @@
 [testenv:lint]
 skip_install = true
 basepython =
     python3.10
 deps =
     build
     twine
-    flake8
-    flake8-bugbear
 
 commands =
     python -m build --sdist --outdir {envtmpdir}/dist {toxinidir}
     twine check {envtmpdir}/dist/*
-    flake8 barnhunt tests
 
 [testenv:mypy]
 usedevelop = true
 basepython =
     python3.10
 deps =
     {[testenv]deps}
-    mypy==0.982
+    mypy==1.2.0
     types-atomicwrites
     types-lxml
     types-requests
-
-    # pikepdf and click both seem to require importlib_metadata to be
-    # installed to type check correctly.  (They do try ... except
-    # Import Error ..., rather than conditional on sys.version_info.)
-    importlib_metadata
-
 commands =
     mypy barnhunt tests
 
-[testenv:devenv{,-py38,-py39,-py310,-py311}]
-# This is just here so that one can generate a development virtualenv by doing
-# something like:
-#
-#  tox -e devenv-py310 --devenv py310
-#
-commands =
-deps =
-    {[testenv]deps}
-    {[testenv:mypy]deps}
-    {[testenv:lint]deps}
-
-
 [flake8]
 max-line-length = 80
 
 exclude =
     .tox,
     .git,
     __pycache__,
```

