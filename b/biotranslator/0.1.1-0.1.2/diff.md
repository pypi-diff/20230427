# Comparing `tmp/biotranslator-0.1.1.tar.gz` & `tmp/biotranslator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotranslator-0.1.1.tar", last modified: Mon Sep  5 08:22:49 2022, max compression
+gzip compressed data, was "dist/biotranslator-0.1.2.tar", last modified: Thu Apr 27 14:51:44 2023, max compression
```

## Comparing `biotranslator-0.1.1.tar` & `biotranslator-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.514462 biotranslator-0.1.1/
--rw-rw-rw-   0        0        0     2361 2022-09-05 08:22:49.513461 biotranslator-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1313 2022-09-05 08:22:13.000000 biotranslator-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.457452 biotranslator-0.1.1/biotranslator/
--rw-rw-rw-   0        0        0      270 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.483463 biotranslator-0.1.1/biotranslator/biotranslator/
--rw-rw-rw-   0        0        0       35 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/biotranslator/__init__.py
--rw-rw-rw-   0        0        0     6032 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/biotranslator/_encoder.py
--rw-rw-rw-   0        0        0     4146 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/biotranslator_function.py
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.487462 biotranslator-0.1.1/biotranslator/config/
--rw-rw-rw-   0        0        0       30 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/config/__init__.py
--rw-rw-rw-   0        0        0     6666 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/config/_config.py
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.489462 biotranslator-0.1.1/biotranslator/loader/
--rw-rw-rw-   0        0        0       33 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/loader/__init__.py
--rw-rw-rw-   0        0        0    18124 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/loader/_bioloader.py
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.495462 biotranslator-0.1.1/biotranslator/metrics/
--rw-rw-rw-   0        0        0      105 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/metrics/__init__.py
--rw-rw-rw-   0        0        0      766 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/metrics/_auroc.py
--rw-rw-rw-   0        0        0      376 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/metrics/_micro_auroc.py
--rw-rw-rw-   0        0        0      267 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/metrics/_roc.py
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.502462 biotranslator-0.1.1/biotranslator/text_encoder/
--rw-rw-rw-   0        0        0      156 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/text_encoder/__init__.py
--rw-rw-rw-   0        0        0     1714 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/text_encoder/_datasets.py
--rw-rw-rw-   0        0        0     2021 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/text_encoder/_get_data.py
--rw-rw-rw-   0        0        0      947 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/text_encoder/_nn.py
--rw-rw-rw-   0        0        0     2601 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/text_encoder/_train.py
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.509462 biotranslator-0.1.1/biotranslator/trainer/
--rw-rw-rw-   0        0        0       39 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/trainer/__init__.py
--rw-rw-rw-   0        0        0    11666 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/trainer/_graph_trainer.py
--rw-rw-rw-   0        0        0    10639 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/trainer/_sequence_trainer.py
--rw-rw-rw-   0        0        0      408 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/trainer/_trainer.py
--rw-rw-rw-   0        0        0     7509 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/trainer/_vector_trainer.py
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.511463 biotranslator-0.1.1/biotranslator/utils/
--rw-rw-rw-   0        0        0       23 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/utils/__init__.py
--rw-rw-rw-   0        0        0    59624 2022-09-05 08:22:13.000000 biotranslator-0.1.1/biotranslator/utils/_utils.py
-drwxrwxrwx   0        0        0        0 2022-09-05 08:22:49.480464 biotranslator-0.1.1/biotranslator.egg-info/
--rw-rw-rw-   0        0        0     2361 2022-09-05 08:22:49.000000 biotranslator-0.1.1/biotranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1074 2022-09-05 08:22:49.000000 biotranslator-0.1.1/biotranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-05 08:22:49.000000 biotranslator-0.1.1/biotranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      234 2022-09-05 08:22:49.000000 biotranslator-0.1.1/biotranslator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-09-05 08:22:49.000000 biotranslator-0.1.1/biotranslator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1590 2022-09-05 08:22:13.000000 biotranslator-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-05 08:22:49.514462 biotranslator-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1060 2022-09-05 08:22:13.000000 biotranslator-0.1.1/setup.py
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     2343 2023-04-27 14:51:44.000000 biotranslator-0.1.2/PKG-INFO
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     1319 2023-04-23 19:34:56.000000 biotranslator-0.1.2/README.md
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)      263 2023-04-23 19:34:57.000000 biotranslator-0.1.2/biotranslator/__init__.py
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator/biotranslator/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)       35 2023-04-23 19:34:57.000000 biotranslator-0.1.2/biotranslator/biotranslator/__init__.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     5902 2023-04-23 19:34:57.000000 biotranslator-0.1.2/biotranslator/biotranslator/_encoder.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     4022 2023-04-23 19:44:04.000000 biotranslator-0.1.2/biotranslator/biotranslator_function.py
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator/config/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)       30 2023-04-23 19:34:58.000000 biotranslator-0.1.2/biotranslator/config/__init__.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     6547 2023-04-23 19:34:58.000000 biotranslator-0.1.2/biotranslator/config/_config.py
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator/loader/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)       33 2023-04-23 19:34:58.000000 biotranslator-0.1.2/biotranslator/loader/__init__.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)    17794 2023-04-23 19:34:59.000000 biotranslator-0.1.2/biotranslator/loader/_bioloader.py
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator/metrics/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)      102 2023-04-23 19:34:59.000000 biotranslator-0.1.2/biotranslator/metrics/__init__.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)      746 2023-04-23 19:34:59.000000 biotranslator-0.1.2/biotranslator/metrics/_auroc.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)      366 2023-04-23 19:47:44.000000 biotranslator-0.1.2/biotranslator/metrics/_micro_auroc.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)      258 2023-04-23 19:35:00.000000 biotranslator-0.1.2/biotranslator/metrics/_roc.py
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator/text_encoder/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)      153 2023-04-23 19:35:00.000000 biotranslator-0.1.2/biotranslator/text_encoder/__init__.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     1666 2023-04-23 19:35:00.000000 biotranslator-0.1.2/biotranslator/text_encoder/_datasets.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     1963 2023-04-23 19:35:01.000000 biotranslator-0.1.2/biotranslator/text_encoder/_get_data.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)      921 2023-04-23 19:35:01.000000 biotranslator-0.1.2/biotranslator/text_encoder/_nn.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     2543 2023-04-23 19:35:01.000000 biotranslator-0.1.2/biotranslator/text_encoder/_train.py
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator/trainer/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)       37 2023-04-23 19:35:01.000000 biotranslator-0.1.2/biotranslator/trainer/__init__.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)    11428 2023-04-23 19:35:01.000000 biotranslator-0.1.2/biotranslator/trainer/_graph_trainer.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)    10437 2023-04-23 19:35:02.000000 biotranslator-0.1.2/biotranslator/trainer/_sequence_trainer.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)      394 2023-04-23 19:35:02.000000 biotranslator-0.1.2/biotranslator/trainer/_trainer.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     7363 2023-04-23 19:35:02.000000 biotranslator-0.1.2/biotranslator/trainer/_vector_trainer.py
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator/utils/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)       22 2023-04-23 19:35:03.000000 biotranslator-0.1.2/biotranslator/utils/__init__.py
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)    58060 2023-04-23 19:35:03.000000 biotranslator-0.1.2/biotranslator/utils/_utils.py
+drwxr-sr-x   0 yzhao4   (976606) h2lab    (723133)        0 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator.egg-info/
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     2343 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator.egg-info/PKG-INFO
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     1074 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator.egg-info/SOURCES.txt
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)        1 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator.egg-info/dependency_links.txt
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)      234 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator.egg-info/requires.txt
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)       14 2023-04-27 14:51:44.000000 biotranslator-0.1.2/biotranslator.egg-info/top_level.txt
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     1550 2023-04-23 19:35:05.000000 biotranslator-0.1.2/pyproject.toml
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)       38 2023-04-27 14:51:44.000000 biotranslator-0.1.2/setup.cfg
+-rw-r--r--   0 yzhao4   (976606) h2lab    (723133)     1021 2023-04-27 14:50:14.000000 biotranslator-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `biotranslator-0.1.1/PKG-INFO` & `biotranslator-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: biotranslator
-Version: 0.1.1
-Summary: BioTranslator: Cross-modal Translation for Zero-shot Biomedical Classification
-Home-page: https://github.com/ywzhao2002/biotranslator
-Author: Hanwen Xu, Yunwei Zhao, Addie Woicik, Hoifung Poon, Russ B.Altman, Sheng Wang
-Author-email: swang91@uw.edu
-Maintainer-email: Hanwen Xu <xuhw@cs.washington.edu>, Yunwei Zhao <yzhao4@cs.washington.edu>
-License: MIT Licence
-Project-URL: Documentation, https://biotranslator.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/HanwenXuTHU/BioTranslatorProject
-Keywords: pip,BioTranslator
-Platform: any
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-Provides-Extra: doc
-
-[![Stars](https://img.shields.io/github/stars/scverse/scanpy?logo=GitHub&color=yellow)](https://github.com/HanwenXuTHU/BioTranslatorProject)
-[![PyPI](https://img.shields.io/pypi/v/scanpy?logo=PyPI)](https://pypi.org/project/biotranslator/)
-[![PyPIDownload](https://static.pepy.tech/badge/biotranslator)](https://pepy.tech/project/biotranslator)
-[![Doc](https://readthedocs.org/projects/biotranslator/badge/?version=latest)](https://biotranslator.readthedocs.io/en/latest/?badge=latest)
-
-
-# BioTranslator API
-
-BioTranslator is a cross-modal translator which can annotate biology instances only using user-written texts.
-The codes here can reproduce the main results in BioTranslator paper, including zero-shot protein function prediction, zero-shot cell type prediction, and predict the nodes and edges of a gene pathway.
-BioTranslator takes a user-written textual description of the new discovery and then translates this description to a non-text biological data instance. Our tool frees scientists from limiting their analysis within predefined controlled vocabularies, thus accelerating new biomedical discoveries.
-
-[documentation]: https://biotranslator.readthedocs.io
-
-For more information, please visit the project's main repository [here](https://github.com/HanwenXuTHU/BioTranslatorProject).
+Metadata-Version: 2.1
+Name: biotranslator
+Version: 0.1.2
+Summary: BioTranslator: Cross-modal Translation for Zero-shot Biomedical Classification
+Home-page: https://github.com/ywzhao2002/biotranslator
+Author: Hanwen Xu, Yunwei Zhao, Addie Woicik, Hoifung Poon, Russ B.Altman, Sheng Wang
+Author-email: swang91@uw.edu
+Maintainer-email: Hanwen Xu <xuhw@cs.washington.edu>, Yunwei Zhao <yzhao4@cs.washington.edu>
+License: MIT Licence
+Project-URL: Documentation, https://biotranslator.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/HanwenXuTHU/BioTranslatorProject
+Keywords: pip,BioTranslator
+Platform: any
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+Provides-Extra: doc
+
+[![Stars](https://img.shields.io/github/stars/ywzhao2002/biotranslator?logo=GitHub&color=yellow)](https://github.com/HanwenXuTHU/BioTranslatorProject)
+[![PyPI](https://img.shields.io/pypi/v/biotranslator?logo=PyPI)](https://pypi.org/project/biotranslator/)
+[![PyPIDownload](https://static.pepy.tech/badge/biotranslator)](https://pepy.tech/project/biotranslator)
+[![Doc](https://readthedocs.org/projects/biotranslator/badge/?version=latest)](https://biotranslator.readthedocs.io/en/latest/index.html)
+
+
+# BioTranslator API
+
+BioTranslator is a cross-modal translator which can annotate biology instances only using user-written texts.
+The codes here can reproduce the main results in BioTranslator paper, including zero-shot protein function prediction, zero-shot cell type prediction, and predict the nodes and edges of a gene pathway.
+BioTranslator takes a user-written textual description of the new discovery and then translates this description to a non-text biological data instance. Our tool frees scientists from limiting their analysis within predefined controlled vocabularies, thus accelerating new biomedical discoveries.
+
+[documentation]: https://biotranslator.readthedocs.io
+
+For more information, feel free to visit the project's main repository [here](https://github.com/HanwenXuTHU/BioTranslatorProject).
```

