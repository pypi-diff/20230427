# Comparing `tmp/saltext.salt-describe-0.1.1.tar.gz` & `tmp/saltext.salt-describe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltext.salt-describe-0.1.1.tar", last modified: Fri Mar 31 19:04:04 2023, max compression
+gzip compressed data, was "saltext.salt-describe-1.0.0.tar", last modified: Thu Apr 27 19:29:59 2023, max compression
```

## Comparing `saltext.salt-describe-0.1.1.tar` & `saltext.salt-describe-1.0.0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.308636 saltext.salt-describe-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      720 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.coveragerc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.296636 saltext.salt-describe-0.1.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.300636 saltext.salt-describe-0.1.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     4037 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)     1038 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.github/workflows/deploy-package-action.yml
--rw-r--r--   0 root         (0) root         (0)      903 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.github/workflows/docs-action.yml
--rw-r--r--   0 root         (0) root         (0)     1117 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.github/workflows/package-action.yml
--rw-r--r--   0 root         (0) root         (0)      181 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1744 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.github/workflows/pre-commit-action.yml
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)    11776 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.github/workflows/test-action.yml
--rw-r--r--   0 root         (0) root         (0)     1958 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     8473 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.300636 saltext.salt-describe-0.1.1/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     2159 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.pre-commit-hooks/copyright_headers.py
--rw-r--r--   0 root         (0) root         (0)     1574 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 root         (0) root         (0)    11777 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      548 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)     5246 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     3802 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11364 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      412 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2546 2023-03-31 19:04:04.308636 saltext.salt-describe-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1276 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.300636 saltext.salt-describe-0.1.1/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.300636 saltext.salt-describe-0.1.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/_static/.gitkeep
--rw-r--r--   0 root         (0) root         (0)      142 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/all.rst
--rw-r--r--   0 root         (0) root         (0)     5394 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     4562 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/gettingstarted.rst
--rw-r--r--   0 root         (0) root         (0)      255 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.300636 saltext.salt-describe-0.1.1/docs/ref/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/ref/.gitkeep
--rw-r--r--   0 root         (0) root         (0)       58 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/ref/modules.rst
--rw-r--r--   0 root         (0) root         (0)      141 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/ref/saltext.rst
--rw-r--r--   0 root         (0) root         (0)      476 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/ref/saltext.salt_describe.rst
--rw-r--r--   0 root         (0) root         (0)     3349 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/ref/saltext.salt_describe.runners.rst
--rw-r--r--   0 root         (0) root         (0)      989 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/ref/saltext.salt_describe.utils.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    17751 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/noxfile.py
--rw-r--r--   0 root         (0) root         (0)      321 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.300636 saltext.salt-describe-0.1.1/requirements/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/requirements/docs-auto.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      414 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)     1814 2023-03-31 19:04:04.308636 saltext.salt-describe-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      364 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.296636 saltext.salt-describe-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.296636 saltext.salt-describe-0.1.1/src/saltext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.304636 saltext.salt-describe-0.1.1/src/saltext/salt_describe/
--rw-r--r--   0 root         (0) root         (0)      933 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.304636 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10200 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe.py
--rw-r--r--   0 root         (0) root         (0)     6090 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_cron.py
--rw-r--r--   0 root         (0) root         (0)     3235 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_file.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_firewalld.py
--rw-r--r--   0 root         (0) root         (0)     1904 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_host.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_iptables.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_pip.py
--rw-r--r--   0 root         (0) root         (0)     4962 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_pkg.py
--rw-r--r--   0 root         (0) root         (0)     4262 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_pkgrepo.py
--rw-r--r--   0 root         (0) root         (0)     6313 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_service.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_sysctl.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_timezone.py
--rw-r--r--   0 root         (0) root         (0)     5477 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.304636 saltext.salt-describe-0.1.1/src/saltext/salt_describe/utils/
--rw-r--r--   0 root         (0) root         (0)      731 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/utils/ansible_describe.py
--rw-r--r--   0 root         (0) root         (0)      724 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/utils/chef_describe.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/utils/init.py
--rw-r--r--   0 root         (0) root         (0)     3253 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/utils/salt_describe.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-31 19:04:04.000000 saltext.salt-describe-0.1.1/src/saltext/salt_describe/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.304636 saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2546 2023-03-31 19:04:04.000000 saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3953 2023-03-31 19:04:04.000000 saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 19:04:04.000000 saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-03-31 19:04:04.000000 saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 19:04:04.000000 saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      672 2023-03-31 19:04:04.000000 saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-31 19:04:04.000000 saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.304636 saltext.salt-describe-0.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.304636 saltext.salt-describe-0.1.1/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      515 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.308636 saltext.salt-describe-0.1.1/tests/integration/runners/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe.py
--rw-r--r--   0 root         (0) root         (0)      656 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_file.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_firewalld.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_host.py
--rw-r--r--   0 root         (0) root         (0)      882 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_iptables.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_pip.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_pkg.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_service.py
--rw-r--r--   0 root         (0) root         (0)      687 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_sysctl.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_timezone.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.308636 saltext.salt-describe-0.1.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.308636 saltext.salt-describe-0.1.1/tests/unit/runners/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8216 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_cron.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_file.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_firewalld.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_host.py
--rw-r--r--   0 root         (0) root         (0)     3021 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_iptables.py
--rw-r--r--   0 root         (0) root         (0)     2502 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_pip.py
--rw-r--r--   0 root         (0) root         (0)     5000 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_pkg.py
--rw-r--r--   0 root         (0) root         (0)    22897 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_pkgrepo.py
--rw-r--r--   0 root         (0) root         (0)     7748 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_service.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_sysctl.py
--rw-r--r--   0 root         (0) root         (0)     1275 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_timezone.py
--rw-r--r--   0 root         (0) root         (0)     8736 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_user_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:04:04.308636 saltext.salt-describe-0.1.1/tests/unit/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      971 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/utils/test_ansible_describe.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/utils/test_init.py
--rw-r--r--   0 root         (0) root         (0)     4368 2023-03-31 19:03:54.000000 saltext.salt-describe-0.1.1/tests/unit/utils/test_salt_describe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.668626 saltext.salt-describe-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.coveragerc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.644625 saltext.salt-describe-1.0.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.652625 saltext.salt-describe-1.0.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.github/workflows/deploy-package-action.yml
+-rw-r--r--   0 root         (0) root         (0)      903 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.github/workflows/docs-action.yml
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.github/workflows/package-action.yml
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.github/workflows/pre-commit-action.yml
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)    11776 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.github/workflows/test-action.yml
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     8473 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.656625 saltext.salt-describe-1.0.0/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.pre-commit-hooks/copyright_headers.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.pre-commit-hooks/make-autodocs.py
+-rw-r--r--   0 root         (0) root         (0)    11777 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      548 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     3802 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11364 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-04-27 19:29:59.668626 saltext.salt-describe-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.656625 saltext.salt-describe-1.0.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.656625 saltext.salt-describe-1.0.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/_static/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)      142 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/all.rst
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/gettingstarted.rst
+-rw-r--r--   0 root         (0) root         (0)      255 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.656625 saltext.salt-describe-1.0.0/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/ref/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/ref/modules.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/ref/saltext.rst
+-rw-r--r--   0 root         (0) root         (0)      476 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/ref/saltext.salt_describe.rst
+-rw-r--r--   0 root         (0) root         (0)     3349 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/ref/saltext.salt_describe.runners.rst
+-rw-r--r--   0 root         (0) root         (0)      989 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/ref/saltext.salt_describe.utils.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    17751 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)      321 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.660626 saltext.salt-describe-1.0.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/requirements/docs-auto.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      414 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-04-27 19:29:59.668626 saltext.salt-describe-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      364 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.648625 saltext.salt-describe-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.648625 saltext.salt-describe-1.0.0/src/saltext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.660626 saltext.salt-describe-1.0.0/src/saltext/salt_describe/
+-rw-r--r--   0 root         (0) root         (0)      933 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.664626 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10200 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe.py
+-rw-r--r--   0 root         (0) root         (0)     6017 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_cron.py
+-rw-r--r--   0 root         (0) root         (0)     3448 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_file.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_firewalld.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_host.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_iptables.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_pip.py
+-rw-r--r--   0 root         (0) root         (0)     4928 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_pkg.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_pkgrepo.py
+-rw-r--r--   0 root         (0) root         (0)     6240 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_service.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_sysctl.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_timezone.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.664626 saltext.salt-describe-1.0.0/src/saltext/salt_describe/utils/
+-rw-r--r--   0 root         (0) root         (0)      997 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/utils/ansible_describe.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/utils/chef_describe.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/utils/init.py
+-rw-r--r--   0 root         (0) root         (0)     4169 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/utils/salt_describe.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-27 19:29:59.000000 saltext.salt-describe-1.0.0/src/saltext/salt_describe/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.660626 saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-04-27 19:29:59.000000 saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3953 2023-04-27 19:29:59.000000 saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:29:59.000000 saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-27 19:29:59.000000 saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:29:59.000000 saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      672 2023-04-27 19:29:59.000000 saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-27 19:29:59.000000 saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.664626 saltext.salt-describe-1.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3689 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.664626 saltext.salt-describe-1.0.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.668626 saltext.salt-describe-1.0.0/tests/integration/runners/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe.py
+-rw-r--r--   0 root         (0) root         (0)      656 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_file.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_firewalld.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_host.py
+-rw-r--r--   0 root         (0) root         (0)      882 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_iptables.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_pip.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_pkg.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_service.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_sysctl.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_timezone.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.668626 saltext.salt-describe-1.0.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.668626 saltext.salt-describe-1.0.0/tests/unit/runners/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8216 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe.py
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_cron.py
+-rw-r--r--   0 root         (0) root         (0)     3951 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_file.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_firewalld.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_host.py
+-rw-r--r--   0 root         (0) root         (0)     5074 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_iptables.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_pip.py
+-rw-r--r--   0 root         (0) root         (0)     8922 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_pkg.py
+-rw-r--r--   0 root         (0) root         (0)    26111 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_pkgrepo.py
+-rw-r--r--   0 root         (0) root         (0)     9388 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_service.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_sysctl.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_timezone.py
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_user_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:29:59.668626 saltext.salt-describe-1.0.0/tests/unit/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/utils/test_ansible_describe.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/utils/test_init.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-04-27 19:29:48.000000 saltext.salt-describe-1.0.0/tests/unit/utils/test_salt_describe.py
```

### Comparing `saltext.salt-describe-0.1.1/.coveragerc` & `saltext.salt-describe-1.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.github/workflows/ci.yml` & `saltext.salt-describe-1.0.0/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     uses: ./.github/workflows/deploy-package-action.yml
     if: ${{ inputs.release && success() }}
     needs:
       - pre-commit
       - test
       - docs
       - build-python-package
