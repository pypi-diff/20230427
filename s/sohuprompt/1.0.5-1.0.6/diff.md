# Comparing `tmp/sohuprompt-1.0.5.tar.gz` & `tmp/sohuprompt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sohuprompt-1.0.5.tar", last modified: Tue Apr 25 11:26:09 2023, max compression
+gzip compressed data, was "sohuprompt-1.0.6.tar", last modified: Thu Apr 27 12:28:21 2023, max compression
```

## Comparing `sohuprompt-1.0.5.tar` & `sohuprompt-1.0.6.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:26:09.511956 sohuprompt-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-25 11:26:09.511956 sohuprompt-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6324 2023-04-25 02:49:09.000000 sohuprompt-1.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 11:26:09.512956 sohuprompt-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      724 2023-04-25 11:23:49.000000 sohuprompt-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:26:09.498956 sohuprompt-1.0.5/sohuprompt/
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-25 11:22:45.000000 sohuprompt-1.0.5/sohuprompt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:26:09.502956 sohuprompt-1.0.5/sohuprompt/data_utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:26:09.504956 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/closed_QA.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/coreference.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/entity_typing.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/generation.py
--rw-r--r--   0 root         (0) root         (0)     3857 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/nli.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/paraphrase.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/processor.py
--rw-r--r--   0 root         (0) root         (0)    16857 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/reading_comprehensation.py
--rw-r--r--   0 root         (0) root         (0)     4168 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/relation.py
--rw-r--r--   0 root         (0) root         (0)    11478 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/sentiment.py
--rw-r--r--   0 root         (0) root         (0)     3604 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/summarization.py
--rw-r--r--   0 root         (0) root         (0)     5336 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/data_utils/ZH/topic_classification.py
--rw-r--r--   0 root         (0) root         (0)     2884 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5039 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/conditional_generation_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5009 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/data_sampler.py
--rw-r--r--   0 root         (0) root         (0)    15671 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/fewglue_dataset.py
--rw-r--r--   0 root         (0) root         (0)    10269 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/huggingface_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5583 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/lama_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/nli_dataset.py
--rw-r--r--   0 root         (0) root         (0)    14301 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/relation_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)    16652 2023-04-25 02:48:15.000000 sohuprompt-1.0.5/sohuprompt/data_utils/text_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/typing_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11734 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/data_utils/utils.py
--rw-r--r--   0 root         (0) root         (0)    15913 2023-04-25 03:42:43.000000 sohuprompt-1.0.5/sohuprompt/default_config.py
--rw-r--r--   0 root         (0) root         (0)     8986 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/lm_bff_trainer.py
--rw-r--r--   0 root         (0) root         (0)    33757 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/pipeline_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:26:09.505956 sohuprompt-1.0.5/sohuprompt/plms/
--rw-r--r--   0 root         (0) root         (0)     7763 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/plms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:26:09.506956 sohuprompt-1.0.5/sohuprompt/plms/glm/
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/plms/glm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4119 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/plms/glm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/plms/glm/glm.py
--rw-r--r--   0 root         (0) root         (0)    56656 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/plms/glm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    15054 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/plms/glm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    17877 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/plms/glm/tokenization_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/plms/lm.py
--rw-r--r--   0 root         (0) root         (0)     3820 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/plms/mlm.py
--rw-r--r--   0 root         (0) root         (0)    17199 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/plms/seq2seq.py
--rw-r--r--   0 root         (0) root         (0)     9699 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/plms/utils.py
--rw-r--r--   0 root         (0) root         (0)    27881 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompt_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:26:09.510956 sohuprompt-1.0.5/sohuprompt/prompts/
--rw-r--r--   0 root         (0) root         (0)     3846 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11510 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/automatic_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8002 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/generation_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8815 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/knowledgeable_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/manual_template.py
--rw-r--r--   0 root         (0) root         (0)     9645 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/manual_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8620 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/mixed_template.py
--rw-r--r--   0 root         (0) root         (0)     8052 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/one2one_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)    12707 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/prefix_tuning_template.py
--rw-r--r--   0 root         (0) root         (0)    23406 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/prompt_generator.py
--rw-r--r--   0 root         (0) root         (0)    15008 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/prototypical_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     5266 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/ptr_prompts.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/ptuning_prompts.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/soft_template.py
--rw-r--r--   0 root         (0) root         (0)     9069 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/prompts/soft_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     6948 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/protoverb_trainer.py
--rw-r--r--   0 root         (0) root         (0)    31328 2023-04-25 11:19:17.000000 sohuprompt-1.0.5/sohuprompt/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:26:09.511956 sohuprompt-1.0.5/sohuprompt/utils/
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3866 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/utils/calibrate.py
--rw-r--r--   0 root         (0) root         (0)    10852 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/utils/crossfit_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/utils/cuda.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-04-22 09:08:12.000000 sohuprompt-1.0.5/sohuprompt/utils/logging.py
--rw-r--r--   0 root         (0) root         (0)     5906 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/utils/metrics.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/utils/reproduciblity.py
--rw-r--r--   0 root         (0) root         (0)     2592 2023-04-23 02:06:53.000000 sohuprompt-1.0.5/sohuprompt/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:26:09.499956 sohuprompt-1.0.5/sohuprompt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-25 11:26:09.000000 sohuprompt-1.0.5/sohuprompt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2614 2023-04-25 11:26:09.000000 sohuprompt-1.0.5/sohuprompt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:26:09.000000 sohuprompt-1.0.5/sohuprompt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-25 11:26:09.000000 sohuprompt-1.0.5/sohuprompt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-25 11:26:09.000000 sohuprompt-1.0.5/sohuprompt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.570380 sohuprompt-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-27 12:28:21.570380 sohuprompt-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6324 2023-04-27 12:25:38.000000 sohuprompt-1.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 12:28:21.570380 sohuprompt-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-27 12:24:04.000000 sohuprompt-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.563380 sohuprompt-1.0.6/sohuprompt/
+-rw-r--r--   0 root         (0) root         (0)      366 2023-04-27 12:24:19.000000 sohuprompt-1.0.6/sohuprompt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.565380 sohuprompt-1.0.6/sohuprompt/data_utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.566380 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/closed_QA.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/coreference.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/entity_typing.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/generation.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/nli.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/paraphrase.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/processor.py
+-rw-r--r--   0 root         (0) root         (0)    16857 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/reading_comprehensation.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/relation.py
+-rw-r--r--   0 root         (0) root         (0)    11478 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/sentiment.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/summarization.py
+-rw-r--r--   0 root         (0) root         (0)     5336 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/ZH/topic_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5039 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/conditional_generation_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5009 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/data_sampler.py
+-rw-r--r--   0 root         (0) root         (0)    15671 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/fewglue_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10269 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/huggingface_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/lama_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/nli_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14301 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/relation_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    16652 2023-04-26 03:20:48.000000 sohuprompt-1.0.6/sohuprompt/data_utils/text_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/typing_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11734 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/data_utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15913 2023-04-26 03:20:48.000000 sohuprompt-1.0.6/sohuprompt/default_config.py
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/lm_bff_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    33757 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/pipeline_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.567380 sohuprompt-1.0.6/sohuprompt/plms/
+-rw-r--r--   0 root         (0) root         (0)     7763 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.568380 sohuprompt-1.0.6/sohuprompt/plms/glm/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4119 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/glm.py
+-rw-r--r--   0 root         (0) root         (0)    56656 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    15054 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    17877 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/glm/tokenization_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/lm.py
+-rw-r--r--   0 root         (0) root         (0)     3820 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/mlm.py
+-rw-r--r--   0 root         (0) root         (0)    17199 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/seq2seq.py
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/plms/utils.py
+-rw-r--r--   0 root         (0) root         (0)    27881 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompt_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.569380 sohuprompt-1.0.6/sohuprompt/prompts/
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/automatic_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8002 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/generation_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8815 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/knowledgeable_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/manual_template.py
+-rw-r--r--   0 root         (0) root         (0)     9524 2023-04-26 03:24:53.000000 sohuprompt-1.0.6/sohuprompt/prompts/manual_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/mixed_template.py
+-rw-r--r--   0 root         (0) root         (0)     8052 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/one2one_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)    12707 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/prefix_tuning_template.py
+-rw-r--r--   0 root         (0) root         (0)    23406 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/prompt_generator.py
+-rw-r--r--   0 root         (0) root         (0)    15008 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/prototypical_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     5266 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/ptr_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/ptuning_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/prompts/soft_template.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2023-04-24 04:19:02.000000 sohuprompt-1.0.6/sohuprompt/prompts/soft_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/protoverb_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    31328 2023-04-26 04:32:13.000000 sohuprompt-1.0.6/sohuprompt/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.570380 sohuprompt-1.0.6/sohuprompt/utils/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/calibrate.py
+-rw-r--r--   0 root         (0) root         (0)    10852 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/crossfit_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/cuda.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-04-26 04:32:31.000000 sohuprompt-1.0.6/sohuprompt/utils/logging.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/reproduciblity.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-04-23 06:32:08.000000 sohuprompt-1.0.6/sohuprompt/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 12:28:21.564380 sohuprompt-1.0.6/sohuprompt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-27 12:28:21.000000 sohuprompt-1.0.6/sohuprompt.egg-info/top_level.txt
```

### Comparing `sohuprompt-1.0.5/README.md` & `sohuprompt-1.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   <a href="#预览">预览</a> •
   <a href="#安装">安装</a> •
   <a href="#快速开始">快速开始</a> 
 </p>
 
 </div>
 
