# Comparing `tmp/feed-archiver-2.0.2b0.tar.gz` & `tmp/feed-archiver-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed-archiver-2.0.2b0.tar", last modified: Wed Apr 26 01:35:35 2023, max compression
+gzip compressed data, was "feed-archiver-2.0.3.tar", last modified: Wed Apr 26 22:46:36 2023, max compression
```

## Comparing `feed-archiver-2.0.2b0.tar` & `feed-archiver-2.0.3.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/.dir-locals.el.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/.dockerignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1150 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/.env.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.178572 feed-archiver-2.0.2b0/.github/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/.github/workflows/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/.github/workflows/build-test.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4347 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/.gitlab-ci.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      777 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/.pre-commit-config.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/.prospector.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/CONTRIBUTING.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2481 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3218 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/Dockerfile.devel
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/LICENSE
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    60325 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      180 2023-04-26 00:57:06.000000 feed-archiver-2.0.2b0/NEWS-VERSION.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4031 2023-04-26 00:57:11.000000 feed-archiver-2.0.2b0/NEWS.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25653 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/PKG-INFO
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    24565 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/README.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/TODO.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2759 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/bin/cz-check-bump
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/bin/entrypoint
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/bin/get-base-version
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/bin/hadolint
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/build-host/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/README.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/build-host/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/bin/entrypoint
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      730 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py310.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      673 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py311.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      947 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py37.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py38.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/build-host/requirements-py39.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/build-host/requirements.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/dist/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/dist/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/docker-compose-servarr.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5769 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/docker-compose.override.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      945 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/gitlab-runner/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/gitlab-runner/config/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      566 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/home/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/home/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/home/.pypirc.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/link-fallbacks.feature.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.178572 feed-archiver-2.0.2b0/nginx/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/nginx/templates/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/nginx/templates/default.conf.template
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2940 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/pyproject.toml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      668 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/requirements/build.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/py310/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2567 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py310/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6246 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py310/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py310/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/py311/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2529 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py311/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6020 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py311/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py311/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/py37/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2840 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py37/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6936 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py37/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py37/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.186572 feed-archiver-2.0.2b0/requirements/py38/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2668 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py38/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6286 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py38/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py38/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/requirements/py39/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2565 2023-04-26 00:51:45.000000 feed-archiver-2.0.2b0/requirements/py39/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6273 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py39/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 00:57:13.000000 feed-archiver-2.0.2b0/requirements/py39/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/server/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/server/docker-compose.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2152 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/setup.cfg
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.178572 feed-archiver-2.0.2b0/src/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25653 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7317 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/entry_points.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/requires.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feed_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/__main__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/archive.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/enclosures/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/enclosures/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/enclosures/servarr.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/enclosures/template.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/formats.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/newsfragments/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/newsfragments/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/__init__.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/downloads/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty-feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty-items/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/end-to-end/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink-wo-suffix/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/simple/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.190572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.182572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 01:35:35.194572 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_cli.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_download.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_linking.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/tests/test_urls.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/src/feedarchiver/utils.py
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      162 2023-04-26 01:35:35.000000 feed-archiver-2.0.2b0/src/feedarchiver/version.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3368 2023-04-24 06:43:00.000000 feed-archiver-2.0.2b0/tox.ini
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/.dir-locals.el.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/.dockerignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1150 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/.env.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.070369 feed-archiver-2.0.3/.github/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/.github/workflows/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/.github/workflows/build-test.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/.gitignore
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     4357 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/.gitlab-ci.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      777 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/.pre-commit-config.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/.prospector.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/CONTRIBUTING.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2481 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3218 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/Dockerfile.devel
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/LICENSE
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    60319 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/Makefile
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      176 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/NEWS-VERSION.rst
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     4301 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/NEWS.rst
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26172 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/PKG-INFO
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25086 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/README.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/TODO.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2759 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/bin/cz-check-bump
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/bin/entrypoint
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/bin/get-base-version
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/bin/hadolint
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/build-host/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/README.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/build-host/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/bin/entrypoint
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      730 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py310.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      673 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py311.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      947 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py37.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py38.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py39.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/requirements.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/dist/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/dist/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/docker-compose-servarr.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5769 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/docker-compose.override.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      945 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/gitlab-runner/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/gitlab-runner/config/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      566 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/home/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/home/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/home/.pypirc.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/link-fallbacks.feature.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/nginx/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/nginx/templates/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/nginx/templates/default.conf.template
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2938 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/pyproject.toml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      668 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/requirements/build.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py310/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2567 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py310/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6246 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py310/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py310/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py311/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2529 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py311/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6020 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py311/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py311/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py37/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2840 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py37/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6936 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py37/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py37/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py38/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2668 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py38/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6286 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py38/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py38/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py39/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2565 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py39/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6273 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py39/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py39/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/server/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/server/docker-compose.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2152 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/setup.cfg
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feed_archiver.egg-info/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26172 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7317 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/requires.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/__main__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/archive.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/enclosures/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/enclosures/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/enclosures/servarr.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/enclosures/template.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/formats.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/newsfragments/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/newsfragments/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/__init__.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/downloads/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty-feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty-items/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/end-to-end/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink-wo-suffix/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/simple/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_archive.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_cli.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_download.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_linking.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_urls.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/utils.py
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      160 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feedarchiver/version.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3368 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/tox.ini
```

### Comparing `feed-archiver-2.0.2b0/.dir-locals.el.in` & `feed-archiver-2.0.3/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/.dockerignore` & `feed-archiver-2.0.3/.dockerignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/.env.in` & `feed-archiver-2.0.3/.env.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/.github/workflows/build-test.yml` & `feed-archiver-2.0.3/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/.gitignore` & `feed-archiver-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/.gitlab-ci.yml` & `feed-archiver-2.0.3/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             && $CI_COMMIT_TITLE !~
         /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9].*$/
           )
         )
         && $CI_PIPELINE_SOURCE != "schedule"
   script:
     - >-