+      - deploy-python-package-test-pypi
     secrets:
       PYPI_API_TOKEN: "${{ secrets.PYPI_API_TOKEN }}"
     with:
       test: false
       version: "${{ inputs.version }}"
 
   push-tag:
```

### Comparing `saltext.salt-describe-0.1.1/.github/workflows/deploy-package-action.yml` & `saltext.salt-describe-1.0.0/.github/workflows/deploy-package-action.yml`

 * *Files 14% similar despite different names*

```diff
@@ -14,28 +14,28 @@
       PYPI_API_TOKEN:
         required: false
       TEST_PYPI_API_TOKEN:
         required: false
 
 jobs:
   build:
-    name: Publish Python Wheel
+    name: Publish Python Package to ${{ fromJSON('["PyPI", "Test PyPI"]')[inputs.test] }}
     runs-on: ubuntu-latest
     steps:
       - name: Download Python Package Artifacts
         uses: actions/download-artifact@v3
         with:
           name: salt-describe-${{ inputs.version }}-packages
           path: dist
 
-      - name: Publish distribution to PyPI
+      - name: Publish distribution to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         if: ${{ inputs.test }}
         with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
           repository-url: https://test.pypi.org/legacy/
 
       - name: Publish distribution to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         if: ${{ !inputs.test }}
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `saltext.salt-describe-0.1.1/.github/workflows/docs-action.yml` & `saltext.salt-describe-1.0.0/.github/workflows/docs-action.yml`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.github/workflows/package-action.yml` & `saltext.salt-describe-1.0.0/.github/workflows/package-action.yml`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.github/workflows/pre-commit-action.yml` & `saltext.salt-describe-1.0.0/.github/workflows/pre-commit-action.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
       changed-files:
         required: true
         type: string
         description: JSON string containing information about changed files
 
 jobs:
   Pre-Commit:
-    name: Relenv
+    name: Pre-Commit
     runs-on: ubuntu-latest
     container:
       image: python:3.8.6-slim-buster
 
     steps:
       - name: Install System Deps
         run: |
```

