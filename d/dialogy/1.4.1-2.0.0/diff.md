# Comparing `tmp/dialogy-1.4.1.tar.gz` & `tmp/dialogy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-1.4.1.tar", max compression
+gzip compressed data, was "dialogy-2.0.0.tar", max compression
```

## Comparing `dialogy-1.4.1.tar` & `dialogy-2.0.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0     1069 2023-04-21 05:36:54.194576 dialogy-1.4.1/LICENSE.md
--rw-r--r--   0        0        0        0 2023-04-21 05:36:54.194576 dialogy-1.4.1/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-04-21 05:36:54.194576 dialogy-1.4.1/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-04-21 05:36:54.194576 dialogy-1.4.1/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9794 2023-04-21 05:36:54.194576 dialogy-1.4.1/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-21 05:36:54.194576 dialogy-1.4.1/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15185 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     4676 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     1203 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     3995 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8825 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3746 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11821 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1142 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    13953 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7633 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    39284 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20312 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12300 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      743 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1740 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14080 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11480 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4656 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4204 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4111 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7338 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2281 2023-04-21 05:36:54.198577 dialogy-1.4.1/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4317 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      975 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/utils/__init__.py
--rw-r--r--   0        0        0     2180 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2687 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     6795 2023-04-21 05:36:54.202576 dialogy-1.4.1/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1400 2023-04-21 05:37:18.242654 dialogy-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 dialogy-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 06:36:23.963614 dialogy-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9794 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15324 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     5017 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     2011 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/registry.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     3995 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8868 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3790 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11805 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1179 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2023-04-27 06:36:23.963614 dialogy-2.0.0/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    17162 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7676 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    39327 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20334 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12300 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1792 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14123 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11523 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4699 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     1565 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4247 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4148 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7338 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2281 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4317 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      975 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0    10448 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/config.py
+-rw-r--r--   0        0        0     2180 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2687 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     6845 2023-04-27 06:36:23.967614 dialogy-2.0.0/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1426 2023-04-27 06:36:51.803247 dialogy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 dialogy-2.0.0/PKG-INFO
```

### Comparing `dialogy-1.4.1/LICENSE.md` & `dialogy-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/base/entity_extractor/__init__.py` & `dialogy-2.0.0/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/base/input/__init__.py` & `dialogy-2.0.0/dialogy/base/input/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/base/output/__init__.py` & `dialogy-2.0.0/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/base/plugin/__init__.py` & `dialogy-2.0.0/dialogy/base/plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,22 +195,21 @@
     :code:`replace_output=True`.
 
 """
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any, Callable, List, Optional
-
 import dialogy.constants as const
 from dialogy.base.input import Input
 from dialogy.base.output import Output
 from dialogy.utils.logger import logger
 
 
-Guard = Callable[[Input, Output], bool]
+Guard = Callable[[Input, Output, str], bool]
 
 
 class Plugin(ABC):
     """
     Abstract class to be implemented by all plugins.
 
     :param input_column: Transforms data in this column for a given dataframe, defaults to const.ALTERNATIVES
@@ -233,22 +232,24 @@
         output_column: Optional[str] = None,
         use_transform: bool = False,
         replace_output: bool = False,
         dest: Optional[str] = None,
         guards: Optional[List[Guard]] = None,
         debug: bool = False,
         dynamic_output_path: bool = False,
+        **kwargs: Any
     ) -> None:
         self.debug = debug
         self.guards = guards
         self.dest = dest
         self.replace_output = replace_output
         self.input_column = input_column
         self.output_column = output_column or input_column
         self.use_transform = use_transform
+        self.purpose = kwargs.pop("purpose", const.PRODUCTION)
         self.dynamic_output_path = dynamic_output_path
 
     @abstractmethod
     def utility(self, input_: Input, output: Output) -> Any:
         """
         An abstract method that describes the plugin's functionality.
 
@@ -256,15 +257,15 @@
         :type input: Input
         :param output: The workflow's output.
         :type output: Output
         :return: The value returned by the plugin.
         :rtype: Any
         """
 
-    def __call__(self, input, output):  # type: ignore
+    def __call__(self, input, output, project_name: Optional[str] = None):  # type: ignore
         """
         Set workflow with output.
 
         This important book-keeping method is called by the workflow.
 
         - If the plugin guards evaluate to :code:`True`, we don't run the plugin's business logic.
         - Otherwise, we obtain the plugins transformation and set it on :code:`self.dest` path within the workflow.
@@ -366,15 +367,15 @@
         .. _Guards:
 
         :return: prevent plugin execution if True.
         :rtype: bool
         """
         if not self.guards:
             return False
