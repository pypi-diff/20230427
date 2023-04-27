# Comparing `tmp/pydash-7.0.1.tar.gz` & `tmp/pydash-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash-7.0.1.tar", last modified: Thu Apr 13 14:25:46 2023, max compression
+gzip compressed data, was "pydash-7.0.2.tar", last modified: Thu Apr 27 16:26:18 2023, max compression
```

## Comparing `pydash-7.0.1.tar` & `pydash-7.0.2.tar`

### file list

```diff
@@ -1,633 +1,633 @@
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.745897 pydash-7.0.1/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.706101 pydash-7.0.1/.tox/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.691368 pydash-7.0.1/.tox/.package/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.691462 pydash-7.0.1/.tox/.package/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.691515 pydash-7.0.1/.tox/.package/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.691561 pydash-7.0.1/.tox/.package/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.712310 pydash-7.0.1/.tox/.package/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.1/.tox/.package/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.691672 pydash-7.0.1/.tox/.pkg/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.691716 pydash-7.0.1/.tox/.pkg/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.691756 pydash-7.0.1/.tox/.pkg/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.691797 pydash-7.0.1/.tox/.pkg/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.712446 pydash-7.0.1/.tox/.pkg/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.1/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.691960 pydash-7.0.1/.tox/3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.692010 pydash-7.0.1/.tox/3.11/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.692062 pydash-7.0.1/.tox/3.11/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.694596 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.712590 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.712712 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.712829 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.712945 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.713074 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.713185 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.713316 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.713429 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.713535 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.713629 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.713726 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.713843 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.713949 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.714054 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.714154 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.714261 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.693197 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.714369 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.714497 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.714605 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.714706 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.714816 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.714906 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.715024 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.715122 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.715240 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.715355 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.715482 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.715608 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.715720 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.715833 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.715944 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716047 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716153 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716282 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716380 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716490 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716596 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716697 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716783 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716874 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.1/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.694711 pydash-7.0.1/.tox/py310/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.694831 pydash-7.0.1/.tox/py310/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.694954 pydash-7.0.1/.tox/py310/lib/python3.10/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.697424 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.716977 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.717078 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.717178 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.717283 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.717398 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.717497 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.717598 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.717702 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.717804 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.717909 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718009 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718117 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718217 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718314 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718410 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718517 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718617 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.696051 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718723 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718842 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.718937 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719041 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719152 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719232 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719347 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719446 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719552 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719657 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719763 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719868 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.719965 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720061 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720149 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720235 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720317 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720421 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720512 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720600 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720688 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720775 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720882 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.720961 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721053 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.1/.tox/py310/lib/python3.10/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.697522 pydash-7.0.1/.tox/py311/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.697564 pydash-7.0.1/.tox/py311/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.697606 pydash-7.0.1/.tox/py311/lib/python3.11/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.700155 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721150 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721229 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721309 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721387 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721483 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721572 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721653 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721733 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721811 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721892 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.721981 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722086 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722175 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722269 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722358 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722454 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.698728 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722555 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722665 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722754 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722846 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.722961 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723059 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723169 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723255 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723352 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723439 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723542 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723652 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723743 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723831 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.723938 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724041 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724143 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724269 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724370 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724463 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724556 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724655 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724756 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724856 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.1/.tox/py311/lib/python3.11/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.700271 pydash-7.0.1/.tox/py37/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.700320 pydash-7.0.1/.tox/py37/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.700368 pydash-7.0.1/.tox/py37/lib/python3.7/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.702999 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.724964 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725065 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725149 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725233 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725342 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725442 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725542 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725636 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725735 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725829 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.725948 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726045 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726152 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726251 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726331 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726422 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.701433 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726514 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726628 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726728 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726823 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.726943 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727041 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727152 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727243 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727355 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727450 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727572 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727683 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727776 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727873 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/py/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.702352 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.727979 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/py/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728073 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728167 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728260 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728369 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728453 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728530 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728610 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728691 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728818 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.728927 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.1/.tox/py37/lib/python3.7/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.703106 pydash-7.0.1/.tox/py38/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.703154 pydash-7.0.1/.tox/py38/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.703204 pydash-7.0.1/.tox/py38/lib/python3.8/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.706030 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.729046 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.729149 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.729243 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.729340 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.729456 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.729560 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.729668 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.729830 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.729955 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.730077 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.730200 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.730345 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.730459 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.730595 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.730706 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.730820 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/importlib_resources/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.730936 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.731050 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.704443 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.731166 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.731302 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.731413 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.731529 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.731662 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.731768 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.731895 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.732010 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.732148 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.732267 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.732404 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.732536 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.732644 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.732756 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.732869 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.732964 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.733052 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.733168 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.733276 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.733382 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.733490 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.733597 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.733726 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.733844 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.733960 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.1/.tox/py38/lib/python3.8/site-packages/twine/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.706153 pydash-7.0.1/.tox/py39/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.706205 pydash-7.0.1/.tox/py39/lib/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.706258 pydash-7.0.1/.tox/py39/lib/python3.9/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.709402 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.734069 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/_pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.734186 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/attr/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/attr/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.734295 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/attrs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.734436 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/babel/
--rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/babel/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.734546 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/black/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/black/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.734647 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/build/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/build/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.734762 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/certifi/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.734872 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/chardet/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.734978 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.735080 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/click/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/click/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.735182 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/coverage/
--rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.735310 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.735421 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/filelock/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.735527 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/idna/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/idna/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.735649 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.735753 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/iniconfig/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.735864 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/isort/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.707604 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.735981 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/isort/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.736107 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/jinja2/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.736239 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/keyring/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.736345 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/markdown_it/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.736472 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/markupsafe/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.736580 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/mdurl/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.736695 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/more_itertools/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.736797 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/mypy/
--rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.736915 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/packaging/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737012 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pathspec/
--rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737131 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pip/
--rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pip/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737247 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pkginfo/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737343 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/platformdirs/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737439 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737542 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pyproject_api/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737637 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pytest/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737726 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737838 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/readme_renderer/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.737934 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/rich/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/rich/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.738025 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/sphinx/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.738120 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.738212 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/tomli/
--rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.738324 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/tomlkit/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.738423 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/tox/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/tox/py.typed
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.738521 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/twine/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.1/.tox/py39/lib/python3.9/site-packages/twine/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)     1257 2021-06-27 18:15:07.000000 pydash-7.0.1/AUTHORS.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    40123 2023-04-13 14:15:46.000000 pydash-7.0.1/CHANGELOG.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.1/CONTRIBUTING.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.1/LICENSE.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.1/MANIFEST.in
--rw-r--r--   0 dgilland   (501) staff       (20)    43598 2023-04-13 14:25:46.745991 pydash-7.0.1/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.1/README.rst
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.740647 pydash-7.0.1/docs/
--rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/Makefile
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.740834 pydash-7.0.1/docs/_static/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.1/docs/_static/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)      137 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/_static/theme_override.css
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.740941 pydash-7.0.1/docs/_templates/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.1/docs/_templates/.gitignore
--rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/api.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.1/docs/authors.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/callbacks.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.1/docs/chaining.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/changelog.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     5733 2022-09-23 13:07:13.000000 pydash-7.0.1/docs/conf.py
--rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.1/docs/contributing.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/deeppath.rst
--rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.1/docs/devguide.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/differences.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.1/docs/index.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.1/docs/installation.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/kudos.rst
--rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.1/docs/license.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/quickstart.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/templating.rst
--rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.1/docs/upgrading.rst
--rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.1/docs/versioning.rst
--rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.1/pylintrc
--rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.1/pyproject.toml
--rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.1/requirements.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     2533 2023-04-13 14:25:46.746389 pydash-7.0.1/setup.cfg
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.709837 pydash-7.0.1/src/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.742298 pydash-7.0.1/src/pydash/
--rw-r--r--   0 dgilland   (501) staff       (20)     5373 2023-04-13 14:16:25.000000 pydash-7.0.1/src/pydash/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    69680 2023-04-12 02:13:49.000000 pydash-7.0.1/src/pydash/arrays.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.743304 pydash-7.0.1/src/pydash/chaining/
--rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.1/src/pydash/chaining/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.1/src/pydash/chaining/all_funcs.py
--rw-r--r--   0 dgilland   (501) staff       (20)   123183 2023-04-12 02:15:39.000000 pydash-7.0.1/src/pydash/chaining/all_funcs.pyi
--rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.1/src/pydash/chaining/chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.1/src/pydash/collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.1/src/pydash/exceptions.py
--rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.1/src/pydash/functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.1/src/pydash/helpers.py
--rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.1/src/pydash/numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.1/src/pydash/objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.1/src/pydash/predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.1/src/pydash/py.typed
--rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.1/src/pydash/strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)      593 2023-03-18 22:34:56.000000 pydash-7.0.1/src/pydash/types.py
--rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.1/src/pydash/utilities.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.742840 pydash-7.0.1/src/pydash.egg-info/
--rw-r--r--   0 dgilland   (501) staff       (20)    43598 2023-04-13 14:25:44.000000 pydash-7.0.1/src/pydash.egg-info/PKG-INFO
--rw-r--r--   0 dgilland   (501) staff       (20)    16310 2023-04-13 14:25:46.000000 pydash-7.0.1/src/pydash.egg-info/SOURCES.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-04-13 14:25:44.000000 pydash-7.0.1/src/pydash.egg-info/dependency_links.txt
--rw-r--r--   0 dgilland   (501) staff       (20)      293 2023-04-13 14:25:44.000000 pydash-7.0.1/src/pydash.egg-info/requires.txt
--rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-04-13 14:25:44.000000 pydash-7.0.1/src/pydash.egg-info/top_level.txt
--rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.1/tasks.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.744646 pydash-7.0.1/tests/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.1/tests/__init__.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.710117 pydash-7.0.1/tests/build/
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.744773 pydash-7.0.1/tests/build/testresults/
--rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.1/tests/build/testresults/junit.xml
--rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.1/tests/conftest.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.1/tests/helpers.py
-drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-13 14:25:46.745789 pydash-7.0.1/tests/pytest_mypy_testing/
--rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.1/tests/pytest_mypy_testing/__init__.py
--rw-r--r--   0 dgilland   (501) staff       (20)    16142 2023-04-12 02:13:49.000000 pydash-7.0.1/tests/pytest_mypy_testing/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.1/tests/pytest_mypy_testing/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.1/tests/pytest_mypy_testing/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.1/tests/pytest_mypy_testing/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.1/tests/pytest_mypy_testing/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.1/tests/pytest_mypy_testing/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.1/tests/pytest_mypy_testing/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.1/tests/pytest_mypy_testing/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.1/tests/pytest_mypy_testing/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.1/tests/test_annotations.py
--rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.1/tests/test_arrays.py
--rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.1/tests/test_chaining.py
--rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.1/tests/test_collections.py
--rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.1/tests/test_functions.py
--rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.1/tests/test_numerical.py
--rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.1/tests/test_objects.py
--rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.1/tests/test_predicates.py
--rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.1/tests/test_strings.py
--rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.1/tests/test_utilities.py
--rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.1/tox.ini
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.466705 pydash-7.0.2/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414261 pydash-7.0.2/.tox/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400546 pydash-7.0.2/.tox/.package/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400608 pydash-7.0.2/.tox/.package/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400655 pydash-7.0.2/.tox/.package/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400705 pydash-7.0.2/.tox/.package/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421087 pydash-7.0.2/.tox/.package/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:46.000000 pydash-7.0.2/.tox/.package/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400826 pydash-7.0.2/.tox/.pkg/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400864 pydash-7.0.2/.tox/.pkg/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400903 pydash-7.0.2/.tox/.pkg/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.400940 pydash-7.0.2/.tox/.pkg/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421374 pydash-7.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:04.000000 pydash-7.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.401048 pydash-7.0.2/.tox/3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.401085 pydash-7.0.2/.tox/3.11/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.401129 pydash-7.0.2/.tox/3.11/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.403638 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421610 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421699 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421784 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.421870 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422164 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422256 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422353 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422467 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422568 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422662 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.422765 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423048 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423148 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423239 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423330 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423422 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.402244 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423514 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423799 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.423904 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424005 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424264 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424365 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424573 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424651 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424884 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.424977 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425197 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:23:03.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425405 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425485 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425567 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:35:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425663 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425752 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:22.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.425850 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426100 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426185 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426277 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426365 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426448 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:21.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426538 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:23.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426621 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:23:24.000000 pydash-7.0.2/.tox/3.11/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.403741 pydash-7.0.2/.tox/py310/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.403779 pydash-7.0.2/.tox/py310/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.403816 pydash-7.0.2/.tox/py310/lib/python3.10/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.406074 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426709 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426800 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426889 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.426977 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427242 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427318 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427399 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427474 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427550 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427635 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427729 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.427979 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428064 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428148 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428229 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428318 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428409 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.404791 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428493 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428776 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428866 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.428947 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429170 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429250 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429494 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429588 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429806 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.429893 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430123 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:53:26.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430318 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430402 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430494 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:41.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430582 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430678 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:42.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.430770 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431018 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431097 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431178 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431264 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431352 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:53:40.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431679 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:40.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431782 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:43.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431883 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:53:44.000000 pydash-7.0.2/.tox/py310/lib/python3.10/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.406167 pydash-7.0.2/.tox/py311/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.406203 pydash-7.0.2/.tox/py311/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.406241 pydash-7.0.2/.tox/py311/lib/python3.11/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.408814 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.431985 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432068 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432157 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432252 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432517 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432599 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432678 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432764 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432847 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.432940 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433028 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433273 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433354 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433446 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433528 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433615 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.407209 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433709 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.433966 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434044 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434128 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434404 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434516 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434807 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.434910 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435156 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435254 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435501 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 02:01:09.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435731 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435825 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435916 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 02:06:00.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.435996 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436079 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:36.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436173 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436408 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436497 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436586 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436669 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436751 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:35.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436833 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:37.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.436924 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:54:38.000000 pydash-7.0.2/.tox/py311/lib/python3.11/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.408936 pydash-7.0.2/.tox/py37/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.408979 pydash-7.0.2/.tox/py37/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.409018 pydash-7.0.2/.tox/py37/lib/python3.7/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.411424 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437013 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437096 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437173 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437250 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437473 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437553 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437639 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437719 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437797 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.437878 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438152 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438246 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438340 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438433 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438512 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438603 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.409998 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438690 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.438920 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439001 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439091 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439371 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439461 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439689 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439773 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.439972 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440053 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440248 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:49:52.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440446 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440529 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:32.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440607 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.410863 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440688 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/_vendored_packages/iniconfig/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/py/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440774 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:31.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440857 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.440937 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441155 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441235 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441315 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441394 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441479 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:50:30.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441715 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:30.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441800 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:50:33.000000 pydash-7.0.2/.tox/py37/lib/python3.7/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.411550 pydash-7.0.2/.tox/py38/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.411585 pydash-7.0.2/.tox/py38/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.411622 pydash-7.0.2/.tox/py38/lib/python3.8/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414204 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441883 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.441971 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442077 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442176 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442456 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442560 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442645 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442740 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442840 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.442942 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443050 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443335 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443431 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443518 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443616 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443715 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/importlib_resources/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/importlib_resources/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443823 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.443951 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.412680 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444068 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444349 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444458 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444558 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444824 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.444930 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445201 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445322 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445542 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445651 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.445919 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:51:24.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446176 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446291 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446408 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:36.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446523 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446634 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:37.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.446740 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447048 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447174 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447301 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447423 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447540 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:51:35.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447803 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:35.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.447919 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:38.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448038 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:51:39.000000 pydash-7.0.2/.tox/py38/lib/python3.8/site-packages/twine/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414298 pydash-7.0.2/.tox/py39/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414337 pydash-7.0.2/.tox/py39/lib/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.414387 pydash-7.0.2/.tox/py39/lib/python3.9/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.417498 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448159 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/_pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/_pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448271 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/attr/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/attr/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448374 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/attrs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/attrs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448476 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/babel/
+-rw-r--r--   0 dgilland   (501) staff       (20)       59 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/babel/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448757 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/black/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/black/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448868 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/build/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/build/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.448970 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/certifi/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/certifi/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449059 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/chardet/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/chardet/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449157 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/charset_normalizer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/charset_normalizer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449263 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/click/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/click/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449375 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/coverage/
+-rw-r--r--   0 dgilland   (501) staff       (20)       72 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/coverage/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449649 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/exceptiongroup/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/exceptiongroup/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449755 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/filelock/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/filelock/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449865 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/idna/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/idna/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.449979 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/importlib_metadata/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/importlib_metadata/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450089 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/iniconfig/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/iniconfig/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450201 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.415679 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/_vendored/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450315 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/_vendored/tomli/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/isort/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450583 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/jinja2/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/jinja2/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450701 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/keyring/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/keyring/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.450811 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/markdown_it/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/markdown_it/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451060 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/markupsafe/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/markupsafe/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451170 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/mdurl/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/mdurl/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451395 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/more_itertools/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/more_itertools/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451521 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/mypy/
+-rw-r--r--   0 dgilland   (501) staff       (20)       64 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/mypy/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451739 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/packaging/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/packaging/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.451841 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pathspec/
+-rw-r--r--   0 dgilland   (501) staff       (20)       68 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pathspec/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452127 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 dgilland   (501) staff       (20)      286 2023-04-06 01:52:27.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pip/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452335 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pkginfo/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pkginfo/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452417 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/platformdirs/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/platformdirs/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452499 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:39.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pydash/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452588 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pyproject_api/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pyproject_api/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452685 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pytest/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:40.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pytest/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.452789 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)       77 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/pytest_mypy_testing/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453034 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/readme_renderer/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/readme_renderer/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453126 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/rich/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/rich/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453223 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/sphinx/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/sphinx/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453328 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/sphinx_autodoc_typehints/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453432 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tomli/
+-rw-r--r--   0 dgilland   (501) staff       (20)       26 2023-04-06 01:52:38.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tomli/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453664 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tomlkit/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:38.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tomlkit/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453769 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tox/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/tox/py.typed
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.453872 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/twine/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-04-06 01:52:41.000000 pydash-7.0.2/.tox/py39/lib/python3.9/site-packages/twine/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)     1257 2021-06-27 18:15:07.000000 pydash-7.0.2/AUTHORS.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    40342 2023-04-27 16:17:02.000000 pydash-7.0.2/CHANGELOG.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2581 2020-10-29 15:03:50.000000 pydash-7.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1072 2021-01-05 22:53:19.000000 pydash-7.0.2/LICENSE.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      283 2023-03-18 22:34:56.000000 pydash-7.0.2/MANIFEST.in
+-rw-r--r--   0 dgilland   (501) staff       (20)    43817 2023-04-27 16:26:18.466780 pydash-7.0.2/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)     1243 2020-10-29 02:16:13.000000 pydash-7.0.2/README.rst
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.456801 pydash-7.0.2/docs/
+-rw-r--r--   0 dgilland   (501) staff       (20)     3937 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/Makefile
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.457028 pydash-7.0.2/docs/_static/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.2/docs/_static/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)      137 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/_static/theme_override.css
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.457168 pydash-7.0.2/docs/_templates/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-30 00:13:44.000000 pydash-7.0.2/docs/_templates/.gitignore
+-rw-r--r--   0 dgilland   (501) staff       (20)     2885 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/api.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       28 2014-07-29 03:38:06.000000 pydash-7.0.2/docs/authors.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4065 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/callbacks.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2927 2021-09-28 21:40:18.000000 pydash-7.0.2/docs/chaining.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       30 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/changelog.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     5733 2022-09-23 13:07:13.000000 pydash-7.0.2/docs/conf.py
+-rw-r--r--   0 dgilland   (501) staff       (20)       33 2014-07-29 03:34:57.000000 pydash-7.0.2/docs/contributing.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      760 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/deeppath.rst
+-rw-rw-r--   0 dgilland   (501) staff       (20)       29 2020-10-28 20:30:40.000000 pydash-7.0.2/docs/devguide.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     2045 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/differences.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      605 2020-10-29 19:54:30.000000 pydash-7.0.2/docs/index.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      187 2021-06-27 18:15:05.000000 pydash-7.0.2/docs/installation.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      100 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/kudos.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)       45 2021-01-05 22:53:19.000000 pydash-7.0.2/docs/license.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     1499 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/quickstart.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      562 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/templating.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)    10538 2019-02-04 01:30:20.000000 pydash-7.0.2/docs/upgrading.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)      497 2014-08-20 02:16:49.000000 pydash-7.0.2/docs/versioning.rst
+-rw-r--r--   0 dgilland   (501) staff       (20)     4371 2021-07-15 23:20:06.000000 pydash-7.0.2/pylintrc
+-rw-r--r--   0 dgilland   (501) staff       (20)      274 2022-09-23 12:58:40.000000 pydash-7.0.2/pyproject.toml
+-rw-r--r--   0 dgilland   (501) staff       (20)       10 2020-10-28 20:38:46.000000 pydash-7.0.2/requirements.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     2528 2023-04-27 16:26:18.467153 pydash-7.0.2/setup.cfg
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.417917 pydash-7.0.2/src/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.460127 pydash-7.0.2/src/pydash/
+-rw-r--r--   0 dgilland   (501) staff       (20)    11148 2023-04-27 16:17:18.000000 pydash-7.0.2/src/pydash/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    69680 2023-04-12 02:13:49.000000 pydash-7.0.2/src/pydash/arrays.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.461728 pydash-7.0.2/src/pydash/chaining/
+-rw-r--r--   0 dgilland   (501) staff       (20)      111 2023-03-18 22:34:56.000000 pydash-7.0.2/src/pydash/chaining/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1364 2023-03-20 14:30:38.000000 pydash-7.0.2/src/pydash/chaining/all_funcs.py
+-rw-r--r--   0 dgilland   (501) staff       (20)   123183 2023-04-12 02:15:39.000000 pydash-7.0.2/src/pydash/chaining/all_funcs.pyi
+-rw-r--r--   0 dgilland   (501) staff       (20)     8218 2023-03-20 14:30:38.000000 pydash-7.0.2/src/pydash/chaining/chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    54698 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      431 2023-03-18 22:34:56.000000 pydash-7.0.2/src/pydash/exceptions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    39876 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8901 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/helpers.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    27145 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    62990 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    26652 2023-03-20 14:30:38.000000 pydash-7.0.2/src/pydash/predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.2/src/pydash/py.typed
+-rw-r--r--   0 dgilland   (501) staff       (20)    57917 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      690 2023-04-27 16:14:56.000000 pydash-7.0.2/src/pydash/types.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    38320 2023-04-12 02:03:04.000000 pydash-7.0.2/src/pydash/utilities.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.460739 pydash-7.0.2/src/pydash.egg-info/
+-rw-r--r--   0 dgilland   (501) staff       (20)    43817 2023-04-27 16:26:16.000000 pydash-7.0.2/src/pydash.egg-info/PKG-INFO
+-rw-r--r--   0 dgilland   (501) staff       (20)    16310 2023-04-27 16:26:18.000000 pydash-7.0.2/src/pydash.egg-info/SOURCES.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        1 2023-04-27 16:26:16.000000 pydash-7.0.2/src/pydash.egg-info/dependency_links.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)      293 2023-04-27 16:26:16.000000 pydash-7.0.2/src/pydash.egg-info/requires.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)        7 2023-04-27 16:26:16.000000 pydash-7.0.2/src/pydash.egg-info/top_level.txt
+-rw-r--r--   0 dgilland   (501) staff       (20)     6510 2023-04-06 20:16:10.000000 pydash-7.0.2/tasks.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.464327 pydash-7.0.2/tests/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2014-07-23 03:21:55.000000 pydash-7.0.2/tests/__init__.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.418208 pydash-7.0.2/tests/build/
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.464479 pydash-7.0.2/tests/build/testresults/
+-rw-r--r--   0 dgilland   (501) staff       (20)      925 2023-04-06 01:12:00.000000 pydash-7.0.2/tests/build/testresults/junit.xml
+-rw-r--r--   0 dgilland   (501) staff       (20)      143 2022-09-23 13:25:56.000000 pydash-7.0.2/tests/conftest.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1870 2022-09-23 13:11:57.000000 pydash-7.0.2/tests/helpers.py
+drwxr-xr-x   0 dgilland   (501) staff       (20)        0 2023-04-27 16:26:18.466591 pydash-7.0.2/tests/pytest_mypy_testing/
+-rw-r--r--   0 dgilland   (501) staff       (20)        0 2023-03-18 22:34:56.000000 pydash-7.0.2/tests/pytest_mypy_testing/__init__.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    16142 2023-04-12 02:13:49.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     1234 2023-04-12 02:10:33.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8643 2023-04-12 02:10:41.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9870 2023-04-12 02:15:39.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     5582 2023-04-12 02:10:58.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13212 2023-04-12 02:11:04.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    10786 2023-04-12 02:15:39.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    13294 2023-04-12 02:15:39.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     8532 2023-04-12 02:15:39.000000 pydash-7.0.2/tests/pytest_mypy_testing/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      178 2021-06-27 18:15:05.000000 pydash-7.0.2/tests/test_annotations.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    24160 2021-09-28 21:40:18.000000 pydash-7.0.2/tests/test_arrays.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     4229 2023-03-18 22:34:56.000000 pydash-7.0.2/tests/test_chaining.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    29669 2022-09-23 13:19:05.000000 pydash-7.0.2/tests/test_collections.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     9935 2022-09-23 13:25:56.000000 pydash-7.0.2/tests/test_functions.py
+-rw-r--r--   0 dgilland   (501) staff       (20)     7640 2021-06-27 18:15:05.000000 pydash-7.0.2/tests/test_numerical.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    28249 2023-03-18 22:34:56.000000 pydash-7.0.2/tests/test_objects.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    12617 2022-09-23 13:19:37.000000 pydash-7.0.2/tests/test_predicates.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    33926 2023-04-06 01:12:00.000000 pydash-7.0.2/tests/test_strings.py
+-rw-r--r--   0 dgilland   (501) staff       (20)    18221 2023-03-18 22:34:56.000000 pydash-7.0.2/tests/test_utilities.py
+-rw-r--r--   0 dgilland   (501) staff       (20)      296 2023-01-28 17:36:13.000000 pydash-7.0.2/tox.ini
```

### Comparing `pydash-7.0.1/AUTHORS.rst` & `pydash-7.0.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/CHANGELOG.rst` & `pydash-7.0.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.2 (2023-04-27)
+-------------------
+
+- Fix issue where using ``pyright`` as a type checker with ``reportPrivateUsage=true`` would report errors that objects are not exported from ``pydash``. Thanks DeviousStoat_!
+
+
 v7.0.1 (2023-04-13)
 -------------------
 
 - Fix missing install dependency, ``typing-extensions``, for package.
 
 
 v7.0.0 (2023-04-11)