### Comparing `saltext.salt-describe-0.1.1/.github/workflows/release.yml` & `saltext.salt-describe-1.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.github/workflows/test-action.yml` & `saltext.salt-describe-1.0.0/.github/workflows/test-action.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         python-version:
           - 3.8
           - 3.9
         salt-version:
           - 3004.2
           - 3005.1
         include:
-          - python-version: 3.10.10
+          - python-version: 3.10.11
             salt-version: 3006.0rc1
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
@@ -281,15 +281,15 @@
     strategy:
       fail-fast: false
       max-parallel: 3
       matrix:
         include:
           - python-version: 3.9
             salt-version: 3005.1
-          - python-version: 3.10.10
+          - python-version: 3.10.11
             salt-version: 3006.0rc1
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
```

### Comparing `saltext.salt-describe-0.1.1/.gitignore` & `saltext.salt-describe-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.pre-commit-config.yaml` & `saltext.salt-describe-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.pre-commit-hooks/check-cli-examples.py` & `saltext.salt-describe-1.0.0/.pre-commit-hooks/check-cli-examples.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.pre-commit-hooks/copyright_headers.py` & `saltext.salt-describe-1.0.0/.pre-commit-hooks/copyright_headers.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.pre-commit-hooks/make-autodocs.py` & `saltext.salt-describe-1.0.0/.pre-commit-hooks/make-autodocs.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.pylintrc` & `saltext.salt-describe-1.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/.readthedocs.yaml` & `saltext.salt-describe-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/CODE_OF_CONDUCT.md` & `saltext.salt-describe-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/CONTRIBUTING.md` & `saltext.salt-describe-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/LICENSE` & `saltext.salt-describe-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/PKG-INFO` & `saltext.salt-describe-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltext.salt-describe
-Version: 0.1.1
+Version: 1.0.0
 Summary: Salt Describe Runner
 Home-page: http://github.com/saltstack//salt-describe/
 Author: Megan Wilhite, Gareth J. Greenaway
 Author-email: mwilhite@vmware.com, ggreenaway@vmware.com
 License: Apache Software License
 Project-URL: Source, http://github.com/saltstack//salt-describe/
 Project-URL: Tracker, http://github.com/saltstack//salt-describe/issues
```

### Comparing `saltext.salt-describe-0.1.1/README.md` & `saltext.salt-describe-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/docs/Makefile` & `saltext.salt-describe-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/docs/conf.py` & `saltext.salt-describe-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/docs/gettingstarted.rst` & `saltext.salt-describe-1.0.0/docs/gettingstarted.rst`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,21 @@
 Salt describe is hosted as a pip package on pypi, so you only need to install the pip package
 for the install.
 
 If you are using onedir Salt packages, you need to run the following:
 
 .. code-block:: bash
 
-   # salt-pip install salt-describe
+   # salt-pip install saltext.salt-describe
 
 If you are using the Salt pip packages, you need to run the following:
 
 .. code-block:: bash
 
-   # pip install salt-describe
+   # pip install saltext.salt-describe
 
 
 How to use Salt describe
 ========================
 
 Now you are ready to start using Salt describe, and auto generating your SLS files for all
 of the systems you want to manage. Salt describe is a Salt runner, so you need to use the cli
```

### Comparing `saltext.salt-describe-0.1.1/docs/make.bat` & `saltext.salt-describe-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/docs/ref/saltext.salt_describe.runners.rst` & `saltext.salt-describe-1.0.0/docs/ref/saltext.salt_describe.runners.rst`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/docs/ref/saltext.salt_describe.utils.rst` & `saltext.salt-describe-1.0.0/docs/ref/saltext.salt_describe.utils.rst`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/noxfile.py` & `saltext.salt-describe-1.0.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/setup.cfg` & `saltext.salt-describe-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/__init__.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/__init__.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_cron.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_cron.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,11 @@
         final_sls = {}
         for sls_contents in (env_sls, crons_sls, specials_sls):
             for state_name in sls_contents:
                 final_sls[state_name] = sls_contents[state_name]
 
         sls_yaml = yaml.dump(final_sls)
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, sls_yaml, sls_name="cron", config_system=config_system
-                )
-            )
+            generate_files(__opts__, minion, sls_yaml, sls_name="cron", config_system=config_system)
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_file.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -90,21 +90,24 @@
     for minion in list(state_contents.keys()):
         state = yaml.dump(state_contents[minion])
         minion_state_root = get_minion_state_file_root(__opts__, minion, config_system="salt")
 
         for path in file_contents[minion]:
             path_obj = pathlib.Path(path)
             path_file = minion_state_root / "files" / path_obj.relative_to(path_obj.anchor)