-        return any(guard(input_, output) for guard in self.guards)
+        return any(guard(input_, output, self.purpose) for guard in self.guards)
 
     def train(self, _: Any) -> Any:
         """
         Train a plugin.
         """
         return None
```

### Comparing `dialogy-1.4.1/dialogy/cli/__init__.py` & `dialogy-2.0.0/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/cli/project.py` & `dialogy-2.0.0/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/cli/workflow.py` & `dialogy-2.0.0/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/constants/__init__.py` & `dialogy-2.0.0/dialogy/constants/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -202,7 +202,19 @@
 TEXT = "text"
 CANONICALIZED_TRANSCRIPTS = "canonicalized_transcripts"
 REFERENCE_TIME = "reftime"
 ENTITY_COLUMN = "entities"
 
 FUZZY_DP = "fuzzy_dp"
 ENTITY_VALUE_TOKEN = "__value__"
+
+OUTPUT_DIR = "output_dir"
+BEST_MODEL_DIR = "best_model_dir"
+BEST_MODEL = BEST_MODEL_DIR
+MODELS = "models"
+METRICS = "metrics"
+DATASETS = "datasets"
+CLASSIFICATION = "classification"
+EPOCHS = "epochs"
+PIPELINE_CONFIG_FILE = "pipeline_config.yaml"
+CORE_PLUGINS_CONFIG_FILE = "core_plugins_config.yaml"
+MODEL_CONFIG_FILE = "model_config.yaml"
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/address_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-2.0.0/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/plugins/text/address_parser/maps.py` & `dialogy-2.0.0/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/plugins/text/calibration/xgb.py` & `dialogy-2.0.0/dialogy/plugins/text/calibration/xgb.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,22 +98,24 @@
         dest: Optional[str] = None,
         guards: Optional[List[Guard]] = None,
         debug: bool = False,
         input_column: str = const.ALTERNATIVES,
         output_column: Optional[str] = const.ALTERNATIVES,
         use_transform: bool = False,
         model_name: str = "calibration.pkl",
+        **kwargs: Any
     ) -> None:
         super().__init__(
             dest=dest,
             guards=guards,
             debug=debug,
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
+            **kwargs
         )
         self.extraction_pipeline = FeatureExtractor()
         self.clf = XGBRegressor(n_jobs=1)
         self.threshold = threshold
         self.model_name = model_name
 
     def train(self, df: pd.DataFrame) -> None:
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,24 @@
         guards: Optional[List[Guard]] = None,
         entity_column: str = const.ENTITY_COLUMN,
         input_column: str = const.ALTERNATIVES,
         output_column: Optional[str] = None,
         use_transform: bool = False,
         threshold: float = 0.0,
         debug: bool = False,
+        **kwargs: Any,
     ) -> None:
         super().__init__(
             dest=dest,
             guards=guards,
             debug=debug,
             use_transform=use_transform,
             input_column=input_column,
             output_column=output_column,
+            **kwargs
         )
         self.mask = mask
         self.mask_tokens = mask_tokens or []
         self._mask_patterns: List[re.Pattern[str]] = [
             re.compile(r"\b%s\b" % token, re.I | re.U) for token in self.mask_tokens
         ]
         self.serializer = serializer
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/classification/mlp.py` & `dialogy-2.0.0/dialogy/plugins/text/classification/mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         score_round_off: int = 5,
         purpose: str = const.TRAIN,
         fallback_label: str = const.ERROR_LABEL,
         data_column: str = const.DATA,
         label_column: str = const.LABELS,
         args_map: Optional[Dict[str, Any]] = None,
         skip_labels: Optional[List[str]] = None,
-        kwargs: Optional[Dict[str, Any]] = None,
+        **kwargs: Any,
     ) -> None:
 
