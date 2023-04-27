# Comparing `tmp/augmenty-1.3.2.tar.gz` & `tmp/augmenty-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmenty-1.3.2.tar", last modified: Mon Mar  6 12:38:02 2023, max compression
+gzip compressed data, was "augmenty-1.3.3.tar", last modified: Thu Apr 27 19:19:23 2023, max compression
```

## Comparing `augmenty-1.3.2.tar` & `augmenty-1.3.3.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.611278 augmenty-1.3.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.591278 augmenty-1.3.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.591278 augmenty-1.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      729 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      283 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/ISSUE_TEMPLATE/04_augmenter-request.md
--rw-r--r--   0 root         (0) root         (0)      625 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.591278 augmenty-1.3.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1013 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1280 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2697 2023-03-06 12:37:51.000000 augmenty-1.3.2/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      186 2023-03-06 12:37:51.000000 augmenty-1.3.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)      797 2023-03-06 12:37:51.000000 augmenty-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1662 2023-03-06 12:37:52.000000 augmenty-1.3.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1075 2023-03-06 12:37:51.000000 augmenty-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7212 2023-03-06 12:38:02.611278 augmenty-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      372 2023-03-06 12:37:51.000000 augmenty-1.3.2/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.595278 augmenty-1.3.2/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.595278 augmenty-1.3.2/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   385037 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   395381 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)     2308 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/adding_an_augmenter.rst
--rw-r--r--   0 root         (0) root         (0)     6366 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/augmenters_overview.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/augmenty.augment_utilities.rst
--rw-r--r--   0 root         (0) root         (0)     1009 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/augmenty.character.rst
--rw-r--r--   0 root         (0) root         (0)      733 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/augmenty.doc.rst
--rw-r--r--   0 root         (0) root         (0)      409 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/augmenty.keyboard.rst
--rw-r--r--   0 root         (0) root         (0)      500 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/augmenty.lang.rst
--rw-r--r--   0 root         (0) root         (0)      334 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/augmenty.span.rst
--rw-r--r--   0 root         (0) root         (0)     1089 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/augmenty.token.rst
--rw-r--r--   0 root         (0) root         (0)      330 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/augmenty.util.rst
--rw-r--r--   0 root         (0) root         (0)     4190 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/create_augmenters_table.py
--rw-r--r--   0 root         (0) root         (0)     3444 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2578 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1055 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     1149 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)       61 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.595278 augmenty-1.3.2/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    15539 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/tutorials/introduction.ipynb
--rw-r--r--   0 root         (0) root         (0)      210 2023-03-06 12:37:51.000000 augmenty-1.3.2/docs/tutorials/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.595278 augmenty-1.3.2/img/
--rw-r--r--   0 root         (0) root         (0)   385037 2023-03-06 12:37:51.000000 augmenty-1.3.2/img/icon.png
--rw-r--r--   0 root         (0) root         (0)     3152 2023-03-06 12:37:52.000000 augmenty-1.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     4521 2023-03-06 12:37:51.000000 augmenty-1.3.2/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-06 12:38:02.611278 augmenty-1.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.587278 augmenty-1.3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.599278 augmenty-1.3.2/src/augmenty/
--rw-r--r--   0 root         (0) root         (0)     2053 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/__init__.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/about.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/augment_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.599278 augmenty-1.3.2/src/augmenty/character/
--rw-r--r--   0 root         (0) root         (0)      355 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/character/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/character/casing.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/character/replace.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/character/spacing.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/character/swap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.599278 augmenty-1.3.2/src/augmenty/doc/
--rw-r--r--   0 root         (0) root         (0)      184 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/doc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/doc/casing.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/doc/subset.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.599278 augmenty-1.3.2/src/augmenty/lang/
--rw-r--r--   0 root         (0) root         (0)      784 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.599278 augmenty-1.3.2/src/augmenty/lang/da/
--rw-r--r--   0 root         (0) root         (0)      195 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1878 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/da/augmenters.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/da/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.599278 augmenty-1.3.2/src/augmenty/lang/de/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/de/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/de/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.599278 augmenty-1.3.2/src/augmenty/lang/el/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/el/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/el/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/en/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/en/__init__.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/en/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/es/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/es/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/es/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/fr/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/fr/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/hu/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/hu/__init__.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/hu/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/it/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/it/__init__.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/it/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/lt/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/lt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      794 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/lt/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/mk/
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/mk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/mk/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/nb/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/nb/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/nl/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/nl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/nl/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/pl/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/pl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/pl/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.603278 augmenty-1.3.2/src/augmenty/lang/pt/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/pt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/pt/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.607278 augmenty-1.3.2/src/augmenty/lang/ro/
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/ro/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/ro/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.607278 augmenty-1.3.2/src/augmenty/lang/ru/
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/ru/__init__.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/lang/ru/keyboard.py
--rw-r--r--   0 root         (0) root         (0)     8801 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.607278 augmenty-1.3.2/src/augmenty/span/
--rw-r--r--   0 root         (0) root         (0)      177 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/span/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12131 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/span/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.607278 augmenty-1.3.2/src/augmenty/token/
--rw-r--r--   0 root         (0) root         (0)      680 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/token/casing.py
--rw-r--r--   0 root         (0) root         (0)    12158 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/token/insert.py
--rw-r--r--   0 root         (0) root         (0)    11343 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/token/replace.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/token/spacing.py
--rw-r--r--   0 root         (0) root         (0)     2325 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/token/static_embedding_util.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/token/swap.py
--rw-r--r--   0 root         (0) root         (0)      814 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/token/wordnet_util.py
--rw-r--r--   0 root         (0) root         (0)     3798 2023-03-06 12:37:51.000000 augmenty-1.3.2/src/augmenty/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.599278 augmenty-1.3.2/src/augmenty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7212 2023-03-06 12:38:02.000000 augmenty-1.3.2/src/augmenty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3399 2023-03-06 12:38:02.000000 augmenty-1.3.2/src/augmenty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-06 12:38:02.000000 augmenty-1.3.2/src/augmenty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      566 2023-03-06 12:38:02.000000 augmenty-1.3.2/src/augmenty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-06 12:38:02.000000 augmenty-1.3.2/src/augmenty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.611278 augmenty-1.3.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20399 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-06 12:38:02.611278 augmenty-1.3.2/tests/lang/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/lang/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/lang/test_da.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2960 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_all_augmenters.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_augmentation_utilities.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_character.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_doc.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_general.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_spans.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_static_embedding.py
--rw-r--r--   0 root         (0) root         (0)     7445 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)      397 2023-03-06 12:37:51.000000 augmenty-1.3.2/tests/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.207014 augmenty-1.3.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.187014 augmenty-1.3.3/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.187014 augmenty-1.3.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      283 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/04_augmenter-request.md
+-rw-r--r--   0 root         (0) root         (0)      625 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.187014 augmenty-1.3.3/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-04-27 19:19:12.000000 augmenty-1.3.3/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-27 19:19:12.000000 augmenty-1.3.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      797 2023-04-27 19:19:12.000000 augmenty-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-04-27 19:19:13.000000 augmenty-1.3.3/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-04-27 19:19:12.000000 augmenty-1.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-04-27 19:19:23.207014 augmenty-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-27 19:19:12.000000 augmenty-1.3.3/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.191014 augmenty-1.3.3/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.191014 augmenty-1.3.3/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   385037 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   395381 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/adding_an_augmenter.rst
+-rw-r--r--   0 root         (0) root         (0)     6366 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenters_overview.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.augment_utilities.rst
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.character.rst
+-rw-r--r--   0 root         (0) root         (0)      733 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.doc.rst
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.keyboard.rst
+-rw-r--r--   0 root         (0) root         (0)      500 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.lang.rst
+-rw-r--r--   0 root         (0) root         (0)      334 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.span.rst
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.token.rst
+-rw-r--r--   0 root         (0) root         (0)      330 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/augmenty.util.rst
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/create_augmenters_table.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.191014 augmenty-1.3.3/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    15539 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/tutorials/introduction.ipynb
+-rw-r--r--   0 root         (0) root         (0)      210 2023-04-27 19:19:12.000000 augmenty-1.3.3/docs/tutorials/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/img/
+-rw-r--r--   0 root         (0) root         (0)   385037 2023-04-27 19:19:12.000000 augmenty-1.3.3/img/icon.png
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-04-27 19:19:13.000000 augmenty-1.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-04-27 19:19:12.000000 augmenty-1.3.3/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 19:19:23.207014 augmenty-1.3.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.187014 augmenty-1.3.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/about.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/augment_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/character/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/casing.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/replace.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/spacing.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/character/swap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/doc/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/doc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/doc/casing.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/doc/subset.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/lang/
+-rw-r--r--   0 root         (0) root         (0)      784 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/lang/da/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/da/augmenters.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/da/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty/lang/de/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/de/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/de/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/el/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/el/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/el/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/en/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/en/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/es/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/es/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/fr/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/fr/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/hu/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/hu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/hu/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/it/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/it/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/it/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/lt/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/lt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      794 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/lt/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/mk/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/mk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/mk/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/nb/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/nb/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/nl/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/nl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/nl/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/pl/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/pl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/pl/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.199014 augmenty-1.3.3/src/augmenty/lang/pt/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/pt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/pt/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.203014 augmenty-1.3.3/src/augmenty/lang/ro/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/ro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/ro/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.203014 augmenty-1.3.3/src/augmenty/lang/ru/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/ru/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/lang/ru/keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.203014 augmenty-1.3.3/src/augmenty/span/
+-rw-r--r--   0 root         (0) root         (0)      177 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/span/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11636 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/span/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.203014 augmenty-1.3.3/src/augmenty/token/
+-rw-r--r--   0 root         (0) root         (0)      680 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/casing.py
+-rw-r--r--   0 root         (0) root         (0)    12158 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/insert.py
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/replace.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/spacing.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/static_embedding_util.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/swap.py
+-rw-r--r--   0 root         (0) root         (0)      814 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/token/wordnet_util.py
+-rw-r--r--   0 root         (0) root         (0)     3798 2023-04-27 19:19:12.000000 augmenty-1.3.3/src/augmenty/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.195014 augmenty-1.3.3/src/augmenty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      566 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-27 19:19:23.000000 augmenty-1.3.3/src/augmenty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.207014 augmenty-1.3.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20399 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:19:23.207014 augmenty-1.3.3/tests/lang/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/lang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/lang/test_da.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_all_augmenters.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_augmentation_utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_character.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_doc.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_general.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_spans.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_static_embedding.py
+-rw-r--r--   0 root         (0) root         (0)     7445 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      397 2023-04-27 19:19:12.000000 augmenty-1.3.3/tests/test_util.py
```

### Comparing `augmenty-1.3.2/.github/ISSUE_TEMPLATE/01_bugs.md` & `augmenty-1.3.3/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/.github/ISSUE_TEMPLATE/config.yml` & `augmenty-1.3.3/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/.github/dependabot.yml` & `augmenty-1.3.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/.github/workflows/dependabot_automerge.yml` & `augmenty-1.3.3/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/.github/workflows/documentation.yml` & `augmenty-1.3.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/.github/workflows/release.yml` & `augmenty-1.3.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/.github/workflows/tests.yml` & `augmenty-1.3.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/.pre-commit-config.yaml` & `augmenty-1.3.3/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 
   - repo: https://github.com/asottile/add-trailing-comma
     rev: v2.4.0
     hooks:
       - id: add-trailing-comma
 
   - repo: https://github.com/PyCQA/docformatter