-            path_file.parent.mkdir(parents=True, exist_ok=True)
+            try:
+                path_file.parent.mkdir(parents=True, exist_ok=True)
+            except PermissionError:
+                log.warning(
+                    f"Unable to create directory {str(path_file.parent)}.  "
+                    "Check that the salt user has the correct permissions."
+                )
+                return False
 
             with salt.utils.files.fopen(path_file, "w") as fp_:
                 fp_.write(file_contents[minion][path])
 
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name="files", config_system=config_system
-                )
-            )
+            generate_files(__opts__, minion, state, sls_name="files", config_system=config_system)
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_firewalld.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_firewalld.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,13 @@
 
             state_contents[state_id][state_func] = kwargs
             count += 1
 
         state = yaml.dump(state_contents)
 
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name="firewalld", config_system=config_system
-                )
+            generate_files(
+                __opts__, minion, state, sls_name="firewalld", config_system=config_system
             )
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_host.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_host.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,11 @@
                 state_contents[sls_id] = {state_func: [{"ip": []}, {"names": []}]}
                 state_contents[sls_id][state_func][0]["ip"] = key
                 state_contents[sls_id][state_func][1]["names"] = value["aliases"]
                 count += 1
 
         state = yaml.dump(state_contents)
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name="host", config_system=config_system
-                )
-            )
+            generate_files(__opts__, minion, state, sls_name="host", config_system=config_system)
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_iptables.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_iptables.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,13 @@
                         kwargs.append({kwarg.replace("_", "-"): " ".join(_rule[kwarg])})
                     state_contents[state_id][state_func] = kwargs
                     count += 1
 
         state = yaml.dump(state_contents)
 
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name="iptables", config_system=config_system
-                )
+            generate_files(
+                __opts__, minion, state, sls_name="iptables", config_system=config_system
             )
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_pip.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_pip.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,13 +89,11 @@
         minion_pip_list = ret[minion]
         state_contents = getattr(sys.modules[__name__], f"_parse_{config_system}")(
             minion, minion_pip_list, **kwargs
         )
         state = yaml.dump(state_contents)
 
         sls_files.append(
-            str(
-                generate_files(__opts__, minion, state, sls_name="pip", config_system=config_system)
-            )
+            generate_files(__opts__, minion, state, sls_name="pip", config_system=config_system)
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_pkg.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_pkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,13 @@
             minion, pkgs, single_state, include_version, pkg_cmd, **kwargs
         )
 
         if config_system in ("ansible", "salt"):
             state = yaml.dump(state_contents)
         else:
             state = "\n".join(state_contents)