-      entrypoint make -e release-bump
+      entrypoint make -e test-push release-bump
 
 # Workaround GitLab's handling of pipeline status when pushing both a branch and a tag:
 release-version:
   stage: "release-version"
   needs: []
   dependencies: []
   rules:
```

### Comparing `feed-archiver-2.0.2b0/.pre-commit-config.yaml` & `feed-archiver-2.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/.prospector.yaml` & `feed-archiver-2.0.3/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/CONTRIBUTING.rst` & `feed-archiver-2.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/Dockerfile` & `feed-archiver-2.0.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/Dockerfile.devel` & `feed-archiver-2.0.3/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/LICENSE` & `feed-archiver-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/Makefile` & `feed-archiver-2.0.3/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -666,31 +666,30 @@
 
 .PHONY: test-push
 ### Perform any checks that should only be run before pushing.
 test-push: $(VCS_FETCH_TARGETS) \
 		$(HOME)/.local/var/log/feed-archiver-host-install.log \
 		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
 		build-docker-volumes-$(PYTHON_ENV) ./.env
+	vcs_compare_rev="$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH)"
 ifeq ($(CI),true)
 ifneq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
 # Don't waste CI time, only check for the canonical version:
 	exit
 endif
-endif
 ifeq ($(VCS_COMPARE_BRANCH),main)
 # On `main`, compare with the previous commit on `main`
 	vcs_compare_rev="$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH)^"
-else
-	vcs_compare_rev="$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH)"
+endif
+endif
 	if ! git fetch "$(VCS_COMPARE_REMOTE)" "$(VCS_COMPARE_BRANCH)"
 	then
 # Compare with the pre-release branch if this branch hasn't been pushed yet:
 	    vcs_compare_rev="$(VCS_COMPARE_REMOTE)/develop"
 	fi
-endif
 	exit_code=0
 	(
 	    $(TOX_EXEC_BUILD_ARGS) -- \
 	        cz check --rev-range "$${vcs_compare_rev}..HEAD" &&
 	    $(TOX_EXEC_BUILD_ARGS) -- \
 	        python ./bin/cz-check-bump --compare-ref "$${vcs_compare_rev}"
 	) || exit_code=$$?
@@ -824,35 +823,36 @@
 	then
 	    set +x
 	    echo "CRITICAL: Cannot bump version with staged changes"
 	    false
 	fi
 # Ensure the local branch is updated to the forthcoming version bump commit:
 	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)" --
-ifeq ($(VCS_BRANCH),main)
-	if ! ./.tox/build/bin/python ./bin/get-base-version $$(
-	    ./.tox/build/bin/cz version --project
-	)
-	then
-# There's no pre-release for which to publish a final release:
-	    exit
-	fi
-else
-# Only release if required by conventional commits:
+# Check if a release is required:
 	exit_code=0