-        super().__init__(dest=dest, guards=guards, debug=debug)
+        super().__init__(dest=dest, guards=guards, debug=debug, **kwargs)
         self.model_pipeline: Any = None
         self.fallback_label = fallback_label
         self.data_column = data_column
         self.label_column = label_column
         self.mlp_model_path = os.path.join(model_dir, const.MLPMODEL_FILE)
         self.threshold = threshold
         self.skip_labels = set(skip_labels or set())
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-2.0.0/dialogy/plugins/text/classification/retain_intent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 .. _RetainOriginalIntentPlugin:
 
 We may apply transforms over predicted intents. This makes it hard to track the impact of classifiers. 
 Here, we will track the original intent, the one produced by a classifier.
 """
-from typing import List, Optional
+from typing import List, Optional, Any
 
 from dialogy import constants as const
 from dialogy.base import Guard, Input, Output, Plugin
 from dialogy.base.output import ORIGINAL_INTENT_TYPE
 from dialogy.types import Intent
 
 
 class RetainOriginalIntentPlugin(Plugin):
     def __init__(
         self,
         replace_output: bool = False,
         dest: Optional[str] = "output.original_intent",
         guards: Optional[List[Guard]] = None,
         debug: bool = False,
+        **kwargs: Any
     ) -> None:
         super().__init__(
-            replace_output=replace_output, dest=dest, guards=guards, debug=debug
+            replace_output=replace_output, dest=dest, guards=guards, debug=debug, **kwargs
         )
 
     def retain(self, intents: List[Intent]) -> ORIGINAL_INTENT_TYPE:
         if not intents:
             return {}
 
         intent, *_ = intents
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/classification/xlmr.py` & `dialogy-2.0.0/dialogy/plugins/text/classification/xlmr.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,169 +3,232 @@
 
 This module provides a trainable XLMR classifier.
 [read-more](https://arxiv.org/abs/1911.02116)
 """
 import importlib
 import os
 import pickle
-import random
-from typing import Any, Dict, List, Optional
+import requests
+from typing import Any, Dict, List, Optional, Tuple
+from pprint import pformat
 
 import numpy as np
 import pandas as pd
 from sklearn import preprocessing
 from tqdm import tqdm
 
 import dialogy.constants as const
 from dialogy.base import Guard, Input, Output, Plugin
 from dialogy.types import Intent
 from dialogy.utils import load_file, logger, read_from_json, save_file
+import torch
 from torch.profiler import profile, record_function, ProfilerActivity
 
 
 class XLMRMultiClass(Plugin):
     """
     This plugin provides a classifier based on `XLM-Roberta <https://arxiv.org/abs/1911.02116>`.
 
     .. _XLMRMultiClass:
     The use_state flag in the XLMRMultiClass plugin is used to enable the use of state variable as the part of the text input.
     """
 
     def __init__(
         self,
-        model_dir: str,
         dest: Optional[str] = None,
+        timeout: float = 0.5,
+        url: str = "http://0.0.0.0:8000/",
         guards: Optional[List[Guard]] = None,
         debug: bool = False,
         threshold: float = 0.1,
-        use_cuda: bool = False,
         score_round_off: int = 5,
-        purpose: str = const.TRAIN,
         fallback_label: str = const.ERROR_LABEL,
         use_state: bool = False,
         data_column: str = const.DATA,
         label_column: str = const.LABELS,
         state_column: str = const.STATE,
         lang_column: str = const.LANG,
         nls_label_column: str = const.NLS_LABEL,
         args_map: Optional[Dict[str, Any]] = None,
         skip_labels: Optional[List[str]] = None,
         prompts_map: Dict[Any, Any] = {const.LANG: []},
         use_prompt: bool = False,
         null_prompt_token: str = const.NULL_PROMPT_TOKEN,
-        kwargs: Optional[Dict[str, Any]] = None,
+        **kwargs: Any,
     ) -> None:
-        try:
-            classifer = getattr(
-                importlib.import_module(const.XLMR_MODULE), const.XLMR_MULTI_CLASS_MODEL
-            )
-        except ModuleNotFoundError as error:
-            raise ModuleNotFoundError(
-                "Plugin requires simpletransformers -- https://simpletransformers.ai/docs/installation/"
-            ) from error
-
-        super().__init__(dest=dest, guards=guards, debug=debug)
-        self.labelencoder = preprocessing.LabelEncoder()
-        self.classifier = classifer
-        self.model: Any = None
-        self.model_dir = model_dir
+        super().__init__(dest=dest, guards=guards, debug=debug, **kwargs)
         self.fallback_label = fallback_label
         self.data_column = data_column
         self.label_column = label_column
         self.state_column = state_column
         self.lang_column = lang_column
         self.nls_label_column = nls_label_column
-        self.use_cuda = use_cuda
         self.use_state = use_state
         self.use_prompt = use_prompt
         self.null_prompt_token = null_prompt_token
         self.prompts_map = prompts_map
