# Comparing `tmp/innerverz_package-0.0.1.tar.gz` & `tmp/innerverz_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz_package-0.0.1.tar", last modified: Thu Apr 27 06:42:30 2023, max compression
+gzip compressed data, was "innerverz_package-0.0.2.tar", last modified: Thu Apr 27 07:09:55 2023, max compression
```

## Comparing `innerverz_package-0.0.1.tar` & `innerverz_package-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 06:42:30.651495 innerverz_package-0.0.1/
--rw-r--r--   0 compu     (1000) compu     (1000)     1073 2023-01-27 06:12:58.000000 innerverz_package-0.0.1/LICENSE.txt
--rw-rw-r--   0 compu     (1000) compu     (1000)      213 2023-04-27 06:42:30.651495 innerverz_package-0.0.1/PKG-INFO
--rw-r--r--   0 compu     (1000) compu     (1000)       10 2023-01-27 06:13:12.000000 innerverz_package-0.0.1/README.md
-drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 06:42:30.651495 innerverz_package-0.0.1/innerverz_package.egg-info/
--rw-rw-r--   0 compu     (1000) compu     (1000)      213 2023-04-27 06:42:30.000000 innerverz_package-0.0.1/innerverz_package.egg-info/PKG-INFO
--rw-rw-r--   0 compu     (1000) compu     (1000)      259 2023-04-27 06:42:30.000000 innerverz_package-0.0.1/innerverz_package.egg-info/SOURCES.txt
--rw-rw-r--   0 compu     (1000) compu     (1000)        1 2023-04-27 06:42:30.000000 innerverz_package-0.0.1/innerverz_package.egg-info/dependency_links.txt
--rw-rw-r--   0 compu     (1000) compu     (1000)       50 2023-04-27 06:42:30.000000 innerverz_package-0.0.1/innerverz_package.egg-info/requires.txt
--rw-rw-r--   0 compu     (1000) compu     (1000)        1 2023-04-27 06:42:30.000000 innerverz_package-0.0.1/innerverz_package.egg-info/top_level.txt
--rw-r--r--   0 compu     (1000) compu     (1000)       89 2023-01-27 04:47:26.000000 innerverz_package-0.0.1/pyproject.toml
--rw-r--r--   0 compu     (1000) compu     (1000)       38 2023-04-27 06:42:30.651495 innerverz_package-0.0.1/setup.cfg
--rw-r--r--   0 compu     (1000) compu     (1000)      789 2023-04-27 06:42:17.000000 innerverz_package-0.0.1/setup.py
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 07:09:55.313275 innerverz_package-0.0.2/
+-rw-r--r--   0 compu     (1000) compu     (1000)     1073 2023-01-27 06:12:58.000000 innerverz_package-0.0.2/LICENSE.txt
+-rw-rw-r--   0 compu     (1000) compu     (1000)      213 2023-04-27 07:09:55.313275 innerverz_package-0.0.2/PKG-INFO
+-rw-r--r--   0 compu     (1000) compu     (1000)       10 2023-01-27 06:13:12.000000 innerverz_package-0.0.2/README.md
+drwxrwxr-x   0 compu     (1000) compu     (1000)        0 2023-04-27 07:09:55.313275 innerverz_package-0.0.2/innerverz_package.egg-info/
+-rw-rw-r--   0 compu     (1000) compu     (1000)      213 2023-04-27 07:09:55.000000 innerverz_package-0.0.2/innerverz_package.egg-info/PKG-INFO
+-rw-rw-r--   0 compu     (1000) compu     (1000)      259 2023-04-27 07:09:55.000000 innerverz_package-0.0.2/innerverz_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 compu     (1000) compu     (1000)        1 2023-04-27 07:09:55.000000 innerverz_package-0.0.2/innerverz_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 compu     (1000) compu     (1000)       50 2023-04-27 07:09:55.000000 innerverz_package-0.0.2/innerverz_package.egg-info/requires.txt
+-rw-rw-r--   0 compu     (1000) compu     (1000)        1 2023-04-27 07:09:55.000000 innerverz_package-0.0.2/innerverz_package.egg-info/top_level.txt
+-rw-r--r--   0 compu     (1000) compu     (1000)       89 2023-01-27 04:47:26.000000 innerverz_package-0.0.2/pyproject.toml
+-rw-r--r--   0 compu     (1000) compu     (1000)       38 2023-04-27 07:09:55.313275 innerverz_package-0.0.2/setup.cfg
+-rw-r--r--   0 compu     (1000) compu     (1000)      789 2023-04-27 07:09:22.000000 innerverz_package-0.0.2/setup.py
```

### Comparing `innerverz_package-0.0.1/LICENSE.txt` & `innerverz_package-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz_package-0.0.1/setup.py` & `innerverz_package-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz_package",
-    version="0.0.1",
+    version="0.0.2",
     author="Innerverz-by.JJY",
     author_email="pensee0.0a@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