-	./.tox/build/bin/python ./bin/cz-check-bump || exit_code=$$?
-	if (( $$exit_code == 3 || $$exit_code == 21 ))
-	then
+	if [ "$(VCS_BRANCH)" = "main" ] &&
+	    ./.tox/build/bin/python ./bin/get-base-version $$(
+	        ./.tox/build/bin/cz version --project
+	    )
+	then
+# Release a previous pre-release as final regardless of whether commits since then
+# require a release:
+	    true
+	else
+# Is a release required by conventional commits:
+	    ./.tox/build/bin/python ./bin/cz-check-bump || exit_code=$$?
+	    if (( $$exit_code == 3 || $$exit_code == 21 ))
+	    then
 # No commits require a release:
-	    exit
-	elif (( $$exit_code != 0 ))
-	then
-	    exit $$exit_code
+	        exit
+	    elif (( $$exit_code != 0 ))
+	    then
+	        exit $$exit_code
+	    fi
 	fi
-endif
 # Collect the versions involved in this release according to conventional commits:
 	cz_bump_args="--check-consistency --no-verify"
 ifneq ($(VCS_BRANCH),main)
 	cz_bump_args+=" --prerelease beta"
 endif
 ifeq ($(RELEASE_PUBLISH),true)
 	cz_bump_args+=" --gpg-sign"
@@ -878,16 +878,14 @@
 	$(TOX_EXEC_BUILD_ARGS) -- cz bump $${cz_bump_args}
 # Ensure the container image reflects the version bump but we don't need to update the
 # requirements again.
 	touch \
 	    $(PYTHON_ENVS:%=./requirements/%/user.txt) \
 	    $(PYTHON_ENVS:%=./requirements/%/devel.txt) \
 	    $(PYTHON_ENVS:%=./build-host/requirements-%.txt)
-# Ensure the image is up-to-date for subsequent recipes.
-	$(MAKE) -e "./var/docker/$(PYTHON_ENV)/log/build-user.log"
 ifeq ($(VCS_BRANCH),main)
 # Merge the bumped version back into `develop`:
 	bump_rev="$$(git rev-parse HEAD)"
 	git switch -C "develop" --track "$(VCS_COMPARE_REMOTE)/develop" --
 	git merge --ff --gpg-sign \
 	    -m "Merge branch 'main' release back into develop" "$${bump_rev}"
 ifeq ($(CI),true)
```

### Comparing `feed-archiver-2.0.2b0/NEWS.rst` & `feed-archiver-2.0.3/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+feed-archiver 2.0.3 (2023-04-26)
+================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Wed Apr 26 05:24:13 PM UTC 2023.
+
+
+feed-archiver 2.0.2 (2023-04-26)
+================================
+
+No significant changes.
+
+
 feed-archiver 2.0.2b0 (2023-04-26)
 ==================================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Tue Apr 25 11:00:28 PM UTC 2023.
```

### Comparing `feed-archiver-2.0.2b0/PKG-INFO` & `feed-archiver-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.2b0
+Version: 2.0.3
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
@@ -63,15 +63,15 @@
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/feed-archiver/releases
        .. figure:: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
           :target: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml
-       .. figure:: https://app.codecov.io/github/rpatterson/feed-archiver/branch/main/graph/badge.svg?token=GNKVQ8VYOU
+       .. figure:: https://codecov.io/github/rpatterson/feed-archiver/branch/main/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
 	  :target: https://app.codecov.io/github/rpatterson/feed-archiver
        .. figure:: https://img.shields.io/github/stars/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/feed-archiver/
 
      - .. figure:: https://img.shields.io/docker/v/merpatterson/feed-archiver/main?sort=semver&logo=docker
@@ -118,20 +118,20 @@
 
     An alternate hierarchy of feed item enclosures better suited for ingestion into
     other media software, such as media library servers.  For example, your podcast
     episodes can also be made available in your `Jellyfin`_/Emby/Plex library.
 
 .. contents:: Table of Contents
 
-********************
+****************************************************************************************
 Detailed Description
-********************
+****************************************************************************************
 
 Mirror of Feed Enclosures and Assets
-====================================
+========================================================================================
 
 To serve use case #1, ``feed-archiver`` downloads enclosures and external assets
 (e.g. feed and item logos specified as URLs in the feed XMLs) to the archive's local
 filesystem, adjusts the URLs of the downloaded items in the feed XML, and saves the feed
 XML into the archive as well.  This makes the local archive filesystem suitable for
 serving to feed clients/subscribers using a simple static site server such as `nginx`_.
 