-![version](https://img.shields.io/badge/version-v1.0.3-green)
+![version](https://img.shields.io/badge/version-v1.0.6-green)
 
 
 
 
 ## 新闻
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
  #
                  [https://s1.ax1x.com/2023/04/23/p9e0XDA.png]
                       é¢è§ â¢ å®è£ â¢ å¿«éå¼å§
-![version](https://img.shields.io/badge/version-v1.0.3-green) ## æ°é» -
+![version](https://img.shields.io/badge/version-v1.0.6-green) ## æ°é» -
 âï¸ 2023å¹´4æï¼çæ¬æ´æ°ï¼æ¯æ[ChatGLM](https://github.com/THUDM/
 ChatGLM-6B), å¯ä»¥ä½¿ç¨SohuPromptå·¥å·å¯¹ChatGLMè¿è¡å¾®è°ã -
 2023å¹´4æï¼SohuPrompt
 v1.0.1çæ¬åå¸ï¼æ¬¢è¿å¤§å®¶ä¸ºSohuPromptè´¡ç®ä»£ç ã ## é¢è§ Prompt-
 learningæ¯ææ°çè®­ç»èå¼ï¼å®å¯ä»¥å°é¢è®­ç»è¯­è¨æ¨¡åï¼PLMsï¼æ´å¥½çééä¸æ¸¸NLPä»»å¡ãSohuPromptåºæä¾äºä¸ä¸ªæ åãçµæ´»åå¯æ©å±çæ¡æ¶ï¼ç¨äºé¨ç½²prompt-
 learningæµæ°´çº¿ï¼å®æ¯æç´æ¥ä»[huggingface transformers](https://
 github.com/huggingface/transformers)å è½½PLMsãå¨æªæ¥ï¼æä»¬å°æ¯æ
```

### Comparing `sohuprompt-1.0.5/setup.py` & `sohuprompt-1.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(name='sohuprompt',
-        version='1.0.5',
+        version='1.0.6',
         packages=find_packages(),  # 查找包的路径
         # package_dir={'': 'src'},  # 包的root路径映射到的实际路径
         # include_package_data=False,
         # package_data={'data': []},
         description='A python lib for sohuprompt',
         # long_description='',
         author='senhaowang,chencheng',
         author_email='senhaowang@sohu-inc.com',
         # url='http://www.xxxxx.com/',  # homepage
         license='MIT',
-        install_requires=['transformers', 'torch', 'numpy', 'pandas', 'tqdm', 'sklearn', 'jieba', 'tensorboardX', 'icetk', 'yacs', 'rouge'],
+        install_requires=['transformers', 'torch', 'numpy', 'pandas', 'tqdm', 'scikit-learn', 'jieba', 'tensorboard==2.9.0', 'icetk', 'yacs', 'rouge', 'openpyxl'],
         )
```

### Comparing `sohuprompt-1.0.5/sohuprompt/config.py` & `sohuprompt-1.0.6/sohuprompt/config.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/closed_QA.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/closed_QA.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/coreference.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/coreference.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/entity_typing.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/entity_typing.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/generation.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/generation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/nli.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/nli.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/paraphrase.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/paraphrase.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/reading_comprehensation.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/reading_comprehensation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/relation.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/relation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/sentiment.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/sentiment.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/summarization.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/summarization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/ZH/topic_classification.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/ZH/topic_classification.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/__init__.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/conditional_generation_dataset.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/conditional_generation_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/data_processor.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/data_processor.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/data_sampler.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/data_sampler.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/fewglue_dataset.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/fewglue_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/huggingface_dataset.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/huggingface_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/lama_dataset.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/lama_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/nli_dataset.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/nli_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/relation_classification_dataset.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/relation_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/text_classification_dataset.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/typing_dataset.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/typing_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/data_utils/utils.py` & `sohuprompt-1.0.6/sohuprompt/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/default_config.py` & `sohuprompt-1.0.6/sohuprompt/default_config.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/lm_bff_trainer.py` & `sohuprompt-1.0.6/sohuprompt/lm_bff_trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/pipeline_base.py` & `sohuprompt-1.0.6/sohuprompt/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/__init__.py` & `sohuprompt-1.0.6/sohuprompt/plms/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/glm/configuration_chatglm.py` & `sohuprompt-1.0.6/sohuprompt/plms/glm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/glm/glm.py` & `sohuprompt-1.0.6/sohuprompt/plms/glm/glm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/glm/modeling_chatglm.py` & `sohuprompt-1.0.6/sohuprompt/plms/glm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/glm/quantization.py` & `sohuprompt-1.0.6/sohuprompt/plms/glm/quantization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/glm/tokenization_chatglm.py` & `sohuprompt-1.0.6/sohuprompt/plms/glm/tokenization_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/lm.py` & `sohuprompt-1.0.6/sohuprompt/plms/lm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/mlm.py` & `sohuprompt-1.0.6/sohuprompt/plms/mlm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/seq2seq.py` & `sohuprompt-1.0.6/sohuprompt/plms/seq2seq.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/plms/utils.py` & `sohuprompt-1.0.6/sohuprompt/plms/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompt_base.py` & `sohuprompt-1.0.6/sohuprompt/prompt_base.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/__init__.py` & `sohuprompt-1.0.6/sohuprompt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/automatic_verbalizer.py` & `sohuprompt-1.0.6/sohuprompt/prompts/automatic_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/generation_verbalizer.py` & `sohuprompt-1.0.6/sohuprompt/prompts/generation_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/knowledgeable_verbalizer.py` & `sohuprompt-1.0.6/sohuprompt/prompts/knowledgeable_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/manual_template.py` & `sohuprompt-1.0.6/sohuprompt/prompts/manual_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/manual_verbalizer.py` & `sohuprompt-1.0.6/sohuprompt/prompts/manual_verbalizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,15 @@
         r"""In basic manual template, the parameters are generated from label words directly.
         In this implementation, the label_words should not be tokenized into more than one token.
         """
         all_ids = []
         for words_per_label in self.label_words:
             ids_per_label = []
             for word in words_per_label:
-                print('word',word)
-                print(self.tokenizer.tokenize(word))
                 ids = self.tokenizer.encode(word, add_special_tokens=False)
-                print('ids',ids)
                 ids_per_label.append(ids)
             all_ids.append(ids_per_label)
 
         max_len  = max([max([len(ids) for ids in ids_per_label]) for ids_per_label in all_ids])
         max_num_label_words = max([len(ids_per_label) for ids_per_label in all_ids])
         words_ids_mask = torch.zeros(max_num_label_words, max_len)
         words_ids_mask = [[[1]*len(ids) + [0]*(max_len-len(ids)) for ids in ids_per_label]
```

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/mixed_template.py` & `sohuprompt-1.0.6/sohuprompt/prompts/mixed_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/one2one_verbalizer.py` & `sohuprompt-1.0.6/sohuprompt/prompts/one2one_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/prefix_tuning_template.py` & `sohuprompt-1.0.6/sohuprompt/prompts/prefix_tuning_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/prompt_generator.py` & `sohuprompt-1.0.6/sohuprompt/prompts/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/prototypical_verbalizer.py` & `sohuprompt-1.0.6/sohuprompt/prompts/prototypical_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/ptr_prompts.py` & `sohuprompt-1.0.6/sohuprompt/prompts/ptr_prompts.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/ptuning_prompts.py` & `sohuprompt-1.0.6/sohuprompt/prompts/ptuning_prompts.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/soft_template.py` & `sohuprompt-1.0.6/sohuprompt/prompts/soft_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/prompts/soft_verbalizer.py` & `sohuprompt-1.0.6/sohuprompt/prompts/soft_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/protoverb_trainer.py` & `sohuprompt-1.0.6/sohuprompt/protoverb_trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/trainer.py` & `sohuprompt-1.0.6/sohuprompt/trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/utils/calibrate.py` & `sohuprompt-1.0.6/sohuprompt/utils/calibrate.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/utils/crossfit_metrics.py` & `sohuprompt-1.0.6/sohuprompt/utils/crossfit_metrics.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/utils/cuda.py` & `sohuprompt-1.0.6/sohuprompt/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/utils/logging.py` & `sohuprompt-1.0.6/sohuprompt/utils/logging.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/utils/metrics.py` & `sohuprompt-1.0.6/sohuprompt/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt/utils/utils.py` & `sohuprompt-1.0.6/sohuprompt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.5/sohuprompt.egg-info/SOURCES.txt` & `sohuprompt-1.0.6/sohuprompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