+
         sls_files.append(
-            str(
-                generate_files(__opts__, minion, state, sls_name="pkg", config_system=config_system)
-            )
+            generate_files(__opts__, minion, state, sls_name="pkg", config_system=config_system)
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_pkgrepo.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_pkgrepo.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,13 @@
                             state_contents[sls_id][state_func].append(
                                 {"architectures": architectures}
                             )
 
         state = yaml.dump(state_contents)
 
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name=state_name, config_system=config_system
-                )
+            generate_files(
+                __opts__, minion, state, sls_name=state_name, config_system=config_system
             )
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_service.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,11 @@
             minion, service_status, enabled_services, disabled_services, **kwargs
         )
         if config_system in ("ansible", "salt"):
             state = yaml.dump(state_contents)
         else:
             state = "\n".join(state_contents)
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name="service", config_system=config_system
-                )
-            )
+            generate_files(__opts__, minion, state, sls_name="service", config_system=config_system)
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_sysctl.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_sysctl.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,11 @@
                 payload = [{"name": current}, {"value": sysctls[minion][current]}]
                 state_contents[f"sysctl-{current}"] = {"sysctl.present": payload}
             else:
                 log.error("%s not found in sysctl", current)
 
         state = yaml.dump(state_contents)
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name="sysctl", config_system=config_system
-                )
-            )
+            generate_files(__opts__, minion, state, sls_name="sysctl", config_system=config_system)
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_timezone.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_timezone.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,13 @@
 
         state_contents = {}
         state_contents = {timezone: {"timezone.system": []}}
 
         state = yaml.dump(state_contents)
 
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name="timezone", config_system=config_system
-                )
+            generate_files(
+                __opts__, minion, state, sls_name="timezone", config_system=config_system
             )
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/runners/salt_describe_user.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/runners/salt_describe_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,19 +119,15 @@
             passwd = shadow["passwd"]
             if passwd != "*":
                 pillars["users"].update({user["name"]: f"{passwd}"})
 
         state = yaml.dump(state_contents)
         pillars = yaml.dump(pillars)
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name="users", config_system=config_system
-                )
-            )
+            generate_files(__opts__, minion, state, sls_name="users", config_system=config_system)
         )
         generate_pillars(__opts__, minion, pillars, sls_name="users")
     return ret_info(sls_files, mod=mod_name)
 
 
 def group(
     tgt,
@@ -171,15 +167,11 @@
             if include_members is True:
                 payload.append({"members": group["members"]})
             state_contents[f"group-{groupname}"] = {"group.present": payload}
 
         state = yaml.dump(state_contents)
 
         sls_files.append(
-            str(
-                generate_files(
-                    __opts__, minion, state, sls_name="groups", config_system=config_system
-                )
-            )
+            generate_files(__opts__, minion, state, sls_name="groups", config_system=config_system)
         )
 
     return ret_info(sls_files, mod=mod_name)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/utils/ansible_describe.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/utils/chef_describe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
+import logging
 import pathlib
 
 import salt.config
 import salt.syspaths
 import salt.utils.files
 import yaml
 
+log = logging.getLogger(__name__)
+
 
 def generate_files(opts, minion, state, sls_name="default", env="base", root=None):
     """
     Generate an sls file for the minion with given state contents
     """
     if not root:
-        minion_state_root = pathlib.Path("/srv", "ansible", minion)
+        minion_state_root = pathlib.Path("/srv", "chef", minion)
     else:
-        minion_state_root = pathlib.Path(root, "ansible", minion)
-    minion_state_root.mkdir(parents=True, exist_ok=True)
+        minion_state_root = pathlib.Path(root, "chef", minion)
+    try:
+        minion_state_root.mkdir(parents=True, exist_ok=True)
+    except PermissionError:
+        log.warning(
+            f"Unable to create directory {str(minion_state_root)}.  Check that the salt user has the correct permissions."
+        )
+        return False
 
-    minion_state_file = minion_state_root / f"{sls_name}.yml"
+    minion_state_file = minion_state_root / f"{sls_name}.rb"
 
     with salt.utils.files.fopen(minion_state_file, "w") as fp_:
         fp_.write(state)
 
     return minion_state_file
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/utils/init.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/utils/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,28 +13,32 @@
 
 def generate_files(opts, minion, state, sls_name="default", env="base", config_system="salt"):
     """
     Generate the files for the given config management system
     """
     config = getattr(saltext.salt_describe.utils, f"{config_system}_describe")
 
-    return config.generate_files(opts, minion, state, sls_name=sls_name, env=env)
+    res = config.generate_files(opts, minion, state, sls_name=sls_name, env=env)
+    if res:
+        return str(res)
+    else:
+        return res
 
 
 def get_minion_state_file_root(opts, minion, env="base", config_system="salt"):
     """
     Return the state file root for the given minion
     """
     config = getattr(saltext.salt_describe.utils, f"{config_system}_describe")
 
     return config.get_minion_state_file_root(opts, minion, env=env)
 
 
 def ret_info(sls_files, mod=None):
-    if not sls_files:
+    if not any(sls_files):
         if mod:
             log.error("Could not generate SLS file for %s", mod)
         return False
     return {"Generated SLS file locations": sls_files}
 
 
 def parse_salt_ret(ret, tgt):
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext/salt_describe/utils/salt_describe.py` & `saltext.salt-describe-1.0.0/src/saltext/salt_describe/utils/salt_describe.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
+import logging
 import pathlib
 
 import salt.config
 import salt.syspaths
 import salt.utils.files
 import yaml
 
+log = logging.getLogger(__name__)
+
 
 def get_state_file_root(opts, env="base"):
     """
     Get the state file root
     """
     return pathlib.Path(opts.get("file_roots").get(env)[0])
 
@@ -38,15 +41,21 @@
 
 
 def generate_files(opts, minion, state, sls_name="default", env="base"):
     """
     Generate an sls file for the minion with given state contents
     """
     minion_state_root = get_minion_state_file_root(opts, minion, env=env)
-    minion_state_root.mkdir(parents=True, exist_ok=True)
+    try:
+        minion_state_root.mkdir(parents=True, exist_ok=True)
+    except PermissionError:
+        log.warning(
+            f"Unable to create directory {str(minion_state_root)}.  Check that the salt user has the correct permissions."
+        )
+        return False
 
     minion_state_file = minion_state_root / f"{sls_name}.sls"
 
     with salt.utils.files.fopen(minion_state_file, "w") as fp_:
         fp_.write(state)
 
     generate_init(opts, minion, env=env)
@@ -54,15 +63,21 @@
 
 
 def generate_init(opts, minion=None, env="base"):
     """
     Generate the init.sls for the minion or minions
     """
     minion_state_root = get_minion_state_file_root(opts, minion, env=env)
-    minion_state_root.mkdir(parents=True, exist_ok=True)
+    try:
+        minion_state_root.mkdir(parents=True, exist_ok=True)
+    except PermissionError:
+        log.warning(
+            f"Unable to create directory {str(minion_state_root)}.  Check that the salt user has the correct permissions."
+        )
+        return False
 
     minion_init_file = minion_state_root / "init.sls"
 
     include_files = []
     for file in minion_state_root.iterdir():
         if file.suffix == ".sls" and file.stem != "init":
             _file = file.stem
@@ -77,15 +92,21 @@
 
 
 def generate_pillar_init(opts, minion=None, env="base"):
     """
     Generate the init.sls for the minion or minions
     """
     minion_pillar_root = get_minion_pillar_file_root(opts, minion, env=env)
-    minion_pillar_root.mkdir(parents=True, exist_ok=True)
+    try:
+        minion_pillar_root.mkdir(parents=True, exist_ok=True)
+    except PermissionError:
+        log.warning(
+            f"Unable to create directory {str(minion_pillar_root)}.  Check that the salt user has the correct permissions."
+        )
+        return False
 
     minion_init_file = minion_pillar_root / "init.sls"
 
     include_files = []
     for file in minion_pillar_root.iterdir():
         if file.suffix == ".sls" and file.stem != "init":
             _file = file.stem
@@ -100,15 +121,21 @@
 
 
 def generate_pillars(opts, minion, pillar, sls_name="default", env="base"):
     """
     Generate pillar files for the minion to hold more sensitive information
     """
     minion_pillar_root = get_minion_pillar_file_root(opts, minion, env=env)
-    minion_pillar_root.mkdir(parents=True, exist_ok=True)
+    try:
+        minion_pillar_root.mkdir(parents=True, exist_ok=True)
+    except PermissionError:
+        log.warning(
+            f"Unable to create directory {str(minion_pillar_root)}.  Check that the salt user has the correct permissions."
+        )
+        return False
 
     minion_pillar_file = minion_pillar_root / f"{sls_name}.sls"
 
     with salt.utils.files.fopen(minion_pillar_file, "w") as fp_:
         fp_.write(pillar)
 
     generate_pillar_init(opts, minion, env=env)
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/PKG-INFO` & `saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltext.salt-describe
-Version: 0.1.1
+Version: 1.0.0
 Summary: Salt Describe Runner
 Home-page: http://github.com/saltstack//salt-describe/
 Author: Megan Wilhite, Gareth J. Greenaway
 Author-email: mwilhite@vmware.com, ggreenaway@vmware.com
 License: Apache Software License
 Project-URL: Source, http://github.com/saltstack//salt-describe/
 Project-URL: Tracker, http://github.com/saltstack//salt-describe/issues
```

### Comparing `saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/SOURCES.txt` & `saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/src/saltext.salt_describe.egg-info/requires.txt` & `saltext.salt-describe-1.0.0/src/saltext.salt_describe.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/integration/conftest.py` & `saltext.salt-describe-1.0.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe.py` & `saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_file.py` & `saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_file.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_firewalld.py` & `saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_firewalld.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_iptables.py` & `saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_iptables.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_service.py` & `saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_service.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_sysctl.py` & `saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_sysctl.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/integration/runners/test_salt_describe_user.py` & `saltext.salt-describe-1.0.0/tests/integration/runners/test_salt_describe_user.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe.py` & `saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_firewalld.py` & `saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_firewalld.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import logging
+from pathlib import PosixPath
+from pathlib import WindowsPath
 from unittest.mock import MagicMock
 from unittest.mock import patch
 
 import pytest
 import saltext.salt_describe.runners.salt_describe_firewalld as salt_describe_firewalld_runner
 import yaml
 
@@ -18,19 +20,17 @@
         salt_describe_firewalld_runner: {
             "__salt__": {"salt.execute": MagicMock()},
             "__opts__": {},
         },
     }
 
 
