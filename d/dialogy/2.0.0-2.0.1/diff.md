# Comparing `tmp/dialogy-2.0.0.tar.gz` & `tmp/dialogy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-2.0.0.tar", max compression
+gzip compressed data, was "dialogy-2.0.1.tar", max compression
```

## Comparing `dialogy-2.0.0.tar` & `dialogy-2.0.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1069 2023-04-27 06:36:23.963614 dialogy-2.0.0/LICENSE.md
--rw-r--r--   0        0        0        0 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9794 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15324 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     5017 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     2011 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/registry.py
--rw-r--r--   0        0        0        0 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     3995 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8868 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3790 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11805 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1179 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    17162 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7676 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    39327 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20334 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12300 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      743 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1792 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14123 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11523 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4699 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4247 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4148 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7338 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2281 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4317 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      975 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/__init__.py
--rw-r--r--   0        0        0    10448 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/config.py
--rw-r--r--   0        0        0     2180 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2687 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     6845 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1426 2023-04-27 06:36:51.803247 dialogy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 dialogy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 10:07:11.700619 dialogy-2.0.1/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9794 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15288 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     5017 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     2011 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/registry.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     3995 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8868 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3790 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11805 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1179 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    17162 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7676 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    39327 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20334 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12300 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1792 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14123 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11523 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4699 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     1565 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4247 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4148 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7338 2023-04-27 10:07:11.700619 dialogy-2.0.1/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2281 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4317 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      975 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0    10469 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/utils/config.py
+-rw-r--r--   0        0        0     2180 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2687 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     6795 2023-04-27 10:07:11.704620 dialogy-2.0.1/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1426 2023-04-27 10:07:30.825827 dialogy-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 dialogy-2.0.1/PKG-INFO
```

### Comparing `dialogy-2.0.0/LICENSE.md` & `dialogy-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/base/entity_extractor/__init__.py` & `dialogy-2.0.1/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/base/input/__init__.py` & `dialogy-2.0.1/dialogy/base/input/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/base/output/__init__.py` & `dialogy-2.0.1/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/base/plugin/__init__.py` & `dialogy-2.0.1/dialogy/base/plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         :type input: Input
         :param output: The workflow's output.
         :type output: Output
         :return: The value returned by the plugin.
         :rtype: Any
         """
 
-    def __call__(self, input, output, project_name: Optional[str] = None):  # type: ignore
+    def __call__(self, input, output):  # type: ignore
         """
         Set workflow with output.
 
         This important book-keeping method is called by the workflow.
 
         - If the plugin guards evaluate to :code:`True`, we don't run the plugin's business logic.
         - Otherwise, we obtain the plugins transformation and set it on :code:`self.dest` path within the workflow.
```

### Comparing `dialogy-2.0.0/dialogy/cli/__init__.py` & `dialogy-2.0.1/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/cli/project.py` & `dialogy-2.0.1/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/cli/workflow.py` & `dialogy-2.0.1/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/constants/__init__.py` & `dialogy-2.0.1/dialogy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/registry.py` & `dialogy-2.0.1/dialogy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/address_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-2.0.1/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/address_parser/maps.py` & `dialogy-2.0.1/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/calibration/xgb.py` & `dialogy-2.0.1/dialogy/plugins/text/calibration/xgb.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/classification/mlp.py` & `dialogy-2.0.1/dialogy/plugins/text/classification/mlp.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-2.0.1/dialogy/plugins/text/classification/retain_intent.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/classification/xlmr.py` & `dialogy-2.0.1/dialogy/plugins/text/classification/xlmr.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-2.0.1/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-2.0.1/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-2.0.1/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-2.0.1/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/oos_filter/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/oos_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-2.0.1/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-2.0.1/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/__init__.py` & `dialogy-2.0.1/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/address/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/base_entity/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/base_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/deserialize/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/duration/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/keyword/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/numerical/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/people/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/pincode/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/time/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/entity/time_interval/__init__.py` & `dialogy-2.0.1/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/intent/__init__.py` & `dialogy-2.0.1/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/types/slots/__init__.py` & `dialogy-2.0.1/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/utils/__init__.py` & `dialogy-2.0.1/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/utils/config.py` & `dialogy-2.0.1/dialogy/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,33 +29,37 @@
                 raise ValueError(f"Fetching {attribute} from config failed.")
         else:
             return vars(self).get(attribute)
 
 
 @attr.s
 class Task(BaseConfig):