-
-        self.labelencoder_file_path = os.path.join(
-            self.model_dir, const.LABELENCODER_FILE
-        )
-        self.ts_parameter: float = (
-            read_from_json(
-                [const.TS_PARAMETER], model_dir, const.CALIBRATION_CONFIG_FILE
-            ).get(const.TS_PARAMETER)
-            or 1.0
-        )
-
-        self.threshold = threshold
         self.skip_labels = set(skip_labels or set())
-        self.purpose = purpose
+        self.threshold = threshold
         self.round = score_round_off
-        if args_map and (
-            const.TRAIN not in args_map
-            or const.TEST not in args_map
-            or const.PRODUCTION not in args_map
-        ):
+
+        if not args_map and self.purpose != const.PRODUCTION:
             raise ValueError(
-                f"Attempting to set invalid {args_map}. "
-                f"It is missing some of {const.TRAIN}, {const.TEST}, {const.PRODUCTION} in configs."
-            )
-        self.args_map = args_map
-        self.kwargs = kwargs or {}
-        try:
-            if os.path.exists(self.labelencoder_file_path):
-                self.init_model()
-        except EOFError:
-            logger.error(
-                f"Plugin {self} Failed to load labelencoder from {self.labelencoder_file_path}. "
-                "Ignore this message if you are training but if you are using this in production or testing, then this is serious!"
+                f"args_map was set to None with purpose={self.purpose} which is not allowed."
             )
+        if args_map and self.purpose not in args_map:
+            raise ValueError(
+                f"Attempting to set invalid `args_map`. "
+                f"It is missing {self.purpose}. `purpose` has to be one of "
+                f"{const.TRAIN}, {const.TEST}, {const.PRODUCTION} in configs."
+            )
+        if args_map:
+            self.args_map = args_map[self.purpose]
+        else:
+            self.args_map = {}
+
+        self.use_calibration = self.args_map.get(const.MODEL_CALIBRATION, False)
+
+        self.ts_parameter: float = self.args_map.get("ts_parameter") or 1.0
+
+        # flag that specifies whether plugin is being imported externally solely for model
+        imported = kwargs.get("imported", False)
+
+        if self.purpose in [const.TRAIN, const.TEST] or imported:
+            self.use_cuda = torch.cuda.is_available()
+            try:
+                classifer = getattr(
+                    importlib.import_module(const.XLMR_MODULE), const.XLMR_MULTI_CLASS_MODEL
+                )
+            except ModuleNotFoundError as error:
+                raise ModuleNotFoundError(
+                    "Plugin requires simpletransformers -- https://simpletransformers.ai/docs/installation/"
+                ) from error
+
+            self.model_dir = self.args_map.get("best_model_dir")
+            if not self.model_dir:
+                raise ValueError(
+                    f"'best_model_dir' missing in passed args_map."
+                )
+            
+            self.labelencoder = preprocessing.LabelEncoder()
+            self.classifier = classifer
+            self.model: Any = None
+
+            self.labelencoder_file_path = os.path.join(
+                self.model_dir, const.LABELENCODER_FILE
+            )
+
+            self.kwargs = kwargs or {}
+
+            # TODO: check if this can be avoided
+            if "name" in self.kwargs:
+                del self.kwargs["name"]
+            if "imported" in self.kwargs:
+                del self.kwargs["imported"]
+
+            try:
+                if os.path.exists(self.labelencoder_file_path):
+                    logger.debug(f"initializing label encoder file from {self.labelencoder_file_path}")
+                    self.init_model()
+            except EOFError:
+                logger.error(
+                    f"Plugin {self} Failed to load labelencoder from {self.labelencoder_file_path}. "
+                    "Ignore this message if you are training but if you are using this in "
+                    "production or testing, then this should be checked!"
+                )
+
+        elif self.purpose == const.PRODUCTION:
+            # model inference service session configuration
+            self.url = url
+            self.timeout = timeout
+            self.session = requests.Session()
+            self.session.mount(
+                "http://",
+                requests.adapters.HTTPAdapter(
+                    max_retries=1, pool_maxsize=10, pool_block=True
+                ),
+            )
+            self.headers: Dict[str, str] = {
+                "Content-Type": "application/json"
+            }
+
         self.debug = debug
 
     def init_model(self, label_count: Optional[int] = None) -> None:
         """
         Initialize the model if artifacts are available.
-
         :param label_count: number of labels to train on or predict, defaults to None
         :type label_count: Optional[int], optional
         :raises ValueError: In case n is not provided or can't be calculated.
         """