@@ -161,15 +161,15 @@
 As feeds change over time, ``feed-archiver`` preserves the earliest form of feed content
 as much as possible.  If a feed item is changed in a subsequent retrieval of the feed,
 the remote item XML is preserved instead of updating to the newer XML.  More
 specifically, items will be ignored on subsequent retrievals of the same feed if they
 have the same ``guid``/``id`` as items that have previously been archived for that feed.
 
 Ingest Feed Enclosures Into Media Libraries
-===========================================
+========================================================================================
 
 To serve use case #2, ``feed-archiver`` links the downloaded feed item enclosures into
 an alternate hierarchy based on feed item metadata that better reflects the
 show-with-episodes nature of most feeds, such as podcasts, with media enclosures.  What
 feed item metadata is used and how it's used to assemble the media library path
 enclosures are linked into is configurable on a per-feed basis.  This can be used, for
 example, simply to make your podcasts accessible from your media library software.  In a
@@ -311,17 +311,17 @@
 update`` sub-command, the enclosures of new items are linked as configured.  If the
 ``enclosures`` configuration changes or any of the used plugins refer to external
 resources that may change, such as the with the ``sonarr`` plugin when `Sonarr`_ has
 upgraded or renamed the corresponding video files, use the  ``$ feed-archiver relink``
 command to update all existing links.
 
 
-*******
+****************************************************************************************
 Plugins
-*******
+****************************************************************************************
 
 How feed item enclosures are linked into a media library is delegated to plugins or
 add-ons.  Specifically, the ``plugin`` key in a ``enclosures`` configuration must be a
 string which is the name of `a Python entry point`_ registered in the
 ``feedarchiver.enclosures`` group.  The entry point object reference must point to a
 ``feedarchiver.enclosures.EnclosurePlugin`` subclass which accepts the following arguments
 when instantiated:
@@ -431,27 +431,27 @@
 	  match-pattern: "\
 	  (?P<item_title>.+) \\((?P<series_title>.+) \
 	  (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
 	  stem-append: "-garply"
   ...
 
 Default Template Plugin
-=======================
+========================================================================================
 
 If no ``plugin`` key is specified, the ``template`` plugin is used.  The link
 path config may include the ``template`` key containing a `Python format string`_ which
 will be expanded to determine where the feed item enclosure should be linked to.  The
 default ``template`` is::
 
   ./Feeds/{utils.quote_sep(feed_parsed.feed.title).strip()}/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}
 
 The format strings may reference any of `the arguments passed into enclosure plugins`_.
 
 Sonarr TV Series Plugin
-=======================
+========================================================================================
 
 The ``sonarr`` plugin uses values from the enclosure configuration and/or the ``match``
 groups to lookup a TV series/show managed by `Sonarr`_, then lookup an episode video
 file that corresponds to the feed item enclosure, and link the enclosure next to that
 video file.  The ``enclosures`` configuration or ``match`` groups must contain:
 
 - ``url`` and ``api-key`` used to `connect to the Sonarr API`_
```

### Comparing `feed-archiver-2.0.2b0/README.rst` & `feed-archiver-2.0.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/feed-archiver/releases
        .. figure:: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
           :target: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml
-       .. figure:: https://app.codecov.io/github/rpatterson/feed-archiver/branch/main/graph/badge.svg?token=GNKVQ8VYOU
+       .. figure:: https://codecov.io/github/rpatterson/feed-archiver/branch/main/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
 	  :target: https://app.codecov.io/github/rpatterson/feed-archiver
        .. figure:: https://img.shields.io/github/stars/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/feed-archiver/
 
      - .. figure:: https://img.shields.io/docker/v/merpatterson/feed-archiver/main?sort=semver&logo=docker
@@ -90,20 +90,20 @@
 
     An alternate hierarchy of feed item enclosures better suited for ingestion into
     other media software, such as media library servers.  For example, your podcast
     episodes can also be made available in your `Jellyfin`_/Emby/Plex library.
 
 .. contents:: Table of Contents
 
-********************
+****************************************************************************************
 Detailed Description
-********************
+****************************************************************************************
 
 Mirror of Feed Enclosures and Assets
-====================================
+========================================================================================
 
 To serve use case #1, ``feed-archiver`` downloads enclosures and external assets
 (e.g. feed and item logos specified as URLs in the feed XMLs) to the archive's local
 filesystem, adjusts the URLs of the downloaded items in the feed XML, and saves the feed
 XML into the archive as well.  This makes the local archive filesystem suitable for
 serving to feed clients/subscribers using a simple static site server such as `nginx`_.
 