-    rev: v1.5.1
+    rev: v1.6.3
     hooks:
       - id: docformatter
         args: [--in-place]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: [--line-length, "88"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.252
+    rev: v0.0.262
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.1
+    rev: v1.2.0
     hooks:
       - id: mypy
```

### Comparing `augmenty-1.3.2/CHANGELOG.md` & `augmenty-1.3.3/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.3 (2023-04-27)
+### Fix
+* Adjust dep. annotations for ent augmenter ([`00bbc56`](https://github.com/KennethEnevoldsen/augmenty/commit/00bbc561211ca5bde68f030c191ea20caad6dbfc))
+
+### Documentation
+* Fix formatting such that is rendered as intended in the docs ([`a77c362`](https://github.com/KennethEnevoldsen/augmenty/commit/a77c362a09762bf4473d0e4afd1289cbbb15e526))
+
 ## v1.3.2 (2023-03-06)
 ### Fix
 * Test sem release ([`bab9525`](https://github.com/KennethEnevoldsen/augmenty/commit/bab9525d1117a0f5692eac36d371de55dfba9421))
 
 ### Documentation
 * Added github logo to footer ([`5f4ffee`](https://github.com/KennethEnevoldsen/augmenty/commit/5f4ffee209009ea82134b716bd5e1d6d11448f96))
 * Fixed error in docstring leading to missing variable docuementation ([`723ce45`](https://github.com/KennethEnevoldsen/augmenty/commit/723ce452b75729f199424f7d3cb1404be48df124))
```

### Comparing `augmenty-1.3.2/LICENSE` & `augmenty-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/PKG-INFO` & `augmenty-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmenty
-Version: 1.3.2
+Version: 1.3.3
 Summary: An augmentation library based on SpaCy for joint augmentation of text and labels.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: augmenty Version: 1.3.2 Summary: An augmentation
+Metadata-Version: 2.1 Name: augmenty Version: 1.3.3 Summary: An augmentation
 library based on SpaCy for joint augmentation of text and labels. Author-email:
 Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `augmenty-1.3.2/docs/Makefile` & `augmenty-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/_static/favicon.ico` & `augmenty-1.3.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/_static/icon.png` & `augmenty-1.3.3/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/_static/icon_dark.png` & `augmenty-1.3.3/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/adding_an_augmenter.rst` & `augmenty-1.3.3/docs/adding_an_augmenter.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/augmenters_overview.md` & `augmenty-1.3.3/docs/augmenters_overview.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/augmenty.character.rst` & `augmenty-1.3.3/docs/augmenty.character.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/augmenty.doc.rst` & `augmenty-1.3.3/docs/augmenty.doc.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/augmenty.token.rst` & `augmenty-1.3.3/docs/augmenty.token.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/conf.py` & `augmenty-1.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/create_augmenters_table.py` & `augmenty-1.3.3/docs/create_augmenters_table.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/faq.rst` & `augmenty-1.3.3/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/index.rst` & `augmenty-1.3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/installation.rst` & `augmenty-1.3.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/make.bat` & `augmenty-1.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/news.rst` & `augmenty-1.3.3/docs/news.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/docs/tutorials/introduction.ipynb` & `augmenty-1.3.3/docs/tutorials/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/img/icon.png` & `augmenty-1.3.3/img/icon.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/pyproject.toml` & `augmenty-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "augmenty"
-version = "1.3.2"
+version = "1.3.3"
 description = "An augmentation library based on SpaCy for joint augmentation of text and labels."
 authors = [{name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
```

### Comparing `augmenty-1.3.2/readme.md` & `augmenty-1.3.3/readme.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/__init__.py` & `augmenty-1.3.3/src/augmenty/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/augment_utilities.py` & `augmenty-1.3.3/src/augmenty/augment_utilities.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/character/casing.py` & `augmenty-1.3.3/src/augmenty/character/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/character/replace.py` & `augmenty-1.3.3/src/augmenty/character/replace.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/character/spacing.py` & `augmenty-1.3.3/src/augmenty/character/spacing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/character/swap.py` & `augmenty-1.3.3/src/augmenty/character/swap.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/doc/casing.py` & `augmenty-1.3.3/src/augmenty/doc/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/doc/subset.py` & `augmenty-1.3.3/src/augmenty/doc/subset.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/keyboard.py` & `augmenty-1.3.3/src/augmenty/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/__init__.py` & `augmenty-1.3.3/src/augmenty/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/da/augmenters.py` & `augmenty-1.3.3/src/augmenty/lang/da/augmenters.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/da/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/da/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/de/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/de/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/el/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/el/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/en/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/en/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/es/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/es/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/fr/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/fr/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/hu/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/hu/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/it/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/it/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/lt/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/lt/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/mk/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/mk/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/nb/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/nb/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/nl/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/nl/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/pl/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/pl/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/pt/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/pt/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/ro/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/ro/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/lang/ru/keyboard.py` & `augmenty-1.3.3/src/augmenty/lang/ru/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/meta.json` & `augmenty-1.3.3/src/augmenty/meta.json`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/span/entities.py` & `augmenty-1.3.3/src/augmenty/span/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             tok_anno["ORTH"][i] = new_ent
             tok_anno["LEMMA"][i] = new_ent
 
             tok_anno["TAG"][i] = ["PROPN"] * len_ent
             tok_anno["POS"][i] = ["PROPN"] * len_ent
 
             tok_anno["MORPH"][i] = [""] * len_ent
-            tok_anno["DEP"][i] = [tok_anno["DEP"][i][0]] + ["flat"] * (len_ent - 1)
+            tok_anno["DEP"][i] = [ent[0].dep_] + ["flat"] * (len_ent - 1)
 
             tok_anno["SENT_START"][i] = [tok_anno["SENT_START"][i][0]] + [0] * (
                 len_ent - 1
             )
             tok_anno["SPACY"][i] = [True] * (len_ent - 1) + (
                 tok_anno["SPACY"][i][-1:]  # set last spacing
             )
@@ -109,26 +109,26 @@
     replace_consistency: bool = True,
     resolve_dependencies: bool = True,
 ) -> Callable[[Language, Example], Iterator[Example]]:
     """Create an augmenter which replaces an entity based on a dictionary
     lookup.
 
     Args:
-        level (float): the percentage of entities to be augmented.
-        ent_dict (Dict[str, Iterable[List[str]]]): A dictionary with keys corresponding
+        level: the percentage of entities to be augmented.
+        ent_dict: A dictionary with keys corresponding
             the the entity type you wish to replace (e.g. "PER") and a itarable of the
             replacements. A replacement is a list of string of the desired entity
             replacement ["Kenneth", "Enevoldsen"].
-        replace_consistency (bool, optional): Should an entity always be replaced with
+        replace_consistency: Should an entity always be replaced with
             the same entity? Defaults to True.
-        resolve_dependencies (bool, optional): Attempts to resolve the dependency tree
-            by setting head of the original entitity as
-        the head of the first token in the new entity. The remainder is the passed as
+        resolve_dependencies: Attempts to resolve the dependency tree
+            by setting head of the original entitity aa the head of the
+            first token in the new entity. The remainder is the passed as
     Returns:
-        Callable[[Language, Example], Iterator[Example]]: The augmenter
+        The augmenter
 
     Example:
         >>> ent_dict = {"ORG": [["Google"], ["Apple"]],
         >>>             "PERSON": [["Kenneth"], ["Lasse", "Hansen"]]}
         >>> # augment 10% of names
         >>> ent_augmenter = create_ent_augmenter(ent_dict, level = 0.1)
     """
@@ -173,33 +173,33 @@
     replace_consistency: bool = True,
     person_tag: str = "PERSON",
 ) -> Callable[[Language, Example], Iterator[Example]]:
     """Create an augmenter which replaces a name (PER) with a news sampled from
     the names dictionary.
 
     Args:
-        names (Dict[str, List[str]]): A dictionary of list of names to sample from.
+        names: A dictionary of list of names to sample from.
             These could for example include first name and last names.
-        pattern (List[List[str]]): The pattern to create the names. This should be a
+        pattern: The pattern to create the names. This should be a
             list of patterns.
             Where a pattern is a list of strings, where the string denote the list in
             the names dictionary in which to sample from.
-        level (float): The proportion of PER entities to replace.
-        names_p (Dict[str, List[float]], optional): The probability to sample each name.
+        level: The proportion of PER entities to replace.
+        names_p: The probability to sample each name.
             Defaults to {}, indicating equal probability for each name.
-        patterns_p (Optional[List[float]], optional): The probability to sample each
+        patterns_p: The probability to sample each
             pattern. Defaults to None, indicating equal probability for each pattern.
-        replace_consistency (bool, optional): Should the entity always be replaced with
+        replace_consistency: Should the entity always be replaced with
             the same entity? Defaults to True.
-        person_tag (str, optional): The tag of the person entity. Defaults to "PERSON".
+        person_tag: The tag of the person entity. Defaults to "PERSON".
             However it should be noted that much such as the Danish spacy model uses
             "PER" instead.
 
     Returns:
-        Callable[[Language, Example], Iterator[Example]]: The augmenter
+        The augmenter
 
     Example:
         >>> names = {"firstname": ["Kenneth", "Lasse"],
         >>>          "lastname": ["Enevoldsen", "Hansen"]}
         >>> patterns = [["firstname"], ["firstname", "lastname"],
         >>>             ["firstname", "firstname", "lastname"]]
         >>> person_tag = "PERSON"
@@ -263,31 +263,31 @@
     level: float,
     ent_types: Optional[List[str]] = None,
 ) -> Callable[[Language, Example], Iterator[Example]]:
     """Creates an augmenter which reorders and formats a entity according to
     reordering and formatting functions.
 
     Args:
-        reordering (List[Union[int, None]]): A reordering consisting of a the desired
+        reordering: A reordering consisting of a the desired
             order of the list of indices, where None denotes the remainder. For
             instance if this function was solely used on names [-1, None] indicate last
             name (the last token in the name) followed by the remainder of the name.
             Similarly one could more use the reordering [3, 1, 2] e.g. indicating last
             name, first name, middle name. Note that if the entity only include two
             tokens the 3 will be ignored producing the pattern [1, 2].
-        formatter (List[Union[Callable[[Token], str], None]]): A list of function
+        formatter: A list of function
             taking in a spaCy Token returning the reformatted str. E.g. the function
             `lambda token: token.text[0] + "."` would abbreviate the token and add
             punctuation. None corresponds to no augmentation.
-        level (float): The probability of an entities being augmented.
-        ent_types (Optional[Iterable[str]], optional):  The entity types which should
+        level: The probability of an entities being augmented.
+        ent_types:  The entity types which should
             be augmented. Defaults to None, indicating all entity types.
 
     Returns:
-        Callable[[Language, Example], Iterator[Example]]: The augmenter
+        The augmenter
 
     Example:
         >>> import augmenty
         >>> import spacy
         >>> nlp = spacy.load("en_core_web_sm")
         >>> abbreviate = lambda token: token.text[0] + "."
         >>> augmenter = augmenty.load("ents_format_v1", reordering = [-1, None],
```

### Comparing `augmenty-1.3.2/src/augmenty/token/__init__.py` & `augmenty-1.3.3/src/augmenty/token/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/token/casing.py` & `augmenty-1.3.3/src/augmenty/token/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/token/insert.py` & `augmenty-1.3.3/src/augmenty/token/insert.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/token/replace.py` & `augmenty-1.3.3/src/augmenty/token/replace.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/token/spacing.py` & `augmenty-1.3.3/src/augmenty/token/spacing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/token/static_embedding_util.py` & `augmenty-1.3.3/src/augmenty/token/static_embedding_util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/token/swap.py` & `augmenty-1.3.3/src/augmenty/token/swap.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/token/wordnet_util.py` & `augmenty-1.3.3/src/augmenty/token/wordnet_util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty/util.py` & `augmenty-1.3.3/src/augmenty/util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty.egg-info/PKG-INFO` & `augmenty-1.3.3/src/augmenty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmenty
-Version: 1.3.2
+Version: 1.3.3
 Summary: An augmentation library based on SpaCy for joint augmentation of text and labels.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: augmenty Version: 1.3.2 Summary: An augmentation
+Metadata-Version: 2.1 Name: augmenty Version: 1.3.3 Summary: An augmentation
 library based on SpaCy for joint augmentation of text and labels. Author-email:
 Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `augmenty-1.3.2/src/augmenty.egg-info/SOURCES.txt` & `augmenty-1.3.3/src/augmenty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/src/augmenty.egg-info/requires.txt` & `augmenty-1.3.3/src/augmenty.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/tests/books.py` & `augmenty-1.3.3/tests/books.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/tests/fixtures.py` & `augmenty-1.3.3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/tests/lang/test_da.py` & `augmenty-1.3.3/tests/lang/test_da.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/tests/test_all_augmenters.py` & `augmenty-1.3.3/tests/test_all_augmenters.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/tests/test_augmentation_utilities.py` & `augmenty-1.3.3/tests/test_augmentation_utilities.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/tests/test_character.py` & `augmenty-1.3.3/tests/test_character.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/tests/test_doc.py` & `augmenty-1.3.3/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/tests/test_spans.py` & `augmenty-1.3.3/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.2/tests/test_token.py` & `augmenty-1.3.3/tests/test_token.py`

 * *Files identical despite different names*