-        model_dir = const.XLMR_MODEL_TIER
         if os.path.exists(self.labelencoder_file_path):
             self.load()
             label_count = len(self.labelencoder.classes_)
-            model_dir = self.model_dir
         if not label_count:
             raise ValueError(
                 f"Plugin {self} needs either the training data "
                 "or an existing labelencoder to initialize."
             )
-        args = (
-            self.args_map[self.purpose]
-            if self.args_map and self.purpose in self.args_map
-            else {}
-        )
-        self.use_calibration = args.get(const.MODEL_CALIBRATION)
+
         try:
+            logger.debug(f"loading model weights from {self.model_dir}")
             self.model = self.classifier(
                 const.XLMR_MODEL,
-                model_dir,
+                self.model_dir,
                 num_labels=label_count,
                 use_cuda=self.use_cuda,
-                args=args,
+                args=self.args_map,
                 **self.kwargs,
             )
         except OSError:
+            logger.info(f"Model not found at {self.model_dir}. "
+                        f"Default model weights will be loaded")
             self.model = self.classifier(
                 const.XLMR_MODEL,
                 const.XLMR_MODEL_TIER,
                 num_labels=label_count,
                 use_cuda=self.use_cuda,
-                args=args,
+                args=self.args_map,
                 **self.kwargs,
             )
 
     @property
     def valid_labelencoder(self) -> bool:
         return hasattr(self.labelencoder, "classes_")
 
+    def _request_model_inference(self, texts: List[str]) -> Tuple[Any, Any]:
+        payload = {"transcripts": texts}
+
+        try:
+            response = self.session.post(
+                self.url, json=payload, headers=self.headers, timeout=self.timeout
+            )
+
+            if response.status_code == 200:
+                # The API call was successful, expect the following to contain entities.
+                # A list of dicts or an empty list.
+                result = response.json()
+                return result.get("intents", []), result.get("logits", [])
+            
+        except requests.exceptions.Timeout as timeout_exception:
+            logger.error(f"Model Inference Service timed out: {timeout_exception}")  # pragma: no cover
+            logger.error(pformat(payload))  # pragma: no cover
+            return [], []  # pragma: no cover
+        
+        except requests.exceptions.ConnectionError as connection_error:
+            logger.error(f"Model Inference Service is turned off?: {connection_error}")
+            logger.error(pformat(payload))
+            raise requests.exceptions.ConnectionError from connection_error
+
+        # Control flow reaching here would mean the API call wasn't successful.
+        # To prevent rest of the things from crashing, we will raise an exception.
+        raise ValueError(
+            f"Model Inference Service API call failed | [{response.status_code}]: {response.text}"
+        )
+
     def inference(
         self,
         texts: Optional[List[str]],
         state: Optional[str] = None,
         lang: Optional[str] = None,
         nls_label: Optional[str] = None,
     ) -> List[Intent]:
