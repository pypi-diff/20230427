# Comparing `tmp/code_eval_score-0.1.0.tar.gz` & `tmp/code_eval_score-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/code_eval_score-0.1.0.tar", last modified: Thu Apr 27 06:38:33 2023, max compression
+gzip compressed data, was "dist/code_eval_score-0.2.0.tar", last modified: Thu Apr 27 08:59:23 2023, max compression
```

## Comparing `code_eval_score-0.1.0.tar` & `code_eval_score-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 lizhuo    (1001) lizhuo    (1001)        0 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     1068 2023-04-26 12:40:12.000000 code_eval_score-0.1.0/LICENSE
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     1126 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/PKG-INFO
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)      452 2023-04-26 12:39:27.000000 code_eval_score-0.1.0/README.rst
-drwxrwxr-x   0 lizhuo    (1001) lizhuo    (1001)        0 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/code_eval_score/
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)        0 2023-04-27 06:04:57.000000 code_eval_score-0.1.0/code_eval_score/__init__.py
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)      324 2023-04-27 06:37:44.000000 code_eval_score-0.1.0/code_eval_score/demo.py
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     3648 2023-04-27 06:37:19.000000 code_eval_score-0.1.0/code_eval_score/genscore.py
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)    10243 2023-04-27 06:26:27.000000 code_eval_score-0.1.0/code_eval_score/matchscore.py
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)    17337 2023-04-27 06:32:36.000000 code_eval_score-0.1.0/code_eval_score/utils.py
-drwxrwxr-x   0 lizhuo    (1001) lizhuo    (1001)        0 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/code_eval_score.egg-info/
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     1126 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/code_eval_score.egg-info/PKG-INFO
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)      356 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/code_eval_score.egg-info/SOURCES.txt
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)        1 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/code_eval_score.egg-info/dependency_links.txt
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)       67 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/code_eval_score.egg-info/requires.txt
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)       16 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/code_eval_score.egg-info/top_level.txt
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)       38 2023-04-27 06:38:33.000000 code_eval_score-0.1.0/setup.cfg
--rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     3924 2023-04-27 06:31:58.000000 code_eval_score-0.1.0/setup.py
+drwxrwxr-x   0 lizhuo    (1001) lizhuo    (1001)        0 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     1068 2023-04-26 12:40:12.000000 code_eval_score-0.2.0/LICENSE
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)      741 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/PKG-INFO
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     1344 2023-04-27 07:34:52.000000 code_eval_score-0.2.0/README.md
+drwxrwxr-x   0 lizhuo    (1001) lizhuo    (1001)        0 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/code_eval_score/
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)        0 2023-04-27 06:04:57.000000 code_eval_score-0.2.0/code_eval_score/__init__.py
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)      367 2023-04-27 06:46:34.000000 code_eval_score-0.2.0/code_eval_score/demo.py
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     3648 2023-04-27 06:37:19.000000 code_eval_score-0.2.0/code_eval_score/genscore.py
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     8839 2023-04-27 08:46:54.000000 code_eval_score-0.2.0/code_eval_score/matchscore.py
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)    17337 2023-04-27 06:32:36.000000 code_eval_score-0.2.0/code_eval_score/utils.py
+drwxrwxr-x   0 lizhuo    (1001) lizhuo    (1001)        0 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/code_eval_score.egg-info/
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)      741 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/code_eval_score.egg-info/PKG-INFO
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)      355 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/code_eval_score.egg-info/SOURCES.txt
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)        1 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/code_eval_score.egg-info/dependency_links.txt
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)       67 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/code_eval_score.egg-info/requires.txt
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)       16 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/code_eval_score.egg-info/top_level.txt
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)       38 2023-04-27 08:59:23.000000 code_eval_score-0.2.0/setup.cfg
+-rw-rw-r--   0 lizhuo    (1001) lizhuo    (1001)     3924 2023-04-27 08:59:17.000000 code_eval_score-0.2.0/setup.py
```

### Comparing `code_eval_score-0.1.0/LICENSE` & `code_eval_score-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `code_eval_score-0.1.0/code_eval_score/genscore.py` & `code_eval_score-0.2.0/code_eval_score/genscore.py`

 * *Files identical despite different names*