```

### Comparing `pydash-7.0.1/CONTRIBUTING.rst` & `pydash-7.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/LICENSE.rst` & `pydash-7.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/PKG-INFO` & `pydash-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.1
+Version: 7.0.2
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,20 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.2 (2023-04-27)
+-------------------
+
+- Fix issue where using ``pyright`` as a type checker with ``reportPrivateUsage=true`` would report errors that objects are not exported from ``pydash``. Thanks DeviousStoat_!
+
+
 v7.0.1 (2023-04-13)
 -------------------
 
 - Fix missing install dependency, ``typing-extensions``, for package.
 
 
 v7.0.0 (2023-04-11)
```

### Comparing `pydash-7.0.1/README.rst` & `pydash-7.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/Makefile` & `pydash-7.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/api.rst` & `pydash-7.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/callbacks.rst` & `pydash-7.0.2/docs/callbacks.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/chaining.rst` & `pydash-7.0.2/docs/chaining.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/conf.py` & `pydash-7.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/deeppath.rst` & `pydash-7.0.2/docs/deeppath.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/differences.rst` & `pydash-7.0.2/docs/differences.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/index.rst` & `pydash-7.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/quickstart.rst` & `pydash-7.0.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/templating.rst` & `pydash-7.0.2/docs/templating.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/docs/upgrading.rst` & `pydash-7.0.2/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/pylintrc` & `pydash-7.0.2/pylintrc`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/setup.cfg` & `pydash-7.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 [bdist_wheel]
 python_tag = py3
 
 [flake8]
 exclude = .tox,venv,env
 max_line_length = 100
 max_complexity = 12
-ignore = F401,F811,E203,W503
+ignore = F811,E203,W503
 
 [mypy]
 show_column_numbers = True
 show_error_context = False
 ignore_missing_imports = True
 warn_return_any = False
 strict_optional = True
```