@@ -179,22 +242,17 @@
         :type texts: List[str]
         :type state: List[str]
         :raises AttributeError: In case the labelencoder is not available.
         :return: A list of intents corresponding to texts.
         :rtype: List[Intent]
         """
 
+        # validation
         fallback_output = Intent(name=self.fallback_label, score=1.0).add_parser(self)
-
         if not texts:
-            logger.error(f"texts passed to model {texts}!")
-            return [fallback_output]
-
-        if self.model is None:
-            logger.error(f"No model found for plugin {self.__class__.__name__}!")
             return [fallback_output]
 
         if self.use_state and not state:
             raise ValueError(
                 f"Plugin {self.__class__.__name__} requires state to be passed to the model."
             )
 
@@ -204,43 +262,54 @@
             )
 
         if self.use_prompt and not lang:
             raise ValueError(
                 f"In order to use prompts as feature, Plugin {self.__class__.__name__} is requires lang to be passed to the model."
             )
 
+        # preprocessing
         if self.use_prompt and nls_label:
             texts[0] += "<s> " + self.lookup_prompt(lang, nls_label) + " </s>"
 
         if self.use_state and state:
             texts[0] += "<s> " + state + " </s>"
 
-        if not self.valid_labelencoder:
-            raise AttributeError(
-                "Seems like you forgot to "
-                f"save the {self.__class__.__name__} plugin."
-            )
-
         logger.debug(f"Classifier Input:\n{texts}")
 
-        predictions, logits = self.model.predict(texts)
-
-        if not predictions:
-            return [fallback_output]
+        # inference
+        if self.purpose == const.PRODUCTION:
+            predicted_intents, logits = self._request_model_inference(texts)
+            # postprocessing
+            logits = np.array(logits)
+
+        elif self.purpose == const.TEST:
+            if not self.model:
+                return [fallback_output]
+            predictions, logits = self.model.predict(texts)
+            if not predictions:
+                return [fallback_output]
+
+        else:
+            raise RuntimeError(f"Inference method called with purpose "
+                               f"set to '{self.purpose}'. Valid "
+                               f"values - [{const.PRODUCTION}, {const.TEST}]")
 
         logits = logits / self.ts_parameter
         confidence_scores = [np.exp(logit) / sum(np.exp(logit)) for logit in logits]
         intents_confidence_order = np.argsort(confidence_scores)[0][::-1]
-        predicted_intents = self.labelencoder.inverse_transform(
-            intents_confidence_order
-        )
+
         ordered_confidence_scores = [
             confidence_scores[0][idx] for idx in intents_confidence_order
         ]
 
+        if self.purpose == const.TEST:
+            predicted_intents = self.labelencoder.inverse_transform(
+                intents_confidence_order
+            )
+
         if self.use_calibration:
             ordered_confidence_scores = [
                 logits[0][idx] for idx in np.argsort(logits)[0][::-1]
             ]  # ordered logits for calibration
 
         return [
             Intent(name=intent, score=round(score, self.round)).add_parser(self)
@@ -270,19 +339,18 @@
             expected_columns.append(self.state_column)
 
         for column in expected_columns:
             if column not in training_data.columns:
                 logger.warning(f"Column {column} not found in training data")
                 return False
         return True
-
+    
     def train(self, training_data: pd.DataFrame) -> None:
         """
         Train an intent-classifier on the provided training data.
-
         The training is skipped if the data-format is not valid.
         While training with the use_state flag as true, make sure that the state column is the part of the training_data dataframe
         :param training_data: A pandas dataframe containing at least list of strings and corresponding labels.
         :type training_data: pd.DataFrame
         """
         if not self.validate(training_data):
             logger.warning(
@@ -331,15 +399,14 @@
 
         self.model.train_model(training_data)
         self.save()
 
     def save(self) -> None:
         """
         Save the plugin artifacts.