@@ -133,15 +133,15 @@
 As feeds change over time, ``feed-archiver`` preserves the earliest form of feed content
 as much as possible.  If a feed item is changed in a subsequent retrieval of the feed,
 the remote item XML is preserved instead of updating to the newer XML.  More
 specifically, items will be ignored on subsequent retrievals of the same feed if they
 have the same ``guid``/``id`` as items that have previously been archived for that feed.
 
 Ingest Feed Enclosures Into Media Libraries
-===========================================
+========================================================================================
 
 To serve use case #2, ``feed-archiver`` links the downloaded feed item enclosures into
 an alternate hierarchy based on feed item metadata that better reflects the
 show-with-episodes nature of most feeds, such as podcasts, with media enclosures.  What
 feed item metadata is used and how it's used to assemble the media library path
 enclosures are linked into is configurable on a per-feed basis.  This can be used, for
 example, simply to make your podcasts accessible from your media library software.  In a
@@ -283,17 +283,17 @@
 update`` sub-command, the enclosures of new items are linked as configured.  If the
 ``enclosures`` configuration changes or any of the used plugins refer to external
 resources that may change, such as the with the ``sonarr`` plugin when `Sonarr`_ has
 upgraded or renamed the corresponding video files, use the  ``$ feed-archiver relink``
 command to update all existing links.
 
 
-*******
+****************************************************************************************
 Plugins
-*******
+****************************************************************************************
 
 How feed item enclosures are linked into a media library is delegated to plugins or
 add-ons.  Specifically, the ``plugin`` key in a ``enclosures`` configuration must be a
 string which is the name of `a Python entry point`_ registered in the
 ``feedarchiver.enclosures`` group.  The entry point object reference must point to a
 ``feedarchiver.enclosures.EnclosurePlugin`` subclass which accepts the following arguments
 when instantiated:
@@ -403,27 +403,27 @@
 	  match-pattern: "\
 	  (?P<item_title>.+) \\((?P<series_title>.+) \
 	  (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
 	  stem-append: "-garply"
   ...
 
 Default Template Plugin
-=======================
+========================================================================================
 
 If no ``plugin`` key is specified, the ``template`` plugin is used.  The link
 path config may include the ``template`` key containing a `Python format string`_ which
 will be expanded to determine where the feed item enclosure should be linked to.  The
 default ``template`` is::
 
   ./Feeds/{utils.quote_sep(feed_parsed.feed.title).strip()}/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}
 
 The format strings may reference any of `the arguments passed into enclosure plugins`_.
 
 Sonarr TV Series Plugin
-=======================
+========================================================================================
 
 The ``sonarr`` plugin uses values from the enclosure configuration and/or the ``match``
 groups to lookup a TV series/show managed by `Sonarr`_, then lookup an episode video
 file that corresponds to the feed item enclosure, and link the enclosure next to that
 video file.  The ``enclosures`` configuration or ``match`` groups must contain:
 
 - ``url`` and ``api-key`` used to `connect to the Sonarr API`_
```

### Comparing `feed-archiver-2.0.2b0/TODO.rst` & `feed-archiver-2.0.3/TODO.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/bin/cz-check-bump` & `feed-archiver-2.0.3/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/bin/entrypoint` & `feed-archiver-2.0.3/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/bin/get-base-version` & `feed-archiver-2.0.3/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/build-host/Dockerfile` & `feed-archiver-2.0.3/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/build-host/Makefile` & `feed-archiver-2.0.3/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/build-host/README.rst` & `feed-archiver-2.0.3/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/build-host/bin/entrypoint` & `feed-archiver-2.0.3/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/build-host/requirements-py310.txt` & `feed-archiver-2.0.3/build-host/requirements-py39.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py310.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py39.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
@@ -16,23 +16,23 @@
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.5.0
+tox==4.5.1
     # via -r build-host/requirements.txt.in
 virtualenv==20.22.0
     # via tox
```

### Comparing `feed-archiver-2.0.2b0/build-host/requirements-py311.txt` & `feed-archiver-2.0.3/build-host/requirements-py311.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
-tox==4.5.0
+tox==4.5.1
     # via -r build-host/requirements.txt.in
 virtualenv==20.22.0
     # via tox
```

### Comparing `feed-archiver-2.0.2b0/build-host/requirements-py37.txt` & `feed-archiver-2.0.3/build-host/requirements-py37.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,27 +21,27 @@
     #   pluggy
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.5.0
+tox==4.5.1
     # via -r build-host/requirements.txt.in
 typing-extensions==4.5.0
     # via
     #   importlib-metadata
     #   platformdirs
     #   tox
 virtualenv==20.22.0