### Comparing `pydash-7.0.1/src/pydash/arrays.py` & `pydash-7.0.2/src/pydash/arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/chaining/all_funcs.py` & `pydash-7.0.2/src/pydash/chaining/all_funcs.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/chaining/all_funcs.pyi` & `pydash-7.0.2/src/pydash/chaining/all_funcs.pyi`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/chaining/chaining.py` & `pydash-7.0.2/src/pydash/chaining/chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/collections.py` & `pydash-7.0.2/src/pydash/collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/functions.py` & `pydash-7.0.2/src/pydash/functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/helpers.py` & `pydash-7.0.2/src/pydash/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/numerical.py` & `pydash-7.0.2/src/pydash/numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/objects.py` & `pydash-7.0.2/src/pydash/objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/predicates.py` & `pydash-7.0.2/src/pydash/predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/strings.py` & `pydash-7.0.2/src/pydash/strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash/types.py` & `pydash-7.0.2/src/pydash/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import typing as t
 
 from typing_extensions import Protocol
 
 
 if t.TYPE_CHECKING:
-    from decimal import Decimal
+    # F401: imported but unused
+    # py3.7 flake8 doesn't get it for type aliases
+    from decimal import Decimal  # noqa: F401
 
 IterateeObjT = t.Union[int, str, t.List, t.Tuple, t.Dict]
 NumberT = t.Union[float, int, "Decimal"]
 NumberNoDecimalT = t.Union[float, int]
 PathT = t.Union[t.Hashable, t.List[t.Hashable]]