-
         :raises ValueError: In case the labelencoder is not trained.
         """
         if not self.model or not self.valid_labelencoder:
             raise ValueError(
                 f"Plugin {self.__class__.__name__} seems to be un-trained."
             )
         save_file(
@@ -356,15 +423,15 @@
         try:
             return self.prompts_map[lang][nls_label]
         except Exception as e:
             if self.debug:
                 logger.debug(e)
                 logger.debug(f"Prompt not found for Lang: {lang} \t State: {nls_label}")
             return self.null_prompt_token
-
+        
     def load(self) -> None:
         """
         Load the plugin artifacts.
         """
         self.labelencoder = load_file(
             self.labelencoder_file_path, mode="rb", loader=pickle.load
         )
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,23 +90,25 @@
         guards: Optional[List[Guard]] = None,
         input_column: str = const.ALTERNATIVES,
         output_column: Optional[str] = None,
         replace_output: bool = True,
         use_transform: bool = False,
         trigger_intents: Optional[List[str]] = None,
         debug: bool = False,
+        **kwargs: Any
     ) -> None:
         super().__init__(
             dest=dest,
             guards=guards,
             replace_output=replace_output,
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
             debug=debug,
+            **kwargs
         )
         self.trigger_intents = trigger_intents
 
     def join(
         self, current_entity: TimeEntity, previous_entity: TimeEntity
     ) -> BaseEntity:
         current_turn_datetime = current_entity.get_value()
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,25 +589,27 @@
         threshold: Optional[float] = None,
         activate_latent_entities: Union[Callable[..., bool], bool] = False,
         reference_time_column: str = const.REFERENCE_TIME,
         input_column: str = const.ALTERNATIVES,
         output_column: Optional[str] = None,
         use_transform: bool = False,
         debug: bool = False,
+        **kwargs: Any
     ) -> None:
         """
         constructor
         """
         super().__init__(
             dest=dest,
             guards=guards,
             debug=debug,
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
+            **kwargs
         )
         self.dimensions = dimensions
         self.locale = locale
         self.timezone = timezone
         self.timeout = timeout
         self.threshold = threshold
         self.url = url
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-2.0.0/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,14 +513,15 @@
     def __init__(
         self,
         rules: List[Dict[str, Any]],
         dest: Optional[str] = None,
         guards: Optional[List[Guard]] = None,
         replace_output: bool = True,
         debug: bool = False,
+        **kwargs: Any
     ) -> None:
         self.rules = Rule.from_list(rules)
         self.dest = dest
         self.guards = guards or []
         self.replace_output = replace_output
         self.debug = debug
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-2.0.0/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Optional
 
 from pydash import partition
 
 from dialogy import constants as const
 from dialogy.base import Guard, Input, Output
-from dialogy.plugins import DucklingPlugin
+from dialogy.plugins.registry import DucklingPlugin
 from dialogy.types import BaseEntity
 
 
 class DucklingPluginLB(DucklingPlugin):
     # Constructor
     def __init__(
         self,
@@ -21,14 +21,15 @@
         dest: Optional[str] = None,
         guards: Optional[List[Guard]] = None,
         reference_time_column: str = const.REFERENCE_TIME,
         input_column: str = const.ALTERNATIVES,
         output_column: Optional[str] = None,
         use_transform: bool = False,
         debug: bool = False,
+        **kwargs: Any
     ):
         super().__init__(
             dimensions,
             timezone,
             timeout=timeout,
             url=url,
             locale=locale,
@@ -37,14 +38,15 @@
             dest=dest,
             guards=guards,
             reference_time_column=reference_time_column,
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
             debug=debug,
+            **kwargs
         )
 
     def utility(self, input_: Input, output: Output) -> List[BaseEntity]:
         entity_list = super().utility(input_, output)
         datetime_list, other_list = partition(
             entity_list, lambda x: x.entity_type in ["datetime", "date", "time"]
         )
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,22 +131,24 @@
         labels: Optional[List[str]] = None,
         threshold: Optional[float] = None,
         input_column: str = const.ALTERNATIVES,
         output_column: Optional[str] = None,
         use_transform: bool = True,
         flags: re.RegexFlag = re.I | re.U,
         debug: bool = False,
+        **kwargs: Any
     ):
         super().__init__(
             dest=dest,
             guards=guards,
             debug=debug,
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
+            **kwargs
         )
         self.__style_search_map = {
             const.SPACY: self.ner_search,
             const.REGEX: self.regex_search,
         }
 
         self.style = style or const.REGEX
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,22 +65,24 @@
         guards: Optional[List[Guard]] = None,
         input_column: str = const.ALTERNATIVES,
         output_column: Optional[str] = None,
         use_transform: bool = True,
         flags: re.RegexFlag = re.I | re.U,
         debug: bool = False,
         fuzzy_threshold: Optional[float] = 0.1,
+        **kwargs: Any
     ):
         super().__init__(
             dest=dest,
             guards=guards,
             debug=debug,
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
+            **kwargs
         )
         self.__style_search_map = {
             const.FUZZY_DP: self.get_fuzzy_dp_search,
         }
 
         self.style = (
             const.FUZZY_DP
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-2.0.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,22 +86,24 @@
         self,
         input_column: str = const.ALTERNATIVES,
         output_column: Optional[str] = None,
         use_transform: bool = False,
         dest: Optional[str] = None,
         guards: Optional[List[Guard]] = None,
         debug: bool = False,
+        **kwargs: Any
     ) -> None:
         super().__init__(
             dest=dest,
             guards=guards,
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
             debug=debug,
+            **kwargs
         )
 
     def utility(self, input: Input, _: Output) -> Any:
         return merge_asr_output(input.utterances)
 
     def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         if not self.use_transform:
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/oos_filter/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/oos_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,24 @@
         input_column: str = const.ALTERNATIVES,
         output_column: Optional[str] = None,
         use_transform: bool = False,
         dest: Optional[str] = None,
         guards: Optional[List[Guard]] = None,
         debug: bool = False,
         drop_conflicting_labels: bool = True,
+        **kwargs: Any
     ) -> None:
         super().__init__(
             dest=dest,
             guards=guards,
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
             debug=debug,
+            **kwargs
         )
         self.discarded_output_path = discarded_output_path
         self.drop_conflicting_labels = drop_conflicting_labels
 
     @staticmethod
     def identify_conflicting_labels(training_data: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `dialogy-1.4.1/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-2.0.0/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-2.0.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 While we describe :ref:`slots <Slot>` in the linked doc. The slot filling is part of an :ref:`intent's<Intent>`
 role. This plugin orchestrates the execution of slot filling via methods available on intents.
 
 #. We eagerly apply slot placeholders using the :ref:`apply<ApplySlot>` method. 
 #. Once entities are found, we check if the slots can fill them using the :ref:`fill<FillSlot>` method.
 #. If no slots were filled, we remove the placeholders using :ref:`cleanup<CleanupSlot>` method.
 """