```

### Comparing `feed-archiver-2.0.2b0/build-host/requirements-py38.txt` & `feed-archiver-2.0.3/build-host/requirements-py38.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.5.0
+tox==4.5.1
     # via -r build-host/requirements.txt.in
 virtualenv==20.22.0
     # via tox
```

### Comparing `feed-archiver-2.0.2b0/docker-compose-servarr.yml` & `feed-archiver-2.0.3/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/docker-compose.override.yml` & `feed-archiver-2.0.3/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/docker-compose.yml` & `feed-archiver-2.0.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/gitlab-runner/config/config.toml.in` & `feed-archiver-2.0.3/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/gitlab-runner/docker-compose.yml` & `feed-archiver-2.0.3/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/nginx/templates/default.conf.template` & `feed-archiver-2.0.3/nginx/templates/default.conf.template`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/pyproject.toml` & `feed-archiver-2.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "2.0.2b0"
+version = "2.0.3"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `feed-archiver-2.0.2b0/requirements/build.txt.in` & `feed-archiver-2.0.3/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/requirements/py310/build.txt` & `feed-archiver-2.0.3/requirements/py310/build.txt`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -83,15 +83,15 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.28.2
+requests==2.29.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
```

### Comparing `feed-archiver-2.0.2b0/requirements/py310/devel.txt` & `feed-archiver-2.0.3/requirements/py310/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
@@ -213,15 +213,15 @@
     #   bandit
     #   feed-archiver (pyproject.toml)
     #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.28.2
+requests==2.29.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
```

### Comparing `feed-archiver-2.0.2b0/requirements/py310/user.txt` & `feed-archiver-2.0.3/requirements/py310/user.txt`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     #   anyio
     #   httpx
     #   requests
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.28.2
+requests==2.29.0
     # via arrapi
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
```

### Comparing `feed-archiver-2.0.2b0/requirements/py311/build.txt` & `feed-archiver-2.0.3/requirements/py38/build.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py311/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==2.1.2
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
@@ -37,14 +37,16 @@
 idna==3.4
     # via requests
 importlib-metadata==4.13.0
     # via
     #   commitizen
     #   keyring
     #   twine
+importlib-resources==5.12.0
+    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -63,15 +65,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -83,15 +85,15 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.28.2
+requests==2.29.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
@@ -101,28 +103,34 @@
     # via keyring
 setuptools-scm==7.1.0
     # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
+tomli==2.0.1
+    # via setuptools-scm
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via setuptools-scm
+    # via
+    #   rich
+    #   setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
 virtualenv==20.22.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `feed-archiver-2.0.2b0/requirements/py311/devel.txt` & `feed-archiver-2.0.3/requirements/py311/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
@@ -211,15 +211,15 @@
     #   bandit
     #   feed-archiver (pyproject.toml)
     #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.28.2
+requests==2.29.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
```

### Comparing `feed-archiver-2.0.2b0/requirements/py311/user.txt` & `feed-archiver-2.0.3/requirements/py311/user.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     #   anyio
     #   httpx
     #   requests
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.28.2
+requests==2.29.0
     # via arrapi
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
```

### Comparing `feed-archiver-2.0.2b0/requirements/py37/build.txt` & `feed-archiver-2.0.3/requirements/py37/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via virtualenv
 pre-commit==2.21.0
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -89,15 +89,15 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.28.2
+requests==2.29.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
```

### Comparing `feed-archiver-2.0.2b0/requirements/py37/devel.txt` & `feed-archiver-2.0.3/requirements/py37/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==2.21.0
@@ -230,15 +230,15 @@
     #   bandit
     #   feed-archiver (pyproject.toml)
     #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.28.2
+requests==2.29.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
```

### Comparing `feed-archiver-2.0.2b0/requirements/py37/user.txt` & `feed-archiver-2.0.3/requirements/py37/user.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     # via
     #   argcomplete
     #   feed-archiver (pyproject.toml)
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.28.2
+requests==2.29.0
     # via arrapi
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
```

### Comparing `feed-archiver-2.0.2b0/requirements/py38/build.txt` & `feed-archiver-2.0.3/requirements/py311/build.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py311/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==2.1.2
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
@@ -37,16 +37,14 @@
 idna==3.4
     # via requests
 importlib-metadata==4.13.0
     # via
     #   commitizen
     #   keyring
     #   twine