-def test_firewalld():
-    """
-    test describe.firewalld
-    """
-    firewalld_ret = {
+@pytest.fixture
+def firewalld_ret():
+    yield {
         "minion": {
             "public": {
                 "target": ["default"],
                 "icmp-block-inversion": ["no"],
                 "interfaces": [""],
                 "sources": [""],
                 "services": ["dhcpv6-client ssh"],
@@ -42,14 +42,19 @@
                 "source-ports": [""],
                 "icmp-blocks": [""],
                 "rich rules": [""],
             }
         }
     }
 
+
+def test_firewalld(firewalld_ret):
+    """
+    test describe.firewalld
+    """
     firewalld_sls_contents = {
         "add_firewalld_rule_0": {
             "firewalld.present": [{"name": "public"}, {"services": ["dhcpv6-client", "ssh"]}]
         }
     }
     firewalld_sls = yaml.dump(firewalld_sls_contents)
 
@@ -76,7 +81,22 @@
 
     with patch.dict(
         salt_describe_firewalld_runner.__salt__,
         {"salt.execute": MagicMock(return_value=firewalld_ret)},
     ):
         with patch.object(salt_describe_firewalld_runner, "generate_files") as generate_mock:
             ret = salt_describe_firewalld_runner.firewalld("minion")
+
+
+def test_firewalld_permissioned_denied(minion_opts, caplog, firewalld_ret, perm_denied_error_log):
+    with patch.dict(
+        salt_describe_firewalld_runner.__salt__,
+        {"salt.execute": MagicMock(return_value=firewalld_ret)},
+    ):
+        with patch.dict(salt_describe_firewalld_runner.__opts__, minion_opts):
+            with patch.object(PosixPath, "mkdir", side_effect=PermissionError), patch.object(
+                WindowsPath, "mkdir", side_effect=PermissionError
+            ):
+                with caplog.at_level(logging.WARNING):
+                    ret = salt_describe_firewalld_runner.firewalld("minion")
+                    assert not ret
+                    assert perm_denied_error_log in caplog.text
```

### Comparing `saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_host.py` & `saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_host.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import logging
+from pathlib import PosixPath
+from pathlib import WindowsPath
 from unittest.mock import MagicMock
 from unittest.mock import patch
 
 import pytest
 import saltext.salt_describe.runners.salt_describe_host as salt_describe_host_runner
 import yaml
 
@@ -58,7 +60,36 @@
         salt_describe_host_runner.__salt__, {"salt.execute": MagicMock(return_value=host_list)}
     ):
         with patch.object(salt_describe_host_runner, "generate_files") as generate_mock:
             assert "Generated SLS file locations" in salt_describe_host_runner.host("minion")
             generate_mock.assert_called_with(
                 {}, "minion", host_sls, sls_name="host", config_system="salt"
             )
+
+
+def test_host_permissioned_denied(minion_opts, caplog, perm_denied_error_log):
+    """
+    test describe.host
+    """
+    host_list = {
+        "minion": {
+            "comment-0": ["# Host addresses"],
+            "comment-1": ["# comment"],
+            "127.0.0.1": {"aliases": ["localhost"]},
+            "127.0.1.1": {"aliases": ["megan-precision5550"]},
+            "::1": {"aliases": ["localhost", "ip6-localhost", "ip6-loopback"]},
+            "ff02::1": {"aliases": ["ip6-allnodes"]},
+            "ff02::2": {"aliases": ["ip6-allrouters"]},
+        }
+    }
+
+    with patch.dict(
+        salt_describe_host_runner.__salt__, {"salt.execute": MagicMock(return_value=host_list)}
+    ):
+        with patch.dict(salt_describe_host_runner.__opts__, minion_opts):
+            with patch.object(PosixPath, "mkdir", side_effect=PermissionError), patch.object(
+                WindowsPath, "mkdir", side_effect=PermissionError
+            ):
+                with caplog.at_level(logging.WARNING):
+                    ret = salt_describe_host_runner.host("minion")
+                    assert not ret
+                    assert perm_denied_error_log in caplog.text
```

### Comparing `saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_pip.py` & `saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_pip.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import logging
+from pathlib import PosixPath
+from pathlib import WindowsPath
 from unittest.mock import MagicMock
 from unittest.mock import patch
 
 import pytest
 import saltext.salt_describe.runners.salt_describe_pip as salt_describe_pip_runner
 import yaml
 
@@ -81,7 +83,29 @@
             generate_mock.assert_called_with(
                 {},
                 "minion",
                 expected_yml_write,
                 sls_name="pip",
                 config_system="ansible",
             )
+
+
+def test_pip_permission_denied(minion_opts, caplog, perm_denied_error_log):
+    pip_list = {
+        "minion": [
+            "requests==0.1.2",
+            "salt==3004.1",
+            "argcomplete==2.3.4-5",
+        ],
+    }
+
+    with patch.dict(
+        salt_describe_pip_runner.__salt__, {"salt.execute": MagicMock(return_value=pip_list)}
+    ):
+        with patch.dict(salt_describe_pip_runner.__opts__, minion_opts):
+            with patch.object(PosixPath, "mkdir", side_effect=PermissionError), patch.object(
+                WindowsPath, "mkdir", side_effect=PermissionError
+            ):
+                with caplog.at_level(logging.WARNING):
+                    ret = salt_describe_pip_runner.pip("minion")
+                    assert not ret
+                    assert perm_denied_error_log in caplog.text
```

### Comparing `saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_pkgrepo.py` & `saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_pkgrepo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import logging
+from pathlib import PosixPath
+from pathlib import WindowsPath
 from unittest.mock import MagicMock
 from unittest.mock import patch
 
 import pytest
 import saltext.salt_describe.runners.salt_describe_pkgrepo as salt_describe_pkgrepo_runner
 import yaml
 
