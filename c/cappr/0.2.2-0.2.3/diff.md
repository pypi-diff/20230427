# Comparing `tmp/cappr-0.2.2.tar.gz` & `tmp/cappr-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cappr-0.2.2.tar", last modified: Wed Apr 19 02:05:05 2023, max compression
+gzip compressed data, was "cappr-0.2.3.tar", last modified: Thu Apr 27 21:27:34 2023, max compression
```

## Comparing `cappr-0.2.2.tar` & `cappr-0.2.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.966942 cappr-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.970942 cappr-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-19 02:04:53.000000 cappr-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-19 02:04:53.000000 cappr-0.2.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 02:04:53.000000 cappr-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-19 02:04:53.000000 cappr-0.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 02:04:53.000000 cappr-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-04-19 02:05:05.982943 cappr-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-04-19 02:04:53.000000 cappr-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.970942 cappr-0.2.2/demos/
--rw-r--r--   0 runner    (1001) docker     (123)  2760040 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/computational_analysis.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.974943 cappr-0.2.2/demos/raft/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/ade.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/b77.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/nis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/ose.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/over.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/sot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/sri.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/tai.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/tc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/teh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/raft/tos.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.974943 cappr-0.2.2/demos/superglue/
--rw-r--r--   0 runner    (1001) docker     (123)    64027 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/superglue/copa.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42865 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/superglue/wsc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-19 02:04:53.000000 cappr-0.2.2/demos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.974943 cappr-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/1_is_for_me.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/2_motivation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/3_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/4_user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/5_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/6_computational_performance.rst
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/7_future_research.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/_static/github-mark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/docs/source/_static/scaling_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    53692 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/_static/scaling_classes/batch_size_32.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.huggingface.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.huggingface.classify_no_cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.huggingface.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.openai.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.openai.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.openai.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.utils.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/cappr.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/related_work.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/research.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 02:04:53.000000 cappr-0.2.2/docs/source/walkthrough.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 02:04:53.000000 cappr-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 02:05:05.982943 cappr-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-19 02:04:53.000000 cappr-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.966942 cappr-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/huggingface/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34123 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/huggingface/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/huggingface/classify_no_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23104 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/openai/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/utils/_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-04-19 02:04:53.000000 cappr-0.2.2/src/cappr/utils/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.978943 cappr-0.2.2/src/cappr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 02:05:05.000000 cappr-0.2.2/src/cappr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/tests/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/huggingface/test_huggingface_classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/openai/test_openai_classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:05:05.982943 cappr-0.2.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/utils/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-19 02:04:53.000000 cappr-0.2.2/tests/utils/test_utils_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.303793 cappr-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.287793 cappr-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.287793 cappr-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-27 21:27:19.000000 cappr-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-27 21:27:19.000000 cappr-0.2.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 21:27:19.000000 cappr-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-27 21:27:19.000000 cappr-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 21:27:19.000000 cappr-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-04-27 21:27:34.299793 cappr-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-04-27 21:27:19.000000 cappr-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.291793 cappr-0.2.3/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)  2760040 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/computational_analysis.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.295793 cappr-0.2.3/demos/raft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/ade.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/b77.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/nis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/ose.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/over.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/sot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/sri.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/tai.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/tc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/teh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/raft/tos.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.295793 cappr-0.2.3/demos/superglue/
+-rw-r--r--   0 runner    (1001) docker     (123)    64027 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/superglue/copa.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42865 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/superglue/wsc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-27 21:27:20.000000 cappr-0.2.3/demos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.295793 cappr-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/1_is_for_me.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/2_motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/3_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/4_user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/5_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/6_computational_performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/7_future_research.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/_static/github-mark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/docs/source/_static/scaling_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    53692 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/_static/scaling_classes/batch_size_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.huggingface.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.huggingface.classify_no_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.huggingface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.openai.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.openai.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.openai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.utils.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/cappr.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/related_work.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/research.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-27 21:27:20.000000 cappr-0.2.3/docs/source/walkthrough.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-27 21:27:20.000000 cappr-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:27:34.303793 cappr-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-27 21:27:20.000000 cappr-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.287793 cappr-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/huggingface/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34123 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/huggingface/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/huggingface/classify_no_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25167 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/openai/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/utils/_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-04-27 21:27:20.000000 cappr-0.2.3/src/cappr/utils/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/src/cappr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 21:27:34.000000 cappr-0.2.3/src/cappr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/tests/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/huggingface/test_huggingface_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/openai/test_openai_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:27:34.299793 cappr-0.2.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/utils/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-27 21:27:20.000000 cappr-0.2.3/tests/utils/test_utils_classify.py
```

### Comparing `cappr-0.2.2/.github/workflows/python-publish.yml` & `cappr-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/.github/workflows/test.yml` & `cappr-0.2.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/LICENSE` & `cappr-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/PKG-INFO` & `cappr-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cappr
-Version: 0.2.2
+Version: 0.2.3
 Summary: Zero-shot text classification using autoregressive language models.
 Home-page: https://github.com/kddubey/cappr/
 Author-email: kushdubey63@gmail.com
 License: Apache License 2.0
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: hf
@@ -28,14 +28,15 @@
 > **C**ompletion<br>
   **A**fter<br>
   **P**rompt<br>
   **Pr**obability<br>
 
 The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
 