-from typing import List, Union, Set
+from typing import List, Union, Set, Any
 
 from dialogy.base import Guard, Input, Output, Plugin
 from dialogy.types import BaseEntity
 from dialogy.types.intent import Intent
 from dialogy.types.slots import Rule
 
 
@@ -49,29 +49,30 @@
         rules: Rule,
         dest: Union[str, None] = None,
         guards: Union[List[Guard], None] = None,
         replace_output: bool = True,
         fill_multiple: bool = True,
         sort_by_score: bool = True,
         debug: bool = False,
+        **kwargs: Any
     ) -> None:
         """
         constructor
         """
         # rules
         #
         # A `Dict` where each key is an intent name, and each value is another `Dict`,
         # in which, each key is an entity and value contains the `slot_name` and `entity_type.`
         #
         # example:
         # ```
         # rules = {"intent": {"slot_name": "entity_type"}}
         # ```
         super().__init__(
-            dest=dest, guards=guards, debug=debug, replace_output=replace_output
+            dest=dest, guards=guards, debug=debug, replace_output=replace_output, **kwargs
         )
         self.rules: Rule = rules or {}
 
         # fill_multiple
         # A boolean value that commands the slot filler to add multiple values of the
         # same entity type within a slot.
         self.fill_multiple = fill_multiple
```

### Comparing `dialogy-1.4.1/dialogy/types/__init__.py` & `dialogy-2.0.0/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/address/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/base_entity/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/base_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/deserialize/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/duration/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/keyword/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/numerical/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/people/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/pincode/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/time/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/entity/time_interval/__init__.py` & `dialogy-2.0.0/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/intent/__init__.py` & `dialogy-2.0.0/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/types/slots/__init__.py` & `dialogy-2.0.0/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/utils/__init__.py` & `dialogy-2.0.0/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/utils/datetime.py` & `dialogy-2.0.0/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/utils/file_handler.py` & `dialogy-2.0.0/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/utils/logger.py` & `dialogy-2.0.0/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/utils/misc.py` & `dialogy-2.0.0/dialogy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/utils/naive_lang_detect.py` & `dialogy-2.0.0/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/utils/normalize_utterance.py` & `dialogy-2.0.0/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/utils/temperature_scaling.py` & `dialogy-2.0.0/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-1.4.1/dialogy/workflow/workflow.py` & `dialogy-2.0.0/dialogy/workflow/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         Post init hook.
         """
         self.lock = Lock()
         for plugin in self.plugins:
             if isinstance(plugin, Plugin):
                 plugin.debug = self.debug & plugin.debug
 
-    def run(self, input: Input, output: Output = None):  # type: ignore
+    def run(self, input: Input, output: Output = None, project_name: Optional[str] = None):  # type: ignore
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
-                input, output = plugin(input, output)
+                input, output = plugin(input, output, project_name)
             end = time.perf_counter()
 
             # logs are available only when debug=False during class initialization
             if self.debug:
                 history["after"] = {
                     "input": input.dict(),
                     "output": output.dict(),
```

### Comparing `dialogy-1.4.1/pyproject.toml` & `dialogy-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialogy"
-version = "1.4.1"
+version = "2.0.0"
 description = "Dialogy is a library for building and managing SLU applications."
 authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
@@ -50,13 +50,14 @@
 Sphinx = "4.4.0"
 sphinx-copybutton = "^0.3.1"
 sphinx-autodoc-typehints = "^1.16.0"
 sphinxcontrib-mermaid = "^0.7.1"
 pytest-mock = "^3.7.0"
 spacy = "^3.3.1"
 ipykernel = "^6.15.0"
+types-PyYAML = "6.0.12.9"
 
 [tool.poetry.scripts]
 dialogy = "dialogy.cli:main"
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dialogy-1.4.1/PKG-INFO` & `dialogy-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 1.4.1
+Version: 2.0.0
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