@@ -543,7 +545,74 @@
                 assert "Generated SLS file locations" in salt_describe_pkgrepo_runner.pkgrepo(
                     "minion"
                 )
                 minion_data_mock.assert_called_with("minion", {})
                 generate_mock.assert_called_with(
                     {}, "minion", debian_sls, sls_name="pkgrepo", config_system="salt"
                 )
+
+
+def test_pkgrepo_permission_denied(minion_opts, caplog, perm_denied_error_log):
+    pkgrepo_list = {
+        "minion": {
+            "baseos": {
+                "name": "CentOS Stream $releasever - BaseOS",
+                "metalink": "https://mirrors.centos.org/metalink?repo=centos-baseos-$stream&arch=$basearch&protocol=https,http",
+                "gpgkey": "file:///etc/pki/rpm-gpg/RPM-GPG-KEY-centosofficial",
+                "gpgcheck": "1",
+                "repo_gpgcheck": "0",
+                "metadata_expire": "6h",
+                "countme": "1",
+                "enabled": "1",
+                "file": "/etc/yum.repos.d/centos.repo",
+            },
+            "baseos-source": {
+                "name": "CentOS Stream $releasever - BaseOS - Source",
+                "metalink": "https://mirrors.centos.org/metalink?repo=centos-baseos-source-$stream&arch=source&protocol=https,http",
+                "gpgkey": "file:///etc/pki/rpm-gpg/RPM-GPG-KEY-centosofficial",
+                "gpgcheck": "1",
+                "repo_gpgcheck": "0",
+                "metadata_expire": "6h",
+                "enabled": "0",
+                "file": "/etc/yum.repos.d/centos.repo",
+            },
+            "appstream": {
+                "name": "CentOS Stream $releasever - AppStream",
+                "metalink": "https://mirrors.centos.org/metalink?repo=centos-appstream-$stream&arch=$basearch&protocol=https,http",
+                "gpgkey": "file:///etc/pki/rpm-gpg/RPM-GPG-KEY-centosofficial",
+                "gpgcheck": "1",
+                "repo_gpgcheck": "0",
+                "metadata_expire": "6h",
+                "countme": "1",
+                "enabled": "1",
+                "file": "/etc/yum.repos.d/centos.repo",
+            },
+            "appstream-source": {
+                "name": "CentOS Stream $releasever - AppStream - Source",
+                "metalink": "https://mirrors.centos.org/metalink?repo=centos-appstream-source-$stream&arch=source&protocol=https,http",
+                "gpgkey": "file:///etc/pki/rpm-gpg/RPM-GPG-KEY-centosofficial",
+                "gpgcheck": "1",
+                "repo_gpgcheck": "0",
+                "metadata_expire": "6h",
+                "enabled": "0",
+                "file": "/etc/yum.repos.d/centos.repo",
+            },
+        }
+    }
+
+    mock_minion_data = ({}, {"os_family": "RedHat"}, {})
+
+    with patch.dict(
+        salt_describe_pkgrepo_runner.__salt__,
+        {"salt.execute": MagicMock(return_value=pkgrepo_list)},
+    ):
+        with patch(
+            "salt.utils.minions.get_minion_data", MagicMock(return_value=mock_minion_data)
+        ) as minion_data_mock:
+            with patch.dict(salt_describe_pkgrepo_runner.__opts__, minion_opts):
+                with patch.object(PosixPath, "mkdir", side_effect=PermissionError), patch.object(
+                    WindowsPath, "mkdir", side_effect=PermissionError
+                ):
+                    with caplog.at_level(logging.WARNING):
+                        ret = salt_describe_pkgrepo_runner.pkgrepo("minion")
+                        assert not ret
+                        assert perm_denied_error_log in caplog.text
```

### Comparing `saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_service.py` & `saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import logging
 import sys
+from pathlib import PosixPath
+from pathlib import WindowsPath
 from unittest.mock import MagicMock
 from unittest.mock import patch
 
 import pytest
 import saltext.salt_describe.runners.salt_describe_service as salt_describe_service_runner
 import yaml
 
@@ -236,7 +238,48 @@
         with patch.object(salt_describe_service_runner, "generate_files") as generate_mock:
             assert "Generated SLS file locations" in salt_describe_service_runner.service(
                 "minion", config_system="chef"
             )
             generate_mock.assert_called_with(
                 {}, "minion", service_rb_contents, sls_name="service", config_system="chef"
             )
+
+
+def test_service_permission_denied(minion_opts, caplog, perm_denied_error_log):
+
+    if sys.platform.startswith("darwin"):
+        enabled_retval = {"minion": ["com.saltstack.salt.master", "com.saltstack.salt.minion"]}
+
+        list_retval = {
+            "minion": "PID\tStatus\tLabel\n358\t0\tcom.saltstack.salt.minion\n359\t0\tcom.saltstack.salt.master\n"
+        }
+
+        disabled_retval = {"minion": "'service.get_disabled' is not available."}
+
+        execute_retvals = [enabled_retval, disabled_retval, list_retval]
+    else:
+        enabled_retval = {"minion": ["salt-master", "salt-api"]}
+
+        status_retval = {
+            "minion": {
+                "salt-master": True,
+                "salt-minion": True,
+                "salt-api": False,
+                "random-service": True,
+            },
+        }
+        disabled_retval = {"minion": ["salt-minion"]}
+
+        execute_retvals = [enabled_retval, disabled_retval, status_retval]
+
+    with patch.dict(
+        salt_describe_service_runner.__salt__,
+        {"salt.execute": MagicMock(side_effect=execute_retvals)},
+    ):
+        with patch.dict(salt_describe_service_runner.__opts__, minion_opts):
+            with patch.object(PosixPath, "mkdir", side_effect=PermissionError), patch.object(
+                WindowsPath, "mkdir", side_effect=PermissionError
+            ):
+                with caplog.at_level(logging.WARNING):
+                    ret = salt_describe_service_runner.service("minion")
+                    assert not ret
+                    assert perm_denied_error_log in caplog.text
```

### Comparing `saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_timezone.py` & `saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_timezone.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import logging
+from pathlib import PosixPath
+from pathlib import WindowsPath
 from unittest.mock import MagicMock
 from unittest.mock import patch
 
 import pytest
 import saltext.salt_describe.runners.salt_describe_timezone as salt_describe_timezone_runner
 import yaml
 