-    use: bool = attr.ib(
+    use = attr.ib(
         type=bool, kw_only=True, validator=attr.validators.instance_of(bool)
     )
-    threshold: float = attr.ib(
+    threshold = attr.ib(
         type=float, kw_only=True, validator=attr.validators.instance_of(float)
     )
-    model_args: Dict[str, Any] = attr.ib(
-        type=dict, kw_only=True, validator=attr.validators.instance_of(dict)
+    model_args = attr.ib(
+        type=Dict[Any, Any], kw_only=True, validator=attr.validators.instance_of(dict)
     )
-    alias: Dict[str, Any] = attr.ib(
+    alias = attr.ib(
+        type=Dict[Any, Any],
         factory=dict, kw_only=True, validator=attr.validators.instance_of(dict)
     )
-    skip: List[str] = attr.ib(
+    skip = attr.ib(
+        type=List[Any],
         factory=list, kw_only=True, validator=attr.validators.instance_of(list)
     )
-    confidence_levels: List[float] = attr.ib(
+    confidence_levels = attr.ib(
+        type=List[Any],
         factory=list, kw_only=True, validator=attr.validators.instance_of(list)
     )
-    format: Optional[str] = attr.ib(
+    format = attr.ib(
+        type=str,
         factory=str,
         kw_only=True,
         validator=attr.validators.optional(attr.validators.instance_of(str)),
     )
 
     def update_paths(self, project_config_path: str) -> None:
         for purpose in self.model_args:
```

### Comparing `dialogy-2.0.0/dialogy/utils/datetime.py` & `dialogy-2.0.1/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/utils/file_handler.py` & `dialogy-2.0.1/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/utils/logger.py` & `dialogy-2.0.1/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/utils/misc.py` & `dialogy-2.0.1/dialogy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/utils/naive_lang_detect.py` & `dialogy-2.0.1/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/utils/normalize_utterance.py` & `dialogy-2.0.1/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/utils/temperature_scaling.py` & `dialogy-2.0.1/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.0/dialogy/workflow/workflow.py` & `dialogy-2.0.1/dialogy/workflow/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         Post init hook.
         """
         self.lock = Lock()
         for plugin in self.plugins:
             if isinstance(plugin, Plugin):
                 plugin.debug = self.debug & plugin.debug
 
-    def run(self, input: Input, output: Output = None, project_name: Optional[str] = None):  # type: ignore
+    def run(self, input: Input, output: Output = None):  # type: ignore
         """
         .. _workflow_run:
 
         Get final results from the workflow.
 
         The current workflow exhibits the following simple procedure:
         pre-processing -> inference -> post-processing.
@@ -203,15 +203,15 @@
                         "input": input.dict(),
                         "output": output.dict(),
                     },
                 }
 
             start = time.perf_counter()
             with self.lock:
-                input, output = plugin(input, output, project_name)
+                input, output = plugin(input, output)
             end = time.perf_counter()
 
             # logs are available only when debug=False during class initialization
             if self.debug:
                 history["after"] = {
                     "input": input.dict(),
                     "output": output.dict(),
```

### Comparing `dialogy-2.0.0/pyproject.toml` & `dialogy-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialogy"
-version = "2.0.0"
+version = "2.0.1"
 description = "Dialogy is a library for building and managing SLU applications."
 authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `dialogy-2.0.0/PKG-INFO` & `dialogy-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