-importlib-resources==5.12.0
-    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -65,15 +63,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -85,15 +83,15 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.28.2
+requests==2.29.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
@@ -103,34 +101,28 @@
     # via keyring
 setuptools-scm==7.1.0
     # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomli==2.0.1
-    # via setuptools-scm
 tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via
-    #   rich
-    #   setuptools-scm
+    # via setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
 virtualenv==20.22.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `feed-archiver-2.0.2b0/requirements/py38/devel.txt` & `feed-archiver-2.0.3/requirements/py38/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
@@ -213,15 +213,15 @@
     #   bandit
     #   feed-archiver (pyproject.toml)
     #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.28.2
+requests==2.29.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
```

### Comparing `feed-archiver-2.0.2b0/requirements/py38/user.txt` & `feed-archiver-2.0.3/requirements/py38/user.txt`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     #   anyio
     #   httpx
     #   requests
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.28.2
+requests==2.29.0
     # via arrapi
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
```

### Comparing `feed-archiver-2.0.2b0/requirements/py39/build.txt` & `feed-archiver-2.0.3/requirements/py39/build.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -83,15 +83,15 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.28.2
+requests==2.29.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
```

### Comparing `feed-archiver-2.0.2b0/requirements/py39/devel.txt` & `feed-archiver-2.0.3/requirements/py39/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.3.0
+platformdirs==3.4.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
@@ -213,15 +213,15 @@
     #   bandit
     #   feed-archiver (pyproject.toml)
     #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.28.2
+requests==2.29.0
     # via
     #   arrapi
     #   pyroma
     #   requests-mock
     #   xenon
 requests-mock==1.10.0
     # via feed-archiver (pyproject.toml)
```

### Comparing `feed-archiver-2.0.2b0/requirements/py39/user.txt` & `feed-archiver-2.0.3/requirements/py39/user.txt`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     #   anyio
     #   httpx
     #   requests
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.28.2
+requests==2.29.0
     # via arrapi
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
```

### Comparing `feed-archiver-2.0.2b0/server/docker-compose.yml` & `feed-archiver-2.0.3/server/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/setup.cfg` & `feed-archiver-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feed_archiver.egg-info/PKG-INFO` & `feed-archiver-2.0.3/src/feed_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.2b0
+Version: 2.0.3
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
@@ -63,15 +63,15 @@
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/feed-archiver/releases
        .. figure:: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
           :target: https://github.com/rpatterson/feed-archiver/actions/workflows/build-test.yml
-       .. figure:: https://app.codecov.io/github/rpatterson/feed-archiver/branch/main/graph/badge.svg?token=GNKVQ8VYOU
+       .. figure:: https://codecov.io/github/rpatterson/feed-archiver/branch/main/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
 	  :target: https://app.codecov.io/github/rpatterson/feed-archiver
        .. figure:: https://img.shields.io/github/stars/rpatterson/feed-archiver?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/feed-archiver/
 
      - .. figure:: https://img.shields.io/docker/v/merpatterson/feed-archiver/main?sort=semver&logo=docker
@@ -118,20 +118,20 @@
 
     An alternate hierarchy of feed item enclosures better suited for ingestion into
     other media software, such as media library servers.  For example, your podcast
     episodes can also be made available in your `Jellyfin`_/Emby/Plex library.
 
 .. contents:: Table of Contents
 
-********************
+****************************************************************************************
 Detailed Description
-********************
+****************************************************************************************
 
 Mirror of Feed Enclosures and Assets
-====================================
+========================================================================================
 
 To serve use case #1, ``feed-archiver`` downloads enclosures and external assets
 (e.g. feed and item logos specified as URLs in the feed XMLs) to the archive's local
 filesystem, adjusts the URLs of the downloaded items in the feed XML, and saves the feed
 XML into the archive as well.  This makes the local archive filesystem suitable for
 serving to feed clients/subscribers using a simple static site server such as `nginx`_.
 
@@ -161,15 +161,15 @@
 As feeds change over time, ``feed-archiver`` preserves the earliest form of feed content
 as much as possible.  If a feed item is changed in a subsequent retrieval of the feed,
 the remote item XML is preserved instead of updating to the newer XML.  More
 specifically, items will be ignored on subsequent retrievals of the same feed if they
 have the same ``guid``/``id`` as items that have previously been archived for that feed.
 
 Ingest Feed Enclosures Into Media Libraries