### Comparing `biotranslator-0.1.1/README.md` & `biotranslator-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-[![Stars](https://img.shields.io/github/stars/scverse/scanpy?logo=GitHub&color=yellow)](https://github.com/HanwenXuTHU/BioTranslatorProject)
-[![PyPI](https://img.shields.io/pypi/v/scanpy?logo=PyPI)](https://pypi.org/project/biotranslator/)
-[![PyPIDownload](https://static.pepy.tech/badge/biotranslator)](https://pepy.tech/project/biotranslator)
-[![Doc](https://readthedocs.org/projects/biotranslator/badge/?version=latest)](https://biotranslator.readthedocs.io/en/latest/?badge=latest)
-
-
-# BioTranslator API
-
-BioTranslator is a cross-modal translator which can annotate biology instances only using user-written texts.
-The codes here can reproduce the main results in BioTranslator paper, including zero-shot protein function prediction, zero-shot cell type prediction, and predict the nodes and edges of a gene pathway.
-BioTranslator takes a user-written textual description of the new discovery and then translates this description to a non-text biological data instance. Our tool frees scientists from limiting their analysis within predefined controlled vocabularies, thus accelerating new biomedical discoveries.
-
-[documentation]: https://biotranslator.readthedocs.io
-
-For more information, please visit the project's main repository [here](https://github.com/HanwenXuTHU/BioTranslatorProject).
+[![Stars](https://img.shields.io/github/stars/ywzhao2002/biotranslator?logo=GitHub&color=yellow)](https://github.com/HanwenXuTHU/BioTranslatorProject)
+[![PyPI](https://img.shields.io/pypi/v/biotranslator?logo=PyPI)](https://pypi.org/project/biotranslator/)
+[![PyPIDownload](https://static.pepy.tech/badge/biotranslator)](https://pepy.tech/project/biotranslator)
+[![Doc](https://readthedocs.org/projects/biotranslator/badge/?version=latest)](https://biotranslator.readthedocs.io/en/latest/index.html)
+
+
+# BioTranslator API
+
+BioTranslator is a cross-modal translator which can annotate biology instances only using user-written texts.
+The codes here can reproduce the main results in BioTranslator paper, including zero-shot protein function prediction, zero-shot cell type prediction, and predict the nodes and edges of a gene pathway.
+BioTranslator takes a user-written textual description of the new discovery and then translates this description to a non-text biological data instance. Our tool frees scientists from limiting their analysis within predefined controlled vocabularies, thus accelerating new biomedical discoveries.
+
+[documentation]: https://biotranslator.readthedocs.io
+
+For more information, feel free to visit the project's main repository [here](https://github.com/HanwenXuTHU/BioTranslatorProject).
```

### Comparing `biotranslator-0.1.1/biotranslator/biotranslator/_encoder.py` & `biotranslator-0.1.2/biotranslator/biotranslator/_encoder.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-# -*- coding: utf-8 -*-
-import itertools
-import numpy as np
-from torch import nn
-from torch.nn import init
-from transformers import AutoTokenizer, AutoModel
-import torch
-import collections
-from ..utils import init_weights
-
-
-class BioDataEncoder(nn.Module):
-    def __init__(self,
-                 feature=None,
-                 hidden_dim=1000,
-                 seq_input_nc=4,
-                 seq_in_nc=512,
-                 seq_max_kernels=129,
-                 seq_length=2000,
-                 network_dim=800,
-                 description_dim=768,
-                 expression_dim=1000,
-                 drop_out=0.01,
-                 text_dim=768):
-        super(BioDataEncoder, self).__init__()
-        if feature is None:
-            feature = ['seqs', 'network', 'description', 'expression']
-        self.feature = feature
-        self.text_dim = text_dim
-        if 'seqs' in self.feature:
-            self.para_conv, self.para_pooling = [], []
-            kernels = range(8, seq_max_kernels, 8)
-            self.kernel_num = len(kernels)
-            for i in range(len(kernels)):
-                exec(
-                    "self.conv1d_{} = nn.Conv1d(in_channels=seq_input_nc, out_channels=seq_in_nc, kernel_size=kernels[i], padding=0, stride=1)".format(
-                        i))
-                exec("self.pool1d_{} = nn.MaxPool1d(kernel_size=seq_length - kernels[i] + 1, stride=1)".format(i))
-            self.fc_seq = [nn.Linear(len(kernels) * seq_in_nc, hidden_dim), nn.LeakyReLU(inplace=True)]
-            self.fc_seq = nn.Sequential(*self.fc_seq)
-        if 'description' in self.feature:
-            self.fc_description = [nn.Linear(description_dim, hidden_dim), nn.LeakyReLU(inplace=True)]
-            self.fc_description = nn.Sequential(*self.fc_description)
-        if 'network' in self.feature:
-            self.fc_network = [nn.Linear(network_dim, hidden_dim), nn.LeakyReLU(inplace=True)]
-            self.fc_network = nn.Sequential(*self.fc_network)
-        if 'expression' in self.feature:
-            self.fc_expr = [nn.Linear(expression_dim, hidden_dim), nn.ReLU(inplace=True), nn.Dropout(p=drop_out)]
-            self.fc_expr = nn.Sequential(*self.fc_expr)
-        self.cat2emb = nn.Linear(len(self.feature) * hidden_dim, text_dim)
-
-    def forward(self, x=None, x_description=None, x_vector=None, x_expr=None):
-        x_list = []
-        features = collections.OrderedDict()
-        if 'seqs' in self.feature:
-            for i in range(self.kernel_num):
-                exec("x_i = self.conv1d_{}(x)".format(i))
-                exec("x_i = self.pool1d_{}(x_i)".format(i))
-                exec("x_list.append(torch.squeeze(x_i).reshape([x.size(0), -1]))")
-            features['seqs'] = self.fc_seq(torch.cat(tuple(x_list), dim=1))
-        if 'description' in self.feature:
-            features['description'] = self.fc_description(x_description)
-        if 'network' in self.feature:
-            features['network'] = self.fc_network(x_vector)
-        if 'expression' in self.feature:
-            features['expression'] = self.fc_expr(x_expr)
-        for i in range(len(self.feature)):
-            if i == 0:
-                x_enc = features[self.feature[0]]
-            else:
-                x_enc = torch.cat((x_enc, features[self.feature[i]]), dim=1)
-        # x_enc = torch.nn.functional.normalize(x_cat, p=2, dim=1)
-        return self.cat2emb(x_enc)
-
-
-class BioTranslator(nn.Module):
-    def __init__(self, cfg):
-        super(BioTranslator, self).__init__()
-        self.loss_func = torch.nn.BCELoss()
-        if cfg.tp in ['seq', 'graph']:
-            kwargs = dict(feature=cfg.features,
-                          hidden_dim=cfg.hidden_dim,
-                          seq_input_nc=cfg.seq_input_nc,
-                          seq_in_nc=cfg.seq_in_nc,
-                          seq_max_kernels=cfg.seq_max_kernels,
-                          network_dim=cfg.network_dim,
-                          seq_length=cfg.max_length,
-                          text_dim=cfg.term_enc_dim)
-        elif cfg.tp == 'vec':
-            kwargs = dict(feature=cfg.features,
-                           hidden_dim=cfg.hidden_dim,
-                           expression_dim=cfg.expr_dim,
-                           drop_out=cfg.drop_out,
-                           text_dim=cfg.term_enc_dim)
-        else:
-            raise NotImplementedError
-        self.data_encoder = BioDataEncoder(**kwargs)
-
-        if cfg.tp == "seq" or cfg.tp == "graph":
-            self.activation = torch.nn.Sigmoid()
-            # self.text_encoder = torch.load(model_config.text_encoder)
-            self.temperature = torch.tensor(0.07, requires_grad=True)
-        elif cfg.tp == "vec":
-            self.activation = torch.nn.Softmax(dim=1)
-        else:
-            raise NotImplementedError
-
-        self.text_dim = cfg.term_enc_dim
-        init_weights(self.data_encoder, init_type='xavier')
-        if len(cfg.gpu_ids) > 0:
-            self.data_encoder = self.data_encoder.to('cuda')
-            self.temperature = self.temperature.to('cuda')
-            self.activation = self.activation.to('cuda')
-
-    def forward(self, data_type=None, input_seq=None, input_description=None, input_vector=None, input_expr=None, texts=None):
-        # get textual description encodings
-        text_encodings = texts.permute(1, 0)
-        # get biology instance encodings
-        if data_type == "seq" or data_type == "graph":
-            data_encodings = self.data_encoder(x=input_seq,
-                                               x_description=input_description,
-                                               x_vector=input_vector)
-        elif data_type == "vec":
-            data_encodings = self.data_encoder(x_expr=input_expr)
-        else:
-            raise NotImplementedError
-
-        # compute logits
-        logits = torch.matmul(data_encodings, text_encodings)
-        return self.activation(logits)
+# -*- coding: utf-8 -*-
+import itertools
+import numpy as np
+from torch import nn
+from torch.nn import init
+from transformers import AutoTokenizer, AutoModel
+import torch
+import collections
+from ..utils import init_weights
+
+
+class BioDataEncoder(nn.Module):
+    def __init__(self,
+                 feature=None,
+                 hidden_dim=1000,
+                 seq_input_nc=4,
+                 seq_in_nc=512,
+                 seq_max_kernels=129,
+                 seq_length=2000,
+                 network_dim=800,
+                 description_dim=768,
+                 expression_dim=1000,
+                 drop_out=0.01,
+                 text_dim=768):
+        super(BioDataEncoder, self).__init__()
+        if feature is None:
+            feature = ['seqs', 'network', 'description', 'expression']
+        self.feature = feature
+        self.text_dim = text_dim
+        if 'seqs' in self.feature:
+            self.para_conv, self.para_pooling = [], []
+            kernels = range(8, seq_max_kernels, 8)
+            self.kernel_num = len(kernels)
+            for i in range(len(kernels)):
+                exec(
+                    "self.conv1d_{} = nn.Conv1d(in_channels=seq_input_nc, out_channels=seq_in_nc, kernel_size=kernels[i], padding=0, stride=1)".format(
+                        i))
+                exec("self.pool1d_{} = nn.MaxPool1d(kernel_size=seq_length - kernels[i] + 1, stride=1)".format(i))
+            self.fc_seq = [nn.Linear(len(kernels) * seq_in_nc, hidden_dim), nn.LeakyReLU(inplace=True)]
+            self.fc_seq = nn.Sequential(*self.fc_seq)
+        if 'description' in self.feature:
+            self.fc_description = [nn.Linear(description_dim, hidden_dim), nn.LeakyReLU(inplace=True)]
+            self.fc_description = nn.Sequential(*self.fc_description)
+        if 'network' in self.feature:
+            self.fc_network = [nn.Linear(network_dim, hidden_dim), nn.LeakyReLU(inplace=True)]
+            self.fc_network = nn.Sequential(*self.fc_network)
+        if 'expression' in self.feature:
+            self.fc_expr = [nn.Linear(expression_dim, hidden_dim), nn.ReLU(inplace=True), nn.Dropout(p=drop_out)]
+            self.fc_expr = nn.Sequential(*self.fc_expr)
+        self.cat2emb = nn.Linear(len(self.feature) * hidden_dim, text_dim)
+
+    def forward(self, x=None, x_description=None, x_vector=None, x_expr=None):
+        x_list = []
+        features = collections.OrderedDict()
+        if 'seqs' in self.feature:
+            for i in range(self.kernel_num):
+                exec("x_i = self.conv1d_{}(x)".format(i))
+                exec("x_i = self.pool1d_{}(x_i)".format(i))
+                exec("x_list.append(torch.squeeze(x_i).reshape([x.size(0), -1]))")
+            features['seqs'] = self.fc_seq(torch.cat(tuple(x_list), dim=1))
+        if 'description' in self.feature:
+            features['description'] = self.fc_description(x_description)
+        if 'network' in self.feature:
+            features['network'] = self.fc_network(x_vector)
+        if 'expression' in self.feature:
+            features['expression'] = self.fc_expr(x_expr)
+        for i in range(len(self.feature)):
+            if i == 0:
+                x_enc = features[self.feature[0]]
+            else:
+                x_enc = torch.cat((x_enc, features[self.feature[i]]), dim=1)
+        # x_enc = torch.nn.functional.normalize(x_cat, p=2, dim=1)
+        return self.cat2emb(x_enc)
+
+
+class BioTranslator(nn.Module):
+    def __init__(self, cfg):
+        super(BioTranslator, self).__init__()
+        self.loss_func = torch.nn.BCELoss()
+        if cfg.tp in ['seq', 'graph']:
+            kwargs = dict(feature=cfg.features,
+                          hidden_dim=cfg.hidden_dim,
+                          seq_input_nc=cfg.seq_input_nc,
+                          seq_in_nc=cfg.seq_in_nc,
+                          seq_max_kernels=cfg.seq_max_kernels,
+                          network_dim=cfg.network_dim,
+                          seq_length=cfg.max_length,
+                          text_dim=cfg.term_enc_dim)
+        elif cfg.tp == 'vec':
+            kwargs = dict(feature=cfg.features,
+                           hidden_dim=cfg.hidden_dim,
+                           expression_dim=cfg.expr_dim,
+                           drop_out=cfg.drop_out,
+                           text_dim=cfg.term_enc_dim)
+        else:
+            raise NotImplementedError
+        self.data_encoder = BioDataEncoder(**kwargs)
+
+        if cfg.tp == "seq" or cfg.tp == "graph":
+            self.activation = torch.nn.Sigmoid()
+            # self.text_encoder = torch.load(model_config.text_encoder)
+            self.temperature = torch.tensor(0.07, requires_grad=True)
+        elif cfg.tp == "vec":
+            self.activation = torch.nn.Softmax(dim=1)
+        else:
+            raise NotImplementedError
+
+        self.text_dim = cfg.term_enc_dim
+        init_weights(self.data_encoder, init_type='xavier')
+        if len(cfg.gpu_ids) > 0:
+            self.data_encoder = self.data_encoder.to('cuda')
+            self.temperature = self.temperature.to('cuda')
+            self.activation = self.activation.to('cuda')
+
+    def forward(self, data_type=None, input_seq=None, input_description=None, input_vector=None, input_expr=None, texts=None):
+        # get textual description encodings
+        text_encodings = texts.permute(1, 0)
+        # get biology instance encodings
+        if data_type == "seq" or data_type == "graph":
+            data_encodings = self.data_encoder(x=input_seq,
+                                               x_description=input_description,
+                                               x_vector=input_vector)
+        elif data_type == "vec":
+            data_encodings = self.data_encoder(x_expr=input_expr)
+        else:
+            raise NotImplementedError
+
+        # compute logits
+        logits = torch.matmul(data_encodings, text_encodings)
+        return self.activation(logits)
```

### Comparing `biotranslator-0.1.1/biotranslator/biotranslator_function.py` & `biotranslator-0.1.2/biotranslator/biotranslator_function.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import torch
-import logging
-import collections
-from .config import BioConfig
-from .loader import BioLoader
-from .trainer import build_trainer
-from torch.utils.data import DataLoader
-from .text_encoder import NeuralNetwork as nn_config
-from transformers import AutoTokenizer, AutoConfig
-from .text_encoder import TrainOntologyDataset, get_data, train
-
-device = torch.device('cuda') if torch.cuda.is_available() else torch.device('cpu')
-
-
-def setup_config(config, data_type='seq'):
-    args_names = dict(
-        seq=[
-            'task', 'max_length', 'features'
-        ],
-        vec=[
-            'task', 'eval_dataset', 'vec_ontology_repo'
-        ],
-        graph=[
-            'max_length', 'eval_dataset', 'graph_excludes', 'features'
-        ],
-        general=[
-            'data_repo', 'dataset', 'encoder_path', 'rst_dir', 'emb_dir',
-            'ws_dir', 'hidden_dim', 'lr', 'epoch', 'batch_size', 'gpu_ids',
-        ]
-    )
-    args_need = args_names[data_type]
-    args_need.extend(list(args_names['general']))
-    model_args = {k: config[k] for k in args_need}
-    return BioConfig(data_type, model_args)
-
-
-def train_text_encoder(data_dir: str, save_path: str):
-    """Fine-tune the PubMedBert on 225 Ontologies, except cl and go
-    Parameters
-    ----------
-    data_dir
-        the Ontologies dataset
-    save_path
-        where you save the model
-    """
-    print("Using {} device".format('cuda'))
-    bert_name = 'microsoft/BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext'
-    tokenizer = AutoTokenizer.from_pretrained(bert_name)
-    config = AutoConfig.from_pretrained(bert_name)
-    config.attention_probs_dropout_prob = 0.3
-    config.hidden_dropout_prob = 0.3
-    output_way = 'pooler'
-    assert output_way in ['pooler', 'cls', 'avg']
-
-    lr = 1e-5
-    batch_size = 16
-    max_len = 256
-    print(f'Batch Size: {batch_size}, Max Length: {max_len}')
-
-    model = nn_config(bert_name, output_way, config).to('cuda')
-    optimizer = torch.optim.AdamW(model.parameters(), lr=lr)
-    train_texts, test_texts = get_data(data_dir)
-
-    train_data = TrainOntologyDataset(train_texts, tokenizer, max_len)
-    train_dataloader = DataLoader(train_data, batch_size=batch_size)
-    test_data = TrainOntologyDataset(test_texts, tokenizer, max_len)
-    test_dataloader = DataLoader(test_data, batch_size=batch_size, shuffle=True)
-
-    epochs = 1
-    for t in range(epochs):
-        print(f"Epoch {t + 1}\n-------------------------------")
-        train(train_dataloader, test_dataloader, model, optimizer, save_path, device='cuda')
-    print("Train Done!")
-
-
-def train_biotranslator(cfgs):
-    """Train the BioTranslator
-
-    Parameters
-    ----------
-    cfgs: [config1, config2, config3, ...]
-
-    Returns
-    ------
-    encoder_list
-        List of trained translator
-    """
-    trainer_dict = collections.OrderedDict()
-    translators = collections.OrderedDict()
-    # We may only train one data type each time in this method
-    for cfg in cfgs:
-        if cfg.tp in ['graph', 'seq', 'vec']:
-            files = BioLoader(cfg)
-        else:
-            logging.info('Data type is not supported yet.')
-            raise NotImplementedError
-        trainer_dict[cfg.tp] = (build_trainer(files=files, cfg=cfg), files, cfg)
-    for key, trainer_tup in trainer_dict.items():
-        torch.cuda.set_device(eval(trainer_tup[2].gpu_ids))
-        trainer = trainer_tup[0]
-        print(f'Train encoder for {trainer_tup[2].tp} data:')
-        trainer.train(trainer_tup[1], trainer_tup[2])
-        translators[key] = trainer
-    return translators
-
-
-def test_biotranslator(data_dir, anno_data, cfg, translator, task):
-    """
-    Annotate the proteins with textual description embeddings
-
-    Parameters
-    ----------
-    data_dir: Input data path.
-    anno_data: data needs to be annotated
-    cfg: config
-    translator: biotranslator encoder
-    task: task name
-
-    Returns
-    -------
-    """
-    files = BioLoader(cfg)
-    anno = translator.annotate(files, cfg, data_dir, anno_data, task)
-    return anno
+import torch
+import logging
+import collections
+from .config import BioConfig
+from .loader import BioLoader
+from .trainer import build_trainer
+from torch.utils.data import DataLoader
+from .text_encoder import NeuralNetwork as nn_config
+from transformers import AutoTokenizer, AutoConfig
+from .text_encoder import TrainOntologyDataset, get_data, train
+
+device = torch.device('cuda') if torch.cuda.is_available() else torch.device('cpu')
+
+
+def setup_config(config, data_type='seq'):
+    args_names = dict(
+        seq=[
+            'task', 'max_length', 'features'
+        ],
+        vec=[
+            'task', 'eval_dataset', 'vec_ontology_repo'
+        ],
+        graph=[
+            'max_length', 'eval_dataset', 'graph_excludes', 'features'
+        ],
+        general=[
+            'data_repo', 'dataset', 'encoder_path', 'rst_dir', 'emb_dir',
+            'ws_dir', 'hidden_dim', 'lr', 'epoch', 'batch_size', 'gpu_ids',
+        ]
+    )
+    args_need = args_names[data_type]
+    args_need.extend(list(args_names['general']))
+    model_args = {k: config[k] for k in args_need}
+    return BioConfig(data_type, model_args)
+
+
+def train_text_encoder(data_dir: str, save_path: str):
+    """Fine-tune the PubMedBert on 225 Ontologies, except cl and go
+    Parameters
+    ----------
+    data_dir
+        the Ontologies dataset
+    save_path
+        where you save the model
+    """
+    print("Using {} device".format('cuda'))
+    bert_name = 'microsoft/BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext'
+    tokenizer = AutoTokenizer.from_pretrained(bert_name)
+    config = AutoConfig.from_pretrained(bert_name)
+    config.attention_probs_dropout_prob = 0.3
+    config.hidden_dropout_prob = 0.3
+    output_way = 'pooler'
+    assert output_way in ['pooler', 'cls', 'avg']
+
+    lr = 1e-5
+    batch_size = 16
+    max_len = 256
+    print(f'Batch Size: {batch_size}, Max Length: {max_len}')
+
+    model = nn_config(bert_name, output_way, config).to('cuda')
+    optimizer = torch.optim.AdamW(model.parameters(), lr=lr)
+    train_texts, test_texts = get_data(data_dir)
+
+    train_data = TrainOntologyDataset(train_texts, tokenizer, max_len)
+    train_dataloader = DataLoader(train_data, batch_size=batch_size)
+    test_data = TrainOntologyDataset(test_texts, tokenizer, max_len)
+    test_dataloader = DataLoader(test_data, batch_size=batch_size, shuffle=True)
+
+    epochs = 1
+    for t in range(epochs):
+        print(f"Epoch {t + 1}\n-------------------------------")
+        train(train_dataloader, test_dataloader, model, optimizer, save_path, device='cuda')
+    print("Train Done!")
+
+
+def train_biotranslator(cfgs):
+    """Train the BioTranslator
+
+    Parameters
+    ----------
+    cfgs: [config1, config2, config3, ...]
+
+    Returns
+    ------
+    encoder_list
+        List of trained translator
+    """
+    trainer_dict = collections.OrderedDict()
+    translators = collections.OrderedDict()
+    # We may only train one data type each time in this method
+    for cfg in cfgs:
+        if cfg.tp in ['graph', 'seq', 'vec']:
+            files = BioLoader(cfg)
+        else:
+            logging.info('Data type is not supported yet.')
+            raise NotImplementedError
+        trainer_dict[cfg.tp] = (build_trainer(files=files, cfg=cfg), files, cfg)
+    for key, trainer_tup in trainer_dict.items():
+        torch.cuda.set_device(eval(trainer_tup[2].gpu_ids))
+        trainer = trainer_tup[0]
+        print(f'Train encoder for {trainer_tup[2].tp} data:')
+        trainer.train(trainer_tup[1], trainer_tup[2])
+        translators[key] = trainer
+    return translators
+
+
+def test_biotranslator(data_dir, anno_data, cfg, translator, task):
+    """
+    Annotate the proteins with textual description embeddings
+
+    Parameters
+    ----------
+    data_dir: Input data path.
+    anno_data: data needs to be annotated
+    cfg: config
+    translator: biotranslator encoder
+    task: task name
+
+    Returns
+    -------
+    """
+    files = BioLoader(cfg)
+    anno = translator.annotate(files, cfg, data_dir, anno_data, task)
+    return anno
```

### Comparing `biotranslator-0.1.1/biotranslator/config/_config.py` & `biotranslator-0.1.2/biotranslator/config/_config.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-class BioConfig:
-    def __init__(self, data_type, args: dict):
-        # load args
-        self.tp = data_type
-        self.load_args(args)
-        # load dir of the dataaset
-        data_dir = self.data_repo + self.dataset + '/'
-        print("data_dir: ", data_dir)
-        # load dataset file
-        if self.tp == "graph":
-            self.go_file, self.train_file, _, _, \
-            self.train_terms_file, _, self.train_prot_network_file, \
-            self.train_prot_description_file = self.read_dataset_file(data_dir)
-        elif self.tp == "seq":
-            self.go_file, _, self.train_fold_file, self.validation_fold_file, \
-            self.terms_file, self.zero_shot_term_path, self.prot_network_file, \
-            self.prot_description_file = self.read_dataset_file(data_dir)
-
-        if self.tp == "graph":
-            # load pathway dataset file
-            eval_data_dir = self.data_repo + self.eval_dataset + '/'
-            _, _, _, _, \
-            self.eval_terms_file, _, self.eval_prot_network_file, \
-            self.eval_prot_description_file = self.read_dataset_file(eval_data_dir)
-            self.eval_file = eval_data_dir + 'pathway_dataset.pkl'
-        # generate other parameters
-        self.gen_other_parameters()
-
-    def load_args(self, args):
-        # load the settings in args
-        # Note: eval_dataset, task, ontology_repo, max_length, excludes
-        self.dataset = args['dataset'].strip()
-        self.eval_dataset = args['eval_dataset'].strip() if 'eval_dataset' in args else ""
-        self.excludes = args['graph_excludes'] if 'graph_excludes' in args else ""
-        self.method = 'BioTranslator'
-        self.data_repo = args['data_repo'].strip()
-        self.encoder_path = args['encoder_path'].strip()
-        self.ontology_repo = args['vec_ontology_repo'].strip() if 'vec_ontology_repo' in args else ""
-        self.emb_dir = args['emb_dir'].strip()
-        self.task = args['task'].strip() if 'task' in args else ""
-        self.ws_dir = args['ws_dir'].strip()
-        self.rst_dir = args['rst_dir'].strip()
-        self.max_length = args['max_length'] if 'max_length' in args else -1
-        self.hidden_dim = args['hidden_dim']
-        self.features = args['features'].split(', ') if 'features' in args else ""
-        self.lr = args['lr']
-        self.epoch = args['epoch']
-        self.batch_size = args['batch_size']
-        self.gpu_ids = args['gpu_ids'].strip()
-
-    def read_dataset_file(self, data_dir: str):
-        go_file = data_dir + 'go.obo'
-        train_file = data_dir + 'dataset.pkl'
-        train_fold_file = data_dir + 'train_data_fold_{}.pkl'
-        validation_fold_file = data_dir + 'validation_data_fold_{}.pkl'
-        terms_file = data_dir + 'terms.pkl'
-        zero_shot_term_path = data_dir + 'zero_shot_terms_fold_{}.pkl'
-        prot_network_file = data_dir + 'prot_network.pkl'
-        prot_description_file = data_dir + 'prot_description.pkl'
-        return go_file, train_file, train_fold_file, validation_fold_file, terms_file, zero_shot_term_path, prot_network_file, prot_description_file
-
-    def gen_other_parameters(self):
-        # Other parameters
-        # number of amino acids of protein sequences
-        self.seq_input_nc = 21
-        # number of channels in the CNN architecture
-        self.seq_in_nc = 512
-        # the max size of CNN kernels
-        self.seq_max_kernels = 129
-        # the dimension of term text/graph embeddings
-        self.term_enc_dim = 768
-        # where you store the deep learning model
-        self.save_model_path = self.ws_dir + f'{self.task}/' + 'model/{}_{}_{}_{}.pth'
-        # the name of logger file, that contains the information of training process
-        self.logger_name = self.ws_dir + f'{self.task}/log/{self.method}_{self.dataset}.log'
-        # where you save the results of BioTranslator
-        self.results_name = self.ws_dir + f'{self.task}/results/{self.method}_{self.dataset}.pkl'
-        if self.tp in ['seq', 'graph']:
-            if self.tp == 'seq':
-                self.k_fold = 3
-                # load the Diamond score related results
-                if self.task == 'few_shot':
-                    self.diamond_score_path = self.data_repo + self.dataset + '/validation_data_fold_{}.res'
-                    self.blast_preds_path = self.data_repo + self.dataset + '/blast_preds_fold_{}.pkl'
-                    # the alhpa paramter we used in DeepGOPlus
-                    self.ont_term_syn = {'biological_process': 'bp', 'molecular_function': 'mf',
-                                         'cellular_component': 'cc'}
-                    self.alphas = {"mf": 0.68, "bp": 0.63, "cc": 0.46}
-                    self.blast_res_name = self.ws_dir + f'{self.task}/results/{self.method}_{self.dataset}_blast.pkl'
-            elif self.tp == 'graph':
-                # select the nearest k GO term embeddings when annotate the pathway
-                self.nearest_k = 5
-                # get the path of pathway textual description embeddings
-                self.pathway_emb_file = self.data_repo + self.eval_dataset + '/pathway_embeddings.pkl'
-            # get the name of train data textual description embeddings
-            self.emb_name = f'{self.method}_go_embeddings.pkl'
-        elif self.tp == 'vec':
-            # use expression as the features
-            self.features = ['expression']
-            # k-fold cross-validation
-            self.n_iter = 5
-            self.unseen_ratio = [0.9, 0.7, 0.5, 0.3, 0.1]
-            self.nfold_sample = 0.2
-            # the dropout
-            self.drop_out = 0.05
-            # set the memory saving mode to True
-            self.memory_saving_mode = True
-            # where you store the backup files
-            self.backup_file = self.ws_dir + f'{self.task}/cache/sparse_backup_raw.h5ad'
-            # get the name of textual description embeddings
-            self.emb_name = f'{self.method}_co_embeddings.pkl'
-            # when the task is cross_dataset
-            if self.task == 'cross_dataset':
-                self.n_iter = 1
-                self.unseen_ratio = ['cross_dataset']
-                self.save_model_path = self.ws_dir + f'{self.task}/' + 'model/{}_{}_{}.pth'
-                self.logger_name = self.ws_dir + f'{self.task}/log/{self.method}_{self.dataset}_{self.eval_dataset}.log'
-                self.eval_backup_file = self.ws_dir + f'{self.task}/cache/sparse_backup_eval.h5ad'
-                self.results_name = self.ws_dir + f'{self.task}/results/{self.method}_{self.dataset}_{self.eval_dataset}.pkl'
+class BioConfig:
+    def __init__(self, data_type, args: dict):
+        # load args
+        self.tp = data_type
+        self.load_args(args)
+        # load dir of the dataaset
+        data_dir = self.data_repo + self.dataset + '/'
+        print("data_dir: ", data_dir)
+        # load dataset file
+        if self.tp == "graph":
+            self.go_file, self.train_file, _, _, \
+            self.train_terms_file, _, self.train_prot_network_file, \
+            self.train_prot_description_file = self.read_dataset_file(data_dir)
+        elif self.tp == "seq":
+            self.go_file, _, self.train_fold_file, self.validation_fold_file, \
+            self.terms_file, self.zero_shot_term_path, self.prot_network_file, \
+            self.prot_description_file = self.read_dataset_file(data_dir)
+
+        if self.tp == "graph":
+            # load pathway dataset file
+            eval_data_dir = self.data_repo + self.eval_dataset + '/'
+            _, _, _, _, \
+            self.eval_terms_file, _, self.eval_prot_network_file, \
+            self.eval_prot_description_file = self.read_dataset_file(eval_data_dir)
+            self.eval_file = eval_data_dir + 'pathway_dataset.pkl'
+        # generate other parameters
+        self.gen_other_parameters()
+
+    def load_args(self, args):
+        # load the settings in args
+        # Note: eval_dataset, task, ontology_repo, max_length, excludes
+        self.dataset = args['dataset'].strip()
+        self.eval_dataset = args['eval_dataset'].strip() if 'eval_dataset' in args else ""
+        self.excludes = args['graph_excludes'] if 'graph_excludes' in args else ""
+        self.method = 'BioTranslator'
+        self.data_repo = args['data_repo'].strip()
+        self.encoder_path = args['encoder_path'].strip()
+        self.ontology_repo = args['vec_ontology_repo'].strip() if 'vec_ontology_repo' in args else ""
+        self.emb_dir = args['emb_dir'].strip()
+        self.task = args['task'].strip() if 'task' in args else ""
+        self.ws_dir = args['ws_dir'].strip()
+        self.rst_dir = args['rst_dir'].strip()
+        self.max_length = args['max_length'] if 'max_length' in args else -1
+        self.hidden_dim = args['hidden_dim']
+        self.features = args['features'].split(', ') if 'features' in args else ""
+        self.lr = args['lr']
+        self.epoch = args['epoch']
+        self.batch_size = args['batch_size']
+        self.gpu_ids = args['gpu_ids'].strip()
+
+    def read_dataset_file(self, data_dir: str):
+        go_file = data_dir + 'go.obo'
+        train_file = data_dir + 'dataset.pkl'
+        train_fold_file = data_dir + 'train_data_fold_{}.pkl'
+        validation_fold_file = data_dir + 'validation_data_fold_{}.pkl'
+        terms_file = data_dir + 'terms.pkl'
+        zero_shot_term_path = data_dir + 'zero_shot_terms_fold_{}.pkl'
+        prot_network_file = data_dir + 'prot_network.pkl'
+        prot_description_file = data_dir + 'prot_description.pkl'
+        return go_file, train_file, train_fold_file, validation_fold_file, terms_file, zero_shot_term_path, prot_network_file, prot_description_file
+
+    def gen_other_parameters(self):
+        # Other parameters
+        # number of amino acids of protein sequences
+        self.seq_input_nc = 21
+        # number of channels in the CNN architecture
+        self.seq_in_nc = 512
+        # the max size of CNN kernels
+        self.seq_max_kernels = 129
+        # the dimension of term text/graph embeddings
+        self.term_enc_dim = 768
+        # where you store the deep learning model
+        self.save_model_path = self.ws_dir + f'{self.task}/' + 'model/{}_{}_{}_{}.pth'
+        # the name of logger file, that contains the information of training process
+        self.logger_name = self.ws_dir + f'{self.task}/log/{self.method}_{self.dataset}.log'
+        # where you save the results of BioTranslator
+        self.results_name = self.ws_dir + f'{self.task}/results/{self.method}_{self.dataset}.pkl'
+        if self.tp in ['seq', 'graph']:
+            if self.tp == 'seq':
+                self.k_fold = 3
+                # load the Diamond score related results
+                if self.task == 'few_shot':
+                    self.diamond_score_path = self.data_repo + self.dataset + '/validation_data_fold_{}.res'
+                    self.blast_preds_path = self.data_repo + self.dataset + '/blast_preds_fold_{}.pkl'
+                    # the alhpa paramter we used in DeepGOPlus
+                    self.ont_term_syn = {'biological_process': 'bp', 'molecular_function': 'mf',
+                                         'cellular_component': 'cc'}
+                    self.alphas = {"mf": 0.68, "bp": 0.63, "cc": 0.46}
+                    self.blast_res_name = self.ws_dir + f'{self.task}/results/{self.method}_{self.dataset}_blast.pkl'
+            elif self.tp == 'graph':
+                # select the nearest k GO term embeddings when annotate the pathway
+                self.nearest_k = 5
+                # get the path of pathway textual description embeddings
+                self.pathway_emb_file = self.data_repo + self.eval_dataset + '/pathway_embeddings.pkl'
+            # get the name of train data textual description embeddings
+            self.emb_name = f'{self.method}_go_embeddings.pkl'
+        elif self.tp == 'vec':
+            # use expression as the features
+            self.features = ['expression']
+            # k-fold cross-validation
+            self.n_iter = 5
+            self.unseen_ratio = [0.9, 0.7, 0.5, 0.3, 0.1]
+            self.nfold_sample = 0.2
+            # the dropout
+            self.drop_out = 0.05
+            # set the memory saving mode to True
+            self.memory_saving_mode = True
+            # where you store the backup files
+            self.backup_file = self.ws_dir + f'{self.task}/cache/sparse_backup_raw.h5ad'
+            # get the name of textual description embeddings
+            self.emb_name = f'{self.method}_co_embeddings.pkl'
+            # when the task is cross_dataset
+            if self.task == 'cross_dataset':
+                self.n_iter = 1
+                self.unseen_ratio = ['cross_dataset']
+                self.save_model_path = self.ws_dir + f'{self.task}/' + 'model/{}_{}_{}.pth'
+                self.logger_name = self.ws_dir + f'{self.task}/log/{self.method}_{self.dataset}_{self.eval_dataset}.log'
+                self.eval_backup_file = self.ws_dir + f'{self.task}/cache/sparse_backup_eval.h5ad'
+                self.results_name = self.ws_dir + f'{self.task}/results/{self.method}_{self.dataset}_{self.eval_dataset}.pkl'
```

### Comparing `biotranslator-0.1.1/biotranslator/loader/_bioloader.py` & `biotranslator-0.1.2/biotranslator/loader/_bioloader.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-"""
-Non-text Encoder
-"""
-
-import os
-import numpy as np
-import pandas as pd
-import collections
-from tqdm import tqdm
-from ..utils import load, load_obj, proteinData, emb2tensor, organize_workingspace, \
-    term_training_numbers, extract_terms_from_dataset, cellData, SplitTrainTest, find_gene_ind, \
-    DataProcessing, read_data, read_data_file, read_ontology_file, get_ontology_embeddings
-
-
-class BioLoader:
-    """
-    This class loads and stores the data we used in BioTranslator
-    """
-
-    def __init__(self, cfg):
-        # Organize the working space
-        organize_workingspace(cfg.ws_dir, cfg.task)
-        if cfg.tp in ["graph", "seq"]:
-            # load gene ontology data
-            self.go_data = load(cfg.go_file)
-            # load mappings between terms and index, also find the intersection with go terms
-            self.load_terms(cfg)
-            if cfg.tp == 'graph':
-                # load proteins which need to be excluded
-                self.load_eval_uniprots(cfg)
-            # load dataset
-            self.load_dataset(cfg)
-            if cfg.tp == 'seq':
-                # register dataset for zero shot task or few shot task
-                self.register_task(cfg)
-            # generate proteinData, which is defined in BioUtils
-            self.gen_protein_data(cfg)
-        # load textual description embeddings of go or co terms
-        self.load_text_emb(cfg)
-        if cfg.tp == 'vec':
-            # load files
-            self.load_files(cfg)
-        print('Data Loading Finished!')
-
-    def load_files(self, cfg):
-        self.cfg = cfg
-        self.terms_with_def = self.text_embeddings.keys()
-        self.cell_type_nlp_emb_file, self.cell_type_network_file, self.cl_obo_file = read_ontology_file(
-            'cell ontology', cfg.ontology_repo)
-        self.DataProcess_obj = DataProcessing(self.cell_type_network_file, self.cell_type_nlp_emb_file,
-                                              memory_saving_mode=cfg.memory_saving_mode,
-                                              terms_with_def=self.terms_with_def)
-        feature_file, filter_key, label_key, label_file, gene_file = read_data_file(cfg.dataset, cfg.data_repo)
-        self.feature, self.genes, self.label, _, _ = read_data(feature_file,
-                                                               cell_ontology_ids=self.DataProcess_obj.cell_ontology_ids,
-                                                               exclude_non_leaf_ontology=True, tissue_key='tissue',
-                                                               filter_key=filter_key, AnnData_label_key=label_key,
-                                                               nlp_mapping=False, cl_obo_file=self.cl_obo_file,
-                                                               cell_ontology_file=self.cell_type_network_file,
-                                                               co2emb=self.DataProcess_obj.co2vec_nlp,
-                                                               memory_saving_mode=cfg.memory_saving_mode,
-                                                               backup_file=cfg.backup_file)
-
-    def load_terms(self, cfg):
-        if cfg.tp == "graph":
-            terms = pd.read_pickle(cfg.train_terms_file)
-        elif cfg.tp == "seq":
-            terms = pd.read_pickle(cfg.terms_file)
-        else:
-            raise NotImplementedError
-        self.i2terms = list(terms['terms'])
-        go_terms = list(self.go_data.keys())
-        self.i2terms = list(set(self.i2terms).intersection(set(go_terms)))
-        self.terms2i = collections.OrderedDict()
-        self.n_classes = len(self.i2terms)
-        print('terms number:{}'.format(len(self.i2terms)))
-        for i in range(len(self.i2terms)): self.terms2i[self.i2terms[i]] = i
-
-    def load_eval_uniprots(self, cfg):
-        eval_dataset = cfg.excludes
-        eval_uniprots = []
-        for d in eval_dataset:
-            data_i = load_obj(cfg.data_repo + d + '/pathway_dataset.pkl')
-            eval_uniprots += list(data_i['proteins'])
-        self.eval_uniprots = set(eval_uniprots)
-
-    def load_dataset(self, cfg):
-        if cfg.tp == 'graph':
-            # load train dataset
-            self.train_data = pd.read_pickle(cfg.train_file)
-
-            # exclude proteins in pathway dataset from the train data
-            drop_index = []
-            for i in self.train_data.index:
-                if self.train_data.loc[i]['proteins'] in self.eval_uniprots:
-                    drop_index.append(i)
-            self.train_data = self.train_data.drop(index=drop_index)
-
-            # load protein network fatures and description features
-            self.train_prot_network = load_obj(cfg.train_prot_network_file)
-            self.network_dim = np.size(list(self.train_prot_network.values())[0])
-            self.train_prot_description = load_obj(cfg.train_prot_description_file)
-
-            # load eval dataset (pathway dataset)
-            self.eval_data = pd.read_pickle(cfg.eval_file)
-            self.eval_prot_network = load_obj(cfg.eval_prot_network_file)
-            self.eval_prot_description = load_obj(cfg.eval_prot_description_file)
-
-            # load eval terms
-            self.eval_terms2i, self.eval_i2terms = extract_terms_from_dataset(self.eval_data)
-            print('eval pathway number:{}'.format(len(self.eval_i2terms)))
-        elif cfg.tp == 'seq':
-            self.k_fold = cfg.k_fold
-            self.fold_train, self.fold_val = self.load_fold_data(cfg.k_fold,
-                                                                 cfg.train_fold_file,
-                                                                 cfg.validation_fold_file)
-
-            # load protein network fatures and description features
-            self.prot_network = load_obj(cfg.prot_network_file)
-            self.network_dim = np.size(list(self.prot_network.values())[0])
-            self.prot_description = load_obj(cfg.prot_description_file)
-
-    def register_task(self, cfg):
-        if cfg.task == 'zero_shot':
-            self.fold_zero_shot_terms_list = self.zero_shot_terms(cfg)
-            self.zero_shot_fold_data(self.fold_zero_shot_terms_list)
-            for fold_i in range(cfg.k_fold):
-                print('Fold {} contains {} zero shot terms'.format(fold_i,
-                                                                   len(self.fold_zero_shot_terms_list[fold_i])))
-        if cfg.task == 'few_shot':
-            self.fold_few_shot_terms_list = self.few_shot_terms(cfg)
-            self.diamond_list = self.load_diamond_score(cfg)
-
-    def gen_protein_data(self, cfg):
-        # generate protein data which can be loaded by torch
-        # the raw train and test data is for blast preds function in BioTrainer
-        if cfg.tp == 'graph':
-            self.raw_train, self.raw_val = self.train_data.copy(deep=True), self.eval_data.copy(deep=True)
-
-            self.train_data = proteinData(self.train_data, self.terms2i, self.train_prot_network,
-                                          self.train_prot_description, gpu_ids=cfg.gpu_ids)
-            self.eval_data = proteinData(self.eval_data, self.eval_terms2i, self.eval_prot_network,
-                                         self.eval_prot_description, gpu_ids=cfg.gpu_ids)
-        elif cfg.tp == 'seq':
-            # generate protein data which can be loaded by torch
-            # the raw train and test data is for blast preds function in BioTrainer
-            self.raw_train, self.raw_val = [], []
-            for fold_i in range(cfg.k_fold):
-                self.raw_train.append(self.fold_train[fold_i].copy(deep=True))
-                self.raw_val.append(self.fold_val[fold_i].copy(deep=True))
-                self.fold_train[fold_i] = proteinData(self.fold_train[fold_i], self.terms2i, self.prot_network,
-                                            self.prot_description, gpu_ids = cfg.gpu_ids)
-                self.fold_val[fold_i] = proteinData(self.fold_val[fold_i], self.terms2i, self.prot_network,
-                                          self.prot_description, gpu_ids = cfg.gpu_ids)
-
-
-    def zero_shot_fold_data(self, fold_zero_shot_terms_list):
-        for i in range(self.k_fold):
-            zero_terms_k = fold_zero_shot_terms_list[i]
-            training, valid = self.fold_train[i], self.fold_val[i]
-            drop_index = []
-            for j in training.index:
-                annts = training.loc[j]['annotations']
-                insct = list(set(annts).intersection(zero_terms_k))
-                if len(insct) > 0: drop_index.append(j)
-            self.fold_train[i] = training.drop(index=drop_index)
-
-    def zero_shot_terms(self, cfg):
-        fold_zero_shot_terms = []
-        for i in tqdm(range(cfg.k_fold)):
-            fold_zero_shot_terms.append(load_obj(cfg.zero_shot_term_path.format(i)))
-        return fold_zero_shot_terms
-
-    def few_shot_terms(self, cfg):
-        fold_few_shot_terms = []
-        for i in tqdm(range(cfg.k_fold)):
-            few_shot_terms = collections.OrderedDict()
-            few_shot_count = term_training_numbers(self.fold_val[i], self.fold_train[i])
-            for j in few_shot_count.keys():
-                if 0 < few_shot_count[j] <= 20:
-                    few_shot_terms[j] = few_shot_count[j]
-            fold_few_shot_terms.append(few_shot_terms)
-        return fold_few_shot_terms
-
-    def load_fold_data(self, k, train_fold_file, validation_fold_file):
-        train_fold, val_fold = [], []
-        for i in range(k):
-            train_fold.append(pd.read_pickle(train_fold_file.format(i)))
-            val_fold.append(pd.read_pickle(validation_fold_file.format(i)))
-        return train_fold, val_fold
-
-    def load_diamond_score(self, cfg):
-        diamond_list = []
-        for i in range(cfg.k_fold):
-            diamond_scores = {}
-            with open(cfg.diamond_score_path.format(i)) as f:
-                for line in f:
-                    it = line.strip().split()
-                    if it[0] not in diamond_scores:
-                        diamond_scores[it[0]] = {}
-                    diamond_scores[it[0]][it[1]] = float(it[2])
-            diamond_list.append(diamond_scores)
-        return diamond_list
-
-    def load_text_emb(self, cfg):
-        if not os.path.exists(cfg.emb_dir):
-            os.mkdir(cfg.emb_dir)
-            print('Warning: We created the embedding folder: {}'.format(cfg.emb_dir))
-        if cfg.emb_name not in os.listdir(cfg.emb_dir):
-            get_ontology_embeddings(cfg)
-        cfg.text_embedding_file = cfg.emb_dir + cfg.emb_name
-        self.text_embeddings = pd.read_pickle(cfg.text_embedding_file)
-        if cfg.tp in ['graph', 'seq']:
-            self.text_embeddings = emb2tensor(self.text_embeddings, self.terms2i)
-            if cfg.tp == 'graph':
-                self.pathway_embeddings = pd.read_pickle(cfg.pathway_emb_file)
-                self.pathway_embeddings = emb2tensor(self.pathway_embeddings, self.eval_terms2i)
-            if len(cfg.gpu_ids) > 0:
-                self.text_embeddings = self.text_embeddings.float().cuda()
-                if cfg.tp == 'graph':
-                    self.pathway_embeddings = self.pathway_embeddings.float().cuda()
-
-    def read_eval_files(self, cfg, eval_dname):
-        feature_file, filter_key, label_key, label_file, gene_file = read_data_file(eval_dname, cfg.data_repo)
-        self.eval_feature, self.eval_genes, self.eval_label, _, _ = read_data(feature_file,
-                                                                              cell_ontology_ids=self.DataProcess_obj.cell_ontology_ids,
-                                                                                 exclude_non_leaf_ontology=True,tissue_key='tissue',
-                                                                                 filter_key=filter_key, AnnData_label_key=label_key,
-                                                                                 nlp_mapping=False, cl_obo_file=self.cl_obo_file,
-                                                                                 cell_ontology_file=self.cell_type_network_file,
-                                                                                 co2emb=self.DataProcess_obj.co2vec_nlp,
-                                                                              memory_saving_mode=cfg.memory_saving_mode,
-                                                                                 backup_file=cfg.eval_backup_file)
-
-    def generate_data(self, iter=None, unseen_ratio=None):
-        if self.cfg.task == 'same_dataset':
-            train_feature, train_label, test_feature, test_label = SplitTrainTest(self.feature,
-                                                                                  self.label,
-                                                                                  nfold_cls=unseen_ratio,
-                                                                                  nfold_sample=self. cfg.nfold_sample,
-                                                                                  random_state=iter,
-                                                                                  memory_saving_mode=self.cfg.memory_saving_mode)
-            train_genes, test_genes = self.genes, self.genes
-            self.DataProcess_obj.EmbedCellTypes(train_label)
-            train_feature, test_feature, train_genes, test_genes = self.DataProcess_obj.ProcessTrainFeature(
-                train_feature, train_label, train_genes, test_feature=test_feature, test_genes=test_genes,
-                batch_correct=False)
-
-            test_feature, mapping = self.DataProcess_obj.ProcessTestFeature(test_feature, test_genes, log_transform=False)
-
-            self.unseen2i = collections.OrderedDict()
-            self.train2i = collections.OrderedDict()
-            self.test2i = collections.OrderedDict()
-            idx = 0
-            for x in set(train_label):
-                self.train2i[x] = idx
-                idx += 1
-
-            idx = 0
-            for x in set(test_label).union(set(train_label)):
-                self.test2i[x] = idx
-                if x not in set(train_label):
-                    self.unseen2i[x] = idx
-                idx += 1
-
-            train_label = [self.train2i[x] for x in train_label]
-            test_label = [self.test2i[x] for x in test_label]
-
-            self.train_data = cellData(train_feature, train_label, nlabel=len(self.train2i.keys()), gpu_ids=self.cfg.gpu_ids)
-            self.test_data = cellData(test_feature, test_label, nlabel=len(self.test2i.keys()), gpu_ids=self.cfg.gpu_ids)
-
-            self.train_emb = emb2tensor(self.text_embeddings, self.train2i)
-            if len(self.cfg.gpu_ids) > 0:
-                self.train_emb = self.train_emb.cuda()
-            self.test_emb = emb2tensor(self.text_embeddings, self.test2i)
-            if len(self.cfg.gpu_ids) > 0:
-                self.test_emb = self.test_emb.cuda()
-
-            self.train_genes = train_genes
-            self.test_genes = test_genes
-            self.ngene = len(train_genes)
-            self.ndim = self.train_emb.size(1)
-
-        elif self.cfg.task == 'cross_dataset':
-            self.read_eval_files(self.cfg, self.cfg.eval_dataset)
-            common_genes = np.sort(list(set(self.genes) & set(self.eval_genes)))
-            gid1 = find_gene_ind(self.genes, common_genes)
-            gid2 = find_gene_ind(self.eval_genes, common_genes)
-            train_feature = self.feature[:, gid1]
-            eval_feature = self.eval_feature[:, gid2]
-            train_genes = common_genes
-            eval_genes = common_genes
-            self.DataProcess_obj.EmbedCellTypes(self.label)
-            train_feature, eval_feature, train_genes, test_genes = self.DataProcess_obj.ProcessTrainFeature(
-                train_feature, self.label, train_genes, test_feature=eval_feature, test_genes=eval_genes,
-                batch_correct=False)
-
-            if self.cfg.memory_saving_mode:
-                eval_feature, mapping = self.DataProcess_obj.ProcessTestFeature(eval_feature, eval_genes,
-                                                                                log_transform=False)
-                train_feature = train_feature.tocsr()
-                eval_feature = eval_feature.tocsr()
-            else:
-                eval_feature = self.DataProcess_obj.ProcessTestFeature(eval_feature, eval_genes,
-                                                                       log_transform=False)
-            self.unseen2i = collections.OrderedDict()
-            self.train2i = collections.OrderedDict()
-            self.test2i = collections.OrderedDict()
-            idx = 0
-            for x in set(self.label):
-                self.train2i[x] = idx
-                idx += 1
-            idx = 0
-            for x in set(self.eval_label):
-                self.test2i[x] = idx
-                if x not in self.train2i.keys():
-                    self.unseen2i[x] = idx
-                idx += 1
-            train_label = [self.train2i[x] for x in self.label]
-            test_label = [self.test2i[x] for x in self.eval_label]
-            self.train_data = cellData(train_feature, train_label, nlabel=len(self.train2i.keys()), gpu_ids=self.cfg.gpu_ids)
-            self.test_data = cellData(eval_feature, test_label, nlabel=len(self.test2i.keys()), gpu_ids=self.cfg.gpu_ids)
-            self.train_emb = emb2tensor(self.text_embeddings, self.train2i)
-            if len(self.cfg.gpu_ids) > 0:
-                self.train_emb = self.train_emb.cuda()
-            self.test_emb = emb2tensor(self.text_embeddings, self.test2i)
-            if len(self.cfg.gpu_ids) > 0:
-                self.test_emb = self.test_emb.cuda()
-            self.ngene = len(train_genes)
-            self.ndim = self.train_emb.size(1)
+"""
+Non-text Encoder
+"""
+
+import os
+import numpy as np
+import pandas as pd
+import collections
+from tqdm import tqdm
+from ..utils import load, load_obj, proteinData, emb2tensor, organize_workingspace, \
+    term_training_numbers, extract_terms_from_dataset, cellData, SplitTrainTest, find_gene_ind, \
+    DataProcessing, read_data, read_data_file, read_ontology_file, get_ontology_embeddings
+
+
+class BioLoader:
+    """
+    This class loads and stores the data we used in BioTranslator
+    """
+
+    def __init__(self, cfg):
+        # Organize the working space
+        organize_workingspace(cfg.ws_dir, cfg.task)
+        if cfg.tp in ["graph", "seq"]:
+            # load gene ontology data
+            self.go_data = load(cfg.go_file)
+            # load mappings between terms and index, also find the intersection with go terms
+            self.load_terms(cfg)
+            if cfg.tp == 'graph':
+                # load proteins which need to be excluded
+                self.load_eval_uniprots(cfg)
+            # load dataset
+            self.load_dataset(cfg)
+            if cfg.tp == 'seq':
+                # register dataset for zero shot task or few shot task
+                self.register_task(cfg)
+            # generate proteinData, which is defined in BioUtils
+            self.gen_protein_data(cfg)
+        # load textual description embeddings of go or co terms
+        self.load_text_emb(cfg)
+        if cfg.tp == 'vec':
+            # load files
+            self.load_files(cfg)
+        print('Data Loading Finished!')
+
+    def load_files(self, cfg):
+        self.cfg = cfg
+        self.terms_with_def = self.text_embeddings.keys()
+        self.cell_type_nlp_emb_file, self.cell_type_network_file, self.cl_obo_file = read_ontology_file(
+            'cell ontology', cfg.ontology_repo)
+        self.DataProcess_obj = DataProcessing(self.cell_type_network_file, self.cell_type_nlp_emb_file,
+                                              memory_saving_mode=cfg.memory_saving_mode,
+                                              terms_with_def=self.terms_with_def)
+        feature_file, filter_key, label_key, label_file, gene_file = read_data_file(cfg.dataset, cfg.data_repo)
+        self.feature, self.genes, self.label, _, _ = read_data(feature_file,
+                                                               cell_ontology_ids=self.DataProcess_obj.cell_ontology_ids,
+                                                               exclude_non_leaf_ontology=True, tissue_key='tissue',
+                                                               filter_key=filter_key, AnnData_label_key=label_key,
+                                                               nlp_mapping=False, cl_obo_file=self.cl_obo_file,
+                                                               cell_ontology_file=self.cell_type_network_file,
+                                                               co2emb=self.DataProcess_obj.co2vec_nlp,
+                                                               memory_saving_mode=cfg.memory_saving_mode,
+                                                               backup_file=cfg.backup_file)
+
+    def load_terms(self, cfg):
+        if cfg.tp == "graph":
+            terms = pd.read_pickle(cfg.train_terms_file)
+        elif cfg.tp == "seq":
+            terms = pd.read_pickle(cfg.terms_file)
+        else:
+            raise NotImplementedError
+        self.i2terms = list(terms['terms'])
+        go_terms = list(self.go_data.keys())
+        self.i2terms = list(set(self.i2terms).intersection(set(go_terms)))
+        self.terms2i = collections.OrderedDict()
+        self.n_classes = len(self.i2terms)
+        print('terms number:{}'.format(len(self.i2terms)))
+        for i in range(len(self.i2terms)): self.terms2i[self.i2terms[i]] = i
+
+    def load_eval_uniprots(self, cfg):
+        eval_dataset = cfg.excludes
+        eval_uniprots = []
+        for d in eval_dataset:
+            data_i = load_obj(cfg.data_repo + d + '/pathway_dataset.pkl')
+            eval_uniprots += list(data_i['proteins'])
+        self.eval_uniprots = set(eval_uniprots)
+
+    def load_dataset(self, cfg):
+        if cfg.tp == 'graph':
+            # load train dataset
+            self.train_data = pd.read_pickle(cfg.train_file)
+
+            # exclude proteins in pathway dataset from the train data
+            drop_index = []
+            for i in self.train_data.index:
+                if self.train_data.loc[i]['proteins'] in self.eval_uniprots:
+                    drop_index.append(i)
+            self.train_data = self.train_data.drop(index=drop_index)
+
+            # load protein network fatures and description features
+            self.train_prot_network = load_obj(cfg.train_prot_network_file)
+            self.network_dim = np.size(list(self.train_prot_network.values())[0])
+            self.train_prot_description = load_obj(cfg.train_prot_description_file)
+
+            # load eval dataset (pathway dataset)
+            self.eval_data = pd.read_pickle(cfg.eval_file)
+            self.eval_prot_network = load_obj(cfg.eval_prot_network_file)
+            self.eval_prot_description = load_obj(cfg.eval_prot_description_file)
+
+            # load eval terms
+            self.eval_terms2i, self.eval_i2terms = extract_terms_from_dataset(self.eval_data)
+            print('eval pathway number:{}'.format(len(self.eval_i2terms)))
+        elif cfg.tp == 'seq':
+            self.k_fold = cfg.k_fold
+            self.fold_train, self.fold_val = self.load_fold_data(cfg.k_fold,
+                                                                 cfg.train_fold_file,
+                                                                 cfg.validation_fold_file)
+
+            # load protein network fatures and description features
+            self.prot_network = load_obj(cfg.prot_network_file)
+            self.network_dim = np.size(list(self.prot_network.values())[0])
+            self.prot_description = load_obj(cfg.prot_description_file)
+
+    def register_task(self, cfg):
+        if cfg.task == 'zero_shot':
+            self.fold_zero_shot_terms_list = self.zero_shot_terms(cfg)
+            self.zero_shot_fold_data(self.fold_zero_shot_terms_list)
+            for fold_i in range(cfg.k_fold):
+                print('Fold {} contains {} zero shot terms'.format(fold_i,
+                                                                   len(self.fold_zero_shot_terms_list[fold_i])))
+        if cfg.task == 'few_shot':
+            self.fold_few_shot_terms_list = self.few_shot_terms(cfg)
+            self.diamond_list = self.load_diamond_score(cfg)
+
+    def gen_protein_data(self, cfg):
+        # generate protein data which can be loaded by torch
+        # the raw train and test data is for blast preds function in BioTrainer
+        if cfg.tp == 'graph':
+            self.raw_train, self.raw_val = self.train_data.copy(deep=True), self.eval_data.copy(deep=True)
+
+            self.train_data = proteinData(self.train_data, self.terms2i, self.train_prot_network,
+                                          self.train_prot_description, gpu_ids=cfg.gpu_ids)
+            self.eval_data = proteinData(self.eval_data, self.eval_terms2i, self.eval_prot_network,
+                                         self.eval_prot_description, gpu_ids=cfg.gpu_ids)
+        elif cfg.tp == 'seq':
+            # generate protein data which can be loaded by torch
+            # the raw train and test data is for blast preds function in BioTrainer
+            self.raw_train, self.raw_val = [], []
+            for fold_i in range(cfg.k_fold):
+                self.raw_train.append(self.fold_train[fold_i].copy(deep=True))
+                self.raw_val.append(self.fold_val[fold_i].copy(deep=True))
+                self.fold_train[fold_i] = proteinData(self.fold_train[fold_i], self.terms2i, self.prot_network,
+                                            self.prot_description, gpu_ids = cfg.gpu_ids)
+                self.fold_val[fold_i] = proteinData(self.fold_val[fold_i], self.terms2i, self.prot_network,
+                                          self.prot_description, gpu_ids = cfg.gpu_ids)
+
+
+    def zero_shot_fold_data(self, fold_zero_shot_terms_list):
+        for i in range(self.k_fold):
+            zero_terms_k = fold_zero_shot_terms_list[i]
+            training, valid = self.fold_train[i], self.fold_val[i]
+            drop_index = []
+            for j in training.index:
+                annts = training.loc[j]['annotations']
+                insct = list(set(annts).intersection(zero_terms_k))
+                if len(insct) > 0: drop_index.append(j)
+            self.fold_train[i] = training.drop(index=drop_index)
+
+    def zero_shot_terms(self, cfg):
+        fold_zero_shot_terms = []
+        for i in tqdm(range(cfg.k_fold)):
+            fold_zero_shot_terms.append(load_obj(cfg.zero_shot_term_path.format(i)))
+        return fold_zero_shot_terms
+
+    def few_shot_terms(self, cfg):
+        fold_few_shot_terms = []
+        for i in tqdm(range(cfg.k_fold)):
+            few_shot_terms = collections.OrderedDict()
+            few_shot_count = term_training_numbers(self.fold_val[i], self.fold_train[i])
+            for j in few_shot_count.keys():
+                if 0 < few_shot_count[j] <= 20:
+                    few_shot_terms[j] = few_shot_count[j]
+            fold_few_shot_terms.append(few_shot_terms)
+        return fold_few_shot_terms
+
+    def load_fold_data(self, k, train_fold_file, validation_fold_file):
+        train_fold, val_fold = [], []
+        for i in range(k):
+            train_fold.append(pd.read_pickle(train_fold_file.format(i)))
+            val_fold.append(pd.read_pickle(validation_fold_file.format(i)))
+        return train_fold, val_fold
+
+    def load_diamond_score(self, cfg):
+        diamond_list = []
+        for i in range(cfg.k_fold):
+            diamond_scores = {}
+            with open(cfg.diamond_score_path.format(i)) as f:
+                for line in f:
+                    it = line.strip().split()
+                    if it[0] not in diamond_scores:
+                        diamond_scores[it[0]] = {}
+                    diamond_scores[it[0]][it[1]] = float(it[2])
+            diamond_list.append(diamond_scores)
+        return diamond_list
+
+    def load_text_emb(self, cfg):
+        if not os.path.exists(cfg.emb_dir):
+            os.mkdir(cfg.emb_dir)
+            print('Warning: We created the embedding folder: {}'.format(cfg.emb_dir))
+        if cfg.emb_name not in os.listdir(cfg.emb_dir):
+            get_ontology_embeddings(cfg)
+        cfg.text_embedding_file = cfg.emb_dir + cfg.emb_name
+        self.text_embeddings = pd.read_pickle(cfg.text_embedding_file)
+        if cfg.tp in ['graph', 'seq']:
+            self.text_embeddings = emb2tensor(self.text_embeddings, self.terms2i)
+            if cfg.tp == 'graph':
+                self.pathway_embeddings = pd.read_pickle(cfg.pathway_emb_file)
+                self.pathway_embeddings = emb2tensor(self.pathway_embeddings, self.eval_terms2i)
+            if len(cfg.gpu_ids) > 0:
+                self.text_embeddings = self.text_embeddings.float().cuda()
+                if cfg.tp == 'graph':
+                    self.pathway_embeddings = self.pathway_embeddings.float().cuda()
+
+    def read_eval_files(self, cfg, eval_dname):
+        feature_file, filter_key, label_key, label_file, gene_file = read_data_file(eval_dname, cfg.data_repo)
+        self.eval_feature, self.eval_genes, self.eval_label, _, _ = read_data(feature_file,
+                                                                              cell_ontology_ids=self.DataProcess_obj.cell_ontology_ids,
+                                                                                 exclude_non_leaf_ontology=True,tissue_key='tissue',
+                                                                                 filter_key=filter_key, AnnData_label_key=label_key,
+                                                                                 nlp_mapping=False, cl_obo_file=self.cl_obo_file,
+                                                                                 cell_ontology_file=self.cell_type_network_file,
+                                                                                 co2emb=self.DataProcess_obj.co2vec_nlp,
+                                                                              memory_saving_mode=cfg.memory_saving_mode,
+                                                                                 backup_file=cfg.eval_backup_file)
+
+    def generate_data(self, iter=None, unseen_ratio=None):
+        if self.cfg.task == 'same_dataset':
+            train_feature, train_label, test_feature, test_label = SplitTrainTest(self.feature,
+                                                                                  self.label,
+                                                                                  nfold_cls=unseen_ratio,
+                                                                                  nfold_sample=self. cfg.nfold_sample,
+                                                                                  random_state=iter,
+                                                                                  memory_saving_mode=self.cfg.memory_saving_mode)
+            train_genes, test_genes = self.genes, self.genes
+            self.DataProcess_obj.EmbedCellTypes(train_label)
+            train_feature, test_feature, train_genes, test_genes = self.DataProcess_obj.ProcessTrainFeature(
+                train_feature, train_label, train_genes, test_feature=test_feature, test_genes=test_genes,
+                batch_correct=False)
+
+            test_feature, mapping = self.DataProcess_obj.ProcessTestFeature(test_feature, test_genes, log_transform=False)
+
+            self.unseen2i = collections.OrderedDict()
+            self.train2i = collections.OrderedDict()
+            self.test2i = collections.OrderedDict()
+            idx = 0
+            for x in set(train_label):
+                self.train2i[x] = idx
+                idx += 1
+
+            idx = 0
+            for x in set(test_label).union(set(train_label)):
+                self.test2i[x] = idx
+                if x not in set(train_label):
+                    self.unseen2i[x] = idx
+                idx += 1
+
+            train_label = [self.train2i[x] for x in train_label]
+            test_label = [self.test2i[x] for x in test_label]
+
+            self.train_data = cellData(train_feature, train_label, nlabel=len(self.train2i.keys()), gpu_ids=self.cfg.gpu_ids)
+            self.test_data = cellData(test_feature, test_label, nlabel=len(self.test2i.keys()), gpu_ids=self.cfg.gpu_ids)
+
+            self.train_emb = emb2tensor(self.text_embeddings, self.train2i)
+            if len(self.cfg.gpu_ids) > 0:
+                self.train_emb = self.train_emb.cuda()
+            self.test_emb = emb2tensor(self.text_embeddings, self.test2i)
+            if len(self.cfg.gpu_ids) > 0:
+                self.test_emb = self.test_emb.cuda()
+
+            self.train_genes = train_genes
+            self.test_genes = test_genes
+            self.ngene = len(train_genes)
+            self.ndim = self.train_emb.size(1)
+
+        elif self.cfg.task == 'cross_dataset':
+            self.read_eval_files(self.cfg, self.cfg.eval_dataset)
+            common_genes = np.sort(list(set(self.genes) & set(self.eval_genes)))
+            gid1 = find_gene_ind(self.genes, common_genes)
+            gid2 = find_gene_ind(self.eval_genes, common_genes)
+            train_feature = self.feature[:, gid1]
+            eval_feature = self.eval_feature[:, gid2]
+            train_genes = common_genes
+            eval_genes = common_genes
+            self.DataProcess_obj.EmbedCellTypes(self.label)
+            train_feature, eval_feature, train_genes, test_genes = self.DataProcess_obj.ProcessTrainFeature(
+                train_feature, self.label, train_genes, test_feature=eval_feature, test_genes=eval_genes,
+                batch_correct=False)
+
+            if self.cfg.memory_saving_mode:
+                eval_feature, mapping = self.DataProcess_obj.ProcessTestFeature(eval_feature, eval_genes,
+                                                                                log_transform=False)
+                train_feature = train_feature.tocsr()
+                eval_feature = eval_feature.tocsr()
+            else:
+                eval_feature = self.DataProcess_obj.ProcessTestFeature(eval_feature, eval_genes,
+                                                                       log_transform=False)
+            self.unseen2i = collections.OrderedDict()
+            self.train2i = collections.OrderedDict()
+            self.test2i = collections.OrderedDict()
+            idx = 0
+            for x in set(self.label):
+                self.train2i[x] = idx
+                idx += 1
+            idx = 0
+            for x in set(self.eval_label):
+                self.test2i[x] = idx
+                if x not in self.train2i.keys():
+                    self.unseen2i[x] = idx
+                idx += 1
+            train_label = [self.train2i[x] for x in self.label]
+            test_label = [self.test2i[x] for x in self.eval_label]
+            self.train_data = cellData(train_feature, train_label, nlabel=len(self.train2i.keys()), gpu_ids=self.cfg.gpu_ids)
+            self.test_data = cellData(eval_feature, test_label, nlabel=len(self.test2i.keys()), gpu_ids=self.cfg.gpu_ids)
+            self.train_emb = emb2tensor(self.text_embeddings, self.train2i)
+            if len(self.cfg.gpu_ids) > 0:
+                self.train_emb = self.train_emb.cuda()
+            self.test_emb = emb2tensor(self.text_embeddings, self.test2i)
+            if len(self.cfg.gpu_ids) > 0:
+                self.test_emb = self.test_emb.cuda()
+            self.ngene = len(train_genes)
+            self.ndim = self.train_emb.size(1)
```

### Comparing `biotranslator-0.1.1/biotranslator/metrics/_auroc.py` & `biotranslator-0.1.2/biotranslator/metrics/_auroc.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import numpy as np
-from ._roc import compute_roc
-
-
-def auroc_metrics(labels, preds):
-    roc_matrix = np.zeros(np.size(preds, 1))
-    for i in range(len(roc_matrix)):
-        pred_i, label_i = preds[:, i], labels[:, i]
-        auroc = compute_roc(label_i, pred_i)
-        roc_matrix[i] = auroc
-
-    auroc_percentage = {0.65: 0, 0.7: 0, 0.75: 0, 0.8: 0, 0.85: 0, 0.95: 0}
-    for j in range(np.size(preds, 1)):
-        preds_id = preds[:, j].reshape([-1, 1])
-        label_id = labels[:, j].reshape([-1, 1])
-        roc_auc_j = compute_roc(label_id, preds_id)
-        for T in auroc_percentage.keys():
-            if T <= roc_auc_j:
-                auroc_percentage[T] += 100.0 / np.size(preds, 1)
-    return np.mean(roc_matrix), auroc_percentage
+import numpy as np
+from ._roc import compute_roc
+
+
+def auroc_metrics(labels, preds):
+    roc_matrix = np.zeros(np.size(preds, 1))
+    for i in range(len(roc_matrix)):
+        pred_i, label_i = preds[:, i], labels[:, i]
+        auroc = compute_roc(label_i, pred_i)
+        roc_matrix[i] = auroc
+
+    auroc_percentage = {0.65: 0, 0.7: 0, 0.75: 0, 0.8: 0, 0.85: 0, 0.95: 0}
+    for j in range(np.size(preds, 1)):
+        preds_id = preds[:, j].reshape([-1, 1])
+        label_id = labels[:, j].reshape([-1, 1])
+        roc_auc_j = compute_roc(label_id, preds_id)
+        for T in auroc_percentage.keys():
+            if T <= roc_auc_j:
+                auroc_percentage[T] += 100.0 / np.size(preds, 1)
+    return np.mean(roc_matrix), auroc_percentage
```

### Comparing `biotranslator-0.1.1/biotranslator/text_encoder/_datasets.py` & `biotranslator-0.1.2/biotranslator/text_encoder/_datasets.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import torch
-import os
-import json
-import random
-from tqdm import tqdm
-import torch.nn as nn
-from torch.nn import functional as F
-from torch.utils.data import Dataset, DataLoader
-from transformers import AutoTokenizer, AutoModel, AutoConfig
-import scipy.stats
-import numpy as np
-
-
-class TrainOntologyDataset(Dataset):
-    def __init__(self, data, tokenizer, max_len, transform=None, target_transform=None):
-        self.data = data
-        self.tokenizer = tokenizer
-        self.max_len = max_len
-        self.transform = transform
-        self.target_transform = target_transform
-
-    def text_to_id(self, source):
-        sample = self.tokenizer([source[0], source[1]], max_length=self.max_len, truncation=True, padding='max_length',
-                                return_tensors='pt')
-        return sample
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, idx):
-        return self.text_to_id(self.data[idx])
-
-
-class TestOntologyDataset:
-    def __init__(self, data, tokenizer, max_len):
-        self.tokenizer = tokenizer
-        self.max_len = max_len
-        self.target_idxs = self.text_to_id([x[0] for x in data])
-        self.source_idxs = self.text_to_id([x[1] for x in data])
-        self.label_list = [int(x[2]) for x in data]
-        assert len(self.target_idxs['input_ids']) == len(self.source_idxs['input_ids'])
-
-    def text_to_id(self, source):
-        sample = self.tokenizer(source, max_length=self.max_len, truncation=True, padding='max_length',
-                                return_tensors='pt')
-        return sample
-
-    def get_data(self):
+import torch
+import os
+import json
+import random
+from tqdm import tqdm
+import torch.nn as nn
+from torch.nn import functional as F
+from torch.utils.data import Dataset, DataLoader
+from transformers import AutoTokenizer, AutoModel, AutoConfig
+import scipy.stats
+import numpy as np
+
+
+class TrainOntologyDataset(Dataset):
+    def __init__(self, data, tokenizer, max_len, transform=None, target_transform=None):
+        self.data = data
+        self.tokenizer = tokenizer
+        self.max_len = max_len
+        self.transform = transform
+        self.target_transform = target_transform
+
+    def text_to_id(self, source):
+        sample = self.tokenizer([source[0], source[1]], max_length=self.max_len, truncation=True, padding='max_length',
+                                return_tensors='pt')
+        return sample
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, idx):
+        return self.text_to_id(self.data[idx])
+
+
+class TestOntologyDataset:
+    def __init__(self, data, tokenizer, max_len):
+        self.tokenizer = tokenizer
+        self.max_len = max_len
+        self.target_idxs = self.text_to_id([x[0] for x in data])
+        self.source_idxs = self.text_to_id([x[1] for x in data])
+        self.label_list = [int(x[2]) for x in data]
+        assert len(self.target_idxs['input_ids']) == len(self.source_idxs['input_ids'])
+
+    def text_to_id(self, source):
+        sample = self.tokenizer(source, max_length=self.max_len, truncation=True, padding='max_length',
+                                return_tensors='pt')
+        return sample
+
+    def get_data(self):
         return self.target_idxs, self.source_idxs, self.label_list
```

### Comparing `biotranslator-0.1.1/biotranslator/text_encoder/_get_data.py` & `biotranslator-0.1.2/biotranslator/text_encoder/_get_data.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import torch
-import os
-import json
-import random
-from tqdm import tqdm
-import torch.nn as nn
-from torch.nn import functional as F
-from torch.utils.data import Dataset, DataLoader
-from transformers import AutoTokenizer, AutoModel, AutoConfig
-import scipy.stats
-import numpy as np
-
-
-def read_ontology_names(folder_path):
-    texts = set()
-    name_lines = open(f'{folder_path}/name.txt').readlines()
-    for i, name_line in enumerate(name_lines):
-        texts.add(name_line)
-    return texts
-
-
-def read_graph_to_dict(folder_path):
-    return json.load(open(f'{folder_path}/graph.json', 'r', encoding='utf8'))
-
-
-def read_text_to_dict(folder_path):
-    texts = dict()
-    name_lines = open(f'{folder_path}/name.txt').readlines()
-    def_lines = open(f'{folder_path}/def.txt').readlines()
-    for i, name in enumerate(name_lines):
-        texts[name.strip()] = f'{name.strip()}. {def_lines[i].strip()}'
-    return texts
-
-
-def get_data(dir_path: str):
-    file_list = os.listdir(dir_path)
-    file_exclude = ['go', 'cl']
-    train_texts, test_texts = [], []
-    exclude_n = 0
-    exclude_name = set()
-    for file in file_exclude:
-        text = read_ontology_names(dir_path + file)
-        exclude_name.update(text)
-    for file in tqdm(file_list):
-        graph = read_graph_to_dict(dir_path + file)
-        text = read_text_to_dict(dir_path + file)
-        if file in file_exclude:
-            test_texts.extend([(text[n1.strip()], text[n2.strip()]) for n1 in graph for n2 in graph[n1]])
-            continue
-        for n1 in graph.keys():
-            for n2 in graph[n1]:
-                if n1.strip() in exclude_name or n2.strip() in exclude_name:
-                    exclude_n += 1
-                    continue
-                train_texts.append((text[n1.strip()], text[n2.strip()]))
-    print('Exclude {} edges related to GO or CL!'.format(exclude_n))
-    random.shuffle(train_texts)
-    print(len(train_texts))
+import torch
+import os
+import json
+import random
+from tqdm import tqdm
+import torch.nn as nn
+from torch.nn import functional as F
+from torch.utils.data import Dataset, DataLoader
+from transformers import AutoTokenizer, AutoModel, AutoConfig
+import scipy.stats
+import numpy as np
+
+
+def read_ontology_names(folder_path):
+    texts = set()
+    name_lines = open(f'{folder_path}/name.txt').readlines()
+    for i, name_line in enumerate(name_lines):
+        texts.add(name_line)
+    return texts
+
+
+def read_graph_to_dict(folder_path):
+    return json.load(open(f'{folder_path}/graph.json', 'r', encoding='utf8'))
+
+
+def read_text_to_dict(folder_path):
+    texts = dict()
+    name_lines = open(f'{folder_path}/name.txt').readlines()
+    def_lines = open(f'{folder_path}/def.txt').readlines()
+    for i, name in enumerate(name_lines):
+        texts[name.strip()] = f'{name.strip()}. {def_lines[i].strip()}'
+    return texts
+
+
+def get_data(dir_path: str):
+    file_list = os.listdir(dir_path)
+    file_exclude = ['go', 'cl']
+    train_texts, test_texts = [], []
+    exclude_n = 0
+    exclude_name = set()
+    for file in file_exclude:
+        text = read_ontology_names(dir_path + file)
+        exclude_name.update(text)
+    for file in tqdm(file_list):
+        graph = read_graph_to_dict(dir_path + file)
+        text = read_text_to_dict(dir_path + file)
+        if file in file_exclude:
+            test_texts.extend([(text[n1.strip()], text[n2.strip()]) for n1 in graph for n2 in graph[n1]])
+            continue
+        for n1 in graph.keys():
+            for n2 in graph[n1]:
+                if n1.strip() in exclude_name or n2.strip() in exclude_name:
+                    exclude_n += 1
+                    continue
+                train_texts.append((text[n1.strip()], text[n2.strip()]))
+    print('Exclude {} edges related to GO or CL!'.format(exclude_n))
+    random.shuffle(train_texts)
+    print(len(train_texts))
     return train_texts.copy(), test_texts.copy()
```

### Comparing `biotranslator-0.1.1/biotranslator/text_encoder/_nn.py` & `biotranslator-0.1.2/biotranslator/text_encoder/_nn.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import torch
-import os
-import json
-import random
-from tqdm import tqdm
-import torch.nn as nn
-from torch.nn import functional as F
-from torch.utils.data import Dataset, DataLoader
-from transformers import AutoTokenizer, AutoModel, AutoConfig
-import scipy.stats
-import numpy as np
-
-
-class NeuralNetwork(nn.Module):
-    def __init__(self, model_path, output_way, config):
-        super(NeuralNetwork, self).__init__()
-        self.bert = AutoModel.from_pretrained(model_path, config=config)
-        self.output_way = output_way
-        assert output_way in ['cls', 'pooler']
-
-    def forward(self, input_ids, attention_mask, token_type_ids):
-        x1 = self.bert(input_ids, attention_mask=attention_mask, token_type_ids=token_type_ids)
-        if self.output_way == 'cls':
-            output = x1.last_hidden_state[:, 0]
-        elif self.output_way == 'pooler':
-            output = x1.pooler_output
+import torch
+import os
+import json
+import random
+from tqdm import tqdm
+import torch.nn as nn
+from torch.nn import functional as F
+from torch.utils.data import Dataset, DataLoader
+from transformers import AutoTokenizer, AutoModel, AutoConfig
+import scipy.stats
+import numpy as np
+
+
+class NeuralNetwork(nn.Module):
+    def __init__(self, model_path, output_way, config):
+        super(NeuralNetwork, self).__init__()
+        self.bert = AutoModel.from_pretrained(model_path, config=config)
+        self.output_way = output_way
+        assert output_way in ['cls', 'pooler']
+
+    def forward(self, input_ids, attention_mask, token_type_ids):
+        x1 = self.bert(input_ids, attention_mask=attention_mask, token_type_ids=token_type_ids)
+        if self.output_way == 'cls':
+            output = x1.last_hidden_state[:, 0]
+        elif self.output_way == 'pooler':
+            output = x1.pooler_output
         return output
```

### Comparing `biotranslator-0.1.1/biotranslator/text_encoder/_train.py` & `biotranslator-0.1.2/biotranslator/text_encoder/_train.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import torch
-import os
-import json
-import random
-from tqdm import tqdm
-import torch.nn as nn
-from torch.nn import functional as F
-from torch.utils.data import Dataset, DataLoader
-from transformers import AutoTokenizer, AutoModel, AutoConfig
-import scipy.stats
-import numpy as np
-
-
-def compute_loss(y_pred, device, lamda=0.05):
-    idxs = torch.arange(y_pred.shape[0], device=device)
-    y_true = idxs + 1 - idxs % 2 * 2
-    similarities = F.cosine_similarity(y_pred.unsqueeze(1), y_pred.unsqueeze(0), dim=2)
-    similarities = similarities - torch.eye(y_pred.shape[0], device=device) * 1e12
-    similarities = similarities / lamda
-    loss = F.cross_entropy(similarities, y_true)
-    return torch.mean(loss)
-
-
-def test(model, test_dl, batch, device):
-    test_size = len(test_dl.dataset)
-    for test_d in test_dl:
-        with torch.no_grad():
-            t_input_ids = test_d['input_ids'].view(len(test_d['input_ids']) * 2, -1).to(device)
-            t_attention_mask = test_d['attention_mask'].view(len(test_d['attention_mask']) * 2, -1).to(
-                device)
-            t_token_type_ids = test_d['token_type_ids'].view(len(test_d['token_type_ids']) * 2, -1).to(
-                device)
-            t_pred = model(t_input_ids, t_attention_mask, t_token_type_ids)
-            t_loss = compute_loss(t_pred, device)
-        t_loss, t_current = t_loss.item(), batch * int(len(t_input_ids) / 2)
-        print(f"Batch: {batch} -> Test loss: {t_loss:>7f}  [{t_current:>5d}/{test_size:>5d}]")
-        break
-
-
-def train(train_dl, test_dl, model, optimizer, save_path, device):
-    model.train()
-    train_size = len(train_dl.dataset)
-    for batch, data in tqdm(enumerate(train_dl)):
-        input_ids = data['input_ids'].view(len(data['input_ids']) * 2, -1).to(device)
-        attention_mask = data['attention_mask'].view(len(data['attention_mask']) * 2, -1).to(device)
-        token_type_ids = data['token_type_ids'].view(len(data['token_type_ids']) * 2, -1).to(device)
-        pred = model(input_ids, attention_mask, token_type_ids)
-        loss = compute_loss(pred, device)
-        # Backpropagation
-        optimizer.zero_grad()
-        loss.backward()
-        optimizer.step()
-        if batch % 100 == 0:
-            loss, current = loss.item(), batch * int(len(input_ids) / 2)
-            print(f"Batch: {batch} -> Training loss: {loss:>7f}  [{current:>5d}/{train_size:>5d}]")
-            test(model, test_dl, batch, device)
-    torch.save(model.state_dict(), save_path)
-    print("Saved PyTorch Model State to {}".format(save_path))
+import torch
+import os
+import json
+import random
+from tqdm import tqdm
+import torch.nn as nn
+from torch.nn import functional as F
+from torch.utils.data import Dataset, DataLoader
+from transformers import AutoTokenizer, AutoModel, AutoConfig
+import scipy.stats
+import numpy as np
+
+
+def compute_loss(y_pred, device, lamda=0.05):
+    idxs = torch.arange(y_pred.shape[0], device=device)
+    y_true = idxs + 1 - idxs % 2 * 2
+    similarities = F.cosine_similarity(y_pred.unsqueeze(1), y_pred.unsqueeze(0), dim=2)
+    similarities = similarities - torch.eye(y_pred.shape[0], device=device) * 1e12
+    similarities = similarities / lamda
+    loss = F.cross_entropy(similarities, y_true)
+    return torch.mean(loss)
+
+
+def test(model, test_dl, batch, device):
+    test_size = len(test_dl.dataset)
+    for test_d in test_dl:
+        with torch.no_grad():
+            t_input_ids = test_d['input_ids'].view(len(test_d['input_ids']) * 2, -1).to(device)
+            t_attention_mask = test_d['attention_mask'].view(len(test_d['attention_mask']) * 2, -1).to(
+                device)
+            t_token_type_ids = test_d['token_type_ids'].view(len(test_d['token_type_ids']) * 2, -1).to(
+                device)
+            t_pred = model(t_input_ids, t_attention_mask, t_token_type_ids)
+            t_loss = compute_loss(t_pred, device)
+        t_loss, t_current = t_loss.item(), batch * int(len(t_input_ids) / 2)
+        print(f"Batch: {batch} -> Test loss: {t_loss:>7f}  [{t_current:>5d}/{test_size:>5d}]")
+        break
+
+
+def train(train_dl, test_dl, model, optimizer, save_path, device):
+    model.train()
+    train_size = len(train_dl.dataset)
+    for batch, data in tqdm(enumerate(train_dl)):
+        input_ids = data['input_ids'].view(len(data['input_ids']) * 2, -1).to(device)
+        attention_mask = data['attention_mask'].view(len(data['attention_mask']) * 2, -1).to(device)
+        token_type_ids = data['token_type_ids'].view(len(data['token_type_ids']) * 2, -1).to(device)
+        pred = model(input_ids, attention_mask, token_type_ids)
+        loss = compute_loss(pred, device)
+        # Backpropagation
+        optimizer.zero_grad()
+        loss.backward()
+        optimizer.step()
+        if batch % 100 == 0:
+            loss, current = loss.item(), batch * int(len(input_ids) / 2)
+            print(f"Batch: {batch} -> Training loss: {loss:>7f}  [{current:>5d}/{train_size:>5d}]")
+            test(model, test_dl, batch, device)
+    torch.save(model.state_dict(), save_path)
+    print("Saved PyTorch Model State to {}".format(save_path))
```

### Comparing `biotranslator-0.1.1/biotranslator/trainer/_graph_trainer.py` & `biotranslator-0.1.2/biotranslator/trainer/_graph_trainer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-import os
-import torch
-import collections
-import numpy as np
-import pandas as pd
-from tqdm import tqdm
-from torch.utils.data import DataLoader
-from ..metrics import compute_roc, micro_auroc
-from ..biotranslator import BioTranslator
-from ..utils import sample_edges, get_logger, edge_probability, extract_terms_from_dataset, get_few_shot_namespace_terms, save_obj, compute_blast_preds, load_obj
-
-
-class GraphTrainer:
-
-    def __init__(self, files, cfg):
-        """
-        This class mainly include the training of BioTranslator Model
-        :param files:
-        """
-        # pass the dataset details to the config class
-        cfg.network_dim = files.network_dim
-
-    def setup_model(self, cfg):
-        self.model = BioTranslator(cfg)
-
-    def setup_training(self, files, cfg):
-        # train epochs
-        self.epoch = cfg.epoch
-        # loss function
-        self.loss_func = torch.nn.BCELoss()
-        # use Adam as optimizer
-        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=cfg.lr)
-        # set up the training dataset and validation dataset
-        self.train_dataset = files.train_data
-        self.val_dataset = files.eval_data
-
-    def backward_model(self, input_seq, input_description, input_vector, emb_tensor, label):
-        logits = self.model(data_type='graph',
-                            input_seq=input_seq,
-                            input_description=input_description,
-                            input_vector=input_vector,
-                            texts=emb_tensor)
-        self.loss = self.loss_func(logits, label)
-        self.optimizer.zero_grad()
-        self.loss.backward()
-        self.optimizer.step()
-        return self.loss.item()
-
-    def train(self, files, cfg):
-        # store the results of pathway prediction
-        node_link_auroc = collections.OrderedDict()
-        # record the performance of our model
-        self.logger = get_logger(cfg.logger_name)
-
-        print('Start training model on :{} ...'.format(cfg.dataset))
-
-        # setup the model architecture according the methods
-        self.setup_model(cfg)
-        # setup dataset, the training loss and optimizer
-        self.setup_training(files, cfg)
-
-        train_loader = DataLoader(files.train_data, batch_size=cfg.batch_size, shuffle=True)
-        eval_loader = DataLoader(files.eval_data, batch_size=cfg.batch_size, shuffle=True)
-
-        # train the model
-        pbar = tqdm(range(self.epoch), desc='Training')
-        for epoch_i in pbar:
-            train_loss = 0
-            train_count = 0
-            for batch in train_loader:
-                train_loss += self.backward_model(batch['prot_seq'],
-                                                  batch['prot_description'],
-                                                  batch['prot_network'],
-                                                  files.text_embeddings,
-                                                  batch['label'])
-                train_count += len(batch)
-                pbar.set_postfix({"epoch": epoch_i,
-                                  "train loss": train_loss / train_count})
-
-        # evaluate the model
-        print('Evaluate Our Model on {}'.format(cfg.pathway_dataset))
-        uniprots, preds, label = [], [], []
-        with torch.no_grad():
-            pbar = tqdm(eval_loader, desc='Pathway Node Classification')
-            for batch in pbar:
-                pred_batch = self.model.data_encoder(batch['prot_seq'], batch['prot_description'],
-                                        batch['prot_network'])
-                uniprots += batch['proteins']
-                self.loss_func.zero_grad()
-                preds.append(pred_batch.cpu().numpy())
-                label.append(batch['label'].cpu().float().numpy())
-
-        data_encodings = np.concatenate(preds, axis=0)
-        pathway_labels = np.concatenate(label, axis=0)
-        pathway_encodings = files.pathway_embeddings.cpu().numpy()
-        go_embeddings = files.text_embeddings.cpu().numpy()
-        nearest_k = 5
-        sims = np.dot(pathway_encodings, np.transpose(go_embeddings))
-        for i in range(np.size(pathway_encodings, 0)):
-            sim_i = sims[i, :]
-            sim_idx = np.argsort(-sim_i)[0: nearest_k]
-            nearest_go_emb = go_embeddings[sim_idx, :]
-            nearest_go_emb = np.vstack((go_embeddings[i, :], nearest_go_emb))
-            emb_i = np.mean(nearest_go_emb, axis=0)
-            pathway_encodings[i, :] = emb_i / np.sqrt(np.sum(np.power(emb_i, 2)))
-        logits = np.dot(data_encodings, np.transpose(pathway_encodings))
-        logits = 1 / (1 + np.exp(-logits))
-
-        # evaluate the performance of BioTranslator on node classification
-        auroc = micro_auroc(pathway_labels, logits)
-        for i in range(len(auroc)):
-            node_link_auroc[files.eval_i2terms[i]] = [auroc[i]]
-
-        self.logger.info(f'Pathway: {cfg.pathway_dataset} Node Classification AUROC: {np.mean(auroc)}')
-
-        # evaluate the performance of BioTranslator on edge prediction
-        pathway_dir = cfg.data_repo + cfg.pathway_dataset + '/'
-        if 'pathway_graph.pkl' in os.listdir(pathway_dir):
-            pathway_graph = load_obj(pathway_dir + 'pathway_graph.pkl')
-            uniprot2index = collections.OrderedDict()
-            id = 0
-            for uniprot_id in uniprots:
-                uniprot2index[uniprot_id] = id
-                id += 1
-
-            graph_auroc = []
-            pbar = tqdm(pathway_graph.keys(), desc='Pathway Edge Prediction')
-            for p_id in pbar:
-                edges_id, edges = [], pathway_graph[p_id]
-
-                # convert edges from uniprot to index
-                for e in range(len(edges)):
-                    if edges[e][0] not in uniprot2index.keys()\
-                            or edges[e][1] not in uniprot2index.keys():
-                        continue
-                    edges_id.append([uniprot2index[edges[e][0]], uniprot2index[edges[e][1]]])
-                if len(edges_id) == 0:
-                    continue
-                false_edges = sample_edges(0, len(uniprots), 10 * len(edges_id), edges_id)
-                true_edges = np.asarray(edges_id)
-
-                # predict edges
-                encodings_i = data_encodings[true_edges[:, 0], :]
-                encodings_j = data_encodings[true_edges[:, 1], :]
-                text_encodings_p = pathway_encodings[files.eval_terms2i[p_id]] / np.sqrt(
-                    np.sum(np.square(pathway_encodings[files.eval_terms2i[p_id]].squeeze())))
-                text_encodings_p = text_encodings_p.reshape([1, -1])
-                true_score = edge_probability(encodings_i, encodings_j, text_encodings_p)
-                encodings_i = data_encodings[false_edges[:, 0], :]
-                encodings_j = data_encodings[false_edges[:, 1], :]
-                false_score = edge_probability(encodings_i, encodings_j, text_encodings_p)
-
-                # compute auroc
-                edge_prediction, edge_label = [], []
-                edge_prediction += list(true_score)
-                edge_prediction += list(false_score)
-                edge_label += list(np.ones(len(true_score)))
-                edge_label += list(np.zeros(len(false_score)))
-                edge_auroc = compute_roc(np.asarray(edge_label), np.asarray(edge_prediction))
-                graph_auroc.append(edge_auroc)
-                node_link_auroc[p_id].append(edge_auroc)
-            self.logger.info(f'Pathway: {cfg.pathway_dataset} Edge Prediction AUROC: {np.mean(graph_auroc)}')
-
-        # save the results
-        save_obj(node_link_auroc, cfg.results_name)
-        # save the model
-        torch.save(self.model, cfg.save_model_path.format(cfg.method, cfg.pathway_dataset))
-
-    def annotate(self, files, cfg, data_dir, anno_data, task='node_cls'):
-        # data_path = data_dir + anno_file
-        # anno_data = pd.read_pickle(data_path)
-        anno_loader = DataLoader(anno_data, batch_size=cfg.batch_size, shuffle=True)
-        print('Annotate {} with our Model'.format(cfg.pathway_dataset))
-        uniprots, preds = [], []
-        with torch.no_grad():
-            pbar = tqdm(anno_loader, desc='Pathway Node Classification')
-            for batch in pbar:
-                pred_batch = self.model.data_encoder(batch['prot_seq'], batch['prot_description'],
-                                                     batch['prot_network'])
-                uniprots += batch['proteins']
-                preds.append(pred_batch.cpu().numpy())
-
-        data_encodings = np.concatenate(preds, axis=0)
-        pathway_encodings = files.pathway_embeddings.cpu().numpy()
-        go_embeddings = files.text_embeddings.cpu().numpy()
-        nearest_k = 5
-        sims = np.dot(pathway_encodings, np.transpose(go_embeddings))
-        for i in range(np.size(pathway_encodings, 0)):
-            sim_i = sims[i, :]
-            sim_idx = np.argsort(-sim_i)[0: nearest_k]
-            nearest_go_emb = go_embeddings[sim_idx, :]
-            nearest_go_emb = np.vstack((go_embeddings[i, :], nearest_go_emb))
-            emb_i = np.mean(nearest_go_emb, axis=0)
-            pathway_encodings[i, :] = emb_i / np.sqrt(np.sum(np.power(emb_i, 2)))
-
-        # result = collections.OrderedDict()
-        if 'node_cls' in task:
-            logits = np.dot(data_encodings, np.transpose(pathway_encodings))
-            logits = 1 / (1 + np.exp(-logits))
-            # result['node_cls'] = logits
-            return logits
-
-        if 'edge_pred' in task:
-            # edge prediction
-            pred_label = collections.OrderedDict()
-            pathway_dir = cfg.data_repo + cfg.pathway_dataset + '/'
-            if 'pathway_graph.pkl' in os.listdir(pathway_dir):
-                pathway_graph = load_obj(pathway_dir + 'pathway_graph.pkl')
-                uniprot2index = collections.OrderedDict()
-                id = 0
-                for uniprot_id in uniprots:
-                    uniprot2index[uniprot_id] = id
-                    id += 1
-
-                pbar = tqdm(pathway_graph.keys(), desc='Pathway Edge Prediction')
-                for p_id in pbar:
-                    edges_id, edges = [], pathway_graph[p_id]
-                    for e in range(len(edges)):
-                        if edges[e][0] not in uniprot2index.keys() or edges[e][1] not in uniprot2index.keys():
-                            continue
-                        edges_id.append([uniprot2index[edges[e][0]], uniprot2index[edges[e][1]]])
-                    if len(edges_id) == 0:
-                        continue
-                    edges = np.asarray(edges_id)
-                    encodings_i, encodings_j = data_encodings[edges[:, 0], :], data_encodings[edges[:, 1], :]
-                    anno_terms2i, _ = extract_terms_from_dataset(anno_data)
-                    text_encodings_p = pathway_encodings[anno_terms2i[p_id]] / np.sqrt(
-                        np.sum(np.square(pathway_encodings[anno_terms2i[p_id]].squeeze())))
-                    text_encodings_p = text_encodings_p.reshape([1, -1])
-                    score = edge_probability(encodings_i, encodings_j, text_encodings_p)
-                    print(score)
-                    if p_id not in pred_label.keys() or pred_label[p_id] is None:
-                        pred_label[p_id] = []
-                    else:
-                        pred_label[p_id].append(score)
-            return pred_label
-            # result['edge_pred'] = pred_label
-        # return result
+import os
+import torch
+import collections
+import numpy as np
+import pandas as pd
+from tqdm import tqdm
+from torch.utils.data import DataLoader
+from ..metrics import compute_roc, micro_auroc
+from ..biotranslator import BioTranslator
+from ..utils import sample_edges, get_logger, edge_probability, extract_terms_from_dataset, get_few_shot_namespace_terms, save_obj, compute_blast_preds, load_obj
+
+
+class GraphTrainer:
+
+    def __init__(self, files, cfg):
+        """
+        This class mainly include the training of BioTranslator Model
+        :param files:
+        """
+        # pass the dataset details to the config class
+        cfg.network_dim = files.network_dim
+
+    def setup_model(self, cfg):
+        self.model = BioTranslator(cfg)
+
+    def setup_training(self, files, cfg):
+        # train epochs
+        self.epoch = cfg.epoch
+        # loss function
+        self.loss_func = torch.nn.BCELoss()
+        # use Adam as optimizer
+        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=cfg.lr)
+        # set up the training dataset and validation dataset
+        self.train_dataset = files.train_data
+        self.val_dataset = files.eval_data
+
+    def backward_model(self, input_seq, input_description, input_vector, emb_tensor, label):
+        logits = self.model(data_type='graph',
+                            input_seq=input_seq,
+                            input_description=input_description,
+                            input_vector=input_vector,
+                            texts=emb_tensor)
+        self.loss = self.loss_func(logits, label)
+        self.optimizer.zero_grad()
+        self.loss.backward()
+        self.optimizer.step()
+        return self.loss.item()
+
+    def train(self, files, cfg):
+        # store the results of pathway prediction
+        node_link_auroc = collections.OrderedDict()
+        # record the performance of our model
+        self.logger = get_logger(cfg.logger_name)
+
+        print('Start training model on :{} ...'.format(cfg.dataset))
+
+        # setup the model architecture according the methods
+        self.setup_model(cfg)
+        # setup dataset, the training loss and optimizer
+        self.setup_training(files, cfg)
+
+        train_loader = DataLoader(files.train_data, batch_size=cfg.batch_size, shuffle=True)
+        eval_loader = DataLoader(files.eval_data, batch_size=cfg.batch_size, shuffle=True)
+
+        # train the model
+        pbar = tqdm(range(self.epoch), desc='Training')
+        for epoch_i in pbar:
+            train_loss = 0
+            train_count = 0
+            for batch in train_loader:
+                train_loss += self.backward_model(batch['prot_seq'],
+                                                  batch['prot_description'],
+                                                  batch['prot_network'],
+                                                  files.text_embeddings,
+                                                  batch['label'])
+                train_count += len(batch)
+                pbar.set_postfix({"epoch": epoch_i,
+                                  "train loss": train_loss / train_count})
+
+        # evaluate the model
+        print('Evaluate Our Model on {}'.format(cfg.pathway_dataset))
+        uniprots, preds, label = [], [], []
+        with torch.no_grad():
+            pbar = tqdm(eval_loader, desc='Pathway Node Classification')
+            for batch in pbar:
+                pred_batch = self.model.data_encoder(batch['prot_seq'], batch['prot_description'],
+                                        batch['prot_network'])
+                uniprots += batch['proteins']
+                self.loss_func.zero_grad()
+                preds.append(pred_batch.cpu().numpy())
+                label.append(batch['label'].cpu().float().numpy())
+
+        data_encodings = np.concatenate(preds, axis=0)
+        pathway_labels = np.concatenate(label, axis=0)
+        pathway_encodings = files.pathway_embeddings.cpu().numpy()
+        go_embeddings = files.text_embeddings.cpu().numpy()
+        nearest_k = 5
+        sims = np.dot(pathway_encodings, np.transpose(go_embeddings))
+        for i in range(np.size(pathway_encodings, 0)):
+            sim_i = sims[i, :]
+            sim_idx = np.argsort(-sim_i)[0: nearest_k]
+            nearest_go_emb = go_embeddings[sim_idx, :]
+            nearest_go_emb = np.vstack((go_embeddings[i, :], nearest_go_emb))
+            emb_i = np.mean(nearest_go_emb, axis=0)
+            pathway_encodings[i, :] = emb_i / np.sqrt(np.sum(np.power(emb_i, 2)))
+        logits = np.dot(data_encodings, np.transpose(pathway_encodings))
+        logits = 1 / (1 + np.exp(-logits))
+
+        # evaluate the performance of BioTranslator on node classification
+        auroc = micro_auroc(pathway_labels, logits)
+        for i in range(len(auroc)):
+            node_link_auroc[files.eval_i2terms[i]] = [auroc[i]]
+
+        self.logger.info(f'Pathway: {cfg.pathway_dataset} Node Classification AUROC: {np.mean(auroc)}')
+
+        # evaluate the performance of BioTranslator on edge prediction
+        pathway_dir = cfg.data_repo + cfg.pathway_dataset + '/'
+        if 'pathway_graph.pkl' in os.listdir(pathway_dir):
+            pathway_graph = load_obj(pathway_dir + 'pathway_graph.pkl')
+            uniprot2index = collections.OrderedDict()
+            id = 0
+            for uniprot_id in uniprots:
+                uniprot2index[uniprot_id] = id
+                id += 1
+
+            graph_auroc = []
+            pbar = tqdm(pathway_graph.keys(), desc='Pathway Edge Prediction')
+            for p_id in pbar:
+                edges_id, edges = [], pathway_graph[p_id]
+
+                # convert edges from uniprot to index
+                for e in range(len(edges)):
+                    if edges[e][0] not in uniprot2index.keys()\
+                            or edges[e][1] not in uniprot2index.keys():
+                        continue
+                    edges_id.append([uniprot2index[edges[e][0]], uniprot2index[edges[e][1]]])
+                if len(edges_id) == 0:
+                    continue
+                false_edges = sample_edges(0, len(uniprots), 10 * len(edges_id), edges_id)
+                true_edges = np.asarray(edges_id)
+
+                # predict edges
+                encodings_i = data_encodings[true_edges[:, 0], :]
+                encodings_j = data_encodings[true_edges[:, 1], :]
+                text_encodings_p = pathway_encodings[files.eval_terms2i[p_id]] / np.sqrt(
+                    np.sum(np.square(pathway_encodings[files.eval_terms2i[p_id]].squeeze())))
+                text_encodings_p = text_encodings_p.reshape([1, -1])
+                true_score = edge_probability(encodings_i, encodings_j, text_encodings_p)
+                encodings_i = data_encodings[false_edges[:, 0], :]
+                encodings_j = data_encodings[false_edges[:, 1], :]
+                false_score = edge_probability(encodings_i, encodings_j, text_encodings_p)
+
+                # compute auroc
+                edge_prediction, edge_label = [], []
+                edge_prediction += list(true_score)
+                edge_prediction += list(false_score)
+                edge_label += list(np.ones(len(true_score)))
+                edge_label += list(np.zeros(len(false_score)))
+                edge_auroc = compute_roc(np.asarray(edge_label), np.asarray(edge_prediction))
+                graph_auroc.append(edge_auroc)
+                node_link_auroc[p_id].append(edge_auroc)
+            self.logger.info(f'Pathway: {cfg.pathway_dataset} Edge Prediction AUROC: {np.mean(graph_auroc)}')
+
+        # save the results
+        save_obj(node_link_auroc, cfg.results_name)
+        # save the model
+        torch.save(self.model, cfg.save_model_path.format(cfg.method, cfg.pathway_dataset))
+
+    def annotate(self, files, cfg, data_dir, anno_data, task='node_cls'):
+        # data_path = data_dir + anno_file
+        # anno_data = pd.read_pickle(data_path)
+        anno_loader = DataLoader(anno_data, batch_size=cfg.batch_size, shuffle=True)
+        print('Annotate {} with our Model'.format(cfg.pathway_dataset))
+        uniprots, preds = [], []
+        with torch.no_grad():
+            pbar = tqdm(anno_loader, desc='Pathway Node Classification')
+            for batch in pbar:
+                pred_batch = self.model.data_encoder(batch['prot_seq'], batch['prot_description'],
+                                                     batch['prot_network'])
+                uniprots += batch['proteins']
+                preds.append(pred_batch.cpu().numpy())
+
+        data_encodings = np.concatenate(preds, axis=0)
+        pathway_encodings = files.pathway_embeddings.cpu().numpy()
+        go_embeddings = files.text_embeddings.cpu().numpy()
+        nearest_k = 5
+        sims = np.dot(pathway_encodings, np.transpose(go_embeddings))
+        for i in range(np.size(pathway_encodings, 0)):
+            sim_i = sims[i, :]
+            sim_idx = np.argsort(-sim_i)[0: nearest_k]
+            nearest_go_emb = go_embeddings[sim_idx, :]
+            nearest_go_emb = np.vstack((go_embeddings[i, :], nearest_go_emb))
+            emb_i = np.mean(nearest_go_emb, axis=0)
+            pathway_encodings[i, :] = emb_i / np.sqrt(np.sum(np.power(emb_i, 2)))
+
+        # result = collections.OrderedDict()
+        if 'node_cls' in task:
+            logits = np.dot(data_encodings, np.transpose(pathway_encodings))
+            logits = 1 / (1 + np.exp(-logits))
+            # result['node_cls'] = logits
+            return logits
+
+        if 'edge_pred' in task:
+            # edge prediction
+            pred_label = collections.OrderedDict()
+            pathway_dir = cfg.data_repo + cfg.pathway_dataset + '/'
+            if 'pathway_graph.pkl' in os.listdir(pathway_dir):
+                pathway_graph = load_obj(pathway_dir + 'pathway_graph.pkl')
+                uniprot2index = collections.OrderedDict()
+                id = 0
+                for uniprot_id in uniprots:
+                    uniprot2index[uniprot_id] = id
+                    id += 1
+
+                pbar = tqdm(pathway_graph.keys(), desc='Pathway Edge Prediction')
+                for p_id in pbar:
+                    edges_id, edges = [], pathway_graph[p_id]
+                    for e in range(len(edges)):
+                        if edges[e][0] not in uniprot2index.keys() or edges[e][1] not in uniprot2index.keys():
+                            continue
+                        edges_id.append([uniprot2index[edges[e][0]], uniprot2index[edges[e][1]]])
+                    if len(edges_id) == 0:
+                        continue
+                    edges = np.asarray(edges_id)
+                    encodings_i, encodings_j = data_encodings[edges[:, 0], :], data_encodings[edges[:, 1], :]
+                    anno_terms2i, _ = extract_terms_from_dataset(anno_data)
+                    text_encodings_p = pathway_encodings[anno_terms2i[p_id]] / np.sqrt(
+                        np.sum(np.square(pathway_encodings[anno_terms2i[p_id]].squeeze())))
+                    text_encodings_p = text_encodings_p.reshape([1, -1])
+                    score = edge_probability(encodings_i, encodings_j, text_encodings_p)
+                    print(score)
+                    if p_id not in pred_label.keys() or pred_label[p_id] is None:
+                        pred_label[p_id] = []
+                    else:
+                        pred_label[p_id].append(score)
+            return pred_label
+            # result['edge_pred'] = pred_label
+        # return result
```

### Comparing `biotranslator-0.1.1/biotranslator/trainer/_sequence_trainer.py` & `biotranslator-0.1.2/biotranslator/trainer/_sequence_trainer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-import os
-import torch
-import collections
-import pandas as pd
-import numpy as np
-from tqdm import tqdm
-from torch.utils.data import DataLoader
-from ..metrics import auroc_metrics
-from ..biotranslator import BioTranslator
-from ..utils import term2preds_label, term_training_numbers, get_logger, get_namespace_terms, \
-    get_few_shot_namespace_terms, save_obj, compute_blast_preds, load_obj
-
-
-class SeqTrainer:
-
-    def __init__(self, files, cfg):
-        """
-        This class mainly include the training of BioTranslator Model
-        :param files:
-        """
-        # pass the dataset details to the config class
-        cfg.network_dim = files.network_dim
-
-    def setup_model(self, cfg):
-        self.model = BioTranslator(cfg)
-
-    def setup_training(self, files, cfg):
-        # train epochs
-        self.epoch = cfg.epoch
-        # loss function
-        self.loss_func = torch.nn.BCELoss()
-        # use Adam as optimizer
-        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=cfg.lr)
-        # set up the training dataset and validation dataset
-        self.train_dataset = files.fold_train
-        self.val_dataset = files.fold_val
-
-    def backward_model(self, input_seq, input_description, input_vector, emb_tensor, label):
-        logits = self.model(data_type='seq',
-                            input_seq=input_seq,
-                            input_description=input_description,
-                            input_vector=input_vector,
-                            texts=emb_tensor)
-        self.loss = self.loss_func(logits, label)
-        self.optimizer.zero_grad()
-        self.loss.backward()
-        self.optimizer.step()
-        return self.loss.item()
-
-    def train(self, files, cfg):
-        # store the results of each fold in one list
-        results_list = []
-        if cfg.task == 'few_shot':
-            with_blast_res_list = []
-        # record the performance of our model
-        self.logger = get_logger(cfg.logger_name)
-        for fold_i in range(cfg.k_fold):
-            print('Start Cross-Validation Fold :{} ...'.format(fold_i))
-
-            # setup the model architecture according the methods
-            self.setup_model(cfg)
-            # setup dataset, the training loss and optimizer
-            self.setup_training(files, cfg)
-            train_loader = DataLoader(files.fold_train[fold_i], batch_size=cfg.batch_size, shuffle=True)
-            eval_loader = DataLoader(files.fold_val[fold_i], batch_size=cfg.batch_size, shuffle=True)
-            # train the model
-            pbar = tqdm(range(self.epoch), desc='Training')
-            for epoch_i in pbar:
-                train_loss = 0
-                train_count = 0
-                for batch in train_loader:
-                    train_loss += self.backward_model(batch['prot_seq'], batch['prot_description'],
-                                                      batch['prot_network'], files.text_embeddings, batch['label'])
-                    train_count += len(batch)
-                    pbar.set_postfix({"Fold": fold_i,
-                                      "epoch": epoch_i,
-                                      "train loss": train_loss / train_count})
-            # evaluate the model
-            print('Evaluate Our Model ...')
-            eval_loss, eval_count = 0, 0
-            logits, prots, label = [], [], []
-            with torch.no_grad():
-                for batch in eval_loader:
-                    pred_batch = self.model(batch['prot_seq'], batch['prot_description'],
-                                            batch['prot_network'], files.text_embeddings)
-                    prots += batch['proteins']
-                    eval_loss += self.loss_func(pred_batch, batch['label']).item()
-                    eval_count += len(batch)
-                    self.loss_func.zero_grad()
-                    logits.append(pred_batch.cpu().numpy())
-                    label.append(batch['label'].cpu().float().numpy())
-            logits, label = np.concatenate(logits, axis=0), np.concatenate(label, axis=0)
-
-            # evaluate the model on the zero shot tasks or the few shot tasks
-            if cfg.task == 'zero_shot':
-                results = collections.OrderedDict()
-                for ont in ['bp', 'mf', 'cc']:
-                    # extract the predictions and labels of zero shot terms
-                    ont_terms = get_namespace_terms(list(files.fold_zero_shot_terms_list[fold_i].keys()), files.go_data, ont)
-                    logits_ont, label_ont = term2preds_label(logits, label, ont_terms, files.terms2i)
-                    auroc_mean, auroc_pct = auroc_metrics(label_ont, logits_ont)
-                    results[ont] = collections.OrderedDict()
-                    results[ont]['auroc'], results[ont]['percentage'] = auroc_mean, auroc_pct
-                    self.logger.info('fold:{} ont: {} roc auc:{}'.format(fold_i, ont, auroc_mean))
-                    for T in auroc_pct.keys():
-                        self.logger.info('fold:{} ont: {} the AUROC of {}% terms is greater than {}'.format(fold_i, ont, auroc_pct[T], T))
-                results_list.append(results)
-                torch.save(self.model, cfg.save_model_path.format(cfg.method, cfg.dataset, fold_i))
-
-            if cfg.task == 'few_shot':
-                # generate blast preds for the few shot task
-                if not os.path.exists(cfg.blast_preds_path.format(fold_i)):
-                    blast_preds = compute_blast_preds(files.diamond_list[fold_i],
-                                                      files.raw_val[fold_i],
-                                                      files.raw_train[fold_i])
-                    save_obj(blast_preds, cfg.blast_preds_path.format(fold_i))
-                else:
-                    blast_preds = load_obj(cfg.blast_preds_path.format(fold_i))
-
-                # compute logits with blast
-                logits_with_blast = logits.copy()
-                for go_id in files.terms2i.keys():
-                    ont = cfg.ont_term_syn[files.go_data[go_id]['namespace']]
-                    for p_i in range(np.size(logits_with_blast, 0)):
-                        if go_id not in blast_preds[prots[p_i]].keys():
-                            logits_with_blast[p_i, files.terms2i[go_id]] = (1 - cfg.alphas[ont]) * logits[p_i, files.terms2i[go_id]] + cfg.alphas[ont] * 0
-                        else:
-                            logits_with_blast[p_i, files.terms2i[go_id]] = (1 - cfg.alphas[ont]) * logits[p_i, files.terms2i[go_id]] + cfg.alphas[ont] * blast_preds[prots[p_i]][go_id]
-
-                results = collections.OrderedDict()
-                with_blast_res = collections.OrderedDict()
-                for ont in ['bp', 'mf', 'cc']:
-                    # extract the predictions and labels of zero shot terms
-                    results[ont] = collections.OrderedDict()
-                    with_blast_res[ont] = collections.OrderedDict()
-                    for n in range(1, 20):
-                        ont_terms = get_few_shot_namespace_terms(files.fold_few_shot_terms_list[fold_i], files.go_data, ont, n)
-                        # evaluate without blast
-                        logits_ont, label_ont = term2preds_label(logits, label, ont_terms, files.terms2i)
-                        auroc_mean, auroc_pct = auroc_metrics(label_ont, logits_ont)
-                        results[ont][n] = auroc_mean
-                        # evaluate with blast
-                        logits_blast_ont, label_ont = term2preds_label(logits_with_blast, label, ont_terms, files.terms2i)
-                        auroc_blast_mean, auroc_blast_pct = auroc_metrics(label_ont, logits_blast_ont)
-                        with_blast_res[ont][n] = auroc_blast_mean
-                        self.logger.info('fold:{} ont: {} sample number: {} roc auc:{} add blast: {}'.format(fold_i, ont, n, auroc_mean, auroc_blast_mean))
-                # append the results of fold i without blast predictions and with blast predictions
-                results_list.append(results)
-                with_blast_res_list.append(with_blast_res)
-
-        # save the results
-        save_obj(results_list, cfg.results_name)
-        if cfg.task == 'few_shot':
-            save_obj(with_blast_res_list, cfg.blast_res_name)
-
-    def annotate(self, files, cfg, data_dir, anno_data, task='prot_func_pred'):
-        def zero_shot_terms():
-            zero_shot_term_path = data_dir + 'zero_shot_terms.pkl'
-            zero_shot_terms = load_obj(zero_shot_term_path)
-            return zero_shot_terms
-
-        def term2preds_label(preds, terms, terms2id):
-            new_preds = []
-            for t_id in terms:
-                new_preds.append(preds[:, terms2id[t_id]].reshape((-1, 1)))
-            new_preds = np.concatenate(new_preds, axis=1)
-            return new_preds
-
-        def zero_shot_data(zero_shot_terms_list, train):
-            drop_index = []
-            for j in train.index:
-                annts = train.loc[j]['annotations']
-                insct = list(set(annts).intersection(zero_shot_terms_list))
-                if len(insct) > 0:
-                    drop_index.append(j)
-            train = train.drop(index=drop_index)
-            return train
-
-        # data_path = data_dir + anno_file
-        # print('Annotate {} dataset in zero shot with our model'.format(data_path))
-        # anno_data = pd.read_pickle(data_path)
-        anno_loader = DataLoader(anno_data, batch_size=cfg.batch_size, shuffle=True)
-
-        print('Annotate Data with Our Model ...')
-        logits, prots = [], []
-        with torch.no_grad():
-            for batch in anno_loader:
-                pred_batch = self.model(batch['prot_seq'], batch['prot_description'],
-                                        batch['prot_network'], files.text_embeddings)
-                prots += batch['proteins']
-                logits.append(pred_batch.cpu().numpy())
-        logits = np.concatenate(logits, axis=0)
-
-        # if cfg.task == 'zero_shot':
-        zero_shot_terms = zero_shot_terms()
-        zero_shot_data(zero_shot_terms, files.raw_train)
-        logits_ont = collections.OrderedDict()
-        for ont in ['bp', 'mf', 'cc']:
-            # extract the predictions and labels of zero shot terms
-            ont_terms = get_namespace_terms(list(files.zero_shot_terms.keys()), files.go_data, ont)
-            logits_ont[ont] = term2preds_label(logits, ont_terms, files.terms2i)
-        return logits_ont
+import os
+import torch
+import collections
+import pandas as pd
+import numpy as np
+from tqdm import tqdm
+from torch.utils.data import DataLoader
+from ..metrics import auroc_metrics
+from ..biotranslator import BioTranslator
+from ..utils import term2preds_label, term_training_numbers, get_logger, get_namespace_terms, \
+    get_few_shot_namespace_terms, save_obj, compute_blast_preds, load_obj
+
+
+class SeqTrainer:
+
+    def __init__(self, files, cfg):
+        """
+        This class mainly include the training of BioTranslator Model
+        :param files:
+        """
+        # pass the dataset details to the config class
+        cfg.network_dim = files.network_dim
+
+    def setup_model(self, cfg):
+        self.model = BioTranslator(cfg)
+
+    def setup_training(self, files, cfg):
+        # train epochs
+        self.epoch = cfg.epoch
+        # loss function
+        self.loss_func = torch.nn.BCELoss()
+        # use Adam as optimizer
+        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=cfg.lr)
+        # set up the training dataset and validation dataset
+        self.train_dataset = files.fold_train
+        self.val_dataset = files.fold_val
+
+    def backward_model(self, input_seq, input_description, input_vector, emb_tensor, label):
+        logits = self.model(data_type='seq',
+                            input_seq=input_seq,
+                            input_description=input_description,
+                            input_vector=input_vector,
+                            texts=emb_tensor)
+        self.loss = self.loss_func(logits, label)
+        self.optimizer.zero_grad()
+        self.loss.backward()
+        self.optimizer.step()
+        return self.loss.item()
+
+    def train(self, files, cfg):
+        # store the results of each fold in one list
+        results_list = []
+        if cfg.task == 'few_shot':
+            with_blast_res_list = []
+        # record the performance of our model
+        self.logger = get_logger(cfg.logger_name)
+        for fold_i in range(cfg.k_fold):
+            print('Start Cross-Validation Fold :{} ...'.format(fold_i))
+
+            # setup the model architecture according the methods
+            self.setup_model(cfg)
+            # setup dataset, the training loss and optimizer
+            self.setup_training(files, cfg)
+            train_loader = DataLoader(files.fold_train[fold_i], batch_size=cfg.batch_size, shuffle=True)
+            eval_loader = DataLoader(files.fold_val[fold_i], batch_size=cfg.batch_size, shuffle=True)
+            # train the model
+            pbar = tqdm(range(self.epoch), desc='Training')
+            for epoch_i in pbar:
+                train_loss = 0
+                train_count = 0
+                for batch in train_loader:
+                    train_loss += self.backward_model(batch['prot_seq'], batch['prot_description'],
+                                                      batch['prot_network'], files.text_embeddings, batch['label'])
+                    train_count += len(batch)
+                    pbar.set_postfix({"Fold": fold_i,
+                                      "epoch": epoch_i,
+                                      "train loss": train_loss / train_count})
+            # evaluate the model
+            print('Evaluate Our Model ...')
+            eval_loss, eval_count = 0, 0
+            logits, prots, label = [], [], []
+            with torch.no_grad():
+                for batch in eval_loader:
+                    pred_batch = self.model(batch['prot_seq'], batch['prot_description'],
+                                            batch['prot_network'], files.text_embeddings)
+                    prots += batch['proteins']
+                    eval_loss += self.loss_func(pred_batch, batch['label']).item()
+                    eval_count += len(batch)
+                    self.loss_func.zero_grad()
+                    logits.append(pred_batch.cpu().numpy())
+                    label.append(batch['label'].cpu().float().numpy())
+            logits, label = np.concatenate(logits, axis=0), np.concatenate(label, axis=0)
+
+            # evaluate the model on the zero shot tasks or the few shot tasks
+            if cfg.task == 'zero_shot':
+                results = collections.OrderedDict()
+                for ont in ['bp', 'mf', 'cc']:
+                    # extract the predictions and labels of zero shot terms
+                    ont_terms = get_namespace_terms(list(files.fold_zero_shot_terms_list[fold_i].keys()), files.go_data, ont)
+                    logits_ont, label_ont = term2preds_label(logits, label, ont_terms, files.terms2i)
+                    auroc_mean, auroc_pct = auroc_metrics(label_ont, logits_ont)
+                    results[ont] = collections.OrderedDict()
+                    results[ont]['auroc'], results[ont]['percentage'] = auroc_mean, auroc_pct
+                    self.logger.info('fold:{} ont: {} roc auc:{}'.format(fold_i, ont, auroc_mean))
+                    for T in auroc_pct.keys():
+                        self.logger.info('fold:{} ont: {} the AUROC of {}% terms is greater than {}'.format(fold_i, ont, auroc_pct[T], T))
+                results_list.append(results)
+                torch.save(self.model, cfg.save_model_path.format(cfg.method, cfg.dataset, fold_i))
+
+            if cfg.task == 'few_shot':
+                # generate blast preds for the few shot task
+                if not os.path.exists(cfg.blast_preds_path.format(fold_i)):
+                    blast_preds = compute_blast_preds(files.diamond_list[fold_i],
+                                                      files.raw_val[fold_i],
+                                                      files.raw_train[fold_i])
+                    save_obj(blast_preds, cfg.blast_preds_path.format(fold_i))
+                else:
+                    blast_preds = load_obj(cfg.blast_preds_path.format(fold_i))
+
+                # compute logits with blast
+                logits_with_blast = logits.copy()
+                for go_id in files.terms2i.keys():
+                    ont = cfg.ont_term_syn[files.go_data[go_id]['namespace']]
+                    for p_i in range(np.size(logits_with_blast, 0)):
+                        if go_id not in blast_preds[prots[p_i]].keys():
+                            logits_with_blast[p_i, files.terms2i[go_id]] = (1 - cfg.alphas[ont]) * logits[p_i, files.terms2i[go_id]] + cfg.alphas[ont] * 0
+                        else:
+                            logits_with_blast[p_i, files.terms2i[go_id]] = (1 - cfg.alphas[ont]) * logits[p_i, files.terms2i[go_id]] + cfg.alphas[ont] * blast_preds[prots[p_i]][go_id]
+
+                results = collections.OrderedDict()
+                with_blast_res = collections.OrderedDict()
+                for ont in ['bp', 'mf', 'cc']:
+                    # extract the predictions and labels of zero shot terms
+                    results[ont] = collections.OrderedDict()
+                    with_blast_res[ont] = collections.OrderedDict()
+                    for n in range(1, 20):
+                        ont_terms = get_few_shot_namespace_terms(files.fold_few_shot_terms_list[fold_i], files.go_data, ont, n)
+                        # evaluate without blast
+                        logits_ont, label_ont = term2preds_label(logits, label, ont_terms, files.terms2i)
+                        auroc_mean, auroc_pct = auroc_metrics(label_ont, logits_ont)
+                        results[ont][n] = auroc_mean
+                        # evaluate with blast
+                        logits_blast_ont, label_ont = term2preds_label(logits_with_blast, label, ont_terms, files.terms2i)
+                        auroc_blast_mean, auroc_blast_pct = auroc_metrics(label_ont, logits_blast_ont)
+                        with_blast_res[ont][n] = auroc_blast_mean
+                        self.logger.info('fold:{} ont: {} sample number: {} roc auc:{} add blast: {}'.format(fold_i, ont, n, auroc_mean, auroc_blast_mean))
+                # append the results of fold i without blast predictions and with blast predictions
+                results_list.append(results)
+                with_blast_res_list.append(with_blast_res)
+
+        # save the results
+        save_obj(results_list, cfg.results_name)
+        if cfg.task == 'few_shot':
+            save_obj(with_blast_res_list, cfg.blast_res_name)
+
+    def annotate(self, files, cfg, data_dir, anno_data, task='prot_func_pred'):
+        def zero_shot_terms():
+            zero_shot_term_path = data_dir + 'zero_shot_terms.pkl'
+            zero_shot_terms = load_obj(zero_shot_term_path)
+            return zero_shot_terms
+
+        def term2preds_label(preds, terms, terms2id):
+            new_preds = []
+            for t_id in terms:
+                new_preds.append(preds[:, terms2id[t_id]].reshape((-1, 1)))
+            new_preds = np.concatenate(new_preds, axis=1)
+            return new_preds
+
+        def zero_shot_data(zero_shot_terms_list, train):
+            drop_index = []
+            for j in train.index:
+                annts = train.loc[j]['annotations']
+                insct = list(set(annts).intersection(zero_shot_terms_list))
+                if len(insct) > 0:
+                    drop_index.append(j)
+            train = train.drop(index=drop_index)
+            return train
+
+        # data_path = data_dir + anno_file
+        # print('Annotate {} dataset in zero shot with our model'.format(data_path))
+        # anno_data = pd.read_pickle(data_path)
+        anno_loader = DataLoader(anno_data, batch_size=cfg.batch_size, shuffle=True)
+
+        print('Annotate Data with Our Model ...')
+        logits, prots = [], []
+        with torch.no_grad():
+            for batch in anno_loader:
+                pred_batch = self.model(batch['prot_seq'], batch['prot_description'],
+                                        batch['prot_network'], files.text_embeddings)
+                prots += batch['proteins']
+                logits.append(pred_batch.cpu().numpy())
+        logits = np.concatenate(logits, axis=0)
+
+        # if cfg.task == 'zero_shot':
+        zero_shot_terms = zero_shot_terms()
+        zero_shot_data(zero_shot_terms, files.raw_train)
+        logits_ont = collections.OrderedDict()
+        for ont in ['bp', 'mf', 'cc']:
+            # extract the predictions and labels of zero shot terms
+            ont_terms = get_namespace_terms(list(files.zero_shot_terms.keys()), files.go_data, ont)
+            logits_ont[ont] = term2preds_label(logits, ont_terms, files.terms2i)
+        return logits_ont
```

### Comparing `biotranslator-0.1.1/biotranslator/trainer/_vector_trainer.py` & `biotranslator-0.1.2/biotranslator/trainer/_vector_trainer.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-import os
-import torch
-import collections
-import numpy as np
-from tqdm import tqdm
-from ..biotranslator import BioTranslator
-from torch.utils.data import DataLoader
-from ..utils import save_obj, load_obj, get_logger, evaluate_auroc, evaluate_unseen_auroc, evaluate_auprc, \
-    evaluate_unseen_auprc
-
-
-class VecTrainer:
-
-    def __init__(self, files, cfg):
-        """
-        This class mainly include the training of BioTranslator Model
-        :param files:
-        """
-
-    def setup_model(self, files, cfg):
-        cfg.expr_dim = files.ngene
-        self.model = BioTranslator(cfg)
-
-    def setup_training(self, cfg):
-        # train epochs
-        self.epoch = cfg.epoch
-        # loss function
-        self.loss_func = torch.nn.BCELoss()
-        # use Adam as optimizer
-        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=cfg.lr)
-
-    def backward_model(self, input_expr, emb_tensor, label):
-        logits = self.model(data_type='vec',
-                            input_expr=input_expr,
-                            texts=emb_tensor)
-        self.loss = self.loss_func(logits, label)
-        self.optimizer.zero_grad()
-        self.loss.backward()
-        self.optimizer.step()
-        return self.loss.item()
-
-    def train(self, files, cfg):
-        # store the results of each fold in one list
-        results_cache = collections.OrderedDict()
-        results_var = ['unseen_auroc', 'auroc', 'unseen_auprc', 'auprc']
-        if cfg.task == 'same_dataset':
-            for var in results_var:
-                results_cache[var] = collections.OrderedDict()
-                for unseen_ratio in cfg.unseen_ratio:
-                    results_cache[var][unseen_ratio] = []
-        # record the performance of our model
-        self.logger = get_logger(cfg.logger_name)
-        for unseen_ratio in cfg.unseen_ratio:
-            for fold_i in range(cfg.n_iter):
-                if cfg.task == 'same_dataset':
-                    print('Start Cross-Validation Fold :{} Unseen Ratio: {}...'.format(fold_i, unseen_ratio))
-                    files.generate_data(fold_i, unseen_ratio)
-                elif cfg.task == 'cross_dataset':
-                    print('Start Cross-Dataset Train :{} Validation: {}...'.format(cfg.dataset, cfg.eval_dataset))
-                    files.generate_data()
-
-                train_loader = DataLoader(files.train_data, batch_size=cfg.batch_size, shuffle=True)
-                eval_loader = DataLoader(files.test_data, batch_size=cfg.batch_size)
-
-                # setup the model architecture according the methods
-                self.setup_model(files, cfg)
-                # setup dataset, the training loss and optimizer
-                self.setup_training(cfg)
-
-                # train the model
-                pbar = tqdm(range(self.epoch), desc='Training')
-                for epoch_i in pbar:
-                    train_loss = 0
-                    train_count = 0
-                    for batch in train_loader:
-                        train_loss += self.backward_model(batch['features'], files.train_emb, batch['label'])
-                        train_count += len(batch)
-                        pbar.set_postfix({"Fold": fold_i,
-                                          "epoch": epoch_i,
-                                          "train loss": train_loss / train_count})
-
-                # evaluate the model
-                print('Evaluate Our Model ...')
-                eval_loss, eval_count = 0, 0
-                logits, label = [], []
-                with torch.no_grad():
-                    for batch in eval_loader:
-                        pred_batch = self.model(input_expr=batch['features'], texts=files.test_emb)
-                        eval_loss += self.loss_func(pred_batch, batch['label']).item()
-                        eval_count += len(batch)
-                        self.loss_func.zero_grad()
-                        logits.append(pred_batch.cpu().numpy())
-                        label.append(batch['label'].cpu().float().numpy())
-                logits, label = np.concatenate(logits, axis=0), np.concatenate(label, axis=0)
-
-                # evaluate the model on the zero shot tasks or the few shot tasks
-                if cfg.task == 'same_dataset':
-                    unseen_auroc = evaluate_unseen_auroc(logits, label, files.unseen2i)
-                    auroc = evaluate_auroc(logits, label)
-                    unseen_auprc = evaluate_unseen_auprc(logits, label, files.unseen2i)
-                    auprc = evaluate_auprc(logits, label)
-                    self.logger.info(
-                        'Test all AUROCs :{} unseen AUROCs:{} AUPRCs :{} unseen AUPRCs:{}'.format(auroc, unseen_auroc,
-                                                                                                  auprc,
-                                                                                                  unseen_auprc))
-                    results_cache['auroc'][unseen_ratio].append(auroc)
-                    results_cache['unseen_auroc'][unseen_ratio].append(unseen_auroc)
-                    results_cache['auprc'][unseen_ratio].append(auprc)
-                    results_cache['unseen_auprc'][unseen_ratio].append(unseen_auprc)
-                    torch.save(self.model, cfg.save_model_path.format(cfg.method, cfg.dataset, fold_i, unseen_ratio))
-
-                if cfg.task == 'cross_dataset':
-                    unseen_auroc = evaluate_unseen_auroc(logits, label, files.unseen2i)
-                    auroc = evaluate_auroc(logits, label)
-                    unseen_auprc = evaluate_unseen_auprc(logits, label, files.unseen2i)
-                    auprc = evaluate_auprc(logits, label)
-                    self.logger.info(
-                        'Test all AUROCs :{} unseen AUROCs:{} AUPRCs :{} unseen AUPRCs:{}'.format(auroc, unseen_auroc,
-                                                                                                  auprc,
-                                                                                                  unseen_auprc))
-                    results_cache['auroc'] = auroc
-                    results_cache['unseen_auroc'] = unseen_auroc
-                    results_cache['auprc'] = auprc
-                    results_cache['unseen_auprc'] = unseen_auprc
-                    torch.save(self.model, cfg.save_model_path.format(cfg.method, cfg.dataset, cfg.eval_dataset))
-
-        # save the results
-        save_obj(results_cache, cfg.results_name)
-
-    def annotate(self, files, cfg, data_dir, anno_data, task='cell_type_cls'):
-        annotation = collections.OrderedDict()
-        # data_path = data_dir + anno_file
-        # anno_data = pd.read_pickle(data_path)
-        for unseen_ratio in cfg.unseen_ratio:
-            print('Start Annotation: {}...'.format(cfg.dataset, cfg.eval_dataset))
-            files.generate_data()
-            anno_loader = DataLoader(anno_data, batch_size=cfg.batch_size)
-            print('Annotate Data with Our Model ...')
-            logits = []
-            with torch.no_grad():
-                for batch in anno_loader:
-                    pred_batch = self.model(input_expr=batch['features'], texts=files.test_emb)
-                    logits.append(pred_batch.cpu().numpy())
-            logits = np.concatenate(logits, axis=0)
-            annotation[unseen_ratio] = logits
-        return annotation
+import os
+import torch
+import collections
+import numpy as np
+from tqdm import tqdm
+from ..biotranslator import BioTranslator
+from torch.utils.data import DataLoader
+from ..utils import save_obj, load_obj, get_logger, evaluate_auroc, evaluate_unseen_auroc, evaluate_auprc, \
+    evaluate_unseen_auprc
+
+
+class VecTrainer:
+
+    def __init__(self, files, cfg):
+        """
+        This class mainly include the training of BioTranslator Model
+        :param files:
+        """
+
+    def setup_model(self, files, cfg):
+        cfg.expr_dim = files.ngene
+        self.model = BioTranslator(cfg)
+
+    def setup_training(self, cfg):
+        # train epochs
+        self.epoch = cfg.epoch
+        # loss function
+        self.loss_func = torch.nn.BCELoss()
+        # use Adam as optimizer
+        self.optimizer = torch.optim.Adam(self.model.parameters(), lr=cfg.lr)
+
+    def backward_model(self, input_expr, emb_tensor, label):
+        logits = self.model(data_type='vec',
+                            input_expr=input_expr,
+                            texts=emb_tensor)
+        self.loss = self.loss_func(logits, label)
+        self.optimizer.zero_grad()
+        self.loss.backward()
+        self.optimizer.step()
+        return self.loss.item()
+
+    def train(self, files, cfg):
+        # store the results of each fold in one list
+        results_cache = collections.OrderedDict()
+        results_var = ['unseen_auroc', 'auroc', 'unseen_auprc', 'auprc']
+        if cfg.task == 'same_dataset':
+            for var in results_var:
+                results_cache[var] = collections.OrderedDict()
+                for unseen_ratio in cfg.unseen_ratio:
+                    results_cache[var][unseen_ratio] = []
+        # record the performance of our model
+        self.logger = get_logger(cfg.logger_name)
+        for unseen_ratio in cfg.unseen_ratio:
+            for fold_i in range(cfg.n_iter):
+                if cfg.task == 'same_dataset':
+                    print('Start Cross-Validation Fold :{} Unseen Ratio: {}...'.format(fold_i, unseen_ratio))
+                    files.generate_data(fold_i, unseen_ratio)
+                elif cfg.task == 'cross_dataset':
+                    print('Start Cross-Dataset Train :{} Validation: {}...'.format(cfg.dataset, cfg.eval_dataset))
+                    files.generate_data()
+
+                train_loader = DataLoader(files.train_data, batch_size=cfg.batch_size, shuffle=True)
+                eval_loader = DataLoader(files.test_data, batch_size=cfg.batch_size)
+
+                # setup the model architecture according the methods
+                self.setup_model(files, cfg)
+                # setup dataset, the training loss and optimizer
+                self.setup_training(cfg)
+
+                # train the model
+                pbar = tqdm(range(self.epoch), desc='Training')
+                for epoch_i in pbar:
+                    train_loss = 0
+                    train_count = 0
+                    for batch in train_loader:
+                        train_loss += self.backward_model(batch['features'], files.train_emb, batch['label'])
+                        train_count += len(batch)
+                        pbar.set_postfix({"Fold": fold_i,
+                                          "epoch": epoch_i,
+                                          "train loss": train_loss / train_count})
+
+                # evaluate the model
+                print('Evaluate Our Model ...')
+                eval_loss, eval_count = 0, 0
+                logits, label = [], []
+                with torch.no_grad():
+                    for batch in eval_loader:
+                        pred_batch = self.model(input_expr=batch['features'], texts=files.test_emb)
+                        eval_loss += self.loss_func(pred_batch, batch['label']).item()
+                        eval_count += len(batch)
+                        self.loss_func.zero_grad()
+                        logits.append(pred_batch.cpu().numpy())
+                        label.append(batch['label'].cpu().float().numpy())
+                logits, label = np.concatenate(logits, axis=0), np.concatenate(label, axis=0)
+
+                # evaluate the model on the zero shot tasks or the few shot tasks
+                if cfg.task == 'same_dataset':
+                    unseen_auroc = evaluate_unseen_auroc(logits, label, files.unseen2i)
+                    auroc = evaluate_auroc(logits, label)
+                    unseen_auprc = evaluate_unseen_auprc(logits, label, files.unseen2i)
+                    auprc = evaluate_auprc(logits, label)
+                    self.logger.info(
+                        'Test all AUROCs :{} unseen AUROCs:{} AUPRCs :{} unseen AUPRCs:{}'.format(auroc, unseen_auroc,
+                                                                                                  auprc,
+                                                                                                  unseen_auprc))
+                    results_cache['auroc'][unseen_ratio].append(auroc)
+                    results_cache['unseen_auroc'][unseen_ratio].append(unseen_auroc)
+                    results_cache['auprc'][unseen_ratio].append(auprc)
+                    results_cache['unseen_auprc'][unseen_ratio].append(unseen_auprc)
+                    torch.save(self.model, cfg.save_model_path.format(cfg.method, cfg.dataset, fold_i, unseen_ratio))
+
+                if cfg.task == 'cross_dataset':
+                    unseen_auroc = evaluate_unseen_auroc(logits, label, files.unseen2i)
+                    auroc = evaluate_auroc(logits, label)
+                    unseen_auprc = evaluate_unseen_auprc(logits, label, files.unseen2i)
+                    auprc = evaluate_auprc(logits, label)
+                    self.logger.info(
+                        'Test all AUROCs :{} unseen AUROCs:{} AUPRCs :{} unseen AUPRCs:{}'.format(auroc, unseen_auroc,
+                                                                                                  auprc,
+                                                                                                  unseen_auprc))
+                    results_cache['auroc'] = auroc
+                    results_cache['unseen_auroc'] = unseen_auroc
+                    results_cache['auprc'] = auprc
+                    results_cache['unseen_auprc'] = unseen_auprc
+                    torch.save(self.model, cfg.save_model_path.format(cfg.method, cfg.dataset, cfg.eval_dataset))
+
+        # save the results
+        save_obj(results_cache, cfg.results_name)
+
+    def annotate(self, files, cfg, data_dir, anno_data, task='cell_type_cls'):
+        annotation = collections.OrderedDict()
+        # data_path = data_dir + anno_file
+        # anno_data = pd.read_pickle(data_path)
+        for unseen_ratio in cfg.unseen_ratio:
+            print('Start Annotation: {}...'.format(cfg.dataset, cfg.eval_dataset))
+            files.generate_data()
+            anno_loader = DataLoader(anno_data, batch_size=cfg.batch_size)
+            print('Annotate Data with Our Model ...')
+            logits = []
+            with torch.no_grad():
+                for batch in anno_loader:
+                    pred_batch = self.model(input_expr=batch['features'], texts=files.test_emb)
+                    logits.append(pred_batch.cpu().numpy())
+            logits = np.concatenate(logits, axis=0)
+            annotation[unseen_ratio] = logits
+        return annotation
```

### Comparing `biotranslator-0.1.1/biotranslator/utils/_utils.py` & `biotranslator-0.1.2/biotranslator/utils/_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1564 +1,1564 @@
-import os
-import sys
-import torch
-import logging
-import scipy
-import time
-import pickle
-import collections
-import numpy as np
-import pandas as pd
-import warnings
-from torch import nn
-import networkx as nx
-from tqdm import tqdm
-from torch import squeeze
-from torch.nn import init
-from collections import deque
-from gensim import corpora, models
-from scipy.sparse.linalg import svds
-from nltk.tokenize import word_tokenize
-from torch.utils.data import ConcatDataset
-from gensim.models.word2vec import Word2Vec
-import torchvision.transforms as transforms
-from transformers import AutoTokenizer, AutoModel
-from gensim.models.doc2vec import Doc2Vec, TaggedDocument
-from scipy import sparse
-from scipy import spatial
-from anndata import read_h5ad
-from collections import Counter
-from scipy.sparse.csr import csr_matrix
-from sklearn.metrics import roc_auc_score, roc_curve
-from sklearn.model_selection import train_test_split
-from sklearn.metrics.pairwise import cosine_similarity
-from scipy.sparse.csgraph._shortest_path import shortest_path
-# from sklearn.utils.graph_shortest_path import graph_shortest_path
-from sklearn.metrics import auc, average_precision_score, precision_recall_curve
-
-import nltk
-
-nltk.download('punkt')
-
-
-def save_obj(obj, name):
-    with open(name, 'wb') as f:
-        pickle.dump(obj, f, pickle.HIGHEST_PROTOCOL)
-
-
-def load_obj(name):
-    with open(name, 'rb') as f:
-        return pickle.load(f)
-
-
-def load(filename, with_rels=True):
-    ont = dict()
-    obj = None
-    with open(filename, 'r') as f:
-        for line in f:
-            line = line.strip()
-            if not line:
-                continue
-            if line == '[Term]':
-                if obj is not None:
-                    ont[obj['id']] = obj
-                obj = dict()
-                obj['is_a'] = list()
-                obj['part_of'] = list()
-                obj['regulates'] = list()
-                obj['alt_ids'] = list()
-                obj['def'] = list()
-                obj['is_obsolete'] = False
-                continue
-            elif line == '[Typedef]':
-                if obj is not None:
-                    ont[obj['id']] = obj
-                obj = None
-            else:
-                if obj is None:
-                    continue
-                l = line.split(": ")
-                if l[0] == 'id':
-                    obj['id'] = l[1]
-                elif l[0] == 'alt_id':
-                    obj['alt_ids'].append(l[1])
-                elif l[0] == 'namespace':
-                    obj['namespace'] = l[1]
-                elif l[0] == 'def':
-                    obj['def'].append(l[1].split('"')[1])
-                elif l[0] == 'is_a':
-                    obj['is_a'].append(l[1].split(' ! ')[0])
-                elif with_rels and l[0] == 'relationship':
-                    it = l[1].split()
-                    # add all types of relationships
-                    obj['is_a'].append(it[1])
-                elif l[0] == 'name':
-                    obj['name'] = l[1]
-                elif l[0] == 'is_obsolete' and l[1] == 'true':
-                    obj['is_obsolete'] = True
-        if obj is not None:
-            ont[obj['id']] = obj
-    for term_id in list(ont.keys()):
-        for t_id in ont[term_id]['alt_ids']:
-            ont[t_id] = ont[term_id]
-        if ont[term_id]['is_obsolete']:
-            del ont[term_id]
-    for term_id, val in ont.items():
-        if 'children' not in val:
-            val['children'] = set()
-        for p_id in val['is_a']:
-            if p_id in ont:
-                if 'children' not in ont[p_id]:
-                    ont[p_id]['children'] = set()
-                ont[p_id]['children'].add(term_id)
-    return ont
-
-
-def get_ontology_embeddings(cfg):
-    """Get the textual description embeddings of Gene Ontology (GO) or Cell Ontology (CO) terms
-
-    Parameters
-    ----------
-    cfg:
-        config
-
-    Returns
-    -------
-    ont_embeddings:
-        the ontology embeddings
-    """
-
-    """This function uses the BioTranslator Text Encoder to embed the Gene Ontology terms
-    :param cfg:
-    :return:
-    """
-    embeddings = collections.OrderedDict()
-    bert_name = 'microsoft/BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext'
-    tokenizer = AutoTokenizer.from_pretrained('microsoft/BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext')
-    model = NeuralNetwork('None', 'cls', bert_name)
-    model.load_state_dict(torch.load(cfg.encoder_path))
-    model = model.to('cuda')
-    model.eval()
-
-    if cfg.tp in ['seq', 'graph']:
-        if cfg.task not in ["single-dataset", "cross-dataset"]:
-            # go embedding
-            data = load(cfg.go_file)
-            classes = list(data.keys())
-            texts = []
-            for i in tqdm(range(len(classes))):
-                with torch.no_grad():
-                    texts.append(data[classes[i]]['name'] + '. ' + data[classes[i]]['def'][0])
-        else:
-            # co embedding
-            text = load_co_text(cfg.ontology_repo + 'cl.obo')
-            classes = list(text.keys())
-            texts = []
-            for i in tqdm(range(len(classes))):
-                with torch.no_grad():
-                    texts.append(text[classes[i]]['text'])
-    elif cfg.tp == 'cell':
-        # co embedding
-        text = load_co_text(cfg.ontology_repo + 'cl.obo')
-        classes = list(text.keys())
-        texts = []
-        for i in tqdm(range(len(classes))):
-            with torch.no_grad():
-                texts.append(text[classes[i]]['text'])
-
-    with torch.no_grad():
-        for i in tqdm(range(len(classes))):
-            text = texts[i]
-            inputs = tokenizer(text, return_tensors='pt').to('cuda')
-            if len(cfg.gpu_ids) > 0:
-                inputs = inputs.to('cuda')
-            sents_len = min(inputs['input_ids'].size(1), 512)
-            input_ids = inputs['input_ids'][0, 0: sents_len].view(len(inputs['input_ids']), -1).to('cuda')
-            attention_mask = inputs['attention_mask'][0, 0: sents_len].view(len(inputs['attention_mask']),
-                                                                            -1).to(
-                'cuda')
-            token_type_ids = inputs['token_type_ids'][0, 0: sents_len].view(len(inputs['token_type_ids']),
-                                                                            -1).to(
-                'cuda')
-
-            pred = model(input_ids, attention_mask, token_type_ids)
-            embeddings[classes[i]] = np.asarray(pred.cpu()).reshape([-1, 768])
-        save_obj(embeddings, cfg.emb_path + cfg.emb_name)
-    return embeddings
-
-
-def get_anchestors(go, term_id):
-    if term_id not in go:
-        return []
-    term_set = []
-    q = deque()
-    q.append(term_id)
-    while (len(q) > 0):
-        t_id = q.popleft()
-        if t_id not in term_set:
-            term_set.append(t_id)
-            for parent_id in go[t_id]['is_a']:
-                if parent_id in go:
-                    q.append(parent_id)
-    return term_set
-
-
-def init_weights(net, init_type='normal', init_gain=0.02):
-    """Initialize network weights.
-    Parameters:
-        net (network)   -- network to be initialized
-        init_type (str) -- the name of an initialization method: normal | xavier | kaiming | orthogonal
-        init_gain (float)    -- scaling factor for normal, xavier and orthogonal.
-    We use 'normal' in the original pix2pix and CycleGAN paper. But xavier and kaiming might
-    work better for some applications. Feel free to try yourself.
-    """
-
-    def init_func(m):  # define the initialization function
-        classname = m.__class__.__name__
-        if hasattr(m, 'weight') and (classname.find('Conv') != -1 or classname.find('Linear') != -1):
-            if init_type == 'normal':
-                init.normal_(m.weight.data, 0.0, init_gain)
-            elif init_type == 'xavier':
-                init.xavier_normal_(m.weight.data, gain=init_gain)
-            elif init_type == 'kaiming':
-                init.kaiming_normal_(m.weight.data, a=0, mode='fan_in')
-            elif init_type == 'orthogonal':
-                init.orthogonal_(m.weight.data, gain=init_gain)
-            else:
-                raise NotImplementedError('initialization method [%s] is not implemented' % init_type)
-            if hasattr(m, 'bias') and m.bias is not None:
-                init.constant_(m.bias.data, 0.0)
-        elif classname.find(
-                'BatchNorm2d') != -1:  # BatchNorm Layer's weight is not a matrix; only normal distribution applies.
-            init.normal_(m.weight.data, 1.0, init_gain)
-            init.constant_(m.bias.data, 0.0)
-
-    print('initialize network with %s' % init_type)
-    net.apply(init_func)  # apply the initialization function <init_func>
-
-
-def get_logger(logfile):
-    '''
-    This function are copied from https://blog.csdn.net/a232884c/article/details/117453011
-    :param logfile:
-    :return:
-    '''
-    logger = logging.getLogger()
-    logger.setLevel(logging.INFO)
-    fh = logging.FileHandler(logfile, mode='w')
-    fh.setLevel(logging.DEBUG)
-    formatter = logging.Formatter("%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s")
-    fh.setFormatter(formatter)
-    logger.addHandler(fh)
-    ch = logging.StreamHandler()
-    ch.setLevel(logging.DEBUG)
-    ch.setFormatter(formatter)
-    logger.addHandler(ch)
-    return logger
-
-
-def renorm(X):
-    Y = X.copy()
-    Y = Y.astype(float)
-    ngene, nsample = Y.shape
-    s = np.sum(Y, axis=0)
-    # print s.shape()
-    for i in range(nsample):
-        if s[i] == 0:
-            s[i] = 1
-            if i < ngene:
-                Y[i, i] = 1
-            else:
-                for j in range(ngene):
-                    Y[j, i] = 1. / ngene
-        Y[:, i] = Y[:, i] / s[i]
-    return Y
-
-
-def DCA_vector(Q, dim):
-    nnode = Q.shape[0]
-    alpha = 1. / (nnode ** 2)
-    Q = np.log(Q + alpha) - np.log(alpha)
-
-    # Q = Q * Q';
-    [U, S, V] = svds(Q, dim)
-    S = np.diag(S)
-    X = np.dot(U, np.sqrt(S))
-    Y = np.dot(np.sqrt(S), V)
-    Y = np.transpose(Y)
-    return X, U, S, V, Y
-
-
-class Dataset(object):
-
-    def __getitem__(self, index):
-        raise NotImplementedError
-
-    def __len__(self):
-        raise NotImplementedError
-
-    def __add__(self, other):
-        return ConcatDataset([self, other])
-
-
-def one_hot(seq, start=0, max_len=2000):
-    '''
-    One-Hot encodings of protein sequences,
-    this function was copied from DeepGOPlus paper
-    :param seq:
-    :param start:
-    :param max_len:
-    :return:
-    '''
-    AALETTER = [
-        'A', 'R', 'N', 'D', 'C', 'Q', 'E', 'G', 'H', 'I',
-        'L', 'K', 'M', 'F', 'P', 'S', 'T', 'W', 'Y', 'V']
-    AAINDEX = dict()
-    for i in range(len(AALETTER)):
-        AAINDEX[AALETTER[i]] = i + 1
-    onehot = np.zeros((21, max_len), dtype=np.int32)
-    l = min(max_len, len(seq))
-    for i in range(start, start + l):
-        onehot[AAINDEX.get(seq[i - start], 0), i] = 1
-    onehot[0, 0:start] = 1
-    onehot[0, start + l:] = 1
-    return onehot
-
-
-class proteinData(Dataset):
-    '''
-    The dataset of protein
-    '''
-
-    def __init__(self, data_df, terms, prot_vector, prot_description, gpu_ids='0'):
-        self.p_ids = []
-        self.pSeq = []
-        self.label = []
-        self.vector = []
-        self.description = []
-        self.gpu_ids = gpu_ids
-        sequences = list(data_df['sequences'])
-        prot_ids = list(data_df['proteins'])
-        annots = list(data_df['annotations'])
-        for i in range(len(annots)):
-            annots[i] = list(annots[i])
-        for i in range(data_df.shape[0]):
-            seqT, annT, protT = sequences[i], annots[i], prot_ids[i]
-            labelT = np.zeros([len(terms), 1])
-            for j in range(len(annT)):
-                if annT[j] in terms.keys():
-                    labelT[terms[annT[j]]] = 1
-            self.p_ids.append(protT)
-            self.pSeq.append(one_hot(seqT))
-            self.label.append(labelT)
-            self.vector.append(prot_vector[protT])
-            self.description.append((prot_description[protT]))
-
-    def __getitem__(self, item):
-        in_seq, label = transforms.ToTensor()(self.pSeq[item]), transforms.ToTensor()(self.label[item])
-        description = torch.from_numpy(self.description[item])
-        vector = torch.from_numpy(self.vector[item])
-        if len(self.gpu_ids) > 0:
-            return {'proteins': self.p_ids[item],
-                    'prot_seq': squeeze(in_seq).float().cuda(),
-                    'prot_description': squeeze(description).float().cuda(),
-                    'prot_network': squeeze(vector).float().cuda(),
-                    'label': squeeze(label).float().cuda()}
-        else:
-            return {'proteins': self.p_ids[item],
-                    'prot_seq': squeeze(in_seq).float(),
-                    'prot_description': squeeze(description).float(),
-                    'prot_network': squeeze(vector).float(),
-                    'label': squeeze(label).float()}
-
-    def __len__(self):
-        return len(self.pSeq)
-
-
-class NeuralNetwork(nn.Module):
-    def __init__(self, model_path, output_way, bert_name):
-        super(NeuralNetwork, self).__init__()
-        self.bert = AutoModel.from_pretrained(bert_name)
-        self.output_way = output_way
-
-    def forward(self, input_ids, attention_mask, token_type_ids):
-        x1 = self.bert(input_ids, attention_mask=attention_mask, token_type_ids=token_type_ids)
-        if self.output_way == 'cls':
-            output = x1.last_hidden_state[:, 0]
-        elif self.output_way == 'pooler':
-            output = x1.pooler_output
-        return output
-
-
-def term2preds_label(preds, label, terms, terms2id):
-    new_preds, new_label = [], []
-    for t_id in terms:
-        new_preds.append(preds[:, terms2id[t_id]].reshape((-1, 1)))
-        new_label.append(label[:, terms2id[t_id]].reshape((-1, 1)))
-    new_preds = np.concatenate(new_preds, axis=1)
-    new_label = np.concatenate(new_label, axis=1)
-    return new_preds, new_label
-
-
-def organize_workingspace(workingspace, task=None):
-    """
-    Make sure that the working space include the zero shot folder, few shot folder,
-    model folder, training log folder and results folder
-    :param workingspace:
-    :return:
-    """
-    task_path = workingspace + task
-    cache_path = task_path + '/cache'
-    model_path = task_path + '/model'
-    logger_path = task_path + '/log'
-    results_path = task_path + '/results'
-    if not os.path.exists(workingspace):
-        os.mkdir(workingspace)
-        print('Warning: We created the working space: {}'.format(workingspace))
-    if not os.path.exists(task_path):
-        os.mkdir(task_path)
-    if not os.path.exists(cache_path):
-        os.mkdir(cache_path)
-    if not os.path.exists(model_path):
-        os.mkdir(model_path)
-    if not os.path.exists(logger_path):
-        os.mkdir(logger_path)
-    if not os.path.exists(results_path):
-        os.mkdir(results_path)
-
-
-def get_namespace_terms(terms, go, namespace):
-    # select terms in the namespace
-    name_dict = {'bp': 'biological_process', 'mf': 'molecular_function', 'cc': 'cellular_component'}
-    new_terms = []
-    for t_id in terms:
-        if go[t_id]['namespace'] == name_dict[namespace]:
-            new_terms.append(t_id)
-    return new_terms
-
-
-def get_few_shot_namespace_terms(term_count, go, namespace, n=10):
-    # select terms in namespace with less than n training sample
-    name_dict = {'bp': 'biological_process', 'mf': 'molecular_function', 'cc': 'cellular_component'}
-    new_terms = []
-    for t_id in term_count.keys():
-        if go[t_id]['namespace'] == name_dict[namespace]:
-            if term_count[t_id] <= n:
-                new_terms.append(t_id)
-    return new_terms
-
-
-def term_training_numbers(val_data, train_data):
-    '''
-    This function calculates how many training samples exists in the
-    :param val_data:
-    :param train_data:
-    :return:
-    '''
-    term2number = collections.OrderedDict()
-    for annt_val in list(val_data['annotations']):
-        for a_id in annt_val:
-            term2number[a_id] = 0
-    training_annt = list(train_data['annotations'])
-    for annt in training_annt:
-        annt = list(set(annt))
-        for a_id in annt:
-            if a_id not in term2number.keys():
-                continue
-            term2number[a_id] += 1
-    return term2number
-
-
-def compute_blast_preds(diamond_scores,
-                        test,
-                        train_data):
-    '''
-    This function computes the predictions of blast results.
-    The codes here are borrowed from the DeepGOPlus paper
-    :param diamond_scores:
-    :param test:
-    :param train_data:
-    :param is_load:
-    :param save_path:
-    :return:
-    '''
-    blast_preds = collections.OrderedDict()
-    print('Diamond preds')
-    annotation_dict = collections.OrderedDict()
-    for i in train_data.index:
-        prot_id = train_data.loc[i]['proteins']
-        annts = set(train_data.loc[i]['annotations'])
-        if prot_id not in annotation_dict.keys():
-            annotation_dict[prot_id] = collections.OrderedDict()
-            for ann_id in annts:
-                annotation_dict[prot_id][ann_id] = None
-        else:
-            for ann_id in annts:
-                annotation_dict[prot_id][ann_id] = None
-
-    for prot_id in tqdm(test.proteins):
-        annots = {}
-
-        # BlastKNN
-        sim = collections.OrderedDict()
-        if prot_id in diamond_scores.keys():
-            sim_prots = diamond_scores[prot_id]
-            allgos = set()
-            total_score = 0.0
-            for p_id, score in sim_prots.items():
-                allgos |= set(annotation_dict[p_id].keys())
-                total_score += score
-            allgos = set(allgos)
-            for go_id in allgos:
-                s = 0.0
-                for p_id in sim_prots.keys():
-                    score = sim_prots[p_id]
-                    if go_id in annotation_dict[p_id].keys():
-                        s += score
-                sim[go_id] = s / total_score
-        blast_preds[prot_id] = sim
-    return blast_preds
-
-
-def extract_terms_from_dataset(dataset):
-    id = 0
-    terms2id = collections.OrderedDict()
-    id2terms = collections.OrderedDict()
-    for i in dataset.index:
-        annts = dataset.iloc[i]['annotations']
-        for annt in annts:
-            if annt not in terms2id:
-                terms2id[annt] = id
-                id2terms[id] = annt
-                id += 1
-    return terms2id, id2terms
-
-
-def coef_vec(A, B):
-    coefs_array = []
-    for i in range(np.size(A, 0)):
-        a1 = A[i, :]
-        b1 = B[i, :]
-        coefs = np.corrcoef(a1, b1)[0, 1]
-        coefs_array.append(coefs)
-    return np.asarray(coefs_array)
-
-
-def sample_edges(st=0, ed=1000, n=100, exclude_edges=[]):
-    samples = []
-    while True:
-        nodes = np.arange(st, ed)
-        np.random.shuffle(nodes)
-        edge = list(nodes[0: 2])
-        if edge not in exclude_edges and edge not in samples:
-            samples.append(edge)
-        if len(samples) == n:
-            break
-    return np.asarray(samples)
-
-
-def edge_probability(encodings_i, encodings_j, text_encodings_p):
-    s1 = np.dot(encodings_i, np.transpose(text_encodings_p))
-    s1 = 1 / (1 + np.exp(-s1))
-    s2 = np.dot(encodings_j, np.transpose(text_encodings_p))
-    s2 = 1 / (1 + np.exp(-s2))
-    s3 = coef_vec(encodings_i, encodings_j)
-    score = s3 * (0.5 * s1.squeeze() + 0.5 * s2.squeeze())
-    return score
-
-
-def RandomWalkRestart(A, rst_prob, delta=1e-4, reset=None, max_iter=50, use_torch=False, return_torch=False):
-    device = torch.device('cpu')
-    if use_torch and torch.cuda.is_available():
-        device = torch.device('cuda:0')
-    nnode = A.shape[0]
-    if reset is None:
-        reset = np.eye(nnode)
-    nsample, nnode = reset.shape
-    # print nsample,nnode
-    P = renorm(A)
-    P = P.T
-    norm_reset = renorm(reset.T)
-    norm_reset = norm_reset.T
-    if use_torch:
-        norm_reset = torch.from_numpy(norm_reset).float().to(device)
-        P = torch.from_numpy(P).float().to(device)
-    Q = norm_reset
-
-    for i in range(1, max_iter):
-        if use_torch:
-            Q_new = rst_prob * norm_reset + (1 - rst_prob) * torch.mm(Q, P)  # .as_numpy_array()
-            delta = torch.norm(Q - Q_new, 2)
-        else:
-            Q_new = rst_prob * norm_reset + (1 - rst_prob) * np.dot(Q, P)  # .as_numpy_array()
-            delta = np.linalg.norm(Q - Q_new, 'fro')
-        Q = Q_new
-        # print (i,Q)
-        sys.stdout.flush()
-        if delta < 1e-4:
-            break
-    if use_torch and not return_torch:
-        Q = Q.cpu().numpy()
-    return Q
-
-
-def read_cell_type_nlp_network(nlp_emb_file, cell_type_network_file):
-    cell_ontology_ids = set()
-    fin = open(cell_type_network_file)
-    co2co_graph = {}
-    for line in fin:
-        w = line.strip().split('\t')
-        if w[0] not in co2co_graph:
-            co2co_graph[w[0]] = set()
-        co2co_graph[w[0]].add(w[1])
-        cell_ontology_ids.add(w[0])
-        cell_ontology_ids.add(w[1])
-    fin.close()
-    if nlp_emb_file is not None:
-        fin = open(nlp_emb_file)
-        co2vec_nlp = {}
-        for line in fin:
-            w = line.strip().split('\t')
-            vec = []
-            for i in range(1, len(w)):
-                vec.append(float(w[i]))
-            co2vec_nlp[w[0]] = np.array(vec)
-        fin.close()
-        co2co_nlp = {}
-        for id1 in co2co_graph:
-            co2co_nlp[id1] = {}
-            for id2 in co2co_graph[id1]:
-                sc = 1 - spatial.distance.cosine(co2vec_nlp[id1], co2vec_nlp[id2])
-                co2co_nlp[id1][id2] = sc
-    else:
-        co2co_nlp = {}
-        for id1 in co2co_graph:
-            co2co_nlp[id1] = {}
-            for id2 in co2co_graph[id1]:
-                co2co_nlp[id1][id2] = 1.
-        co2vec_nlp = {}
-        for c in cell_ontology_ids:
-            co2vec_nlp[c] = np.ones((10))
-    return co2co_graph, co2co_nlp, co2vec_nlp, cell_ontology_ids
-
-
-def subset_cell_type_nlp_network(co2co_graph, co2co_nlp, co2vec_nlp, cell_ontology_ids, subsets):
-    new_co2co_graph, new_co2co_nlp, new_co2vec_nlp = {}, {}, {}
-    new_co_ids = set()
-    for co_i in subsets:
-        if co_i in co2co_graph.keys():
-            co_i_cncts = co2co_graph[co_i]
-            new_cncts = set()
-            for co_i_cnct in co_i_cncts:
-                if co_i_cnct in subsets:
-                    new_cncts.add(co_i_cnct)
-            if len(new_cncts) > 0:
-                new_co2co_graph[co_i] = new_cncts
-        if co_i in co2co_nlp.keys():
-            co_i_cncts = co2co_nlp[co_i]
-            new_cncts = {}
-            for co_i_cnct in co_i_cncts.keys():
-                if co_i_cnct in subsets:
-                    new_co_ids.add(co_i_cnct)
-                    new_cncts[co_i_cnct] = co_i_cncts[co_i_cnct]
-            if len(new_cncts.keys()) > 0:
-                new_co_ids.add(co_i)
-                new_co2co_nlp[co_i] = new_cncts
-    for co_i in new_co_ids:
-        if co_i in co2vec_nlp.keys():
-            new_co2vec_nlp[co_i] = co2vec_nlp[co_i]
-    return new_co2co_graph, new_co2co_nlp, new_co2vec_nlp, new_co_ids
-
-
-def map_genes(test_X, test_genes, train_genes, num_batches=10, memory_saving_mode=False):
-    """
-    Takes in the test set features, test_X, and a list of all the genes in the training and test sets
-    and returns new_test_X, which makes the gene indices of test_X correspond to the same ones from the
-    training set.
-    """
-    ntest_cell = np.shape(test_X)[0]  # Number of cells in the test set
-    ntrain_gene = len(train_genes)  # Number of genes in the train set
-    genes = list(set(test_genes) & set(train_genes))  # Genes that are in both the train and test sets
-    train_genes = list(train_genes)
-    test_genes = list(test_genes)
-    # print("Mapping genes with memory mode =", memory_saving_mode,"...")
-    if not memory_saving_mode:
-        new_test_x = np.zeros((ntest_cell, ntrain_gene))
-        ind1 = []
-        ind2 = []
-        for i, g in enumerate(genes):
-            ind1.append(train_genes.index(g))
-            ind2.append(test_genes.index(g))
-        ind1 = np.array(ind1)
-        ind2 = np.array(ind2)
-        new_test_x[:, ind1] = test_X[:, ind2]
-    else:
-        new_test_x = sparse.csr_matrix((ntest_cell, ntrain_gene))
-        batch_size = int(len(genes) / num_batches)
-        for i in range(num_batches):
-            # print("\tbatch #",i)
-            ind1 = []
-            ind2 = []
-            if i != num_batches - 1:
-                batch = genes[i * batch_size: (i + 1) * batch_size]
-            else:
-                batch = genes[i * batch_size:]
-            for g in batch:
-                ind1.append(train_genes.index(g))
-                ind2.append(test_genes.index(g))
-            ind1 = np.array(ind1)
-            ind2 = np.array(ind2)
-            new_test_x[:, ind1] = test_X[:, ind2]
-    return new_test_x
-
-
-def process_expression(train_X, test_X, train_genes, test_genes):
-    # this data process function is adapted from ACTINN, please check ACTINN for more information.
-    test_X = map_genes(test_X, test_genes, train_genes)
-    c2g = np.vstack([train_X, test_X])
-    c2g = np.array(c2g, dtype=np.float64)
-    c2g = c2g.T
-    index = np.sum(c2g, axis=1) > 0
-    c2g = c2g[index, :]
-    train_genes = train_genes[index]
-    c2g = np.divide(c2g, np.sum(c2g, axis=0, keepdims=True)) * 10000
-    c2g = np.log2(c2g + 1)
-    expr = np.sum(c2g, axis=1)
-    # total_set = total_set[np.logical_and(expr >= np.percentile(expr, 1), expr <= np.percentile(expr, 99)),]
-    index = np.logical_and(expr >= np.percentile(expr, 1), expr <= np.percentile(expr, 99))
-    c2g = c2g[index,]
-    train_genes = train_genes[index]
-    # print (np.logical_and(expr >= np.percentile(expr, 1), expr <= np.percentile(expr, 99)))
-
-    cv = np.std(c2g, axis=1) / np.mean(c2g, axis=1)
-    index = np.logical_and(cv >= np.percentile(cv, 1), cv <= np.percentile(cv, 99))
-    c2g = c2g[index,]
-    train_genes = train_genes[index]
-    c2g = c2g.T
-    c2g_list_new = []
-    index = 0
-    for c in [train_X, test_X]:
-        ncell = np.shape(c)[0]
-        c2g_list_new.append(c2g[index:index + ncell, :])
-        index = ncell
-        assert (len(train_genes) == np.shape(c2g)[1])
-    return c2g_list_new[0], c2g_list_new[1], train_genes
-
-
-def mean_normalization(train_X_mean, test_X):
-    test_X = np.log1p(test_X)
-    test_X_mean = np.mean(test_X, axis=0)
-    test_X = test_X - test_X_mean + train_X_mean
-    return test_X
-
-
-def get_gene_mapping(test_genes, train_genes):
-    """
-    Low-memory version of map_genes. Takes the list of genes used by the test set and the list of
-    genes used in the training set. Provides a numpy array that maps the indices of the test genes
-    to the indices of the training genes.
-    For instance, if gene 'abcd' is at index 1 in train_genes, and at index 7 in test_genes, then
-    the numpy array returned from this function will have a 1 at index 7.
-    """
-    genes = list(set(test_genes) & set(train_genes))  # Genes that are in both the train and test sets
-    train_genes = list(train_genes)
-    test_genes = list(test_genes)
-    # print("Getting gene mapping...")
-
-    gene_idx = np.arange(len(test_genes))
-    for g in genes:
-        train_idx = train_genes.index(g)
-        test_idx = test_genes.index(g)
-        gene_idx[train_idx] = test_idx
-
-    return gene_idx
-
-
-def graph_embedding_dca(A, i2l, mi=0, dim=20, unseen_l=None):
-    nl = np.shape(A)[0]
-    seen_ind = []
-    unseen_ind = []
-    for i in range(nl):
-        if i2l[i] in unseen_l:
-            unseen_ind.append(i)
-        else:
-            seen_ind.append(i)
-    seen_ind = np.array(seen_ind)
-    unseen_ind = np.array(unseen_ind)
-
-    # if len(seen_ind) * 0.8 < dim:
-    #	dim = int(len(seen_ind) * 0.8)
-    if mi == 0 or mi == 1:
-        # sp = graph_shortest_path(A, method='FW', directed=False)
-        sp = shortest_path(A, method='FW', directed=False)
-    else:
-        sp = RandomWalkRestart(A, 0.8)
-
-    sp = sp[seen_ind, :]
-    sp = sp[:, seen_ind]
-    X = np.zeros((np.shape(sp)[0], dim))
-    print("dim: ", np.shape(sp)[0] - 1)
-    print("dim0: ", dim)
-    svd_dim = min(dim, np.shape(sp)[0] - 1)
-    if mi == 0 or mi == 2:
-        print('please set mi=3')
-        # X[:, :svd_dim] = svd_emb(sp, dim=svd_dim)
-    else:
-        X[:, :svd_dim] = DCA_vector(sp, dim=svd_dim)[0]
-    X_ret = np.zeros((nl, dim))
-    X_ret[seen_ind, :] = X
-    if mi == 2 or mi == 3:
-        sp *= -1
-    return sp, X_ret
-
-
-def emb_ontology(i2l, ontology_mat, co2co_nlp, dim=5, mi=0, unseen_l=None):
-    nco = len(i2l)
-    network = np.zeros((nco, nco))
-    for i in range(nco):
-        c1 = i2l[i]
-        for j in range(nco):
-            if ontology_mat[i, j] == 1:
-                network[i, j] = co2co_nlp[c1][i2l[j]]
-                network[j, i] = co2co_nlp[c1][i2l[j]]
-    idd = 0
-    sp, i2emb = graph_embedding_dca(network, i2l, mi=mi, dim=dim, unseen_l=unseen_l)
-    return i2emb
-
-
-def get_ontology_parents(GO_net, g, dfs_depth=100):
-    term_valid = set()
-    ngh_GO = set()
-    ngh_GO.add(g)
-    depth = {}
-    depth[g] = 0
-    while len(ngh_GO) > 0:
-        for GO in list(ngh_GO):
-            for GO1 in GO_net[GO]:
-                ngh_GO.add(GO1)
-                depth[GO1] = depth[GO] + 1
-            ngh_GO.remove(GO)
-            if depth[GO] < dfs_depth:
-                term_valid.add(GO)
-    return term_valid
-
-
-def creat_cell_ontology_matrix(train_Y, co2co_graph, cell_ontology_ids, dfs_depth):
-    lset = set(cell_ontology_ids)
-
-    seen_l = sorted(np.unique(train_Y))
-    unseen_l = sorted(lset - set(train_Y))
-    ys = np.concatenate((seen_l, unseen_l))
-    i2l = {}
-    l2i = {}
-    for l in ys:
-        nl = len(i2l)
-        l2i[l] = nl
-        i2l[nl] = l
-    nco = len(i2l)
-
-    net_dict = collections.defaultdict(dict)
-    net_mat = np.zeros((nco, nco))
-    for co1 in co2co_graph:
-        l1 = l2i[co1]
-        for co2 in co2co_graph[co1]:
-            l2 = l2i[co2]
-            net_dict[l1][l2] = 1
-            net_mat[l1][l2] = 1
-    for n in range(nco):
-        ngh = get_ontology_parents(net_dict, n, dfs_depth)
-        net_dict[n][n] = 1
-        for n1 in ngh:
-            net_dict[n][n1] = 1
-    return unseen_l, l2i, i2l, net_dict, net_mat
-
-
-class DataProcessing:
-    def __init__(self, cell_type_network_file='../../OnClass_data/cell_ontology/cl.ontology',
-                 cell_type_nlp_emb_file='../../OnClass_data/cell_ontology/cl.ontology.nlp.emb',
-                 terms_with_def=set(),
-                 memory_saving_mode=False):
-        """
-        Initialize OnClass model with a given cell-type network and cell-type embedding file.
-        Also, you may set the memory_saving_mode to True to get a model that uses less RAM.
-        """
-        self.cell_type_nlp_emb_file = cell_type_nlp_emb_file
-        self.cell_type_network_file = cell_type_network_file
-        self.co2co_graph, self.co2co_nlp, self.co2vec_nlp, self.cell_ontology_ids = read_cell_type_nlp_network(
-            self.cell_type_nlp_emb_file, self.cell_type_network_file)
-        self.co2co_graph, self.co2co_nlp, self.co2vec_nlp, self.cell_ontology_ids = subset_cell_type_nlp_network(
-            self.co2co_graph, self.co2co_nlp, self.co2vec_nlp, self.cell_ontology_ids, terms_with_def)
-        self.mode = memory_saving_mode
-
-    def ProcessTrainFeature(self, train_feature, train_label, train_genes, test_feature=None, test_genes=None,
-                            batch_correct=False, log_transform=True):
-        """
-        Process the gene expression matrix used to train the model, and optionally the test data.
-        Parameters
-        ----------
-        train_feature: `numpy.ndarray` or `scipy.sparse.csr_matrix` (depends on mode)
-            gene expression matrix of cell types
-        train_label: `numpy.ndarray`
-            labels for the training features
-        train_genes: `list`
-            list of genes used during training
-        test_feature: `numpy.ndarray` or `scipy.sparse.csr_matrix` (depends on mode), optional (None)
-            gene expression matrix of cell types for the test set
-        test_genes: `list`, optional (None)
-            list of genes used in test set
-        batch_correct: `bool`, optional (False)
-            whether to correct for batch effect in data
-        log_transform:`bool`, optional (True)
-            whether to apply log transform to data
-        Returns
-        -------
-        train_feature, test_feature, self.genes, self.genes
-            returns the training feature gene expression matrix and the list of genese associated
-            with it. If test_feature was not none, also returns the test features and their genes.
-        """
-
-        if log_transform is False and np.max(train_feature) > 1000:
-            warnings.warn(
-                "Max expression is" + str(np.max(train_feature)) + '. Consider setting log transform = True\n')
-        self.genes = train_genes
-        # batch correction is currently not supported for memory_saving_mode
-        if batch_correct and test_feature is not None and test_genes is not None and self.mode:
-            train_feature, test_feature, selected_train_genes = process_expression(train_feature, test_feature,
-                                                                                   train_genes, test_genes)
-            self.genes = selected_train_genes
-        elif log_transform:
-            if self.mode:
-                train_feature = csr_matrix.log1p(train_feature)
-            else:
-                train_feature = np.log1p(train_feature)
-
-            if test_feature is not None:
-                if self.mode:
-                    test_feature = csr_matrix.log1p(test_feature)
-                else:
-                    test_feature = np.log1p(test_feature)
-        self.train_feature = train_feature
-        self.train_label = train_label
-        if test_feature is not None:
-            return train_feature, test_feature, self.genes, self.genes
-        else:
-            return train_feature, self.genes
-
-    def ProcessTestFeature(self, test_feature, test_genes, use_pretrain=None, batch_correct=False, log_transform=True):
-        """
-        Process the gene expression matrix used to test the model.
-        Parameters
-        ----------
-        test_feature: `numpy.ndarray` or `scipy.sparse.csr_matrix` (depends on mode)
-            gene expression matrix of cell types for the test set
-        test_genes: `list`
-            list of genes used in test set
-        use_pretrain: `string`, optional (None)
-            name of the pretrained model
-        batch_correct: `bool`, optional (False)
-            whether to correct for batch effect in data
-        log_transform:`bool`, optional (True)
-            whether to apply log transform to data
-        Returns
-        -------
-        gene_mapping or test_feature
-            processes the test features and returns a data structure that encodes the gene
-            expression matrix that should be used for testing. If the model is in memory saving
-            mode, then the function will return a tuple of gene expression matrix and index array,
-            otherwise, it will just return the matrix.
-        """
-        if log_transform is False and np.max(test_feature) > 1000:
-            warnings.warn("Max expression is" + str(np.max(test_feature)) + '. Consider setting log transform = True\n')
-
-        if log_transform:
-            test_feature = np.log1p(test_feature)
-        if batch_correct and not self.mode:
-            test_feature = mean_normalization(self.train_feature_mean, test_feature)
-
-        if self.mode:
-            gene_mapping = get_gene_mapping(test_genes, self.genes)
-            return test_feature, gene_mapping
-        else:
-            test_feature = map_genes(test_feature, test_genes, self.genes, memory_saving_mode=self.mode)
-            return test_feature
-
-    def EmbedCellTypes(self, train_Y_str, dim=5, emb_method=3, use_pretrain=None, write2file=None):
-        """
-        Embed the cell ontology
-        Parameters
-        ----------
-        cell_type_network_file : each line should be cell_type_1\tcell_type_2\tscore for weighted network or cell_type_1\tcell_type_2 for unweighted network
-        dim: `int`, optional (500)
-            Dimension of the cell type embeddings
-        emb_method: `int`, optional (3)
-            dimensionality reduction method
-        use_pretrain: `string`, optional (None)
-            use pretrain file. This should be the numpy file of cell type embeddings. It can read the one set in write2file parameter.
-        write2file: `string`, optional (None)
-            write the cell type embeddings to this file path
-        Returns
-        -------
-        co2emb, co2i, i2co
-            returns three dicts, cell type name to embeddings, cell type name to cell type id and cell type id to embeddings.
-        """
-
-        self.unseen_co, self.co2i, self.i2co, self.ontology_dict, self.ontology_mat = creat_cell_ontology_matrix(
-            train_Y_str, self.co2co_graph, self.cell_ontology_ids, dfs_depth=3)
-        self.nco = len(self.i2co)
-        Y_emb = emb_ontology(self.i2co, self.ontology_mat, dim=dim, mi=emb_method, co2co_nlp=self.co2co_nlp,
-                             unseen_l=self.unseen_co)
-        self.co2emb = np.column_stack((np.eye(self.nco), Y_emb))
-        self.nunseen = len(self.unseen_co)
-        self.nseen = self.nco - self.nunseen
-        self.co2vec_nlp_mat = np.zeros((self.nco, len(self.co2vec_nlp[self.i2co[0]])))
-        for i in range(self.nco):
-            self.co2vec_nlp_mat[i, :] = self.co2vec_nlp[self.i2co[i]]
-        return self.co2emb, self.co2i, self.i2co, self.ontology_mat
-
-
-class cellData(Dataset):
-
-    def __init__(self, expression_matrix, labels, nlabel=0, gpu_ids='0'):
-        self.expression_matrix = expression_matrix
-        self.labels = labels
-        self.nlabel = nlabel
-        self.gpu_ids = gpu_ids
-
-    def __getitem__(self, item):
-        x = np.asarray(self.expression_matrix[item, :].todense()).squeeze()
-        y = np.zeros(self.nlabel)
-        y[self.labels[item]] = float(1)
-        x = torch.from_numpy(x).float()
-        y = torch.from_numpy(y).float()
-        if len(self.gpu_ids) > 0:
-            x = x.cuda()
-            y = y.cuda()
-        return {'features': x, 'label': y}
-
-    def __len__(self):
-        return len(self.labels)
-
-
-def emb2tensor(def_embeddings, terms, add_bias=False):
-    '''
-    This function re-sort the textual description embeddings
-    according to the mapping between terms and index
-    :param text_embeddings:
-    :param terms:
-    :return:
-    '''
-    ann_id = list(terms.keys())
-    embedding_array = np.zeros((len(ann_id), np.size(def_embeddings[ann_id[0]], 1)))
-
-    for t_id in ann_id:
-        t_def = def_embeddings[t_id].reshape([1, -1])
-        t_def = t_def / np.sqrt(np.sum(np.power(t_def, 2), axis=1))
-        embedding_array[terms[t_id], :] = t_def
-    rank_e = np.linalg.matrix_rank(embedding_array)
-    if add_bias:
-        embedding_array = np.column_stack((np.eye(len(ann_id)), embedding_array))
-    print('Rank of your embeddings is {}'.format(rank_e))
-    embedding_array = torch.from_numpy(embedding_array)
-    return embedding_array.float()
-
-
-def read_data_file(dname, data_dir):
-    if 'microcebus' in dname and 'tabula_microcebus' not in dname:
-        tech = '10x'
-        feature_file = data_dir + 'Lemur/' + dname + '.h5ad'
-        filter_key = {'method': tech}
-        label_file = None
-        gene_file = ''
-        label_key = 'cell_ontology_class'
-    elif 'tabula_microcebus' in dname:
-        tech = dname.split('_')[1]
-        feature_file = data_dir + 'Tabula_Microcebus/' + 'LCA_complete_wRaw_toPublish.h5ad'
-        filter_key = {}
-        label_file = None
-        gene_file = ''
-        batch_key = ''
-        label_key = 'cell_ontology_class_v1'
-    elif 'sapiens' in dname:
-        feature_file = data_dir + 'Tabula_Sapiens/' + 'TabulaSapiens.h5ad'
-        filter_key = {}
-        label_file = None
-        gene_file = ''
-        batch_key = ''
-        label_key = 'cell_ontology_class'
-    elif 'muris' in dname:
-        tech = dname.split('_')[1]
-        feature_file = data_dir + 'Tabula_Muris_Senis/' + 'tabula-muris-senis-' + tech + '-official-raw-obj.h5ad'
-        filter_key = {}
-        label_file = None
-        gene_file = ''
-        batch_key = ''
-        label_key = 'cell_ontology_class'
-    elif 'sapiens' in dname:
-        feature_file = data_dir + 'sapiens/' + 'Pilot1_Pilot2_decontX_Oct2020.h5ad'
-        filter_key = {}
-        label_file = None
-        gene_file = ''
-        batch_key = ''
-        label_key = 'cell_ontology_type'
-    elif 'allen' in dname:
-        feature_file = data_dir + '/Allen_Brain/features.pkl'
-        label_file = data_dir + '/Allen_Brain/labels.pkl'
-        gene_file = data_dir + '/Allen_Brain/genes.pkl'
-        label_key = ''
-        filter_key = {}
-    elif 'krasnow' in dname:
-        tech = dname.split('_')[1]
-        feature_file = data_dir + '/HLCA/' + tech + '_features.pkl'
-        label_file = data_dir + '/HLCA/' + tech + '_labels.pkl'
-        gene_file = data_dir + '/HLCA/' + tech + '_genes.pkl'
-        label_key = ''
-        filter_key = {}
-    else:
-        sys.exit('wrong dname ' + dname)
-    if feature_file.endswith('.pkl'):
-        return feature_file, filter_key, label_key, label_file, gene_file
-    elif feature_file.endswith('.h5ad'):
-        return feature_file, filter_key, label_key, label_file, gene_file
-    sys.exit('wrong file suffix')
-
-
-def read_ontology_file(dname, data_folder):
-    if 'allen' in dname:
-        cell_type_network_file = data_folder + 'allen.ontology'
-        cell_type_nlp_emb_file = None
-        cl_obo_file = None
-        if not os.path.isfile(cell_type_network_file):
-            sys.error(cell_type_network_file + ' not found!')
-    else:
-        cell_type_network_file = data_folder + 'cl.ontology'
-        cell_type_nlp_emb_file = data_folder + 'cl.ontology.nlp.emb'
-        cl_obo_file = data_folder + 'cl.obo'
-        if not os.path.isfile(cell_type_nlp_emb_file):
-            sys.exit(cell_type_nlp_emb_file + ' not found!')
-        if not os.path.isfile(cell_type_network_file):
-            sys.exit(cell_type_network_file + ' not found!')
-        if not os.path.isfile(cl_obo_file):
-            sys.exit(cl_obo_file + ' not found!')
-    return cell_type_nlp_emb_file, cell_type_network_file, cl_obo_file
-
-
-def select_cells_based_on_keys(x, features, tissues=None, labels=None, filter_key=None):
-    ncell = np.shape(x.X)[0]
-    select_cells = set(range(ncell))
-    for key in filter_key:
-        value = filter_key[key]
-        select_cells = select_cells & set(np.where(np.array(x.obs[key]) == value)[0])
-    select_cells = sorted(select_cells)
-    features = features[select_cells, :]
-    if labels is not None:
-        labels = labels[select_cells]
-    if tissues is not None:
-        tissues = tissues[select_cells]
-    x = x[select_cells, :]
-    return features, labels, tissues, x
-
-
-def get_ontology_name(obo_file, lower=True):
-    fin = open(obo_file)
-    co2name = {}
-    name2co = {}
-    tag_is_syn = {}
-    for line in fin:
-        if line.startswith('id: '):
-            co = line.strip().split('id: ')[1]
-        if line.startswith('name: '):
-            if lower:
-                name = line.strip().lower().split('name: ')[1]
-            else:
-                name = line.strip().split('name: ')[1]
-            co2name[co] = name
-            name2co[name] = co
-        if line.startswith('synonym: '):
-            if lower:
-                syn = line.strip().lower().split('synonym: "')[1].split('" ')[0]
-            else:
-                syn = line.strip().split('synonym: "')[1].split('" ')[0]
-            if syn in name2co:
-                continue
-            name2co[syn] = co
-    fin.close()
-    return co2name, name2co
-
-
-def fine_nearest_co_using_nlp(sentences, co2emb, obo_file, nlp_mapping_cutoff=0.8):
-    co2name, name2co = get_ontology_name(obo_file=obo_file)
-    from sentence_transformers import SentenceTransformer
-    model = SentenceTransformer('bert-base-nli-mean-tokens')
-    sentences = np.array([sentence.lower() for sentence in sentences])
-    sentence_embeddings = model.encode(sentences)
-    co_embeddings = []
-    cos = []
-    for co in co2emb:
-        co_embeddings.append(co2emb[co])
-        cos.append(co)
-    co_embeddings = np.array(co_embeddings)
-    sent2co = {}
-    for sentence, embedding, ind in zip(sentences, sentence_embeddings, range(len(sentences))):
-        scs = cosine_similarity(co_embeddings, embedding.reshape(1, -1))
-
-        co_id = np.argmax(scs)
-        sc = scs[co_id]
-        if sc > nlp_mapping_cutoff:
-            sent2co[sentence.lower()] = cos[co_id]
-            names = set()
-            for name in name2co:
-                if name2co[name].upper() == cos[co_id]:
-                    names.add(name)
-        # print (sentence, cos[co_id], sc, co2name[cos[co_id]],names)
-    return sent2co
-
-
-def exact_match_co_name_2_co_id(labels, lab2co, cl_obo_file=None):
-    if cl_obo_file is None:
-        return lab2co
-    co2name, name2co = get_ontology_name(obo_file=cl_obo_file)
-    for label in labels:
-        if label.lower() in name2co:
-            lab2co[label.lower()] = name2co[label.lower()]
-    for name in name2co:
-        lab2co[name.lower()] = name2co[name]
-    return lab2co
-
-
-def map_and_select_labels(labels, cell_ontology_ids, obo_file, ct_mapping_key={}, nlp_mapping=True,
-                          nlp_mapping_cutoff=0.8, co2emb=None, cl_obo_file=None):
-    lab2co = {}
-    if nlp_mapping:
-        if co2emb is None:
-            sys.exit('Please provide cell type embedding to do NLP-based mapping.')
-        lab2co = fine_nearest_co_using_nlp(np.unique(labels), co2emb, obo_file, nlp_mapping_cutoff=nlp_mapping_cutoff)
-    lab2co = exact_match_co_name_2_co_id(np.unique(labels), lab2co, cl_obo_file=cl_obo_file)
-    for ct in ct_mapping_key:
-        lab2co[ct_mapping_key[ct]] = lab2co[ct]
-    ind = []
-    lab_id = []
-    unfound_labs = set()
-    for i, l in enumerate(labels):
-        if l in cell_ontology_ids:
-            ind.append(i)
-            lab_id.append(l)
-        elif l.lower() in lab2co:
-            ind.append(i)
-            lab_id.append(lab2co[l.lower()])
-        else:
-            unfound_labs.add(l)
-    frac = len(ind) * 1. / len(labels)
-    ind = np.array(ind)
-    labels = np.array(lab_id)
-    unfound_labs = set(unfound_labs)
-    warn_message = 'Warning: Only: %f precentage of labels are in the Cell Ontology. The remaining cells are excluded! Consider using NLP mapping and choose a small mapping cutoff (nlp_mapping_cutoff)' % (
-            frac * 100)
-    if frac < 0.5:
-        print(warn_message)
-        print('Here are unfound labels:', unfound_labs)
-    return ind, labels, unfound_labs
-
-
-def exclude_parent_child_nodes(cell_ontology_file, labels):
-    uniq_labels = np.unique(labels)
-    excludes = set()
-    net = collections.defaultdict(dict)
-    fin = open(cell_ontology_file)
-    for line in fin:
-        s, p = line.strip().split('\t')
-        net[s][p] = 1  # p is parent
-    fin.close()
-    for n in list(net.keys()):
-        ngh = get_ontology_parents(net, n)
-        for n1 in ngh:
-            net[n][n1] = 1
-    for l1 in uniq_labels:
-        for l2 in uniq_labels:
-            if l1 in net[l2] and l1 != l2:  # l1 is l2 parent
-                excludes.add(l1)
-    # print (excludes)
-    new_ids = []
-    for i in range(len(labels)):
-        if labels[i] not in excludes:
-            new_ids.append(i)
-    new_ids = np.array(new_ids)
-    return new_ids, excludes
-
-
-def read_data(feature_file, cell_ontology_ids, exclude_non_leaf_ontology=False, ct_mapping_key={}, tissue_key=None,
-              seed=1, filter_key=None, AnnData_label_key=None, nlp_mapping=True, nlp_mapping_cutoff=0.8, co2emb=None,
-              label_file=None, cl_obo_file=None, cell_ontology_file=None, memory_saving_mode=False,
-              backup_file='sparse_featurefile_backup'):
-    """
-	Read data from the given feature file, and processes it so that it fits with the other
-	given paramters as needed.
-	Parameters
-	----------
-	feature_file: `string`
-		name of file to extract data from. The data in the file must be stored in h5ad file format.
-	cell_ontology_ids: `set`
-		set of ids from the cell ontology.
-	AnnData_label_key: `numpy.ndarray`, optional (None)
-		mapping of the cell type classes to reindex the labels in the AnnData object
-	co2emb: `map`, optional (None)
-		maps cell-type from the cell ontology to its embedding
-	label_file: `string`, optional (None)
-		file from which to get the labels of the feature file
-	memory_saving_mode: `bool`, optional (False)
-		whether the method should be run under tight RAM constraints.
-	backup_file: `string`, optional ('sparse_featurefile_backup')
-		the name of the file to copy the sparse feature dataset to.
-
-	Returns
-	-------
-	dataset: `numpy.ndarray` or `scipy.sparse.csr_matrix` (depends on mode)
-		gene expression matrix of cell types for the test set
-	genes: `list`
-		list of genes in the dataset
-	labels: `numpy.ndarray`
-		labels from the feature file
-	x: AnnData object stored in the given feature file
-	"""
-
-    np.random.seed(seed)
-
-    if memory_saving_mode:
-        x = read_h5ad(feature_file, backed='r+')
-        if 'Tabula_Microcebus' in feature_file or 'TabulaSapiens' in feature_file:
-            x.raw = None
-        dataset = x.X.to_memory()  # Gets a sparse array in csr matrix form
-    else:
-        x = read_h5ad(feature_file)
-        dataset = x.X.toarray()
-
-    # if memory_saving_mode:
-    #    print_memory_usage("while reading data")
-
-    ncell = np.shape(x.X)[0]
-    genes = np.array([x.upper() for x in x.var.index])
-
-    if tissue_key is not None and 'TabulaSapiens' not in feature_file:
-        tissues = np.array(x.obs[tissue_key].tolist())
-    else:
-        tissues = None
-    if AnnData_label_key is None and label_file is None:
-        print('no label file is provided')
-        labels = None
-        dataset, labels, tissues, x = select_cells_based_on_keys(x, dataset, labels=labels, tissues=tissues,
-                                                                 filter_key=filter_key)
-        return dataset, genes, labels, tissues, x
-    if AnnData_label_key is not None:
-        labels = x.obs[AnnData_label_key].tolist()
-    else:
-        fin = open(label_file)
-        labels = []
-        for line in fin:
-            labels.append(line.strip())
-        fin.close()
-    labels = np.array(labels)
-    dataset, labels, tissues, x = select_cells_based_on_keys(x, dataset, labels=labels, tissues=tissues,
-                                                             filter_key=filter_key)
-
-    if memory_saving_mode:
-        x = x.copy(filename=backup_file)
-
-    ind, labels, unfound_labs = map_and_select_labels(labels, cell_ontology_ids, cl_obo_file,
-                                                      ct_mapping_key=ct_mapping_key, nlp_mapping=nlp_mapping,
-                                                      co2emb=co2emb, nlp_mapping_cutoff=nlp_mapping_cutoff,
-                                                      cl_obo_file=cl_obo_file)
-    if tissue_key is not None and 'TabulaSapiens' not in feature_file:
-        tissues = tissues[ind]
-    dataset = dataset[ind, :]
-
-    if memory_saving_mode:
-        # Need to copy to disk for rewriting to the sparse dataset
-        x = x[ind, :].copy(filename=backup_file)
-    else:
-        x = x[ind, :]
-
-    if exclude_non_leaf_ontology:
-        new_ids, exclude_terms = exclude_parent_child_nodes(cell_ontology_file, labels)
-        if tissues is not None:
-            tissues = tissues[new_ids]
-        dataset = dataset[new_ids, :]
-        labels = labels[new_ids]
-        x = x[new_ids, :]
-
-    ncell = np.shape(dataset)[0]
-    index = np.random.choice(ncell, ncell, replace=False)
-    dataset = dataset[index, :]  # cell by gene matrix
-    labels = labels[index]
-    if tissue_key is not None and 'TabulaSapiens' not in feature_file:
-        tissues = tissues[index]
-    return dataset, genes, labels, tissues, x
-
-
-def load_co_text(co_data_path):
-    ont = dict()
-    obj = None
-    with open(co_data_path, 'r') as f:
-        for line in f:
-            line = line.strip()
-            if not line:
-                continue
-            if line == '[Term]':
-                if obj is not None and len(obj['text']) > 0:
-                    ont[obj['id']] = obj
-                obj = dict()
-                obj['text'] = ""
-                continue
-            elif line == '[Typedef]' and len(obj['text']) > 0:
-                if obj is not None:
-                    ont[obj['id']] = obj
-                obj = None
-            else:
-                if obj is None:
-                    continue
-                l = line.split(": ")
-                if l[0] == 'id':
-                    obj['id'] = l[1]
-                elif l[0] == 'name':
-                    obj['text'] += line.split('name: ')[1].strip() + '. '
-                elif l[0] == 'def':
-                    obj['text'] += line.split('def: ')[1].split('"')[1].strip()
-        if obj is not None and len(obj['text']) > 0:
-            ont[obj['id']] = obj
-    return ont
-
-def extract_data_based_on_class(feats, labels, sel_labels):
-    ind = []
-    for l in sel_labels:
-        id = np.where(labels == l)[0]
-        ind.extend(id)
-    np.random.shuffle(ind)
-    X = feats[ind, :]
-    Y = labels[ind]
-    return X, Y, ind
-
-
-def SplitTrainTest(all_X, all_Y, all_tissues=None, random_state=10, nfold_cls=0.3, nfold_sample=0.2, nmin_size=10,
-                   memory_saving_mode=False):
-    """
-    Utility function for splitting the dataset into a train and test set.
-    Parameters
-    ----------
-    all_X: all the feature data
-    all_Y: the corresponding labels
-
-    Returns
-    -------
-    The labeled training and test sets
-    """
-    np.random.seed(random_state)
-
-    cls = np.unique(all_Y)
-    cls2ct = Counter(all_Y)
-    ncls = len(cls)
-    test_cls = list(np.random.choice(cls, int(ncls * nfold_cls), replace=False))
-    for c in cls2ct:
-        if cls2ct[c] < nmin_size:
-            test_cls.append(c)
-    test_cls = np.unique(test_cls)
-    # add rare class to test, since they cannot be split into train and test by using train_test_split(stratify=True)
-    train_cls = [x for x in cls if x not in test_cls]
-    train_cls = np.array(train_cls)
-    train_X, train_Y, train_ind = extract_data_based_on_class(all_X, all_Y, train_cls)
-    test_X, test_Y, test_ind = extract_data_based_on_class(all_X, all_Y, test_cls)
-    if all_tissues is not None:
-        train_tissues = all_tissues[train_ind]
-        test_tissues = all_tissues[test_ind]
-        train_X_train, train_X_test, train_Y_train, train_Y_test, train_tissues_train, train_tissues_test = train_test_split(
-            train_X, train_Y, train_tissues, test_size=nfold_sample, stratify=train_Y, random_state=random_state)
-        test_tissues = np.concatenate((test_tissues, train_tissues_test))
-        train_tissues = train_tissues_train
-    else:
-        train_X_train, train_X_test, train_Y_train, train_Y_test = train_test_split(
-            train_X, train_Y, test_size=nfold_sample, stratify=train_Y, random_state=random_state)
-
-    # TODO: Added this memory saving mode toggle
-    if memory_saving_mode:
-        test_X = scipy.sparse.vstack((test_X, train_X_test)).tocsr()
-    else:
-        test_X = np.vstack((test_X, train_X_test))
-
-    test_Y = np.concatenate((test_Y, train_Y_test))
-    train_X = train_X_train
-    train_Y = train_Y_train
-    if all_tissues is not None:
-        return train_X, train_Y, train_tissues, test_X, test_Y, test_tissues
-    else:
-        return train_X, train_Y, test_X, test_Y
-
-
-def compute_roc(labels, preds):
-    # Compute ROC curve and ROC area for each class
-    fpr, tpr, _ = roc_curve(labels.flatten(), preds.flatten())
-    roc_auc = auc(fpr, tpr)
-    return roc_auc
-
-
-def compute_prc(labels, preds):
-    # Compute PRC curve and PRC area for each class
-    pr, rc, _ = precision_recall_curve(labels.flatten(), preds.flatten())
-    prc_auc = auc(rc, pr)
-    return prc_auc
-
-
-def evaluate_unseen_auroc(inference_preds, inference_label, unseen2i):
-    roc_macro = np.zeros(len(unseen2i.values()))
-    unseen_id = list(unseen2i.values())
-    cl_i = 0
-    for i in unseen_id:
-        unseen_preds, unseen_labels = inference_preds[:, i], inference_label[:, i]
-        auroc = compute_roc(unseen_labels, unseen_preds)
-        roc_macro[cl_i] = auroc
-        cl_i += 1
-    return np.mean(roc_macro)
-
-
-def evaluate_auroc(inference_preds, inference_label):
-    roc_macro = np.zeros(np.size(inference_label, 1))
-    for cl_i in range(np.size(inference_label, 1)):
-        roc_auc = compute_roc(inference_label[:, cl_i], inference_preds[:, cl_i])
-        roc_macro[cl_i] = roc_auc
-    roc_auc = np.mean(roc_macro)
-    return roc_auc
-
-
-def sampled_auprc(truths, preds):
-    pos = np.where(truths == 1)[0]
-    neg = np.where(truths == 0)[0]
-    assert (len(pos) + len(neg) == len(truths))
-    nneg = len(neg)
-    npos = len(pos)
-    select_neg = np.random.choice(nneg, npos * 3, replace=True)
-    select_ind = np.concatenate((pos, select_neg))
-    return average_precision_score(truths[select_ind], preds[select_ind])
-
-
-def evaluate_unseen_auprc(inference_preds, inference_label, unseen2i):
-    roc_macro = np.zeros(len(unseen2i.values()))
-    unseen_id = list(unseen2i.values())
-    cl_i = 0
-    for i in unseen_id:
-        unseen_preds, unseen_labels = inference_preds[:, i], inference_label[:, i]
-        auroc = sampled_auprc(unseen_labels, unseen_preds)
-        roc_macro[cl_i] = auroc
-        cl_i += 1
-    return np.mean(roc_macro)
-
-
-def evaluate_auprc(inference_preds, inference_label):
-    roc_macro = np.zeros(np.size(inference_label, 1))
-    for cl_i in range(np.size(inference_label, 1)):
-        roc_auc = sampled_auprc(inference_label[:, cl_i], inference_preds[:, cl_i])
-        roc_macro[cl_i] = roc_auc
-    roc_auc = np.mean(roc_macro)
-    return roc_auc
-
-
-def find_gene_ind(genes, common_genes):
-    gid = []
-    for g in common_genes:
-        gid.append(np.where(genes == g)[0][0])
-    gid = np.array(gid)
-    return gid
+import os
+import sys
+import torch
+import logging
+import scipy
+import time
+import pickle
+import collections
+import numpy as np
+import pandas as pd
+import warnings
+from torch import nn
+import networkx as nx
+from tqdm import tqdm
+from torch import squeeze
+from torch.nn import init
+from collections import deque
+from gensim import corpora, models
+from scipy.sparse.linalg import svds
+from nltk.tokenize import word_tokenize
+from torch.utils.data import ConcatDataset
+from gensim.models.word2vec import Word2Vec
+import torchvision.transforms as transforms
+from transformers import AutoTokenizer, AutoModel
+from gensim.models.doc2vec import Doc2Vec, TaggedDocument
+from scipy import sparse
+from scipy import spatial
+from anndata import read_h5ad
+from collections import Counter
+from scipy.sparse.csr import csr_matrix
+from sklearn.metrics import roc_auc_score, roc_curve
+from sklearn.model_selection import train_test_split
+from sklearn.metrics.pairwise import cosine_similarity
+from scipy.sparse.csgraph._shortest_path import shortest_path
+# from sklearn.utils.graph_shortest_path import graph_shortest_path
+from sklearn.metrics import auc, average_precision_score, precision_recall_curve
+
+import nltk
+
+nltk.download('punkt')
+
+
+def save_obj(obj, name):
+    with open(name, 'wb') as f:
+        pickle.dump(obj, f, pickle.HIGHEST_PROTOCOL)
+
+
+def load_obj(name):
+    with open(name, 'rb') as f:
+        return pickle.load(f)
+
+
+def load(filename, with_rels=True):
+    ont = dict()
+    obj = None
+    with open(filename, 'r') as f:
+        for line in f:
+            line = line.strip()
+            if not line:
+                continue
+            if line == '[Term]':
+                if obj is not None:
+                    ont[obj['id']] = obj
+                obj = dict()
+                obj['is_a'] = list()
+                obj['part_of'] = list()
+                obj['regulates'] = list()
+                obj['alt_ids'] = list()
+                obj['def'] = list()
+                obj['is_obsolete'] = False
+                continue
+            elif line == '[Typedef]':
+                if obj is not None:
+                    ont[obj['id']] = obj
+                obj = None
+            else:
+                if obj is None:
+                    continue
+                l = line.split(": ")
+                if l[0] == 'id':
+                    obj['id'] = l[1]
+                elif l[0] == 'alt_id':
+                    obj['alt_ids'].append(l[1])
+                elif l[0] == 'namespace':
+                    obj['namespace'] = l[1]
+                elif l[0] == 'def':
+                    obj['def'].append(l[1].split('"')[1])
+                elif l[0] == 'is_a':
+                    obj['is_a'].append(l[1].split(' ! ')[0])
+                elif with_rels and l[0] == 'relationship':
+                    it = l[1].split()
+                    # add all types of relationships
+                    obj['is_a'].append(it[1])
+                elif l[0] == 'name':
+                    obj['name'] = l[1]
+                elif l[0] == 'is_obsolete' and l[1] == 'true':
+                    obj['is_obsolete'] = True
+        if obj is not None:
+            ont[obj['id']] = obj
+    for term_id in list(ont.keys()):
+        for t_id in ont[term_id]['alt_ids']:
+            ont[t_id] = ont[term_id]
+        if ont[term_id]['is_obsolete']:
+            del ont[term_id]
+    for term_id, val in ont.items():
+        if 'children' not in val:
+            val['children'] = set()
+        for p_id in val['is_a']:
+            if p_id in ont:
+                if 'children' not in ont[p_id]:
+                    ont[p_id]['children'] = set()
+                ont[p_id]['children'].add(term_id)
+    return ont
+
+
+def get_ontology_embeddings(cfg):
+    """Get the textual description embeddings of Gene Ontology (GO) or Cell Ontology (CO) terms
+
+    Parameters
+    ----------
+    cfg:
+        config
+
+    Returns
+    -------
+    ont_embeddings:
+        the ontology embeddings
+    """
+
+    """This function uses the BioTranslator Text Encoder to embed the Gene Ontology terms
+    :param cfg:
+    :return:
+    """
+    embeddings = collections.OrderedDict()
+    bert_name = 'microsoft/BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext'
+    tokenizer = AutoTokenizer.from_pretrained('microsoft/BiomedNLP-PubMedBERT-base-uncased-abstract-fulltext')
+    model = NeuralNetwork('None', 'cls', bert_name)
+    model.load_state_dict(torch.load(cfg.encoder_path))
+    model = model.to('cuda')
+    model.eval()
+
+    if cfg.tp in ['seq', 'graph']:
+        if cfg.task not in ["single-dataset", "cross-dataset"]:
+            # go embedding
+            data = load(cfg.go_file)
+            classes = list(data.keys())
+            texts = []
+            for i in tqdm(range(len(classes))):
+                with torch.no_grad():
+                    texts.append(data[classes[i]]['name'] + '. ' + data[classes[i]]['def'][0])
+        else:
+            # co embedding
+            text = load_co_text(cfg.ontology_repo + 'cl.obo')
+            classes = list(text.keys())
+            texts = []
+            for i in tqdm(range(len(classes))):
+                with torch.no_grad():
+                    texts.append(text[classes[i]]['text'])
+    elif cfg.tp == 'cell':
+        # co embedding
+        text = load_co_text(cfg.ontology_repo + 'cl.obo')
+        classes = list(text.keys())
+        texts = []
+        for i in tqdm(range(len(classes))):
+            with torch.no_grad():
+                texts.append(text[classes[i]]['text'])
+
+    with torch.no_grad():
+        for i in tqdm(range(len(classes))):
+            text = texts[i]
+            inputs = tokenizer(text, return_tensors='pt').to('cuda')
+            if len(cfg.gpu_ids) > 0:
+                inputs = inputs.to('cuda')
+            sents_len = min(inputs['input_ids'].size(1), 512)
+            input_ids = inputs['input_ids'][0, 0: sents_len].view(len(inputs['input_ids']), -1).to('cuda')
+            attention_mask = inputs['attention_mask'][0, 0: sents_len].view(len(inputs['attention_mask']),
+                                                                            -1).to(
+                'cuda')
+            token_type_ids = inputs['token_type_ids'][0, 0: sents_len].view(len(inputs['token_type_ids']),
+                                                                            -1).to(
+                'cuda')
+
+            pred = model(input_ids, attention_mask, token_type_ids)
+            embeddings[classes[i]] = np.asarray(pred.cpu()).reshape([-1, 768])
+        save_obj(embeddings, cfg.emb_path + cfg.emb_name)
+    return embeddings
+
+
+def get_anchestors(go, term_id):
+    if term_id not in go:
+        return []
+    term_set = []
+    q = deque()
+    q.append(term_id)
+    while (len(q) > 0):
+        t_id = q.popleft()
+        if t_id not in term_set:
+            term_set.append(t_id)
+            for parent_id in go[t_id]['is_a']:
+                if parent_id in go:
+                    q.append(parent_id)
+    return term_set
+
+
+def init_weights(net, init_type='normal', init_gain=0.02):
+    """Initialize network weights.
+    Parameters:
+        net (network)   -- network to be initialized
+        init_type (str) -- the name of an initialization method: normal | xavier | kaiming | orthogonal
+        init_gain (float)    -- scaling factor for normal, xavier and orthogonal.
+    We use 'normal' in the original pix2pix and CycleGAN paper. But xavier and kaiming might
+    work better for some applications. Feel free to try yourself.
+    """
+
+    def init_func(m):  # define the initialization function
+        classname = m.__class__.__name__
+        if hasattr(m, 'weight') and (classname.find('Conv') != -1 or classname.find('Linear') != -1):
+            if init_type == 'normal':
+                init.normal_(m.weight.data, 0.0, init_gain)
+            elif init_type == 'xavier':
+                init.xavier_normal_(m.weight.data, gain=init_gain)
+            elif init_type == 'kaiming':
+                init.kaiming_normal_(m.weight.data, a=0, mode='fan_in')
+            elif init_type == 'orthogonal':
+                init.orthogonal_(m.weight.data, gain=init_gain)
+            else:
+                raise NotImplementedError('initialization method [%s] is not implemented' % init_type)
+            if hasattr(m, 'bias') and m.bias is not None:
+                init.constant_(m.bias.data, 0.0)
+        elif classname.find(
+                'BatchNorm2d') != -1:  # BatchNorm Layer's weight is not a matrix; only normal distribution applies.
+            init.normal_(m.weight.data, 1.0, init_gain)
+            init.constant_(m.bias.data, 0.0)
+
+    print('initialize network with %s' % init_type)
+    net.apply(init_func)  # apply the initialization function <init_func>
+
+
+def get_logger(logfile):
+    '''
+    This function are copied from https://blog.csdn.net/a232884c/article/details/117453011
+    :param logfile:
+    :return:
+    '''
+    logger = logging.getLogger()
+    logger.setLevel(logging.INFO)
+    fh = logging.FileHandler(logfile, mode='w')
+    fh.setLevel(logging.DEBUG)
+    formatter = logging.Formatter("%(asctime)s - %(filename)s[line:%(lineno)d] - %(levelname)s: %(message)s")
+    fh.setFormatter(formatter)
+    logger.addHandler(fh)
+    ch = logging.StreamHandler()
+    ch.setLevel(logging.DEBUG)
+    ch.setFormatter(formatter)
+    logger.addHandler(ch)
+    return logger
+
+
+def renorm(X):
+    Y = X.copy()
+    Y = Y.astype(float)
+    ngene, nsample = Y.shape
+    s = np.sum(Y, axis=0)
+    # print s.shape()
+    for i in range(nsample):
+        if s[i] == 0:
+            s[i] = 1
+            if i < ngene:
+                Y[i, i] = 1
+            else:
+                for j in range(ngene):
+                    Y[j, i] = 1. / ngene
+        Y[:, i] = Y[:, i] / s[i]
+    return Y
+
+
+def DCA_vector(Q, dim):
+    nnode = Q.shape[0]
+    alpha = 1. / (nnode ** 2)
+    Q = np.log(Q + alpha) - np.log(alpha)
+
+    # Q = Q * Q';
+    [U, S, V] = svds(Q, dim)
+    S = np.diag(S)
+    X = np.dot(U, np.sqrt(S))
+    Y = np.dot(np.sqrt(S), V)
+    Y = np.transpose(Y)
+    return X, U, S, V, Y
+
+
+class Dataset(object):
+
+    def __getitem__(self, index):
+        raise NotImplementedError
+
+    def __len__(self):
+        raise NotImplementedError
+
+    def __add__(self, other):
+        return ConcatDataset([self, other])
+
+
+def one_hot(seq, start=0, max_len=2000):
+    '''
+    One-Hot encodings of protein sequences,
+    this function was copied from DeepGOPlus paper
+    :param seq:
+    :param start:
+    :param max_len:
+    :return:
+    '''
+    AALETTER = [
+        'A', 'R', 'N', 'D', 'C', 'Q', 'E', 'G', 'H', 'I',
+        'L', 'K', 'M', 'F', 'P', 'S', 'T', 'W', 'Y', 'V']
+    AAINDEX = dict()
+    for i in range(len(AALETTER)):
+        AAINDEX[AALETTER[i]] = i + 1
+    onehot = np.zeros((21, max_len), dtype=np.int32)
+    l = min(max_len, len(seq))
+    for i in range(start, start + l):
+        onehot[AAINDEX.get(seq[i - start], 0), i] = 1
+    onehot[0, 0:start] = 1
+    onehot[0, start + l:] = 1
+    return onehot
+
+
+class proteinData(Dataset):
+    '''
+    The dataset of protein
+    '''
+
+    def __init__(self, data_df, terms, prot_vector, prot_description, gpu_ids='0'):
+        self.p_ids = []
+        self.pSeq = []
+        self.label = []
+        self.vector = []
+        self.description = []
+        self.gpu_ids = gpu_ids
+        sequences = list(data_df['sequences'])
+        prot_ids = list(data_df['proteins'])
+        annots = list(data_df['annotations'])
+        for i in range(len(annots)):
+            annots[i] = list(annots[i])
+        for i in range(data_df.shape[0]):
+            seqT, annT, protT = sequences[i], annots[i], prot_ids[i]
+            labelT = np.zeros([len(terms), 1])
+            for j in range(len(annT)):
+                if annT[j] in terms.keys():
+                    labelT[terms[annT[j]]] = 1
+            self.p_ids.append(protT)
+            self.pSeq.append(one_hot(seqT))
+            self.label.append(labelT)
+            self.vector.append(prot_vector[protT])
+            self.description.append((prot_description[protT]))
+
+    def __getitem__(self, item):
+        in_seq, label = transforms.ToTensor()(self.pSeq[item]), transforms.ToTensor()(self.label[item])
+        description = torch.from_numpy(self.description[item])
+        vector = torch.from_numpy(self.vector[item])
+        if len(self.gpu_ids) > 0:
+            return {'proteins': self.p_ids[item],
+                    'prot_seq': squeeze(in_seq).float().cuda(),
+                    'prot_description': squeeze(description).float().cuda(),
+                    'prot_network': squeeze(vector).float().cuda(),
+                    'label': squeeze(label).float().cuda()}
+        else:
+            return {'proteins': self.p_ids[item],
+                    'prot_seq': squeeze(in_seq).float(),
+                    'prot_description': squeeze(description).float(),
+                    'prot_network': squeeze(vector).float(),
+                    'label': squeeze(label).float()}
+
+    def __len__(self):
+        return len(self.pSeq)
+
+
+class NeuralNetwork(nn.Module):
+    def __init__(self, model_path, output_way, bert_name):
+        super(NeuralNetwork, self).__init__()
+        self.bert = AutoModel.from_pretrained(bert_name)
+        self.output_way = output_way
+
+    def forward(self, input_ids, attention_mask, token_type_ids):
+        x1 = self.bert(input_ids, attention_mask=attention_mask, token_type_ids=token_type_ids)
+        if self.output_way == 'cls':
+            output = x1.last_hidden_state[:, 0]
+        elif self.output_way == 'pooler':
+            output = x1.pooler_output
+        return output
+
+
+def term2preds_label(preds, label, terms, terms2id):
+    new_preds, new_label = [], []
+    for t_id in terms:
+        new_preds.append(preds[:, terms2id[t_id]].reshape((-1, 1)))
+        new_label.append(label[:, terms2id[t_id]].reshape((-1, 1)))
+    new_preds = np.concatenate(new_preds, axis=1)
+    new_label = np.concatenate(new_label, axis=1)
+    return new_preds, new_label
+
+
+def organize_workingspace(workingspace, task=None):
+    """
+    Make sure that the working space include the zero shot folder, few shot folder,
+    model folder, training log folder and results folder
+    :param workingspace:
+    :return:
+    """
+    task_path = workingspace + task
+    cache_path = task_path + '/cache'
+    model_path = task_path + '/model'
+    logger_path = task_path + '/log'
+    results_path = task_path + '/results'
+    if not os.path.exists(workingspace):
+        os.mkdir(workingspace)
+        print('Warning: We created the working space: {}'.format(workingspace))
+    if not os.path.exists(task_path):
+        os.mkdir(task_path)
+    if not os.path.exists(cache_path):
+        os.mkdir(cache_path)
+    if not os.path.exists(model_path):
+        os.mkdir(model_path)
+    if not os.path.exists(logger_path):
+        os.mkdir(logger_path)
+    if not os.path.exists(results_path):
+        os.mkdir(results_path)
+
+
+def get_namespace_terms(terms, go, namespace):
+    # select terms in the namespace
+    name_dict = {'bp': 'biological_process', 'mf': 'molecular_function', 'cc': 'cellular_component'}
+    new_terms = []
+    for t_id in terms:
+        if go[t_id]['namespace'] == name_dict[namespace]:
+            new_terms.append(t_id)
+    return new_terms
+
+
+def get_few_shot_namespace_terms(term_count, go, namespace, n=10):
+    # select terms in namespace with less than n training sample
+    name_dict = {'bp': 'biological_process', 'mf': 'molecular_function', 'cc': 'cellular_component'}
+    new_terms = []
+    for t_id in term_count.keys():
+        if go[t_id]['namespace'] == name_dict[namespace]:
+            if term_count[t_id] <= n:
+                new_terms.append(t_id)
+    return new_terms
+
+
+def term_training_numbers(val_data, train_data):
+    '''
+    This function calculates how many training samples exists in the
+    :param val_data:
+    :param train_data:
+    :return:
+    '''
+    term2number = collections.OrderedDict()
+    for annt_val in list(val_data['annotations']):
+        for a_id in annt_val:
+            term2number[a_id] = 0
+    training_annt = list(train_data['annotations'])
+    for annt in training_annt:
+        annt = list(set(annt))
+        for a_id in annt:
+            if a_id not in term2number.keys():
+                continue
+            term2number[a_id] += 1
+    return term2number
+
+
+def compute_blast_preds(diamond_scores,
+                        test,
+                        train_data):
+    '''
+    This function computes the predictions of blast results.
+    The codes here are borrowed from the DeepGOPlus paper
+    :param diamond_scores:
+    :param test:
+    :param train_data:
+    :param is_load:
+    :param save_path:
+    :return:
+    '''
+    blast_preds = collections.OrderedDict()
+    print('Diamond preds')
+    annotation_dict = collections.OrderedDict()
+    for i in train_data.index:
+        prot_id = train_data.loc[i]['proteins']
+        annts = set(train_data.loc[i]['annotations'])
+        if prot_id not in annotation_dict.keys():
+            annotation_dict[prot_id] = collections.OrderedDict()
+            for ann_id in annts:
+                annotation_dict[prot_id][ann_id] = None
+        else:
+            for ann_id in annts:
+                annotation_dict[prot_id][ann_id] = None
+
+    for prot_id in tqdm(test.proteins):
+        annots = {}
+
+        # BlastKNN
+        sim = collections.OrderedDict()
+        if prot_id in diamond_scores.keys():
+            sim_prots = diamond_scores[prot_id]
+            allgos = set()
+            total_score = 0.0
+            for p_id, score in sim_prots.items():
+                allgos |= set(annotation_dict[p_id].keys())
+                total_score += score
+            allgos = set(allgos)
+            for go_id in allgos:
+                s = 0.0
+                for p_id in sim_prots.keys():
+                    score = sim_prots[p_id]
+                    if go_id in annotation_dict[p_id].keys():
+                        s += score
+                sim[go_id] = s / total_score
+        blast_preds[prot_id] = sim
+    return blast_preds
+
+
+def extract_terms_from_dataset(dataset):
+    id = 0
+    terms2id = collections.OrderedDict()
+    id2terms = collections.OrderedDict()
+    for i in dataset.index:
+        annts = dataset.iloc[i]['annotations']
+        for annt in annts:
+            if annt not in terms2id:
+                terms2id[annt] = id
+                id2terms[id] = annt
+                id += 1
+    return terms2id, id2terms
+
+
+def coef_vec(A, B):
+    coefs_array = []
+    for i in range(np.size(A, 0)):
+        a1 = A[i, :]
+        b1 = B[i, :]
+        coefs = np.corrcoef(a1, b1)[0, 1]
+        coefs_array.append(coefs)
+    return np.asarray(coefs_array)
+
+
+def sample_edges(st=0, ed=1000, n=100, exclude_edges=[]):
+    samples = []
+    while True:
+        nodes = np.arange(st, ed)
+        np.random.shuffle(nodes)
+        edge = list(nodes[0: 2])
+        if edge not in exclude_edges and edge not in samples:
+            samples.append(edge)
+        if len(samples) == n:
+            break
+    return np.asarray(samples)
+
+
+def edge_probability(encodings_i, encodings_j, text_encodings_p):
+    s1 = np.dot(encodings_i, np.transpose(text_encodings_p))
+    s1 = 1 / (1 + np.exp(-s1))
+    s2 = np.dot(encodings_j, np.transpose(text_encodings_p))
+    s2 = 1 / (1 + np.exp(-s2))
+    s3 = coef_vec(encodings_i, encodings_j)
+    score = s3 * (0.5 * s1.squeeze() + 0.5 * s2.squeeze())
+    return score
+
+
+def RandomWalkRestart(A, rst_prob, delta=1e-4, reset=None, max_iter=50, use_torch=False, return_torch=False):
+    device = torch.device('cpu')
+    if use_torch and torch.cuda.is_available():
+        device = torch.device('cuda:0')
+    nnode = A.shape[0]
+    if reset is None:
+        reset = np.eye(nnode)
+    nsample, nnode = reset.shape
+    # print nsample,nnode
+    P = renorm(A)
+    P = P.T
+    norm_reset = renorm(reset.T)
+    norm_reset = norm_reset.T
+    if use_torch:
+        norm_reset = torch.from_numpy(norm_reset).float().to(device)
+        P = torch.from_numpy(P).float().to(device)
+    Q = norm_reset
+
+    for i in range(1, max_iter):
+        if use_torch:
+            Q_new = rst_prob * norm_reset + (1 - rst_prob) * torch.mm(Q, P)  # .as_numpy_array()
+            delta = torch.norm(Q - Q_new, 2)
+        else:
+            Q_new = rst_prob * norm_reset + (1 - rst_prob) * np.dot(Q, P)  # .as_numpy_array()
+            delta = np.linalg.norm(Q - Q_new, 'fro')
+        Q = Q_new
+        # print (i,Q)
+        sys.stdout.flush()
+        if delta < 1e-4:
+            break
+    if use_torch and not return_torch:
+        Q = Q.cpu().numpy()
+    return Q
+
+
+def read_cell_type_nlp_network(nlp_emb_file, cell_type_network_file):
+    cell_ontology_ids = set()
+    fin = open(cell_type_network_file)
+    co2co_graph = {}
+    for line in fin:
+        w = line.strip().split('\t')
+        if w[0] not in co2co_graph:
+            co2co_graph[w[0]] = set()
+        co2co_graph[w[0]].add(w[1])
+        cell_ontology_ids.add(w[0])
+        cell_ontology_ids.add(w[1])
+    fin.close()
+    if nlp_emb_file is not None:
+        fin = open(nlp_emb_file)
+        co2vec_nlp = {}
+        for line in fin:
+            w = line.strip().split('\t')
+            vec = []
+            for i in range(1, len(w)):
+                vec.append(float(w[i]))
+            co2vec_nlp[w[0]] = np.array(vec)
+        fin.close()
+        co2co_nlp = {}
+        for id1 in co2co_graph:
+            co2co_nlp[id1] = {}
+            for id2 in co2co_graph[id1]:
+                sc = 1 - spatial.distance.cosine(co2vec_nlp[id1], co2vec_nlp[id2])
+                co2co_nlp[id1][id2] = sc
+    else:
+        co2co_nlp = {}
+        for id1 in co2co_graph:
+            co2co_nlp[id1] = {}
+            for id2 in co2co_graph[id1]:
+                co2co_nlp[id1][id2] = 1.
+        co2vec_nlp = {}
+        for c in cell_ontology_ids:
+            co2vec_nlp[c] = np.ones((10))
+    return co2co_graph, co2co_nlp, co2vec_nlp, cell_ontology_ids
+
+
+def subset_cell_type_nlp_network(co2co_graph, co2co_nlp, co2vec_nlp, cell_ontology_ids, subsets):
+    new_co2co_graph, new_co2co_nlp, new_co2vec_nlp = {}, {}, {}
+    new_co_ids = set()
+    for co_i in subsets:
+        if co_i in co2co_graph.keys():
+            co_i_cncts = co2co_graph[co_i]
+            new_cncts = set()
+            for co_i_cnct in co_i_cncts:
+                if co_i_cnct in subsets:
+                    new_cncts.add(co_i_cnct)
+            if len(new_cncts) > 0:
+                new_co2co_graph[co_i] = new_cncts
+        if co_i in co2co_nlp.keys():
+            co_i_cncts = co2co_nlp[co_i]
+            new_cncts = {}
+            for co_i_cnct in co_i_cncts.keys():
+                if co_i_cnct in subsets:
+                    new_co_ids.add(co_i_cnct)
+                    new_cncts[co_i_cnct] = co_i_cncts[co_i_cnct]
+            if len(new_cncts.keys()) > 0:
+                new_co_ids.add(co_i)
+                new_co2co_nlp[co_i] = new_cncts
+    for co_i in new_co_ids:
+        if co_i in co2vec_nlp.keys():
+            new_co2vec_nlp[co_i] = co2vec_nlp[co_i]
+    return new_co2co_graph, new_co2co_nlp, new_co2vec_nlp, new_co_ids
+
+
+def map_genes(test_X, test_genes, train_genes, num_batches=10, memory_saving_mode=False):
+    """
+    Takes in the test set features, test_X, and a list of all the genes in the training and test sets
+    and returns new_test_X, which makes the gene indices of test_X correspond to the same ones from the
+    training set.
+    """
+    ntest_cell = np.shape(test_X)[0]  # Number of cells in the test set
+    ntrain_gene = len(train_genes)  # Number of genes in the train set
+    genes = list(set(test_genes) & set(train_genes))  # Genes that are in both the train and test sets
+    train_genes = list(train_genes)
+    test_genes = list(test_genes)
+    # print("Mapping genes with memory mode =", memory_saving_mode,"...")
+    if not memory_saving_mode:
+        new_test_x = np.zeros((ntest_cell, ntrain_gene))
+        ind1 = []
+        ind2 = []
+        for i, g in enumerate(genes):
+            ind1.append(train_genes.index(g))
+            ind2.append(test_genes.index(g))
+        ind1 = np.array(ind1)
+        ind2 = np.array(ind2)
+        new_test_x[:, ind1] = test_X[:, ind2]
+    else:
+        new_test_x = sparse.csr_matrix((ntest_cell, ntrain_gene))
+        batch_size = int(len(genes) / num_batches)
+        for i in range(num_batches):
+            # print("\tbatch #",i)
+            ind1 = []
+            ind2 = []
+            if i != num_batches - 1:
+                batch = genes[i * batch_size: (i + 1) * batch_size]
+            else:
+                batch = genes[i * batch_size:]
+            for g in batch:
+                ind1.append(train_genes.index(g))
+                ind2.append(test_genes.index(g))
+            ind1 = np.array(ind1)
+            ind2 = np.array(ind2)
+            new_test_x[:, ind1] = test_X[:, ind2]
+    return new_test_x
+
+
+def process_expression(train_X, test_X, train_genes, test_genes):
+    # this data process function is adapted from ACTINN, please check ACTINN for more information.
+    test_X = map_genes(test_X, test_genes, train_genes)
+    c2g = np.vstack([train_X, test_X])
+    c2g = np.array(c2g, dtype=np.float64)
+    c2g = c2g.T
+    index = np.sum(c2g, axis=1) > 0
+    c2g = c2g[index, :]
+    train_genes = train_genes[index]
+    c2g = np.divide(c2g, np.sum(c2g, axis=0, keepdims=True)) * 10000
+    c2g = np.log2(c2g + 1)
+    expr = np.sum(c2g, axis=1)
+    # total_set = total_set[np.logical_and(expr >= np.percentile(expr, 1), expr <= np.percentile(expr, 99)),]
+    index = np.logical_and(expr >= np.percentile(expr, 1), expr <= np.percentile(expr, 99))
+    c2g = c2g[index,]
+    train_genes = train_genes[index]
+    # print (np.logical_and(expr >= np.percentile(expr, 1), expr <= np.percentile(expr, 99)))
+
+    cv = np.std(c2g, axis=1) / np.mean(c2g, axis=1)
+    index = np.logical_and(cv >= np.percentile(cv, 1), cv <= np.percentile(cv, 99))
+    c2g = c2g[index,]
+    train_genes = train_genes[index]
+    c2g = c2g.T
+    c2g_list_new = []
+    index = 0
+    for c in [train_X, test_X]:
+        ncell = np.shape(c)[0]
+        c2g_list_new.append(c2g[index:index + ncell, :])
+        index = ncell
+        assert (len(train_genes) == np.shape(c2g)[1])
+    return c2g_list_new[0], c2g_list_new[1], train_genes
+
+
+def mean_normalization(train_X_mean, test_X):
+    test_X = np.log1p(test_X)
+    test_X_mean = np.mean(test_X, axis=0)
+    test_X = test_X - test_X_mean + train_X_mean
+    return test_X
+
+
+def get_gene_mapping(test_genes, train_genes):
+    """
+    Low-memory version of map_genes. Takes the list of genes used by the test set and the list of
+    genes used in the training set. Provides a numpy array that maps the indices of the test genes
+    to the indices of the training genes.
+    For instance, if gene 'abcd' is at index 1 in train_genes, and at index 7 in test_genes, then
+    the numpy array returned from this function will have a 1 at index 7.
+    """
+    genes = list(set(test_genes) & set(train_genes))  # Genes that are in both the train and test sets
+    train_genes = list(train_genes)
+    test_genes = list(test_genes)
+    # print("Getting gene mapping...")
+
+    gene_idx = np.arange(len(test_genes))
+    for g in genes:
+        train_idx = train_genes.index(g)
+        test_idx = test_genes.index(g)
+        gene_idx[train_idx] = test_idx
+
+    return gene_idx
+
+
+def graph_embedding_dca(A, i2l, mi=0, dim=20, unseen_l=None):
+    nl = np.shape(A)[0]
+    seen_ind = []
+    unseen_ind = []
+    for i in range(nl):
+        if i2l[i] in unseen_l:
+            unseen_ind.append(i)
+        else:
+            seen_ind.append(i)
+    seen_ind = np.array(seen_ind)
+    unseen_ind = np.array(unseen_ind)
+
+    # if len(seen_ind) * 0.8 < dim:
+    #	dim = int(len(seen_ind) * 0.8)
+    if mi == 0 or mi == 1:
+        # sp = graph_shortest_path(A, method='FW', directed=False)
+        sp = shortest_path(A, method='FW', directed=False)
+    else:
+        sp = RandomWalkRestart(A, 0.8)
+
+    sp = sp[seen_ind, :]
+    sp = sp[:, seen_ind]
+    X = np.zeros((np.shape(sp)[0], dim))
+    print("dim: ", np.shape(sp)[0] - 1)
+    print("dim0: ", dim)
+    svd_dim = min(dim, np.shape(sp)[0] - 1)
+    if mi == 0 or mi == 2:
+        print('please set mi=3')
+        # X[:, :svd_dim] = svd_emb(sp, dim=svd_dim)
+    else:
+        X[:, :svd_dim] = DCA_vector(sp, dim=svd_dim)[0]
+    X_ret = np.zeros((nl, dim))
+    X_ret[seen_ind, :] = X
+    if mi == 2 or mi == 3:
+        sp *= -1
+    return sp, X_ret
+
+
+def emb_ontology(i2l, ontology_mat, co2co_nlp, dim=5, mi=0, unseen_l=None):
+    nco = len(i2l)
+    network = np.zeros((nco, nco))
+    for i in range(nco):
+        c1 = i2l[i]
+        for j in range(nco):
+            if ontology_mat[i, j] == 1:
+                network[i, j] = co2co_nlp[c1][i2l[j]]
+                network[j, i] = co2co_nlp[c1][i2l[j]]
+    idd = 0
+    sp, i2emb = graph_embedding_dca(network, i2l, mi=mi, dim=dim, unseen_l=unseen_l)
+    return i2emb
+
+
+def get_ontology_parents(GO_net, g, dfs_depth=100):
+    term_valid = set()
+    ngh_GO = set()
+    ngh_GO.add(g)
+    depth = {}
+    depth[g] = 0
+    while len(ngh_GO) > 0:
+        for GO in list(ngh_GO):
+            for GO1 in GO_net[GO]:
+                ngh_GO.add(GO1)
+                depth[GO1] = depth[GO] + 1
+            ngh_GO.remove(GO)
+            if depth[GO] < dfs_depth:
+                term_valid.add(GO)
+    return term_valid
+
+
+def creat_cell_ontology_matrix(train_Y, co2co_graph, cell_ontology_ids, dfs_depth):
+    lset = set(cell_ontology_ids)
+
+    seen_l = sorted(np.unique(train_Y))
+    unseen_l = sorted(lset - set(train_Y))
+    ys = np.concatenate((seen_l, unseen_l))
+    i2l = {}
+    l2i = {}
+    for l in ys:
+        nl = len(i2l)
+        l2i[l] = nl
+        i2l[nl] = l
+    nco = len(i2l)
+
+    net_dict = collections.defaultdict(dict)
+    net_mat = np.zeros((nco, nco))
+    for co1 in co2co_graph:
+        l1 = l2i[co1]
+        for co2 in co2co_graph[co1]:
+            l2 = l2i[co2]
+            net_dict[l1][l2] = 1
+            net_mat[l1][l2] = 1
+    for n in range(nco):
+        ngh = get_ontology_parents(net_dict, n, dfs_depth)
+        net_dict[n][n] = 1
+        for n1 in ngh:
+            net_dict[n][n1] = 1
+    return unseen_l, l2i, i2l, net_dict, net_mat
+
+
+class DataProcessing:
+    def __init__(self, cell_type_network_file='../../OnClass_data/cell_ontology/cl.ontology',
+                 cell_type_nlp_emb_file='../../OnClass_data/cell_ontology/cl.ontology.nlp.emb',
+                 terms_with_def=set(),
+                 memory_saving_mode=False):
+        """
+        Initialize OnClass model with a given cell-type network and cell-type embedding file.
+        Also, you may set the memory_saving_mode to True to get a model that uses less RAM.
+        """
+        self.cell_type_nlp_emb_file = cell_type_nlp_emb_file
+        self.cell_type_network_file = cell_type_network_file
+        self.co2co_graph, self.co2co_nlp, self.co2vec_nlp, self.cell_ontology_ids = read_cell_type_nlp_network(
+            self.cell_type_nlp_emb_file, self.cell_type_network_file)
+        self.co2co_graph, self.co2co_nlp, self.co2vec_nlp, self.cell_ontology_ids = subset_cell_type_nlp_network(
+            self.co2co_graph, self.co2co_nlp, self.co2vec_nlp, self.cell_ontology_ids, terms_with_def)
+        self.mode = memory_saving_mode
+
+    def ProcessTrainFeature(self, train_feature, train_label, train_genes, test_feature=None, test_genes=None,
+                            batch_correct=False, log_transform=True):
+        """
+        Process the gene expression matrix used to train the model, and optionally the test data.
+        Parameters
+        ----------
+        train_feature: `numpy.ndarray` or `scipy.sparse.csr_matrix` (depends on mode)
+            gene expression matrix of cell types
+        train_label: `numpy.ndarray`
+            labels for the training features
+        train_genes: `list`
+            list of genes used during training
+        test_feature: `numpy.ndarray` or `scipy.sparse.csr_matrix` (depends on mode), optional (None)
+            gene expression matrix of cell types for the test set
+        test_genes: `list`, optional (None)
+            list of genes used in test set
+        batch_correct: `bool`, optional (False)
+            whether to correct for batch effect in data
+        log_transform:`bool`, optional (True)
+            whether to apply log transform to data
+        Returns
+        -------
+        train_feature, test_feature, self.genes, self.genes
+            returns the training feature gene expression matrix and the list of genese associated
+            with it. If test_feature was not none, also returns the test features and their genes.
+        """
+
+        if log_transform is False and np.max(train_feature) > 1000:
+            warnings.warn(
+                "Max expression is" + str(np.max(train_feature)) + '. Consider setting log transform = True\n')
+        self.genes = train_genes
+        # batch correction is currently not supported for memory_saving_mode
+        if batch_correct and test_feature is not None and test_genes is not None and self.mode:
+            train_feature, test_feature, selected_train_genes = process_expression(train_feature, test_feature,
+                                                                                   train_genes, test_genes)
+            self.genes = selected_train_genes
+        elif log_transform:
+            if self.mode:
+                train_feature = csr_matrix.log1p(train_feature)
+            else:
+                train_feature = np.log1p(train_feature)
+
+            if test_feature is not None:
+                if self.mode:
+                    test_feature = csr_matrix.log1p(test_feature)
+                else:
+                    test_feature = np.log1p(test_feature)
+        self.train_feature = train_feature
+        self.train_label = train_label
+        if test_feature is not None:
+            return train_feature, test_feature, self.genes, self.genes
+        else:
+            return train_feature, self.genes
+
+    def ProcessTestFeature(self, test_feature, test_genes, use_pretrain=None, batch_correct=False, log_transform=True):
+        """
+        Process the gene expression matrix used to test the model.
+        Parameters
+        ----------
+        test_feature: `numpy.ndarray` or `scipy.sparse.csr_matrix` (depends on mode)
+            gene expression matrix of cell types for the test set
+        test_genes: `list`
+            list of genes used in test set
+        use_pretrain: `string`, optional (None)
+            name of the pretrained model
+        batch_correct: `bool`, optional (False)
+            whether to correct for batch effect in data
+        log_transform:`bool`, optional (True)
+            whether to apply log transform to data
+        Returns
+        -------
+        gene_mapping or test_feature
+            processes the test features and returns a data structure that encodes the gene
+            expression matrix that should be used for testing. If the model is in memory saving
+            mode, then the function will return a tuple of gene expression matrix and index array,
+            otherwise, it will just return the matrix.
+        """
+        if log_transform is False and np.max(test_feature) > 1000:
+            warnings.warn("Max expression is" + str(np.max(test_feature)) + '. Consider setting log transform = True\n')
+
+        if log_transform:
+            test_feature = np.log1p(test_feature)
+        if batch_correct and not self.mode:
+            test_feature = mean_normalization(self.train_feature_mean, test_feature)
+
+        if self.mode:
+            gene_mapping = get_gene_mapping(test_genes, self.genes)
+            return test_feature, gene_mapping
+        else:
+            test_feature = map_genes(test_feature, test_genes, self.genes, memory_saving_mode=self.mode)
+            return test_feature
+
+    def EmbedCellTypes(self, train_Y_str, dim=5, emb_method=3, use_pretrain=None, write2file=None):
+        """
+        Embed the cell ontology
+        Parameters
+        ----------
+        cell_type_network_file : each line should be cell_type_1\tcell_type_2\tscore for weighted network or cell_type_1\tcell_type_2 for unweighted network
+        dim: `int`, optional (500)
+            Dimension of the cell type embeddings
+        emb_method: `int`, optional (3)
+            dimensionality reduction method
+        use_pretrain: `string`, optional (None)
+            use pretrain file. This should be the numpy file of cell type embeddings. It can read the one set in write2file parameter.
+        write2file: `string`, optional (None)
+            write the cell type embeddings to this file path
+        Returns
+        -------
+        co2emb, co2i, i2co
+            returns three dicts, cell type name to embeddings, cell type name to cell type id and cell type id to embeddings.
+        """
+
+        self.unseen_co, self.co2i, self.i2co, self.ontology_dict, self.ontology_mat = creat_cell_ontology_matrix(
+            train_Y_str, self.co2co_graph, self.cell_ontology_ids, dfs_depth=3)
+        self.nco = len(self.i2co)
+        Y_emb = emb_ontology(self.i2co, self.ontology_mat, dim=dim, mi=emb_method, co2co_nlp=self.co2co_nlp,
+                             unseen_l=self.unseen_co)
+        self.co2emb = np.column_stack((np.eye(self.nco), Y_emb))
+        self.nunseen = len(self.unseen_co)
+        self.nseen = self.nco - self.nunseen
+        self.co2vec_nlp_mat = np.zeros((self.nco, len(self.co2vec_nlp[self.i2co[0]])))
+        for i in range(self.nco):
+            self.co2vec_nlp_mat[i, :] = self.co2vec_nlp[self.i2co[i]]
+        return self.co2emb, self.co2i, self.i2co, self.ontology_mat
+
+
+class cellData(Dataset):
+
+    def __init__(self, expression_matrix, labels, nlabel=0, gpu_ids='0'):
+        self.expression_matrix = expression_matrix
+        self.labels = labels
+        self.nlabel = nlabel
+        self.gpu_ids = gpu_ids
+
+    def __getitem__(self, item):
+        x = np.asarray(self.expression_matrix[item, :].todense()).squeeze()
+        y = np.zeros(self.nlabel)
+        y[self.labels[item]] = float(1)
+        x = torch.from_numpy(x).float()
+        y = torch.from_numpy(y).float()
+        if len(self.gpu_ids) > 0:
+            x = x.cuda()
+            y = y.cuda()
+        return {'features': x, 'label': y}
+
+    def __len__(self):
+        return len(self.labels)
+
+
+def emb2tensor(def_embeddings, terms, add_bias=False):
+    '''
+    This function re-sort the textual description embeddings
+    according to the mapping between terms and index
+    :param text_embeddings:
+    :param terms:
+    :return:
+    '''
+    ann_id = list(terms.keys())
+    embedding_array = np.zeros((len(ann_id), np.size(def_embeddings[ann_id[0]], 1)))
+
+    for t_id in ann_id:
+        t_def = def_embeddings[t_id].reshape([1, -1])
+        t_def = t_def / np.sqrt(np.sum(np.power(t_def, 2), axis=1))
+        embedding_array[terms[t_id], :] = t_def
+    rank_e = np.linalg.matrix_rank(embedding_array)
+    if add_bias:
+        embedding_array = np.column_stack((np.eye(len(ann_id)), embedding_array))
+    print('Rank of your embeddings is {}'.format(rank_e))
+    embedding_array = torch.from_numpy(embedding_array)
+    return embedding_array.float()
+
+
+def read_data_file(dname, data_dir):
+    if 'microcebus' in dname and 'tabula_microcebus' not in dname:
+        tech = '10x'
+        feature_file = data_dir + 'Lemur/' + dname + '.h5ad'
+        filter_key = {'method': tech}
+        label_file = None
+        gene_file = ''
+        label_key = 'cell_ontology_class'
+    elif 'tabula_microcebus' in dname:
+        tech = dname.split('_')[1]
+        feature_file = data_dir + 'Tabula_Microcebus/' + 'LCA_complete_wRaw_toPublish.h5ad'
+        filter_key = {}
+        label_file = None
+        gene_file = ''
+        batch_key = ''
+        label_key = 'cell_ontology_class_v1'
+    elif 'sapiens' in dname:
+        feature_file = data_dir + 'Tabula_Sapiens/' + 'TabulaSapiens.h5ad'
+        filter_key = {}
+        label_file = None
+        gene_file = ''
+        batch_key = ''
+        label_key = 'cell_ontology_class'
+    elif 'muris' in dname:
+        tech = dname.split('_')[1]
+        feature_file = data_dir + 'Tabula_Muris_Senis/' + 'tabula-muris-senis-' + tech + '-official-raw-obj.h5ad'
+        filter_key = {}
+        label_file = None
+        gene_file = ''
+        batch_key = ''
+        label_key = 'cell_ontology_class'
+    elif 'sapiens' in dname:
+        feature_file = data_dir + 'sapiens/' + 'Pilot1_Pilot2_decontX_Oct2020.h5ad'
+        filter_key = {}
+        label_file = None
+        gene_file = ''
+        batch_key = ''
+        label_key = 'cell_ontology_type'
+    elif 'allen' in dname:
+        feature_file = data_dir + '/Allen_Brain/features.pkl'
+        label_file = data_dir + '/Allen_Brain/labels.pkl'
+        gene_file = data_dir + '/Allen_Brain/genes.pkl'
+        label_key = ''
+        filter_key = {}
+    elif 'krasnow' in dname:
+        tech = dname.split('_')[1]
+        feature_file = data_dir + '/HLCA/' + tech + '_features.pkl'
+        label_file = data_dir + '/HLCA/' + tech + '_labels.pkl'
+        gene_file = data_dir + '/HLCA/' + tech + '_genes.pkl'
+        label_key = ''
+        filter_key = {}
+    else:
+        sys.exit('wrong dname ' + dname)
+    if feature_file.endswith('.pkl'):
+        return feature_file, filter_key, label_key, label_file, gene_file
+    elif feature_file.endswith('.h5ad'):
+        return feature_file, filter_key, label_key, label_file, gene_file
+    sys.exit('wrong file suffix')
+
+
+def read_ontology_file(dname, data_folder):
+    if 'allen' in dname:
+        cell_type_network_file = data_folder + 'allen.ontology'
+        cell_type_nlp_emb_file = None
+        cl_obo_file = None
+        if not os.path.isfile(cell_type_network_file):
+            sys.error(cell_type_network_file + ' not found!')
+    else:
+        cell_type_network_file = data_folder + 'cl.ontology'
+        cell_type_nlp_emb_file = data_folder + 'cl.ontology.nlp.emb'
+        cl_obo_file = data_folder + 'cl.obo'
+        if not os.path.isfile(cell_type_nlp_emb_file):
+            sys.exit(cell_type_nlp_emb_file + ' not found!')
+        if not os.path.isfile(cell_type_network_file):
+            sys.exit(cell_type_network_file + ' not found!')
+        if not os.path.isfile(cl_obo_file):
+            sys.exit(cl_obo_file + ' not found!')
+    return cell_type_nlp_emb_file, cell_type_network_file, cl_obo_file
+
+
+def select_cells_based_on_keys(x, features, tissues=None, labels=None, filter_key=None):
+    ncell = np.shape(x.X)[0]
+    select_cells = set(range(ncell))
+    for key in filter_key:
+        value = filter_key[key]
+        select_cells = select_cells & set(np.where(np.array(x.obs[key]) == value)[0])
+    select_cells = sorted(select_cells)
+    features = features[select_cells, :]
+    if labels is not None:
+        labels = labels[select_cells]
+    if tissues is not None:
+        tissues = tissues[select_cells]
+    x = x[select_cells, :]
+    return features, labels, tissues, x
+
+
+def get_ontology_name(obo_file, lower=True):
+    fin = open(obo_file)
+    co2name = {}
+    name2co = {}
+    tag_is_syn = {}
+    for line in fin:
+        if line.startswith('id: '):
+            co = line.strip().split('id: ')[1]
+        if line.startswith('name: '):
+            if lower:
+                name = line.strip().lower().split('name: ')[1]
+            else:
+                name = line.strip().split('name: ')[1]
+            co2name[co] = name
+            name2co[name] = co
+        if line.startswith('synonym: '):
+            if lower:
+                syn = line.strip().lower().split('synonym: "')[1].split('" ')[0]
+            else:
+                syn = line.strip().split('synonym: "')[1].split('" ')[0]
+            if syn in name2co:
+                continue
+            name2co[syn] = co
+    fin.close()
+    return co2name, name2co
+
+
+def fine_nearest_co_using_nlp(sentences, co2emb, obo_file, nlp_mapping_cutoff=0.8):
+    co2name, name2co = get_ontology_name(obo_file=obo_file)
+    from sentence_transformers import SentenceTransformer
+    model = SentenceTransformer('bert-base-nli-mean-tokens')
+    sentences = np.array([sentence.lower() for sentence in sentences])
+    sentence_embeddings = model.encode(sentences)
+    co_embeddings = []
+    cos = []
+    for co in co2emb:
+        co_embeddings.append(co2emb[co])
+        cos.append(co)
+    co_embeddings = np.array(co_embeddings)
+    sent2co = {}
+    for sentence, embedding, ind in zip(sentences, sentence_embeddings, range(len(sentences))):
+        scs = cosine_similarity(co_embeddings, embedding.reshape(1, -1))
+
+        co_id = np.argmax(scs)
+        sc = scs[co_id]
+        if sc > nlp_mapping_cutoff:
+            sent2co[sentence.lower()] = cos[co_id]
+            names = set()
+            for name in name2co:
+                if name2co[name].upper() == cos[co_id]:
+                    names.add(name)
+        # print (sentence, cos[co_id], sc, co2name[cos[co_id]],names)
+    return sent2co
+
+
+def exact_match_co_name_2_co_id(labels, lab2co, cl_obo_file=None):
+    if cl_obo_file is None:
+        return lab2co
+    co2name, name2co = get_ontology_name(obo_file=cl_obo_file)
+    for label in labels:
+        if label.lower() in name2co:
+            lab2co[label.lower()] = name2co[label.lower()]
+    for name in name2co:
+        lab2co[name.lower()] = name2co[name]
+    return lab2co
+
+
+def map_and_select_labels(labels, cell_ontology_ids, obo_file, ct_mapping_key={}, nlp_mapping=True,
+                          nlp_mapping_cutoff=0.8, co2emb=None, cl_obo_file=None):
+    lab2co = {}
+    if nlp_mapping:
+        if co2emb is None:
+            sys.exit('Please provide cell type embedding to do NLP-based mapping.')
+        lab2co = fine_nearest_co_using_nlp(np.unique(labels), co2emb, obo_file, nlp_mapping_cutoff=nlp_mapping_cutoff)
+    lab2co = exact_match_co_name_2_co_id(np.unique(labels), lab2co, cl_obo_file=cl_obo_file)
+    for ct in ct_mapping_key:
+        lab2co[ct_mapping_key[ct]] = lab2co[ct]
+    ind = []
+    lab_id = []
+    unfound_labs = set()
+    for i, l in enumerate(labels):
+        if l in cell_ontology_ids:
+            ind.append(i)
+            lab_id.append(l)
+        elif l.lower() in lab2co:
+            ind.append(i)
+            lab_id.append(lab2co[l.lower()])
+        else:
+            unfound_labs.add(l)
+    frac = len(ind) * 1. / len(labels)
+    ind = np.array(ind)
+    labels = np.array(lab_id)
+    unfound_labs = set(unfound_labs)
+    warn_message = 'Warning: Only: %f precentage of labels are in the Cell Ontology. The remaining cells are excluded! Consider using NLP mapping and choose a small mapping cutoff (nlp_mapping_cutoff)' % (
+            frac * 100)
+    if frac < 0.5:
+        print(warn_message)
+        print('Here are unfound labels:', unfound_labs)
+    return ind, labels, unfound_labs
+
+
+def exclude_parent_child_nodes(cell_ontology_file, labels):
+    uniq_labels = np.unique(labels)
+    excludes = set()
+    net = collections.defaultdict(dict)
+    fin = open(cell_ontology_file)
+    for line in fin:
+        s, p = line.strip().split('\t')
+        net[s][p] = 1  # p is parent
+    fin.close()
+    for n in list(net.keys()):
+        ngh = get_ontology_parents(net, n)
+        for n1 in ngh:
+            net[n][n1] = 1
+    for l1 in uniq_labels:
+        for l2 in uniq_labels:
+            if l1 in net[l2] and l1 != l2:  # l1 is l2 parent
+                excludes.add(l1)
+    # print (excludes)
+    new_ids = []
+    for i in range(len(labels)):
+        if labels[i] not in excludes:
+            new_ids.append(i)
+    new_ids = np.array(new_ids)
+    return new_ids, excludes
+
+
+def read_data(feature_file, cell_ontology_ids, exclude_non_leaf_ontology=False, ct_mapping_key={}, tissue_key=None,
+              seed=1, filter_key=None, AnnData_label_key=None, nlp_mapping=True, nlp_mapping_cutoff=0.8, co2emb=None,
+              label_file=None, cl_obo_file=None, cell_ontology_file=None, memory_saving_mode=False,
+              backup_file='sparse_featurefile_backup'):
+    """
+	Read data from the given feature file, and processes it so that it fits with the other
+	given paramters as needed.
+	Parameters
+	----------
+	feature_file: `string`
+		name of file to extract data from. The data in the file must be stored in h5ad file format.
+	cell_ontology_ids: `set`
+		set of ids from the cell ontology.
+	AnnData_label_key: `numpy.ndarray`, optional (None)
+		mapping of the cell type classes to reindex the labels in the AnnData object
+	co2emb: `map`, optional (None)
+		maps cell-type from the cell ontology to its embedding
+	label_file: `string`, optional (None)
+		file from which to get the labels of the feature file
+	memory_saving_mode: `bool`, optional (False)
+		whether the method should be run under tight RAM constraints.
+	backup_file: `string`, optional ('sparse_featurefile_backup')
+		the name of the file to copy the sparse feature dataset to.
+
+	Returns
+	-------
+	dataset: `numpy.ndarray` or `scipy.sparse.csr_matrix` (depends on mode)
+		gene expression matrix of cell types for the test set
+	genes: `list`
+		list of genes in the dataset
+	labels: `numpy.ndarray`
+		labels from the feature file
+	x: AnnData object stored in the given feature file
+	"""
+
+    np.random.seed(seed)
+
+    if memory_saving_mode:
+        x = read_h5ad(feature_file, backed='r+')
+        if 'Tabula_Microcebus' in feature_file or 'TabulaSapiens' in feature_file:
+            x.raw = None
+        dataset = x.X.to_memory()  # Gets a sparse array in csr matrix form
+    else:
+        x = read_h5ad(feature_file)
+        dataset = x.X.toarray()
+
+    # if memory_saving_mode:
+    #    print_memory_usage("while reading data")
+
+    ncell = np.shape(x.X)[0]
+    genes = np.array([x.upper() for x in x.var.index])
+
+    if tissue_key is not None and 'TabulaSapiens' not in feature_file:
+        tissues = np.array(x.obs[tissue_key].tolist())
+    else:
+        tissues = None
+    if AnnData_label_key is None and label_file is None:
+        print('no label file is provided')
+        labels = None
+        dataset, labels, tissues, x = select_cells_based_on_keys(x, dataset, labels=labels, tissues=tissues,
+                                                                 filter_key=filter_key)
+        return dataset, genes, labels, tissues, x
+    if AnnData_label_key is not None:
+        labels = x.obs[AnnData_label_key].tolist()
+    else:
+        fin = open(label_file)
+        labels = []
+        for line in fin:
+            labels.append(line.strip())
+        fin.close()
+    labels = np.array(labels)
+    dataset, labels, tissues, x = select_cells_based_on_keys(x, dataset, labels=labels, tissues=tissues,
+                                                             filter_key=filter_key)
+
+    if memory_saving_mode:
+        x = x.copy(filename=backup_file)
+
+    ind, labels, unfound_labs = map_and_select_labels(labels, cell_ontology_ids, cl_obo_file,
+                                                      ct_mapping_key=ct_mapping_key, nlp_mapping=nlp_mapping,
+                                                      co2emb=co2emb, nlp_mapping_cutoff=nlp_mapping_cutoff,
+                                                      cl_obo_file=cl_obo_file)
+    if tissue_key is not None and 'TabulaSapiens' not in feature_file:
+        tissues = tissues[ind]
+    dataset = dataset[ind, :]
+
+    if memory_saving_mode:
+        # Need to copy to disk for rewriting to the sparse dataset
+        x = x[ind, :].copy(filename=backup_file)
+    else:
+        x = x[ind, :]
+
+    if exclude_non_leaf_ontology:
+        new_ids, exclude_terms = exclude_parent_child_nodes(cell_ontology_file, labels)
+        if tissues is not None:
+            tissues = tissues[new_ids]
+        dataset = dataset[new_ids, :]
+        labels = labels[new_ids]
+        x = x[new_ids, :]
+
+    ncell = np.shape(dataset)[0]
+    index = np.random.choice(ncell, ncell, replace=False)
+    dataset = dataset[index, :]  # cell by gene matrix
+    labels = labels[index]
+    if tissue_key is not None and 'TabulaSapiens' not in feature_file:
+        tissues = tissues[index]
+    return dataset, genes, labels, tissues, x
+
+
+def load_co_text(co_data_path):
+    ont = dict()
+    obj = None
+    with open(co_data_path, 'r') as f:
+        for line in f:
+            line = line.strip()
+            if not line:
+                continue
+            if line == '[Term]':
+                if obj is not None and len(obj['text']) > 0:
+                    ont[obj['id']] = obj
+                obj = dict()
+                obj['text'] = ""
+                continue
+            elif line == '[Typedef]' and len(obj['text']) > 0:
+                if obj is not None:
+                    ont[obj['id']] = obj
+                obj = None
+            else:
+                if obj is None:
+                    continue
+                l = line.split(": ")
+                if l[0] == 'id':
+                    obj['id'] = l[1]
+                elif l[0] == 'name':
+                    obj['text'] += line.split('name: ')[1].strip() + '. '
+                elif l[0] == 'def':
+                    obj['text'] += line.split('def: ')[1].split('"')[1].strip()
+        if obj is not None and len(obj['text']) > 0:
+            ont[obj['id']] = obj
+    return ont
+
+def extract_data_based_on_class(feats, labels, sel_labels):
+    ind = []
+    for l in sel_labels:
+        id = np.where(labels == l)[0]
+        ind.extend(id)
+    np.random.shuffle(ind)
+    X = feats[ind, :]
+    Y = labels[ind]
+    return X, Y, ind
+
+
+def SplitTrainTest(all_X, all_Y, all_tissues=None, random_state=10, nfold_cls=0.3, nfold_sample=0.2, nmin_size=10,
+                   memory_saving_mode=False):
+    """
+    Utility function for splitting the dataset into a train and test set.
+    Parameters
+    ----------
+    all_X: all the feature data
+    all_Y: the corresponding labels
+
+    Returns
+    -------
+    The labeled training and test sets
+    """
+    np.random.seed(random_state)
+
+    cls = np.unique(all_Y)
+    cls2ct = Counter(all_Y)
+    ncls = len(cls)
+    test_cls = list(np.random.choice(cls, int(ncls * nfold_cls), replace=False))
+    for c in cls2ct:
+        if cls2ct[c] < nmin_size:
+            test_cls.append(c)
+    test_cls = np.unique(test_cls)
+    # add rare class to test, since they cannot be split into train and test by using train_test_split(stratify=True)
+    train_cls = [x for x in cls if x not in test_cls]
+    train_cls = np.array(train_cls)
+    train_X, train_Y, train_ind = extract_data_based_on_class(all_X, all_Y, train_cls)
+    test_X, test_Y, test_ind = extract_data_based_on_class(all_X, all_Y, test_cls)
+    if all_tissues is not None:
+        train_tissues = all_tissues[train_ind]
+        test_tissues = all_tissues[test_ind]
+        train_X_train, train_X_test, train_Y_train, train_Y_test, train_tissues_train, train_tissues_test = train_test_split(
+            train_X, train_Y, train_tissues, test_size=nfold_sample, stratify=train_Y, random_state=random_state)
+        test_tissues = np.concatenate((test_tissues, train_tissues_test))
+        train_tissues = train_tissues_train
+    else:
+        train_X_train, train_X_test, train_Y_train, train_Y_test = train_test_split(
+            train_X, train_Y, test_size=nfold_sample, stratify=train_Y, random_state=random_state)
+
+    # TODO: Added this memory saving mode toggle
+    if memory_saving_mode:
+        test_X = scipy.sparse.vstack((test_X, train_X_test)).tocsr()
+    else:
+        test_X = np.vstack((test_X, train_X_test))
+
+    test_Y = np.concatenate((test_Y, train_Y_test))
+    train_X = train_X_train
+    train_Y = train_Y_train
+    if all_tissues is not None:
+        return train_X, train_Y, train_tissues, test_X, test_Y, test_tissues
+    else:
+        return train_X, train_Y, test_X, test_Y
+
+
+def compute_roc(labels, preds):
+    # Compute ROC curve and ROC area for each class
+    fpr, tpr, _ = roc_curve(labels.flatten(), preds.flatten())
+    roc_auc = auc(fpr, tpr)
+    return roc_auc
+
+
+def compute_prc(labels, preds):
+    # Compute PRC curve and PRC area for each class
+    pr, rc, _ = precision_recall_curve(labels.flatten(), preds.flatten())
+    prc_auc = auc(rc, pr)
+    return prc_auc
+
+
+def evaluate_unseen_auroc(inference_preds, inference_label, unseen2i):
+    roc_macro = np.zeros(len(unseen2i.values()))
+    unseen_id = list(unseen2i.values())
+    cl_i = 0
+    for i in unseen_id:
+        unseen_preds, unseen_labels = inference_preds[:, i], inference_label[:, i]
+        auroc = compute_roc(unseen_labels, unseen_preds)
+        roc_macro[cl_i] = auroc
+        cl_i += 1
+    return np.mean(roc_macro)
+
+
+def evaluate_auroc(inference_preds, inference_label):
+    roc_macro = np.zeros(np.size(inference_label, 1))
+    for cl_i in range(np.size(inference_label, 1)):
+        roc_auc = compute_roc(inference_label[:, cl_i], inference_preds[:, cl_i])
+        roc_macro[cl_i] = roc_auc
+    roc_auc = np.mean(roc_macro)
+    return roc_auc
+
+
+def sampled_auprc(truths, preds):
+    pos = np.where(truths == 1)[0]
+    neg = np.where(truths == 0)[0]
+    assert (len(pos) + len(neg) == len(truths))
+    nneg = len(neg)
+    npos = len(pos)
+    select_neg = np.random.choice(nneg, npos * 3, replace=True)
+    select_ind = np.concatenate((pos, select_neg))
+    return average_precision_score(truths[select_ind], preds[select_ind])
+
+
+def evaluate_unseen_auprc(inference_preds, inference_label, unseen2i):
+    roc_macro = np.zeros(len(unseen2i.values()))
+    unseen_id = list(unseen2i.values())
+    cl_i = 0
+    for i in unseen_id:
+        unseen_preds, unseen_labels = inference_preds[:, i], inference_label[:, i]
+        auroc = sampled_auprc(unseen_labels, unseen_preds)
+        roc_macro[cl_i] = auroc
+        cl_i += 1
+    return np.mean(roc_macro)
+
+
+def evaluate_auprc(inference_preds, inference_label):
+    roc_macro = np.zeros(np.size(inference_label, 1))
+    for cl_i in range(np.size(inference_label, 1)):
+        roc_auc = sampled_auprc(inference_label[:, cl_i], inference_preds[:, cl_i])
+        roc_macro[cl_i] = roc_auc
+    roc_auc = np.mean(roc_macro)
+    return roc_auc
+
+
+def find_gene_ind(genes, common_genes):
+    gid = []
+    for g in common_genes:
+        gid.append(np.where(genes == g)[0][0])
+    gid = np.array(gid)
+    return gid
```

### Comparing `biotranslator-0.1.1/biotranslator.egg-info/PKG-INFO` & `biotranslator-0.1.2/biotranslator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: biotranslator
-Version: 0.1.1
-Summary: BioTranslator: Cross-modal Translation for Zero-shot Biomedical Classification
-Home-page: https://github.com/ywzhao2002/biotranslator
-Author: Hanwen Xu, Yunwei Zhao, Addie Woicik, Hoifung Poon, Russ B.Altman, Sheng Wang
-Author-email: swang91@uw.edu
-Maintainer-email: Hanwen Xu <xuhw@cs.washington.edu>, Yunwei Zhao <yzhao4@cs.washington.edu>
-License: MIT Licence
-Project-URL: Documentation, https://biotranslator.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/HanwenXuTHU/BioTranslatorProject
-Keywords: pip,BioTranslator
-Platform: any
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-Provides-Extra: doc
-
-[![Stars](https://img.shields.io/github/stars/scverse/scanpy?logo=GitHub&color=yellow)](https://github.com/HanwenXuTHU/BioTranslatorProject)
-[![PyPI](https://img.shields.io/pypi/v/scanpy?logo=PyPI)](https://pypi.org/project/biotranslator/)
-[![PyPIDownload](https://static.pepy.tech/badge/biotranslator)](https://pepy.tech/project/biotranslator)
-[![Doc](https://readthedocs.org/projects/biotranslator/badge/?version=latest)](https://biotranslator.readthedocs.io/en/latest/?badge=latest)
-
-
-# BioTranslator API
-
-BioTranslator is a cross-modal translator which can annotate biology instances only using user-written texts.
-The codes here can reproduce the main results in BioTranslator paper, including zero-shot protein function prediction, zero-shot cell type prediction, and predict the nodes and edges of a gene pathway.
-BioTranslator takes a user-written textual description of the new discovery and then translates this description to a non-text biological data instance. Our tool frees scientists from limiting their analysis within predefined controlled vocabularies, thus accelerating new biomedical discoveries.
-
-[documentation]: https://biotranslator.readthedocs.io
-
-For more information, please visit the project's main repository [here](https://github.com/HanwenXuTHU/BioTranslatorProject).
+Metadata-Version: 2.1
+Name: biotranslator
+Version: 0.1.2
+Summary: BioTranslator: Cross-modal Translation for Zero-shot Biomedical Classification
+Home-page: https://github.com/ywzhao2002/biotranslator
+Author: Hanwen Xu, Yunwei Zhao, Addie Woicik, Hoifung Poon, Russ B.Altman, Sheng Wang
+Author-email: swang91@uw.edu
+Maintainer-email: Hanwen Xu <xuhw@cs.washington.edu>, Yunwei Zhao <yzhao4@cs.washington.edu>
+License: MIT Licence
+Project-URL: Documentation, https://biotranslator.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/HanwenXuTHU/BioTranslatorProject
+Keywords: pip,BioTranslator
+Platform: any
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+Provides-Extra: doc
+
+[![Stars](https://img.shields.io/github/stars/ywzhao2002/biotranslator?logo=GitHub&color=yellow)](https://github.com/HanwenXuTHU/BioTranslatorProject)
+[![PyPI](https://img.shields.io/pypi/v/biotranslator?logo=PyPI)](https://pypi.org/project/biotranslator/)
+[![PyPIDownload](https://static.pepy.tech/badge/biotranslator)](https://pepy.tech/project/biotranslator)
+[![Doc](https://readthedocs.org/projects/biotranslator/badge/?version=latest)](https://biotranslator.readthedocs.io/en/latest/index.html)
+
+
+# BioTranslator API
+
+BioTranslator is a cross-modal translator which can annotate biology instances only using user-written texts.
+The codes here can reproduce the main results in BioTranslator paper, including zero-shot protein function prediction, zero-shot cell type prediction, and predict the nodes and edges of a gene pathway.
+BioTranslator takes a user-written textual description of the new discovery and then translates this description to a non-text biological data instance. Our tool frees scientists from limiting their analysis within predefined controlled vocabularies, thus accelerating new biomedical discoveries.
+
+[documentation]: https://biotranslator.readthedocs.io
+
+For more information, feel free to visit the project's main repository [here](https://github.com/HanwenXuTHU/BioTranslatorProject).
```

### Comparing `biotranslator-0.1.1/biotranslator.egg-info/SOURCES.txt` & `biotranslator-0.1.2/biotranslator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biotranslator-0.1.1/pyproject.toml` & `biotranslator-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-[build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "biotranslator"
-authors = [
-    {name = "Hanwen Xu"},
-    {name = "Yunwei Zhao"},
-    {name = "Addie Woicik"},
-    {name = "Hoifung Poon"},
-    {name = "Russ B.Altman"},
-    {name = "Sheng Wang"}
-]
-maintainers = [
-    {name = "Hanwen Xu", email = "xuhw@cs.washington.edu"},
-    {name = "Yunwei Zhao", email = "yzhao4@cs.washington.edu"},
-]
-readme = {file = "README.md", content-type="text/markdown"}
-dynamic = ["version", "description"]
-classifiers = [
-    "Intended Audience :: Developers",
-    "Intended Audience :: Science/Research",
-    "Natural Language :: English",
-    "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Topic :: Scientific/Engineering :: Bio-Informatics",
-]
-dependencies = [
-    "sentence-transformers",
-    "anndata>=0.6.4",
-    "fbpca>=1.0",
-    "umap-learn>=0.3.10",
-    "matplotlib>=2.0.2",
-    "numpy>=1.16.4",
-    "scipy>=1.3.1",
-    "scikit-learn>=0.21.3",
-    "scanorama>=1.7.1",
-    "torch==1.7.1",
-    "pandas",
-    "tqdm",
-    "networkx",
-    "gensim",
-    "nltk",
-    "torchvision==0.8.2",
-]
-[project.optional-dependencies]
-doc = [
-    "myst-parser",
-]
-[project.urls]
-Documentation = "https://biotranslator.readthedocs.io/en/latest/"
-Source = "https://github.com/HanwenXuTHU/BioTranslatorProject"
-
-[project.scripts]
-
-[tool.flit.module]
-name = "biotranslator"
-
-[tool.flit.sdist]
-exclude = [
-    "setup.py",
+[build-system]
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "biotranslator"
+authors = [
+    {name = "Hanwen Xu"},
+    {name = "Yunwei Zhao"},
+    {name = "Addie Woicik"},
+    {name = "Hoifung Poon"},
+    {name = "Russ B.Altman"},
+    {name = "Sheng Wang"}
+]
+maintainers = [
+    {name = "Hanwen Xu", email = "xuhw@cs.washington.edu"},
+    {name = "Yunwei Zhao", email = "yzhao4@cs.washington.edu"},
+]
+readme = {file = "README.md", content-type="text/markdown"}
+dynamic = ["version", "description", "keywords", "license"]
+classifiers = [
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "Natural Language :: English",
+    "Operating System :: POSIX :: Linux",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Topic :: Scientific/Engineering :: Bio-Informatics",
+]
+dependencies = [
+    "sentence-transformers",
+    "anndata>=0.6.4",
+    "fbpca>=1.0",
+    "umap-learn>=0.3.10",
+    "matplotlib>=2.0.2",
+    "numpy>=1.16.4",
+    "scipy>=1.3.1",
+    "scikit-learn>=0.21.3",
+    "scanorama>=1.7.1",
+    "torch==1.7.1",
+    "pandas",
+    "tqdm",
+    "networkx",
+    "gensim",
+    "nltk",
+    "torchvision==0.8.2",
+]
+[project.optional-dependencies]
+doc = [
+    "myst-parser",
+]
+[project.urls]
+Documentation = "https://biotranslator.readthedocs.io/en/latest/"
+Source = "https://github.com/HanwenXuTHU/BioTranslatorProject"
+
+[project.scripts]
+
+[tool.flit.module]
+name = "biotranslator"
+
+[tool.flit.sdist]
+exclude = [
+    "setup.py",
 ]
```

### Comparing `biotranslator-0.1.1/setup.py` & `biotranslator-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import io
-from setuptools import setup, find_packages
-
-with io.open('./README.md', encoding='utf-8') as f:
-    readme = f.read()
-
-setup(
-    name = "BioTranslator",
-    version = "0.1.1",
-    keywords = ("pip", "BioTranslator"),
-    description = "BioTranslator: Cross-modal Translation for Zero-shot Biomedical Classification",
-    long_description = readme,
-    license = "MIT Licence",
-
-    url = "https://github.com/ywzhao2002/biotranslator",
-    author = "Sheng Wang",
-    author_email = "swang91@uw.edu",
-
-    packages = find_packages(),
-    include_package_data = True,
-    platforms = "any",
-    install_requires=[
-        "sentence-transformers",
-        "anndata>=0.6.4",
-        "fbpca>=1.0",
-        "umap-learn>=0.3.10",
-        "matplotlib>=2.0.2",
-        "numpy>=1.16.4",
-        "scipy>=1.3.1",
-        "scikit-learn>=0.21.3",
-        "scanorama>=1.7.1",
-        "torch==1.7.1",
-        "pandas",
-        "tqdm",
-        "networkx",
-        "gensim",
-        "nltk",
-        "torchvision==0.8.2",
-    ]
+import io
+from setuptools import setup, find_packages
+
+with io.open('./README.md', encoding='utf-8') as f:
+    readme = f.read()
+
+setup(
+    name = "BioTranslator",
+    version = "0.1.2",
+    keywords = ("pip", "BioTranslator"),
+    description = "BioTranslator: Cross-modal Translation for Zero-shot Biomedical Classification",
+    long_description = readme,
+    license = "MIT Licence",
+
+    url = "https://github.com/ywzhao2002/biotranslator",
+    author = "Sheng Wang",
+    author_email = "swang91@uw.edu",
+
+    packages = find_packages(),
+    include_package_data = True,
+    platforms = "any",
+    install_requires=[
+        "sentence-transformers",
+        "anndata>=0.6.4",
+        "fbpca>=1.0",
+        "umap-learn>=0.3.10",
+        "matplotlib>=2.0.2",
+        "numpy>=1.16.4",
+        "scipy>=1.3.1",
+        "scikit-learn>=0.21.3",
+        "scanorama>=1.7.1",
+        "torch==1.7.1",
+        "pandas",
+        "tqdm",
+        "networkx",
+        "gensim",
+        "nltk",
+        "torchvision==0.8.2",
+    ]
 )
```

