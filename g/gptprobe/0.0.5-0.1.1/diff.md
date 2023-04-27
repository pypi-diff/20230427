# Comparing `tmp/gptprobe-0.0.5.tar.gz` & `tmp/gptprobe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptprobe-0.0.5.tar", last modified: Wed Apr 26 16:14:31 2023, max compression
+gzip compressed data, was "gptprobe-0.1.1.tar", last modified: Thu Apr 27 17:14:31 2023, max compression
```

## Comparing `gptprobe-0.0.5.tar` & `gptprobe-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:14:31.059381 gptprobe-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 16:13:57.000000 gptprobe-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-26 16:14:31.059381 gptprobe-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-26 16:13:57.000000 gptprobe-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:14:31.055380 gptprobe-0.0.5/gptprobe/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/goodtogo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:14:31.055380 gptprobe-0.0.5/gptprobe/openaiwrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/openaiwrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/openaiwrappers/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/openaiwrappers/opendefaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:14:31.059381 gptprobe-0.0.5/gptprobe/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/parsing/askfornumericdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/parsing/parsedictrobustly.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/public_setenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:14:31.059381 gptprobe-0.0.5/gptprobe/utilfortests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/utilfortests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 16:13:57.000000 gptprobe-0.0.5/gptprobe/utilfortests/equivalence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:14:31.055380 gptprobe-0.0.5/gptprobe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-26 16:14:30.000000 gptprobe-0.0.5/gptprobe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 16:14:31.000000 gptprobe-0.0.5/gptprobe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:14:30.000000 gptprobe-0.0.5/gptprobe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 16:14:30.000000 gptprobe-0.0.5/gptprobe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 16:14:30.000000 gptprobe-0.0.5/gptprobe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 16:14:30.000000 gptprobe-0.0.5/gptprobe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:14:31.059381 gptprobe-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 16:13:57.000000 gptprobe-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.994270 gptprobe-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 17:14:02.000000 gptprobe-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 17:14:30.994270 gptprobe-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-27 17:14:02.000000 gptprobe-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.986270 gptprobe-0.1.1/gptprobe/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.994270 gptprobe-0.1.1/gptprobe/askfor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/clarification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/clarificationfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dictfrompoorlyformattedtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dictfromquestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dictfromquestionwithratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dictfromtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/dicttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/flaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/flawfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/ratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/ratificationfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/rephrasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/rephrasingfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/textfrompoorlyformatteddicttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/askfor/textfromquestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/keysinenviron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/public_setenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.994270 gptprobe-0.1.1/gptprobe/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/customtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/enginedefaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-27 17:14:02.000000 gptprobe-0.1.1/gptprobe/utils/parsedictrobustly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:14:30.990270 gptprobe-0.1.1/gptprobe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 17:14:30.000000 gptprobe-0.1.1/gptprobe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:14:30.994270 gptprobe-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-27 17:14:02.000000 gptprobe-0.1.1/setup.py
```

### Comparing `gptprobe-0.0.5/LICENSE` & `gptprobe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gptprobe-0.0.5/setup.py` & `gptprobe-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="gptprobe",
-    version="0.0.5",
+    version="0.1.1",
     description="Probing chatgpt",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/gptprobe/gptprobe",
     author="gptprobe",
     author_email="pcotton@intechinvestments.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
-    packages=["gptprobe","gptprobe.openaiwrappers","gptprobe.utilfortests","gptprobe.parsing"],
+    packages=["gptprobe",
+              "gptprobe.utils",
+              "gptprobe.askfor"],
     test_suite='pytest',
     tests_require=['pytest'],
     include_package_data=True,
     install_requires=["numpy","pandas","getjson","openai"],
     entry_points={
         "console_scripts": [
             "gptprobe=gptprobe.__main__:main",
```