-===========================================
+========================================================================================
 
 To serve use case #2, ``feed-archiver`` links the downloaded feed item enclosures into
 an alternate hierarchy based on feed item metadata that better reflects the
 show-with-episodes nature of most feeds, such as podcasts, with media enclosures.  What
 feed item metadata is used and how it's used to assemble the media library path
 enclosures are linked into is configurable on a per-feed basis.  This can be used, for
 example, simply to make your podcasts accessible from your media library software.  In a
@@ -311,17 +311,17 @@
 update`` sub-command, the enclosures of new items are linked as configured.  If the
 ``enclosures`` configuration changes or any of the used plugins refer to external
 resources that may change, such as the with the ``sonarr`` plugin when `Sonarr`_ has
 upgraded or renamed the corresponding video files, use the  ``$ feed-archiver relink``
 command to update all existing links.
 
 
-*******
+****************************************************************************************
 Plugins
-*******
+****************************************************************************************
 
 How feed item enclosures are linked into a media library is delegated to plugins or
 add-ons.  Specifically, the ``plugin`` key in a ``enclosures`` configuration must be a
 string which is the name of `a Python entry point`_ registered in the
 ``feedarchiver.enclosures`` group.  The entry point object reference must point to a
 ``feedarchiver.enclosures.EnclosurePlugin`` subclass which accepts the following arguments
 when instantiated:
@@ -431,27 +431,27 @@
 	  match-pattern: "\
 	  (?P<item_title>.+) \\((?P<series_title>.+) \
 	  (?P<season_number>[0-9])(?P<episode_numbers>[0-9]+[0-9Ee& -]*)\\)"
 	  stem-append: "-garply"
   ...
 
 Default Template Plugin
-=======================
+========================================================================================
 
 If no ``plugin`` key is specified, the ``template`` plugin is used.  The link
 path config may include the ``template`` key containing a `Python format string`_ which
 will be expanded to determine where the feed item enclosure should be linked to.  The
 default ``template`` is::
 
   ./Feeds/{utils.quote_sep(feed_parsed.feed.title).strip()}/{utils.quote_sep(item_parsed.title).strip()}{enclosure_path.suffix}
 
 The format strings may reference any of `the arguments passed into enclosure plugins`_.
 
 Sonarr TV Series Plugin
-=======================
+========================================================================================
 
 The ``sonarr`` plugin uses values from the enclosure configuration and/or the ``match``
 groups to lookup a TV series/show managed by `Sonarr`_, then lookup an episode video
 file that corresponds to the feed item enclosure, and link the enclosure next to that
 video file.  The ``enclosures`` configuration or ``match`` groups must contain:
 
 - ``url`` and ``api-key`` used to `connect to the Sonarr API`_
```

### Comparing `feed-archiver-2.0.2b0/src/feed_archiver.egg-info/SOURCES.txt` & `feed-archiver-2.0.3/src/feed_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/__init__.py` & `feed-archiver-2.0.3/src/feedarchiver/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/archive.py` & `feed-archiver-2.0.3/src/feedarchiver/archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/enclosures/__init__.py` & `feed-archiver-2.0.3/src/feedarchiver/enclosures/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/enclosures/servarr.py` & `feed-archiver-2.0.3/src/feedarchiver/enclosures/servarr.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/enclosures/template.py` & `feed-archiver-2.0.3/src/feedarchiver/enclosures/template.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/feed.py` & `feed-archiver-2.0.3/src/feedarchiver/feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/formats.py` & `feed-archiver-2.0.3/src/feedarchiver/formats.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/__init__.py` & `feed-archiver-2.0.3/src/feedarchiver/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml` & `feed-archiver-2.0.3/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in` & `feed-archiver-2.0.3/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink/.feed-archiver.yml` & `feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml` & `feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_archive.py` & `feed-archiver-2.0.3/src/feedarchiver/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_cli.py` & `feed-archiver-2.0.3/src/feedarchiver/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_download.py` & `feed-archiver-2.0.3/src/feedarchiver/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_feed.py` & `feed-archiver-2.0.3/src/feedarchiver/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_linking.py` & `feed-archiver-2.0.3/src/feedarchiver/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/tests/test_urls.py` & `feed-archiver-2.0.3/src/feedarchiver/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/src/feedarchiver/utils.py` & `feed-archiver-2.0.3/src/feedarchiver/utils.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.2b0/tox.ini` & `feed-archiver-2.0.3/tox.ini`

 * *Files identical despite different names*