+
 ## Usage
 
 <details>
 <summary>Use a model from the OpenAI API</summary>
 
 Specifically, this model must be compatible with the
 [/v1/completions](https://platform.openai.com/docs/models/model-endpoint-compatibility)
@@ -221,15 +222,15 @@
 
 ```
 python -m pip install cappr[hf]
 ```
 </details>
 
 <details>
-<summary>(Optional) Set up to run demos</summary>
+<summary>(Optional) Install requirements for running demos</summary>
 
 ```
 python -m pip install cappr[demos]
 ```
 </details>
 
 
@@ -276,19 +277,21 @@
 
 ## Results
 
 <details>
 <summary>
 Statistical performance
 </summary>
-Performs ok based on 2 datasets, when compared to classification via sampling (CVS).
-I need to run it on more ofc. Will update
 
-  * [`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
-  * [`demos/superglue/wsc.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb)
+Not too shabby. TODO: summary table comparing CVS vs. CAPPr vs. few-shot methods like
+SetFit and PET.
+
+[2 SuperGLUE datasets](https://github.com/kddubey/cappr/blob/main/demos/superglue)
+
+[RAFT zero-shot training sets](https://github.com/kddubey/cappr/blob/main/demos/raft)
 </details>
 
 
 <details>
 <summary>
 Computational performance
 </summary>
@@ -322,21 +325,23 @@
 ## Related work
 
 While [benchmarking this
 method](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb) on the
 Winograd Schema Challenge, I found that [this paper](https://arxiv.org/abs/1806.02847)
 is very similar:
 
-> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv preprint arXiv:1806.02847 (2018).
+> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv
+> preprint arXiv:1806.02847 (2018).
 
 [PET with multiple masks](https://arxiv.org/abs/2009.07118) also aggregates token
 probabilities to do prompt-completion classification, but these probabilities are
 assumed to come from masked language models like BERT.
 
-> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
+> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language
+> models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
 
 
 ## Contributing
 
 TODO
 
 
@@ -396,15 +401,14 @@
 - [ ] HuggingFace `transformers.AutoModelForCausalLM`
   - [x] Optimize backend to enable greater scaling wrt # completions/classes
   - [x] Get it working on single-GPU, check that it's faster than sampling assuming
   batching
     - [ ] Get to the bottom of why it's slower w/o batching
   - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
   think
-  - [ ] Support few-shot prompt caching. Consider a fit-predict interface (**)
   - [ ] Consider batchifying the completions again, since they technically don't go in
   batches of `batch_size`; the actual batch size is the sum of the number of completions
   corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
   are usually half as long. But it should be configurable at the very least.
   - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
   - [ ] Support [Inference
     Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
```

### Comparing `cappr-0.2.2/README.md` & `cappr-0.2.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 > **C**ompletion<br>
   **A**fter<br>
   **P**rompt<br>
   **Pr**obability<br>
 
 The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
 
+
 ## Usage
 
 <details>
 <summary>Use a model from the OpenAI API</summary>
 
 Specifically, this model must be compatible with the
 [/v1/completions](https://platform.openai.com/docs/models/model-endpoint-compatibility)
@@ -207,15 +208,15 @@
 
 ```
 python -m pip install cappr[hf]
 ```
 </details>
 
 <details>
-<summary>(Optional) Set up to run demos</summary>
+<summary>(Optional) Install requirements for running demos</summary>
 
 ```
 python -m pip install cappr[demos]
 ```
 </details>
 
 
@@ -262,19 +263,21 @@
 
 ## Results
 
 <details>
 <summary>
 Statistical performance
 </summary>
-Performs ok based on 2 datasets, when compared to classification via sampling (CVS).
-I need to run it on more ofc. Will update
 
-  * [`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
-  * [`demos/superglue/wsc.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb)
+Not too shabby. TODO: summary table comparing CVS vs. CAPPr vs. few-shot methods like
+SetFit and PET.
+
+[2 SuperGLUE datasets](https://github.com/kddubey/cappr/blob/main/demos/superglue)
+
+[RAFT zero-shot training sets](https://github.com/kddubey/cappr/blob/main/demos/raft)
 </details>
 
 
 <details>
 <summary>
 Computational performance
 </summary>
@@ -308,21 +311,23 @@
 ## Related work
 
 While [benchmarking this
 method](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb) on the
 Winograd Schema Challenge, I found that [this paper](https://arxiv.org/abs/1806.02847)
 is very similar:
 
-> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv preprint arXiv:1806.02847 (2018).
+> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv
+> preprint arXiv:1806.02847 (2018).
 
 [PET with multiple masks](https://arxiv.org/abs/2009.07118) also aggregates token
 probabilities to do prompt-completion classification, but these probabilities are
 assumed to come from masked language models like BERT.
 
-> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
+> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language
+> models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
 
 
 ## Contributing
 
 TODO
 
 
@@ -382,15 +387,14 @@
 - [ ] HuggingFace `transformers.AutoModelForCausalLM`
   - [x] Optimize backend to enable greater scaling wrt # completions/classes
   - [x] Get it working on single-GPU, check that it's faster than sampling assuming
   batching
     - [ ] Get to the bottom of why it's slower w/o batching
   - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
   think
-  - [ ] Support few-shot prompt caching. Consider a fit-predict interface (**)
   - [ ] Consider batchifying the completions again, since they technically don't go in
   batches of `batch_size`; the actual batch size is the sum of the number of completions
   corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
   are usually half as long. But it should be configurable at the very least.
   - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
   - [ ] Support [Inference
     Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
```

### Comparing `cappr-0.2.2/demos/computational_analysis.ipynb` & `cappr-0.2.3/demos/computational_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/README.md` & `cappr-0.2.3/demos/raft/README.md`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/ade.ipynb` & `cappr-0.2.3/demos/raft/ade.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/b77.ipynb` & `cappr-0.2.3/demos/raft/b77.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/nis.ipynb` & `cappr-0.2.3/demos/raft/nis.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/ose.ipynb` & `cappr-0.2.3/demos/raft/ose.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/over.ipynb` & `cappr-0.2.3/demos/raft/over.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/sot.ipynb` & `cappr-0.2.3/demos/raft/sot.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/sri.ipynb` & `cappr-0.2.3/demos/raft/sri.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/tai.ipynb` & `cappr-0.2.3/demos/raft/tai.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/tc.ipynb` & `cappr-0.2.3/demos/raft/tc.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/teh.ipynb` & `cappr-0.2.3/demos/raft/teh.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/raft/tos.ipynb` & `cappr-0.2.3/demos/raft/tos.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/superglue/copa.ipynb` & `cappr-0.2.3/demos/superglue/copa.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/superglue/wsc.ipynb` & `cappr-0.2.3/demos/superglue/wsc.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/demos/utils.py` & `cappr-0.2.3/demos/utils.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/docs/Makefile` & `cappr-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/docs/make.bat` & `cappr-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/docs/source/1_is_for_me.rst` & `cappr-0.2.3/docs/source/1_is_for_me.rst`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 #. `Plain old BERT embeddings
    <https://huggingface.co/transformers/v3.3.1/training.html>`_.
 
 You should also consider how "subtle" the association is between your input texts and
 their labels. Few-shot methods may be able to pick up more subtle or internally
 specified associations between texts and their labels. Zero-shot methods using LLMs may
-be better at tasks which require less-subtle and more factual knowledge.\ [#]_
+be better at tasks which require more factual knowledge.\ [#]_
 
 
 Footnotes
 ~~~~~~~~~
 
 .. [#] Some quick-and-dirty rationale for this guidance: a Wald 68% confidence interval
    for the expected error rate of a binary classifier—which is estimated to be 80%
@@ -44,8 +44,10 @@
    examples. That's quite wide. Ideally, for zero-shot problems, you still have 200 or
    so labeled examples. I like to separate labeled examples into a set of 50 for
    training and 150 for test. Those 50 are used to estimate a prior, select a prompt
    format, and select an LM. The other 150 are only used for evaluation.
 
 .. [#] You may be interested in the Real-World Few-Shot Text Classification (RAFT)
    benchmark. See the leaderboard `here
-   <https://huggingface.co/spaces/ought/raft-leaderboard>`_.
+   <https://huggingface.co/spaces/ought/raft-leaderboard>`_, and CAPPr's zero-shot
+   performance on the RAFT training set `here
+   <https://github.com/kddubey/cappr/blob/main/demos/raft>`_.
```

### Comparing `cappr-0.2.2/docs/source/2_motivation.rst` & `cappr-0.2.3/docs/source/2_motivation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 Problem
 -------
 
 There are many ways to do zero-shot text classification. The one that this package is
 competing against is what I'll call **classification via sampling (CVS)**. This method
-is pretty common for large language models (LLMs) like GPT-2+, PaLM, etc. CVS is
+is pretty common for large language models (LLMs) like GPT-3+, PaLM, etc. CVS is
 motiviated by the fact that LLMs are great at generating text. It's currently the method
 which the `OpenAI guide on classification`_ covers.
 
 .. _OpenAI guide on classification: https://platform.openai.com/docs/guides/completion/classification
 
 To make CVS more concrete, let's work through an example.
 
@@ -70,41 +70,36 @@
 Herein lies the problem. Because if you've made it this far, then I'm sure you know that
 implementing ``post_process`` can be challenging, as the ``completion`` is sampled from
 the space of all possible sequences of tokens. This means you'll likely have to deal
 with the cases where:
 
 - The ``completion`` includes multiple plausible classes from ``class_names``
 
-- The ``completion`` starts with a bit of fluff before giving an answer in
-  ``class_names``
+- The ``completion`` includes a bit of fluff
 
 - The ``completion``\ 's word casing is different than the one used in ``class_names``,
   or it's spelled or phrased slightly differently. (These discrepancies typically only
   occur for domain-specific text.)
 
-- GPT phrases its uncertainty in three different ways.
+- The LM phrases its uncertainty in three different ways.
 
 The OpenAI community knows that this can be challenging, so `they suggest`_ that you
 modify your code in at least 1 of 2 ways:
 
-#. Transform multi-token class names into a single token. Or, if it works, (as done in
-   CAPPr's `COPA demo`_) point to multi-token class names using a single token.
+#. Point to multi-token class names using a single token—like a multiple choice question
 
-#. Finetune a model so that it learns the mapping to the single tokens.
+#. Transform multi-token class names into a single token, and finetune a model so that
+   it learns the mapping to the single tokens.
 
 .. _they suggest: https://docs.google.com/document/d/1rqj7dkuvl7Byd5KQPUJRxc19BJt8wo0yHNwK84KfU3Q/edit
 
-.. _COPA demo: https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb
-
-These are nontrivial modifications. The single-token transformation could sacrifice
-meaningful semantics in multi-token class names. And in my experience, single-token
-references sacrifice performance when you have quite a few classes, or some
-``class_names`` start with numbers. Finetuning is expensive, requires that you spend
-much of your dataset just to learn the mapping to classes, and goes against the spirit
-of GPT being great at zero-shot tasks.
+These can be nontrivial modifications. Single-token references can sacrifice performance
+when you have quite a few classes, as it's not a typical instruction format.
+Single-token transformations sacrifice useful semantics, and finetuning usually requires
+spending too much money and too much of your data.
 
 **The fact is: you can endlessley accomodate CVS, but you'll still have to write custom
 code to post-process its arbitrary outputs.** Fundamentally, sampling is not a clean
 solution to a classification problem.
 
 
 Solution
@@ -112,17 +107,17 @@
 
 With CAPPr's ``predict`` interface, your job starts and stops at writing up your
 classification task as a ``{prompt}{end_of_prompt}{completion}`` string.
 
 That being said, let's now run CAPPr on that product review classification task. Also,
 let's:
 
-- trivially incorporate a prior (this is optional)
+- trivially incorporate a prior (optional)
 
-- predict a probability distribution over classes, not just the class (also optional)
+- predict a probability distribution over classes (optional)
 
 - replace the expensive ``text-davinci-003`` model call with a ``text-curie-001`` one
 
   - CVS with ``text-curie-001`` typically does not work well for slightly complicated
     tasks, e.g., run that CVS code above with ``model='text-curie-001'``\ .
 
 .. code:: python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cappr-0.2.2/docs/source/3_installation.rst` & `cappr-0.2.3/docs/source/3_installation.rst`

 * *Files 16% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 
 (Optional) Install requirements for HuggingFace models:
 
 ::
 
    python -m pip install cappr[hf]
 
-(Optional) Set up to run demos:
+(Optional) Install requirements for running demos:
 
 ::
 
    python -m pip install cappr[demos]
```

### Comparing `cappr-0.2.2/docs/source/4_user_guide.rst` & `cappr-0.2.3/docs/source/4_user_guide.rst`

 * *Files 7% similar despite different names*

```diff
@@ -12,55 +12,49 @@
 components:
 
 .. code:: python
 
    {prompt}{end_of_prompt}{completion}
 
 The text you want to classify should appear in the ``prompt``. One of the classes which
-the text could belong to should appear in the ``completion``. These are not hard rules,
-but rather guidelines. For example, the `demo for the Winograd Schema Challenge`_ flips
-the roles of the ``prompt`` and ``completion``. (Just don't use the prior keyword
-argument in that case.)
+the text could belong to should appear in the ``completion``. These are not hard rules.
+For example, the `demo for the Winograd Schema Challenge`_ flips the roles of the
+``prompt`` and ``completion``. (Just don't use the prior keyword argument in that case.)
 
 .. _demo for the Winograd Schema Challenge: https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb
 
 One rule is that the ``completion`` text should flow naturally after
 ``{prompt}{end_of_prompt}``. So pay close attention to the use of white spaces,
 newlines, and word casing. :mod:`cappr.openai.classify` does not do any string
 processing for you: **it just concatenates the three strings and sends it**!
 
-And yes, you'll still have to do “prompt engineering”. It's mostly a matter of trial and
+And yes, you'll still have to do "prompt engineering". It's mostly a matter of trial and
 error. Here's an `external guide`_ if you'd like to survey research in this field.\ [#]_
 
-.. warning:: :mod:`cappr.huggingface.classify` currently requires that ``end_of_prompt``
-             is a whitespace.
-
 .. warning:: Currently, :mod:`cappr.openai.classify` must repeat the ``prompt`` for
              however many completions there are. So if your prompt is long and your
-             completions, you may end up spending much more with CAPPr.
-             :mod:`cappr.huggingface.classify` does not have to repeat the prompt
-             because the HuggingFace backend is open source.
+             completions are short, you may end up spending much more with CAPPr.
+             (:mod:`cappr.huggingface.classify` does not have to repeat the prompt
+             because it caches it.)
 
 .. _external guide: https://lilianweng.github.io/posts/2023-03-15-prompt-engineering/
 
 
 Select a language model
 -----------------------
 
-Smaller, non-instruction-trained language models may work fine for non-instruction
-prompt formats. For OpenAI models, there's some rough guidance `here
+CAPPr typically requires larger language models, as it's a zero-shot method. For OpenAI
+models, there's some rough guidance `here
 <https://platform.openai.com/docs/models/overview>`_. Other than that, selecting a
 language model is almost entirely a process of trial and error. It should be easy to
 plug and play though.
 
 Should I use OpenAI or HuggingFace models?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Short answer: try out both.
-
 Currently, OpenAI models perform better. But I'll try to document competitive,
 instruction-trained LMs which are hosted on HuggingFace as more are released. For now,
 you'll need access to beefier hardware to run them, as :mod:`cappr.huggingface`
 currently locally loads HuggingFace models.
 
 .. warning:: Some of OpenAI's `GPT-3.5+ models`_ currently don't return token
    probabilities, so they currently can't be used by CAPPr. I hope this changes soon.
@@ -70,38 +64,36 @@
 .. note:: `HuggingFace Inference Endpoints`_ are not yet supported by this package.
 .. _HuggingFace Inference Endpoints: https://huggingface.co/docs/inference-endpoints/index
 
 
 (Optional) Supply a prior
 -------------------------
 
-A prior is a marginal probability distribution over the classes in your
-classification problem. It nudges language model probabilities towards
-the conditional class probabilities which we need to make good
-decisions.
+A prior is a marginal probability distribution over the classes in your classification
+problem. It nudges language model probabilities towards the conditional class
+probabilities which are needed to make optimal predictions.
 
-If you have a handful of labeled examples, then you may simply compute
-the fraction of examples belonging to each class, e.g.,
+If you have a handful of labeled examples for each possible class, then you may simply
+compute the fraction of examples belonging to each class, e.g.,
 
 .. code:: python
 
    # class_labels[i] is the index of the class which example i belongs to
    class_labels = [0, 0, 0, 1, 1, 1, 1, 1, 2]
 
-   # prior_estimate[k] is the observed fraction of examples which belong to class k
-   prior_estimate = [3/9, 5/9, 1/9]
+   # prior[k] is the observed fraction of examples which belong to class k
+   prior = [3/9, 5/9, 1/9]
+
+There are better but slighly more complicated ways to estimate a prior, e.g., `additive
+smoothing <https://en.wikipedia.org/wiki/Additive_smoothing>`_.
 
-There are better but slighly more complicated ways to estimate a prior,
-e.g., `additive
-smoothing <https://en.wikipedia.org/wiki/Additive_smoothing>`__.
-
-You may also simply guess a prior if you have some domain knowledge. If
-you have absolutely no idea what a reasonable prior could be, then you
-may leave out the ``prior`` keyword argument for this package's ``predict`` and
-``predict_proba`` functions. In this case, a uniform prior is assumed.
+You may also simply guess a prior if you have some domain knowledge. If you have
+absolutely no idea what a reasonable prior could be, then you may leave out the
+``prior`` keyword argument for this package's ``predict`` and ``predict_proba``
+functions. In this case, a uniform prior is assumed.
 
 
 References
 ----------
 
 .. [#] Weng, Lilian. (Mar 2023). Prompt Engineering. Lil'Log.
    https://lilianweng.github.io/posts/2023-03-15-prompt-engineering/.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cappr-0.2.2/docs/source/6_computational_performance.rst` & `cappr-0.2.3/docs/source/6_computational_performance.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/docs/source/7_future_research.rst` & `cappr-0.2.3/docs/source/7_future_research.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/docs/source/_static/github-mark.png` & `cappr-0.2.3/docs/source/_static/github-mark.png`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/docs/source/_static/scaling_classes/batch_size_32.png` & `cappr-0.2.3/docs/source/_static/scaling_classes/batch_size_32.png`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/docs/source/conf.py` & `cappr-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/docs/source/index.rst` & `cappr-0.2.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/docs/source/related_work.rst` & `cappr-0.2.3/docs/source/related_work.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/setup.py` & `cappr-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/src/cappr/_example.py` & `cappr-0.2.3/src/cappr/_example.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/src/cappr/huggingface/_utils.py` & `cappr-0.2.3/src/cappr/huggingface/_utils.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/src/cappr/huggingface/classify.py` & `cappr-0.2.3/src/cappr/huggingface/classify.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/src/cappr/huggingface/classify_no_cache.py` & `cappr-0.2.3/src/cappr/huggingface/classify_no_cache.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/src/cappr/openai/api.py` & `cappr-0.2.3/src/cappr/openai/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,21 @@
 
 end_of_prompt = "\n\n###\n\n"
 ## https://platform.openai.com/docs/guides/fine-tuning/data-formatting
 
 
 Model = Literal[
     "text-ada-001",
-    "ada",
     "text-babbage-001",
-    "babbage",
     "text-curie-001",
-    "curie",
-    "text-davinci-003",
     "text-davinci-002",
-    "davinci",
+    "text-davinci-003",
 ]
 ## https://platform.openai.com/docs/models/model-endpoint-compatibility
-_costs = [0.0004, 0.0004, 0.0005, 0.0005, 0.002, 0.002, 0.02, 0.02, 0.02]
+_costs = [0.0004, 0.0005, 0.002, 0.02, 0.02]
 ## https://openai.com/api/pricing/
 ## TODO: figure out how to get this automatically from openai, if possible
 model_to_cost_per_1k: dict[Model, float] = dict(zip(get_args(Model), _costs))
 
 
 def openai_method_retry(
     openai_method: Callable,
@@ -191,15 +187,15 @@
 
     Returns
     -------
     list[Mapping[str, Any]]
         list with the same length as `texts`. Each element is the ``choices`` mapping
         which the OpenAI text completion endpoint returns.
     """
-    _batch_size = 20  ## max that the API can currently handle
+    _batch_size = 32  ## max that the API can currently handle
     if isinstance(texts, str):
         ## Passing in a string will silently but majorly fail. Handle it
         texts = [texts]
     if ask_if_ok:
         _openai_api_call_is_ok(model, texts, max_tokens=max_tokens)
     choices = []
     with tqdm(total=len(texts), desc=progress_bar_desc) as progress_bar:
@@ -266,15 +262,17 @@
         returns. More specifically, it's a list of
         ``openai.openai_object.OpenAIObject``
     """
     ## TODO: batch, if possible
     if isinstance(texts, str):
         texts = [texts]
     if ask_if_ok:
-        _openai_api_call_is_ok(model=model, texts=texts, max_tokens=max_tokens)
+        _openai_api_call_is_ok(
+            model=model, texts=texts, max_tokens=max_tokens, cost_per_1k_tokens=0.002
+        )
     choices = []
     for text in tqdm(texts, total=len(texts), desc="Completing chats"):
         messages = [
             {"role": "system", "content": system_msg},
             {"role": "user", "content": text},
         ]
         response = openai_method_retry(
```

### Comparing `cappr-0.2.2/src/cappr/openai/classify.py` & `cappr-0.2.3/src/cappr/openai/classify.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,22 +12,41 @@
 import tiktoken
 
 from cappr.utils import _batch, classify
 from cappr import Example
 from cappr import openai
 
 
-def _token_logprobs(
+def token_logprobs(
     texts: Sequence[str], model: openai.api.Model, ask_if_ok: bool = False
 ) -> list[list[float]]:
     """
-    Returns a list `log_probs` where `log_probs[i]` is the value of `'logprobs' ->
-    'token_logprobs'` (from the OpenAI Completion endpoint) for `texts[i]` using
-    `model`. If `texts[i]` is a single token, then `log_probs[i]` is `[None]` (because
-    there's nothing to condition on).
+    For each text, compute each token's log-probability conditional on all previous
+    tokens in the text.
+
+    Parameters
+    ----------
+    texts : Sequence[str]
+        input texts
+    model : cappr.openai.api.Model
+        string for the name of an OpenAI text-completion model, specifically one from
+        the ``/v1/completions`` endpoint:
+        https://platform.openai.com/docs/models/model-endpoint-compatibility
+    ask_if_ok : bool, optional
+        whether or not to prompt you to manually give the go-ahead to run this function,
+        after notifying you of the approximate cost of the OpenAI API calls. By default
+        False
+
+    Returns
+    -------
+    log_probs : list[list[float]]
+        `log_probs[text_idx][token_idx]` is the log-probability of the token at
+        `token_idx` of `texts[text_idx]` conditional on all previous tokens in
+        `texts[text_idx]`. If `texts[text_idx]` is a single token, then
+        `log_probs[text_idx]` is `[None]`.
     """
     ## Need to handle texts which are single tokens. Set their logprobs to [None]
     tokenizer = tiktoken.encoding_for_model(model)
     text_lengths = [len(tokens) for tokens in tokenizer.encode_batch(texts)]
     idxs_multiple_tokens = [i for i, length in enumerate(text_lengths) if length > 1]
     choices = openai.api.gpt_complete(
         texts=[texts[i] for i in idxs_multiple_tokens],
@@ -148,15 +167,15 @@
         raise TypeError("completions must be a Sequence of strings.")
     ## Flat list of prompts and their completions. Will post-process
     texts = [
         prompt + end_of_prompt + completion
         for prompt in prompts
         for completion in completions
     ]
-    log_probs = _token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
+    log_probs = token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
     ## Since log_probs is a flat list, we'll need to batch them by the size and order of
     ## completions to fulfill the spec.
     return [
         _slice_completions(completions, log_probs_batch, model)
         for log_probs_batch in _batch.constant(log_probs, size=len(completions))
     ]
 
@@ -228,15 +247,15 @@
     """
     ## Flat list of prompts and their completions. Will post-process
     texts = [
         example.prompt + example.end_of_prompt + completion
         for example in examples
         for completion in example.completions
     ]
-    log_probs_all = _token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
+    log_probs_all = token_logprobs(texts, model=model, ask_if_ok=ask_if_ok)
     ## Flatten completions in same order as examples were flattened
     completions_all = [
         completion for example in examples for completion in example.completions
     ]
     log_probs_completions_all = _slice_completions(
         completions_all, log_probs_all, model
     )
@@ -251,14 +270,15 @@
 def predict_proba(
     prompts: Sequence[str],
     completions: Sequence[str],
     model: openai.api.Model,
     prior: Optional[Sequence[float]] = None,
     end_of_prompt: str = " ",
     discount_completions: float = 0.0,
+    log_marginal_probs_completions: Optional[Sequence[Sequence[float]]] = None,
     ask_if_ok: bool = False,
 ) -> npt.NDArray[np.floating]:
     """
     Predict probabilities of each completion coming after each prompt.
 
     Parameters
     ----------
@@ -274,18 +294,23 @@
     prior : Sequence[float], optional
         a probability distribution over `completions`, representing a belief about their
         likelihoods regardless of the prompt. By default, each completion in
         `completions` is assumed to be equally likely
     end_of_prompt : str, optional
         the string to tack on at the end of every prompt, by default " "
     discount_completions : float, optional
-        experimental feature: set it to >0.0 (e.g., 1.0 may work well) if a completion
-        is consistently getting too high predicted probabilities. You could instead
-        fudge the `prior`, but this hyperparameter may be easier to tune than the
-        `prior`. By default 0.0
+        experimental feature: set it (e.g., 1.0 may work well) if a completion is
+        consistently getting too high predicted probabilities. You could instead fudge
+        the `prior`, but this hyperparameter may be easier to tune than the `prior`. By
+        default 0.0
+    log_marginal_probs_completions : Sequence[Sequence[float]] , optional
+        experimental feature: pre-computed log probabilities of completion tokens
+        conditional on previous completion tokens (not prompt tokens). Only used if `not
+        discount_completions`. Compute them by passing `completions` and `model` to
+        :func:`cappr.openai.classify.token_logprobs`. By default, None
     ask_if_ok : bool, optional
         whether or not to prompt you to manually give the go-ahead to run this function,
         after notifying you of the approximate cost of the OpenAI API calls. By default
         False
 
     Returns
     -------
@@ -345,39 +370,44 @@
         pred_probs[1,3]
         # 0.7
 
         # predicted probability that 2nd product review says it's too expensive
         pred_probs[1,0]
         # 0.1
     """
-    if discount_completions < 0.0:
+    if not discount_completions and (log_marginal_probs_completions is not None):
         raise ValueError(
-            f"discount_completions must be >= 0.0. Got {discount_completions}"
+            "log_marginal_probs_completions is set, but they will not be used because "
+            "discount_completions was not set."
         )
     log_probs_completions = log_probs_conditional(
         prompts,
         completions,
         model,
         end_of_prompt=end_of_prompt,
         ask_if_ok=ask_if_ok,
     )
-    if discount_completions == 0.0:
+    if not discount_completions:
         return log_probs_completions
-    log_marginal_probs_completions = _token_logprobs(
-        completions, model, ask_if_ok=ask_if_ok
-    )
+    ## log Pr(completion token i | completion token :i) for each completion
+    if log_marginal_probs_completions is None:
+        log_marginal_probs_completions = token_logprobs(
+            completions, model, ask_if_ok=ask_if_ok
+        )
     for x in log_marginal_probs_completions:
         x[0] = 0  ## set it from None to 0, i.e., no discount for the first token
+    ## pre-multiply by the discount amount
+    log_marginal_probs_completions_discounted = [
+        discount_completions * np.array(log_marginal_probs_completion)
+        for log_marginal_probs_completion in log_marginal_probs_completions
+    ]
     return [
         [
             np.array(log_probs_prompt_completions[completion_idx])
-            + (
-                discount_completions
-                * np.array(log_marginal_probs_completions[completion_idx])
-            )
+            + (np.array(log_marginal_probs_completions_discounted[completion_idx]))
             for completion_idx in range(len(completions))
         ]
         for log_probs_prompt_completions in log_probs_completions
     ]
 
 
 @classify._predict_proba_examples
@@ -449,14 +479,15 @@
 def predict(
     prompts: Sequence[str],
     completions: Sequence[str],
     model: openai.api.Model,
     prior: Optional[Sequence[float]] = None,
     end_of_prompt: str = " ",
     discount_completions: float = 0.0,
+    log_marginal_probs_completions: Optional[Sequence[Sequence[float]]] = None,
     ask_if_ok: bool = False,
 ) -> list[str]:
     """
     Predict which completion is most likely to follow each prompt.
 
     Parameters
     ----------
@@ -475,14 +506,19 @@
         `completions` is assumed to be equally likely
     end_of_prompt : str, optional
         the string to tack on at the end of every prompt, by default " "
     discount_completions : float, optional
         experimental feature: set it to >0.0 (e.g., 1.0 may work well) if a completion
         is consistently getting over-predicted. You could instead fudge the `prior`, but
         this hyperparameter may be easier to tune than the `prior`. By default 0.0
+    log_marginal_probs_completions : Sequence[Sequence[float]] , optional
+        experimental feature: pre-computed log probabilities of completion tokens
+        conditional on previous completion tokens (not prompt tokens). Only used if `not
+        discount_completions`. Compute them by passing `completions` and `model` to
+        :func:`cappr.openai.classify.token_logprobs`. By default, None
     ask_if_ok : bool, optional
         whether or not to prompt you to manually give the go-ahead to run this function,
         after notifying you of the approximate cost of the OpenAI API calls. By default
         False
 
     Returns
     -------
```

### Comparing `cappr-0.2.2/src/cappr/utils/_batch.py` & `cappr-0.2.3/src/cappr/utils/_batch.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/src/cappr/utils/_check.py` & `cappr-0.2.3/src/cappr/utils/_check.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/src/cappr/utils/classify.py` & `cappr-0.2.3/src/cappr/utils/classify.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/src/cappr.egg-info/PKG-INFO` & `cappr-0.2.3/src/cappr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cappr
-Version: 0.2.2
+Version: 0.2.3
 Summary: Zero-shot text classification using autoregressive language models.
 Home-page: https://github.com/kddubey/cappr/
 Author-email: kushdubey63@gmail.com
 License: Apache License 2.0
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: hf
@@ -28,14 +28,15 @@
 > **C**ompletion<br>
   **A**fter<br>
   **P**rompt<br>
   **Pr**obability<br>
 
 The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
 
+
 ## Usage
 
 <details>
 <summary>Use a model from the OpenAI API</summary>
 
 Specifically, this model must be compatible with the
 [/v1/completions](https://platform.openai.com/docs/models/model-endpoint-compatibility)
@@ -221,15 +222,15 @@
 
 ```
 python -m pip install cappr[hf]
 ```
 </details>
 
 <details>
-<summary>(Optional) Set up to run demos</summary>
+<summary>(Optional) Install requirements for running demos</summary>
 
 ```
 python -m pip install cappr[demos]
 ```
 </details>
 
 
@@ -276,19 +277,21 @@
 
 ## Results
 
 <details>
 <summary>
 Statistical performance
 </summary>
-Performs ok based on 2 datasets, when compared to classification via sampling (CVS).
-I need to run it on more ofc. Will update
 
-  * [`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
-  * [`demos/superglue/wsc.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb)
+Not too shabby. TODO: summary table comparing CVS vs. CAPPr vs. few-shot methods like
+SetFit and PET.
+
+[2 SuperGLUE datasets](https://github.com/kddubey/cappr/blob/main/demos/superglue)
+
+[RAFT zero-shot training sets](https://github.com/kddubey/cappr/blob/main/demos/raft)
 </details>
 
 
 <details>
 <summary>
 Computational performance
 </summary>
@@ -322,21 +325,23 @@
 ## Related work
 
 While [benchmarking this
 method](https://github.com/kddubey/cappr/blob/main/demos/superglue/wsc.ipynb) on the
 Winograd Schema Challenge, I found that [this paper](https://arxiv.org/abs/1806.02847)
 is very similar:
 
-> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv preprint arXiv:1806.02847 (2018).
+> Trinh, Trieu H., and Quoc V. Le. "A simple method for commonsense reasoning." arXiv
+> preprint arXiv:1806.02847 (2018).
 
 [PET with multiple masks](https://arxiv.org/abs/2009.07118) also aggregates token
 probabilities to do prompt-completion classification, but these probabilities are
 assumed to come from masked language models like BERT.
 
-> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
+> Schick, Timo, and Hinrich Schütze. "It's not just size that matters: Small language
+> models are also few-shot learners." arXiv preprint arXiv:2009.07118 (2020).
 
 
 ## Contributing
 
 TODO
 
 
@@ -396,15 +401,14 @@
 - [ ] HuggingFace `transformers.AutoModelForCausalLM`
   - [x] Optimize backend to enable greater scaling wrt # completions/classes
   - [x] Get it working on single-GPU, check that it's faster than sampling assuming
   batching
     - [ ] Get to the bottom of why it's slower w/o batching
   - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
   think
-  - [ ] Support few-shot prompt caching. Consider a fit-predict interface (**)
   - [ ] Consider batchifying the completions again, since they technically don't go in
   batches of `batch_size`; the actual batch size is the sum of the number of completions
   corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
   are usually half as long. But it should be configurable at the very least.
   - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
   - [ ] Support [Inference
     Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
```

### Comparing `cappr-0.2.2/src/cappr.egg-info/SOURCES.txt` & `cappr-0.2.3/src/cappr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/tests/_test.py` & `cappr-0.2.3/tests/_test.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/tests/huggingface/test_huggingface_classify.py` & `cappr-0.2.3/tests/huggingface/test_huggingface_classify.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/tests/openai/test_openai_classify.py` & `cappr-0.2.3/tests/openai/test_openai_classify.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,17 @@
             completions=("-washed", " learnt", " 🤖"),
             prior=(1 / 6, 2 / 3, 1 / 6),
             end_of_prompt="",
         ),
     ]
 
 
-def test__token_logprobs(model):
+def test_token_logprobs(model):
     texts = ["a b c", "d e"]
-    log_probs = classify._token_logprobs(texts, model)
+    log_probs = classify.token_logprobs(texts, model)
     assert log_probs == [[0, 1, 2], [0, 1]]
 
 
 def test__slice_completions(completions, model):
     log_probs = [[0, 1, 2], [0, 1]]
     log_probs_completions = classify._slice_completions(completions, log_probs, model)
     assert log_probs_completions == [[1, 2], [1]]
```

### Comparing `cappr-0.2.2/tests/utils/test_batch.py` & `cappr-0.2.3/tests/utils/test_batch.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.2/tests/utils/test_utils_classify.py` & `cappr-0.2.3/tests/utils/test_utils_classify.py`

 * *Files identical despite different names*