@@ -38,7 +40,30 @@
         with patch.object(salt_describe_timezone_runner, "generate_files") as generate_mock:
             assert "Generated SLS file locations" in salt_describe_timezone_runner.timezone(
                 "minion"
             )
             generate_mock.assert_called_with(
                 {}, "minion", timezone_sls, sls_name="timezone", config_system="salt"
             )
+
+
+def test_timezone_permission_denied(minion_opts, caplog, perm_denied_error_log):
+    """
+    test describe.timezone
+    """
+    timezone_list = {"minion": "America/Los_Angeles"}
+
+    timezone_sls_contents = {"America/Los_Angeles": {"timezone.system": []}}
+    timezone_sls = yaml.dump(timezone_sls_contents)
+
+    with patch.dict(
+        salt_describe_timezone_runner.__salt__,
+        {"salt.execute": MagicMock(return_value=timezone_list)},
+    ):
+        with patch.dict(salt_describe_timezone_runner.__opts__, minion_opts):
+            with patch.object(PosixPath, "mkdir", side_effect=PermissionError), patch.object(
+                WindowsPath, "mkdir", side_effect=PermissionError
+            ):
+                with caplog.at_level(logging.WARNING):
+                    ret = salt_describe_timezone_runner.timezone("minion")
+                    assert not ret
+                    assert perm_denied_error_log in caplog.text
```

### Comparing `saltext.salt-describe-0.1.1/tests/unit/runners/test_salt_describe_user_group.py` & `saltext.salt-describe-1.0.0/tests/unit/runners/test_salt_describe_user_group.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import json
 import logging
+from pathlib import PosixPath
+from pathlib import WindowsPath
 from unittest.mock import MagicMock
 from unittest.mock import patch
 
 import pytest
 import saltext.salt_describe.runners.salt_describe_user as salt_describe_user_runner
 import yaml
 
@@ -284,7 +286,81 @@
                 )
                 generate_files_mock.assert_called_with(
                     {}, "minion", user_sls, sls_name="users", config_system="salt"
                 )
                 generate_pillars_mock.assert_called_with(
                     {}, "minion", user_pillar, sls_name="users"
                 )
+
+
+def test_group_permission_denied(minion_opts, caplog, perm_denied_error_log):
+    group_getent = {
+        "minion": [
+            {"gid": 4, "members": ["syslog", "whytewolf"], "name": "adm", "passwd": "x"},
+            {"gid": 0, "members": [], "name": "root", "passwd": "x"},
+        ]
+    }
+
+    with patch.dict(
+        salt_describe_user_runner.__salt__, {"salt.execute": MagicMock(return_value=group_getent)}
+    ):
+        with patch.dict(salt_describe_user_runner.__opts__, minion_opts):
+            with patch.object(PosixPath, "mkdir", side_effect=PermissionError), patch.object(
+                WindowsPath, "mkdir", side_effect=PermissionError
+            ):
+                with caplog.at_level(logging.WARNING):
+                    ret = salt_describe_user_runner.group("minion")
+                    assert not ret
+                    assert perm_denied_error_log in caplog.text
+
+
+def test_user_permission_denied(minion_opts, caplog, perm_denied_error_log):
+    user_getent = {
+        "minion": [
+            {
+                "name": "testuser",
+                "uid": 1000,
+                "gid": 1000,
+                "groups": ["adm"],
+                "home": "/home/testuser",
+                "passwd": "x",
+                "shell": "/usr/bin/zsh",
+                "fullname": "",
+                "homephone": "",
+                "other": "",
+                "roomnumber": "",
+                "workphone": "",
+            }
+        ]
+    }
+
+    user_shadow = {
+        "minion": {
+            "expire": -1,
+            "inact": -1,
+            "lstchg": 19103,
+            "max": 99999,
+            "min": 0,
+            "name": "testuser",
+            "passwd": "$5$k69zJBp1LxA3q8az$XKEp1knAex0j.xoi/sdU4XllHpZ0JzYYRfASKGl6qZA",
+            "warn": 7,
+        }
+    }
+
+    fileexists = {"minion": True}
+
+    user_pillar_contents = {
+        "users": {"testuser": "$5$k69zJBp1LxA3q8az$XKEp1knAex0j.xoi/sdU4XllHpZ0JzYYRfASKGl6qZA"},
+    }
+
+    with patch.dict(
+        salt_describe_user_runner.__salt__,
+        {"salt.execute": MagicMock(side_effect=[user_getent, user_shadow, fileexists])},
+    ):
+        with patch.dict(salt_describe_user_runner.__opts__, minion_opts):
+            with patch.object(PosixPath, "mkdir", side_effect=PermissionError), patch.object(
+                WindowsPath, "mkdir", side_effect=PermissionError
+            ):
+                with caplog.at_level(logging.WARNING):
+                    ret = salt_describe_user_runner.user("minion")
+                    assert not ret
+                    assert perm_denied_error_log in caplog.text
```

### Comparing `saltext.salt-describe-0.1.1/tests/unit/utils/test_ansible_describe.py` & `saltext.salt-describe-1.0.0/tests/unit/utils/test_ansible_describe.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/unit/utils/test_init.py` & `saltext.salt-describe-1.0.0/tests/unit/utils/test_init.py`

 * *Files identical despite different names*

### Comparing `saltext.salt-describe-0.1.1/tests/unit/utils/test_salt_describe.py` & `saltext.salt-describe-1.0.0/tests/unit/utils/test_salt_describe.py`

 * *Files identical despite different names*