### Comparing `code_eval_score-0.1.0/code_eval_score/matchscore.py` & `code_eval_score-0.2.0/code_eval_score/matchscore.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-import os
-import sys
 import time
-import pathlib
 import torch
 import numpy as np
-import pandas as pd
 
 from collections import defaultdict
 from transformers import AutoTokenizer
 
-from utils import (
+from code_eval_score.utils import (
     get_model,
     bert_chunk_cos_score,
     get_bert_embedding,
     lang2model,
     model2layers,
     sent_encode,
 )
@@ -43,44 +39,39 @@
     verbose=False,
     idf=False,
     device=None,
     batch_size=64,
     nthreads=4,
     all_layers=False,
     return_hash=False,
-    rescale_with_baseline=False,
-    baseline_path=None,
     no_punc=False,
     sources=None,
     chunk_overlap=0.5,
     use_flow=False
 ):
     """
-    BERTScore metric.
+    Chunked MatchScore metric.
 
     Args:
         - :param: `cands` (list of str): candidate sentences
         - :param: `refs` (list of str or list of list of str): reference sentences
         - :param: `lang` (str): language of the sentences; has to specify
-                  at least one of `model_type` or `lang`. `lang` needs to be
-                  specified when `rescale_with_baseline` is True.
+                  at least one of `model_type` or `lang`.
         - :param: `model_type` (str): bert specification, default using the suggested
                   model for the target langauge; has to specify at least one of
                   `model_type` or `lang`
         - :param: `num_layers` (int): the layer of representation to use.
                   default using the number of layer tuned on WMT16 correlation data
         - :param: `verbose` (bool): turn on intermediate status update
         - :param: `idf` (bool or dict): use idf weighting, can also be a precomputed idf_dict
         - :param: `device` (str): on which the contextual embedding model will be allocated on.
                   If this argument is None, the model lives on cuda:0 if cuda is available.
         - :param: `nthreads` (int): number of threads
         - :param: `batch_size` (int): bert score processing batch size
         - :param: `return_hash` (bool): return hash code of the setting
-        - :param: `rescale_with_baseline` (bool): rescale bertscore with pre-computed baseline
-        - :param: `baseline_path` (str): customized baseline file
         - :param: `no_punc` (bool): Uri: exclude punctuation-only tokens in candidate and reference
         - :param: `sources` (list of str): Uri: a list of a source for each candidate, to be concatenated with the candidates
                    but removed from the similarity computation
         - :param: `chunk_overlap` (float): Uri: how much overlap between chunks, when the input is longer than the models' max length
 
     Return:
         - :param: `(P, R, F)`: each is of shape (N); N = number of input
@@ -89,17 +80,14 @@
                   multiple references, the returned score of this candidate is 
                   the *best* score among all references.
     """
     assert len(cands) == len(refs), "Different number of candidates and references"
 
     assert lang is not None or model_type is not None, "Either lang or model_type should be specified"
 
-    if rescale_with_baseline:
-        assert lang is not None, "Need to specify Language when rescaling with baseline"
-
     if model_type is None:
         lang = lang.lower()
         model_type = lang2model[lang]
     if num_layers is None:
         num_layers = model2layers[model_type]
 
     tokenizer = AutoTokenizer.from_pretrained(model_type)