```

### Comparing `pydash-7.0.1/src/pydash/utilities.py` & `pydash-7.0.2/src/pydash/utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/src/pydash.egg-info/PKG-INFO` & `pydash-7.0.2/src/pydash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash
-Version: 7.0.1
+Version: 7.0.2
 Summary: The kitchen sink of Python utility libraries for doing "stuff" in a functional way. Based on the Lo-Dash Javascript library.
 Home-page: https://github.com/dgilland/pydash
 Author: Derrick Gilland
 Author-email: dgilland@gmail.com
 License: MIT License
 Keywords: pydash utility functional lodash underscore
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,14 +61,20 @@
     :target: https://pypi.python.org/pypi/pydash/
 
 .. _changelog:
 
 Changelog
 =========
 
+v7.0.2 (2023-04-27)
+-------------------
+
+- Fix issue where using ``pyright`` as a type checker with ``reportPrivateUsage=true`` would report errors that objects are not exported from ``pydash``. Thanks DeviousStoat_!
+
+
 v7.0.1 (2023-04-13)
 -------------------
 
 - Fix missing install dependency, ``typing-extensions``, for package.
 
 
 v7.0.0 (2023-04-11)
```

### Comparing `pydash-7.0.1/src/pydash.egg-info/SOURCES.txt` & `pydash-7.0.2/src/pydash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tasks.py` & `pydash-7.0.2/tasks.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/build/testresults/junit.xml` & `pydash-7.0.2/tests/build/testresults/junit.xml`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/helpers.py` & `pydash-7.0.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/pytest_mypy_testing/test_arrays.py` & `pydash-7.0.2/tests/pytest_mypy_testing/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/pytest_mypy_testing/test_chaining.py` & `pydash-7.0.2/tests/pytest_mypy_testing/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/pytest_mypy_testing/test_collections.py` & `pydash-7.0.2/tests/pytest_mypy_testing/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/pytest_mypy_testing/test_functions.py` & `pydash-7.0.2/tests/pytest_mypy_testing/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/pytest_mypy_testing/test_numerical.py` & `pydash-7.0.2/tests/pytest_mypy_testing/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/pytest_mypy_testing/test_objects.py` & `pydash-7.0.2/tests/pytest_mypy_testing/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/pytest_mypy_testing/test_predicates.py` & `pydash-7.0.2/tests/pytest_mypy_testing/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/pytest_mypy_testing/test_strings.py` & `pydash-7.0.2/tests/pytest_mypy_testing/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/pytest_mypy_testing/test_utilities.py` & `pydash-7.0.2/tests/pytest_mypy_testing/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/test_arrays.py` & `pydash-7.0.2/tests/test_arrays.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/test_chaining.py` & `pydash-7.0.2/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/test_collections.py` & `pydash-7.0.2/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/test_functions.py` & `pydash-7.0.2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/test_numerical.py` & `pydash-7.0.2/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/test_objects.py` & `pydash-7.0.2/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/test_predicates.py` & `pydash-7.0.2/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/test_strings.py` & `pydash-7.0.2/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `pydash-7.0.1/tests/test_utilities.py` & `pydash-7.0.2/tests/test_utilities.py`

 * *Files identical despite different names*