@@ -146,43 +134,37 @@
         time_diff = time.perf_counter() - start
         print(f"done in {time_diff:.2f} seconds, {len(refs) / time_diff:.2f} sentences/sec")
 
     return precision, recall
 
 
 def plot_example(
-    candidate, reference, model_type=None, num_layers=None, lang=None, rescale_with_baseline=False,
-    baseline_path=None, fname="",
+    candidate, reference, model_type=None, num_layers=None, lang=None, fname="",
 ):
     """
-    BERTScore metric.
+    MatchScore metric.
 
     Args:
         - :param: `candidate` (str): a candidate sentence
         - :param: `reference` (str): a reference sentence
         - :param: `verbose` (bool): turn on intermediate status update
         - :param: `model_type` (str): bert specification, default using the suggested
                   model for the target langauge; has to specify at least one of
                   `model_type` or `lang`
         - :param: `num_layers` (int): the layer of representation to use
         - :param: `lang` (str): language of the sentences; has to specify
-                  at least one of `model_type` or `lang`. `lang` needs to be
-                  specified when `rescale_with_baseline` is True.
+                  at least one of `model_type` or `lang`.
         - :param: `return_hash` (bool): return hash code of the setting
-        - :param: `rescale_with_baseline` (bool): rescale bertscore with pre-computed baseline
         - :param: `fname` (str): path to save the output plot
     """
     assert isinstance(candidate, str)
     assert isinstance(reference, str)
 
     assert lang is not None or model_type is not None, "Either lang or model_type should be specified"
 
-    if rescale_with_baseline:
-        assert lang is not None, "Need to specify Language when rescaling with baseline"
-
     if model_type is None:
         lang = lang.lower()
         model_type = lang2model[lang]
     if num_layers is None:
         num_layers = model2layers[model_type]
 
     tokenizer = AutoTokenizer.from_pretrained(model_type)
@@ -207,23 +189,14 @@
     sim = sim.squeeze(0).cpu()
 
     # remove [CLS] and [SEP] tokens
     r_tokens = [tokenizer.decode([i]) for i in sent_encode(tokenizer, reference)][1:-1]
     h_tokens = [tokenizer.decode([i]) for i in sent_encode(tokenizer, candidate)][1:-1]
     sim = sim[1:-1, 1:-1]
 
-    if rescale_with_baseline:
-        if baseline_path is None:
-            baseline_path = os.path.join(os.path.dirname(__file__), f"rescale_baseline/{lang}/{model_type}.tsv")
-        if os.path.isfile(baseline_path):
-            baselines = torch.from_numpy(pd.read_csv(baseline_path).iloc[num_layers].to_numpy())[1:].float()
-            sim = (sim - baselines[2].item()) / (1 - baselines[2].item())
-        else:
-            print(f"Warning: Baseline not Found for {model_type} on {lang} at {baseline_path}", file=sys.stderr)
-
     import matplotlib.pyplot as plt
     from mpl_toolkits.axes_grid1 import make_axes_locatable
     fig, ax = plt.subplots(figsize=(len(r_tokens), len(h_tokens)))
     im = ax.imshow(sim, cmap="Blues", vmin=0, vmax=1)
 
     # We want to show all ticks...
     ax.set_xticks(np.arange(len(r_tokens)))
@@ -231,16 +204,14 @@
     # ... and label them with the respective list entries
     ax.set_xticklabels(r_tokens, fontsize=10)
     ax.set_yticklabels(h_tokens, fontsize=10)
     ax.grid(False)
     plt.xlabel("Reference (tokenized)", fontsize=14)
     plt.ylabel("Candidate (tokenized)", fontsize=14)
     title = "Similarity Matrix"
-    if rescale_with_baseline:
-        title += " (after Rescaling)"
     plt.title(title, fontsize=14)
 
     divider = make_axes_locatable(ax)
     cax = divider.append_axes("right", size="2%", pad=0.2)
     fig.colorbar(im, cax=cax)
 
     # Rotate the tick labels and set their alignment.
```

### Comparing `code_eval_score-0.1.0/code_eval_score/utils.py` & `code_eval_score-0.2.0/code_eval_score/utils.py`

 * *Files identical despite different names*

### Comparing `code_eval_score-0.1.0/setup.py` & `code_eval_score-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'code_eval_score'
 DESCRIPTION = 'Automated evaluation of generated code based on CodeBERT and CodeT5.'
 URL = 'https://github.com/Lizhmq/code-eval-score'
 EMAIL = 'lizhmq@pku.edu.cn'
 AUTHOR = 'Zhuo Li'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     'torch', 'torchvision', 'torchaudio', 'numpy',
     'transformers', 'scipy', 'pandas', 'pyemd'
 ]
```

