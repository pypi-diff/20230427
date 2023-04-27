# Comparing `tmp/transition_neural_parser-0.5.2.dev0.tar.gz` & `tmp/transition_neural_parser-0.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transition_neural_parser-0.5.2.dev0.tar", last modified: Thu Mar 16 14:41:18 2023, max compression
+gzip compressed data, was "transition_neural_parser-0.5.3.1.tar", last modified: Thu Apr 27 04:44:36 2023, max compression
```

## Comparing `transition_neural_parser-0.5.2.dev0.tar` & `transition_neural_parser-0.5.3.1.tar`

### file list

```diff
@@ -1,131 +1,163 @@
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.586725 transition_neural_parser-0.5.2.dev0/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10776 2023-02-08 02:38:06.000000 transition_neural_parser-0.5.2.dev0/LICENSE
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9859 2023-03-16 14:41:18.586334 transition_neural_parser-0.5.2.dev0/PKG-INFO
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9263 2023-03-16 13:10:21.000000 transition_neural_parser-0.5.2.dev0/README.md
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      706 2023-03-16 14:39:05.000000 transition_neural_parser-0.5.2.dev0/pyproject.toml
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       38 2023-03-16 14:41:18.586842 transition_neural_parser-0.5.2.dev0/setup.cfg
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1687 2023-03-16 14:39:56.000000 transition_neural_parser-0.5.2.dev0/setup.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:17.804960 transition_neural_parser-0.5.2.dev0/src/
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.272677 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      165 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/__init__.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.273854 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_reform/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_reform/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19730 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.341137 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10043 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8788 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15698 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_binarize.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15835 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21406 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21411 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10755 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_graphmp.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10336 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8638 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/old_action_info.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28857 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/old_action_info_binarize.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6018 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/average_checkpoints.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1100 2023-03-13 13:46:26.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/binarize.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.347229 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/criterions/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      679 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/criterions/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12919 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12636 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.377552 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29683 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29892 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_action_pointer_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30695 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30770 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10918 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_bpe.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9147 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/data_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16218 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/indexed_dataset.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18120 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/language_pair_dataset.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.385316 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6506 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/binarize_encodings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9588 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/composite_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5255 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/mapavg_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8609 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/sentence_encoding.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15325 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/generate.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16901 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/generate_sliding.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.484004 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      796 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8953 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/attention_masks.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5741 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/graph_attention_masks.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8485 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/graphmp_attention_masks.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79650 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84035 2023-03-06 20:36:20.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_bart.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79562 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    74564 2023-03-14 16:00:16.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    73280 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    64589 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_graph.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84683 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.506516 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6304 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/factored_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23865 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/multihead_attention.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23312 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/multihead_attention_old.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    17425 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/transformer_layer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12391 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/transformer_layer_old.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30704 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/options.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20120 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/options_train.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15142 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/preprocess.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18504 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/preprocess_bart.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    14481 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/preprocess_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13349 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/preprocess_graphmp.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.512195 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/roberta/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/roberta/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4761 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/roberta/binarize_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9693 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/roberta/pretrained_embeddings.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9316 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/roberta/pretrained_embeddings_bert.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65291 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/sequence_generator.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65757 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/sequence_generator_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    57973 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/sequence_generator_graph.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62664 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/sequence_generator_graphmp.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.524420 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      580 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    22251 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    26944 2023-03-06 20:37:40.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_bart.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    55372 2023-03-13 13:46:13.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    27591 2023-03-14 16:00:32.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24602 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24616 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       81 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tokenizer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23192 2023-03-06 20:38:42.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/train.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7661 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1052 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/utils_font.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1748 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/fairseq_ext/utils_import.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.552425 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      867 2023-03-16 14:41:03.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/__init__.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.579822 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/__init__.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3749 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/amr_parser.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    37837 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_data_oracle.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13849 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_fake_parse.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62718 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_state_machine.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62580 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15856 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15861 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20120 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/parse.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4040 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/roberta_utils.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1355 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/add_id_to_amr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      635 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/add_sentence_amrs_to_file.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    52645 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    46594 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr_aligner.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5278 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr_constituents.py
--rwxrwxr-x   0 gxxu     (700773) gxxu     (606684)     6746 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr_latex.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    74725 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr_machine.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4756 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/clbar.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5057 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/force_overlap_actions.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    45407 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/gold_subgraph_align.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18047 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/io.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10706 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/make_sliding_splits.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5548 2023-02-02 20:35:10.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/merge_sliding_splits.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    46378 2023-03-14 18:36:39.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/parse.py
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6358 2023-03-14 19:41:57.000000 transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/plots.py
-drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-03-16 14:41:18.585770 transition_neural_parser-0.5.2.dev0/src/transition_neural_parser.egg-info/
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9859 2023-03-16 14:41:17.000000 transition_neural_parser-0.5.2.dev0/src/transition_neural_parser.egg-info/PKG-INFO
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5164 2023-03-16 14:41:17.000000 transition_neural_parser-0.5.2.dev0/src/transition_neural_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        1 2023-03-16 14:41:17.000000 transition_neural_parser-0.5.2.dev0/src/transition_neural_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      116 2023-03-16 14:41:17.000000 transition_neural_parser-0.5.2.dev0/src/transition_neural_parser.egg-info/entry_points.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      235 2023-03-16 14:41:17.000000 transition_neural_parser-0.5.2.dev0/src/transition_neural_parser.egg-info/requires.txt
--rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       34 2023-03-16 14:41:17.000000 transition_neural_parser-0.5.2.dev0/src/transition_neural_parser.egg-info/top_level.txt
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.326697 transition_neural_parser-0.5.3.1/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10776 2023-04-24 13:10:54.000000 transition_neural_parser-0.5.3.1/LICENSE
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16136 2023-04-27 04:44:36.326094 transition_neural_parser-0.5.3.1/PKG-INFO
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15543 2023-04-25 17:50:32.000000 transition_neural_parser-0.5.3.1/README.md
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      704 2023-04-27 04:39:47.000000 transition_neural_parser-0.5.3.1/pyproject.toml
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       38 2023-04-27 04:44:36.326807 transition_neural_parser-0.5.3.1/setup.cfg
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1816 2023-04-27 04:43:18.000000 transition_neural_parser-0.5.3.1/setup.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.115540 transition_neural_parser-0.5.3.1/src/
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.151945 transition_neural_parser-0.5.3.1/src/fairseq_ext/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      165 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/__init__.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.153529 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_reform/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_reform/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19730 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.172583 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10043 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8788 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15698 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15835 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21406 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    21411 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10755 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_graphmp.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10336 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8638 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/old_action_info.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28857 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/old_action_info_binarize.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6018 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/average_checkpoints.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1100 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/binarize.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.176730 transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      679 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12919 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12636 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.190420 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29683 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    29892 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30695 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    30770 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10918 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_bpe.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9147 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/data_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16218 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/indexed_dataset.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18120 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/data/language_pair_dataset.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.198269 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6506 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/binarize_encodings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9588 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/composite_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5255 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/mapavg_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8609 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/sentence_encoding.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15450 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/generate.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16901 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/generate_sliding.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.216327 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      796 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8953 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/attention_masks.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5741 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/graph_attention_masks.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8485 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/graphmp_attention_masks.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79650 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84503 2023-04-24 15:25:46.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bart.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    79562 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    75031 2023-04-24 15:25:04.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    73280 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    64589 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_graph.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    84683 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.226376 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6304 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/factored_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23865 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/multihead_attention.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23312 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/multihead_attention_old.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    17425 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/transformer_layer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    12391 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/transformer_layer_old.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    31215 2023-04-24 14:16:48.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/options.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20449 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/options_train.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15142 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18504 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_bart.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    14481 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13349 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_graphmp.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.231622 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4761 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/binarize_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9693 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/pretrained_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9316 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/pretrained_embeddings_bert.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65291 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    65757 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    57973 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_graph.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62664 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_graphmp.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.243154 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      580 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    22251 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    27439 2023-04-24 15:25:16.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bart.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    55372 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    28086 2023-04-24 15:25:25.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24602 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    24616 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       81 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/tokenizer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    23251 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/train.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7661 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1052 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/utils_font.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1748 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/fairseq_ext/utils_import.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.283621 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1226 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/README.md
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6389 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/align_leamr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8746 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/align_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1958 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/alignment_decoder.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5840 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/amr_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7611 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/ccc.launch_many_jobs.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     9753 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/ccc.summarize.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      687 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/dummy_align.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    26107 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/evaluation.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5402 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/formatter.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4784 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/gcn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      485 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/leamr_align.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     2991 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/lexicon.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    60552 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/main.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1158 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/make_splits.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1752 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/metric_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4322 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/pretrained_embeddings.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13907 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/resolve_manual_alignments.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3752 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_detailed_eval.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      874 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_eval.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    11929 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_model_selection.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     7781 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/run_sampler.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    34661 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/standalone_elmo.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1145 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/tokenize_amr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4869 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/transformer_lm.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    19700 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/tree_lstm.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     8380 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/tree_rnn.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3709 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/view_manual_alignments.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3202 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/vocab.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      380 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/ibm_neural_aligner/vocab_definitions.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.305271 transition_neural_parser-0.5.3.1/src/transition_amr_parser/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      867 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/__init__.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.319685 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        0 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/__init__.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     3749 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/amr_parser.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    37837 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_data_oracle.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    13849 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_fake_parse.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62718 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    62580 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15856 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    15861 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    20120 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/parse.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4040 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/roberta_utils.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     1355 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/add_id_to_amr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      635 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/add_sentence_amrs_to_file.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    52645 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    46594 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_aligner.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5278 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_constituents.py
+-rwxrwxr-x   0 gxxu     (700773) gxxu     (606684)     6746 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_latex.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    74725 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_machine.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     4756 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/clbar.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5057 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/force_overlap_actions.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    45407 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/gold_subgraph_align.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    18047 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/io.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    10706 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/make_sliding_splits.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     5548 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/merge_sliding_splits.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    50199 2023-04-26 18:24:35.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/parse.py
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6358 2023-04-24 13:11:12.000000 transition_neural_parser-0.5.3.1/src/transition_amr_parser/plots.py
+drwxrwxr-x   0 gxxu     (700773) gxxu     (606684)        0 2023-04-27 04:44:36.324556 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)    16136 2023-04-27 04:44:36.321212 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)     6377 2023-04-27 04:44:36.321879 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)        1 2023-04-27 04:44:36.322376 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      116 2023-04-27 04:44:36.323086 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/entry_points.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)      235 2023-04-27 04:44:36.323949 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/requires.txt
+-rw-rw-r--   0 gxxu     (700773) gxxu     (606684)       53 2023-04-27 04:44:36.324652 transition_neural_parser-0.5.3.1/src/transition_neural_parser.egg-info/top_level.txt
```

### Comparing `transition_neural_parser-0.5.2.dev0/LICENSE` & `transition_neural_parser-0.5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/pyproject.toml` & `transition_neural_parser-0.5.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "transition_neural_parser"
-version = '0.5.2-dev'
+version = '0.5.3.1'
 authors = [
   { name="GX", email="GX.Xu@ibm.com" },
 ]
 description = "The package for transition based nueral AMR parser"
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers = [
```

### Comparing `transition_neural_parser-0.5.2.dev0/setup.py` & `transition_neural_parser-0.5.3.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5.2-dev'
+VERSION = '0.5.3.1'
 
 install_requires = [
     "torch==1.13.1",
     'numpy<=1.23.5',
     'tqdm>=4.55.0',
     'fairseq==0.10.2',
     'packaging>=20.8',
@@ -19,33 +19,34 @@
     # for debugging
     'ipdb>=0.13.0',
     'line_profiler>=4.0.2',
     'pyinstrument>=4.4.0',
     # for aws download
     'boto3>=1.26.1',
     'progressbar',
+    # 'torch-scatter @ https://data.pyg.org/whl/torch-1.13.0%2Bcu117/torch_scatter-2.1.0%2Bpt113cu117-cp38-cp38-linux_x86_64.whl',
 ]
 
 if __name__ == '__main__':
     setup(
         name='transition_amr_parser',
         version=VERSION,
         description="Trasition-based neural parser",
         package_dir={"": "src"},
         # packages=['fairseq_ext', 'transition_amr_parser'],
         # packages=['neural_parser'],
-        packages=find_packages("src", exclude=('cenv_*', 'configs', 'tests', 'DATA','dist','docker','ibm_neural_aligner','run','scripts','service','*egg-info')),
+        packages=find_packages("src", exclude=('cenv_*', 'configs', 'tests', 'DATA','dist','docker','run','scripts','service','*egg-info')),
         package_data={'': ['*.txt', '*.md', '*.opt', '*.cu', '*.cpp']},
         entry_points={
             'console_scripts': [
                 'amr-parse = transition_amr_parser.parse:main',
                 'amr-machine = transition_amr_parser.amr_machine:main',
             ]
         },
-        py_modules=['fairseq_ext', 'transition_amr_parser'],
+        py_modules=['fairseq_ext', 'transition_amr_parser',"ibm_neural_aligner"],
         install_requires=install_requires,
         classifiers=[
             "Programming Language :: Python :: 3.8",
             "License :: OSI Approved :: Apache Software License",
             "Topic :: Scientific/Engineering :: Artificial Intelligence",
             "Natural Language :: English",
         ],
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_reform/o10_action_reformer_subtok.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_binarize.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_binarize_graphmp_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/action_info_graphmp_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/old_action_info.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/old_action_info.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/amr_spec/old_action_info_binarize.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/amr_spec/old_action_info_binarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/average_checkpoints.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/average_checkpoints.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/binarize.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/binarize.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/criterions/__init__.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/criterions/label_smoothed_cross_entropy_pointer_alignment.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_bartsv_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_action_pointer_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_goldamr_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_action_pointer_graphmp_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/amr_bpe.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/amr_bpe.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/data_utils.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/indexed_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/data/language_pair_dataset.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/data/language_pair_dataset.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/binarize_encodings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/binarize_encodings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/composite_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/composite_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/mapavg_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/mapavg_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/extract_bart/sentence_encoding.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/extract_bart/sentence_encoding.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/generate.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,19 @@
 def main(args):
     assert args.path is not None, '--path required for generation!'
     assert not args.sampling or args.nbest == args.beam, \
         '--sampling requires --nbest to be equal to --beam'
     assert args.replace_unk is None or args.raw_text, \
         '--replace-unk requires a raw text dataset (--raw-text)'
 
+
+    # otherwise we run into problems with support for Half
+    if not torch.cuda.is_available():
+        args.fp16 = False
+
     import_user_module(args)
 
     if args.max_tokens is None and args.max_sentences is None:
         args.max_tokens = 12000
     print(args)
 
     use_cuda = torch.cuda.is_available() and not args.cpu
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/generate_sliding.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/generate_sliding.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/__init__.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/attention_masks.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/attention_masks.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/graph_attention_masks.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/graph_attention_masks.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/graphmp_attention_masks.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/graphmp_attention_masks.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_bart.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bart.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,14 +295,21 @@
         # ========== at inference time, update the auxiliary BART model if it is bart.large as a workaround
         # NOTE reason: `arch` is not input from outside to `args` from outside at inference time; `args` is loaded from
         # checkpoint to initialize the model, thus containing `arch`.
         # but `task.bart` is initialized first before the checkpoint is loaded with model `args`
         if 'bart_large' in args.arch:
             print('-' * 10 + ' task bart rewind: loading pretrained bart.large model ' + '-' * 10)
             bart = torch.hub.load('pytorch/fairseq', 'bart.large')
+            if 'initialize_with_watbart' in args.__dict__.keys() and args.initialize_with_watbart is not None:
+                try:
+                    bart_local = torch.load(args.initialize_with_watbart)
+                    bart.model.load_state_dict(bart_local['model'])
+                except Exception:
+                    raise ValueError("the specified path at initialize_with_watbart \
+                        is incorrect; please double-check config file.")
             task.bart = bart
             task.bart_dict = bart.task.target_dictionary    # src dictionary is the same
 
         if 'roberta_base' in args.arch:
             print('-' * 10 + ' task bart rewind: loading pretrained roberta.base model ' + '-' * 10)
             bart = torch.hub.load('pytorch/fairseq', 'roberta.base')
             task.bart = bart
@@ -333,15 +340,15 @@
                 )
             if args.decoder_embed_path and (
                 args.decoder_embed_path != args.encoder_embed_path
             ):
                 raise ValueError(
                     "--share-all-embeddings not compatible with --decoder-embed-path"
                 )
-            encoder_embed_tokens = cls.build_embedding(
+            encoder_embed_tokens = cls.build_embedding( 
                 args, src_dict, args.encoder_embed_dim, args.encoder_embed_path
             )
             decoder_embed_tokens = encoder_embed_tokens
             args.share_decoder_input_output_embed = True
         else:
             encoder_embed_tokens = cls.build_embedding(
                 args, src_dict, args.encoder_embed_dim, args.encoder_embed_path
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bart_sattn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bartsv.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,21 @@
         # ========== at inference time, update the auxiliary BART model if it is bart.large as a workaround
         # NOTE reason: `arch` is not input from outside to `args` from outside at inference time; `args` is loaded from
         # checkpoint to initialize the model, thus containing `arch`.
         # but `task.bart` is initialized first before the checkpoint is loaded with model `args`
         if 'bart_large' in args.arch or 'bartsv_large' in args.arch:
             print('-' * 10 + ' task bart rewind: loading pretrained bart.large model ' + '-' * 10)
             bart = torch.hub.load('pytorch/fairseq', 'bart.large')
+            if 'initialize_with_watbart' in args.__dict__.keys() and args.initialize_with_watbart is not None:
+                try:
+                    bart_local = torch.load(args.initialize_with_watbart)
+                    bart.model.load_state_dict(bart_local['model'])
+                except Exception:
+                    raise ValueError("the specified path at initialize_with_watbart \
+                        is incorrect; please double-check config file.")
             task.bart = bart
             task.bart_dict = bart.task.target_dictionary    # src dictionary is the same
         # ================================================================================================
 
         # overwrite the src and tgt dictionary used to build learnable embeddings
         # src_dict, tgt_dict = task.source_dictionary, task.target_dictionary
         bart_dict = task.bart_dict
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_bartsv_sattn.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_graph.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_graph.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/models/transformer_tgt_pointer_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/factored_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/factored_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/multihead_attention.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/multihead_attention_old.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/multihead_attention_old.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/transformer_layer.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/transformer_layer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/modules/transformer_layer_old.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/modules/transformer_layer_old.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/options.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,16 @@
     # Post-process args.
     if hasattr(args, 'max_sentences_valid') and args.max_sentences_valid is None:
         args.max_sentences_valid = args.max_sentences
     if hasattr(args, 'max_tokens_valid') and args.max_tokens_valid is None:
         args.max_tokens_valid = args.max_tokens
     if getattr(args, 'memory_efficient_fp16', False):
         args.fp16 = True
+    if hasattr(args, "initialize_with_watbart") and args.initialize_with_watbart=="0":
+        args.initialize_with_watbart = None
 
     # Apply architecture configuration.
     if hasattr(args, 'arch'):
         ARCH_CONFIG_REGISTRY[args.arch](args)
 
     if parse_known:
         return args, extra
@@ -192,14 +194,16 @@
                         help='enable autograd profiler emit_nvtx')
     parser.add_argument('--model-parallel-size', default=1, type=int,
                         help='total number of GPUs to parallelize model over')
     parser.add_argument('--quantization-config-path', default=None,
                         help='path to quantization config file')
     parser.add_argument('--bf16', default=False, action='store_true',
                         help='use bfloat16; implies --tpu')
+    parser.add_argument('--initialize-with-watbart', default="0",
+                       help='the path to WatBART with which we initilize the BART weight; default is 0: not using watbart')
 
     from fairseq.registry import REGISTRIES
     for registry_name, REGISTRY in REGISTRIES.items():
         parser.add_argument(
             '--' + registry_name.replace('_', '-'),
             default=REGISTRY['default'],
             choices=REGISTRY['registry'].keys(),
@@ -559,22 +563,25 @@
     group.add_argument('--input', default='-', type=str, metavar='FILE',
                        help='file to read from; use - for stdin')
     # fmt: on
 
 
 def add_model_args(parser):
     group = parser.add_argument_group('Model configuration')
+
     # fmt: off
 
     # Model definitions can be found under fairseq/models/
     #
     # The model architecture can be specified in several ways.
     # In increasing order of priority:
     # 1) model defaults (lowest priority)
     # 2) --arch argument
     # 3) --encoder/decoder-* arguments (highest priority)
     from fairseq.models import ARCH_MODEL_REGISTRY
     group.add_argument('--arch', '-a', default='fconv', metavar='ARCH', required=True,
                        choices=ARCH_MODEL_REGISTRY.keys(),
                        help='Model Architecture')
+    group.add_argument('--initialize-with-watbart', default="0",
+                       help='the path to WatBART with which we initilize the BART weight; default is 0: not using watbart')
     # fmt: on
     return group
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/options_train.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/options_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,17 @@
         args.batch_size_valid = args.batch_size
     if hasattr(args, "max_tokens_valid") and args.max_tokens_valid is None:
         args.max_tokens_valid = args.max_tokens
     if getattr(args, "memory_efficient_fp16", False):
         args.fp16 = True
     if getattr(args, "memory_efficient_bf16", False):
         args.bf16 = True
+    if hasattr(args, "initialize_with_watbart") and args.initialize_with_watbart=="0":
+        args.initialize_with_watbart = None
+        
     args.tpu = getattr(args, "tpu", False)
     args.bf16 = getattr(args, "bf16", False)
     if args.bf16:
         args.tpu = True
     if args.tpu and args.fp16:
         raise ValueError("Cannot combine --fp16 and --tpu, use --bf16 on TPUs")
 
@@ -441,14 +444,16 @@
     # 1) model defaults (lowest priority)
     # 2) --arch argument
     # 3) --encoder/decoder-* arguments (highest priority)
     from fairseq.models import ARCH_MODEL_REGISTRY
     group.add_argument('--arch', '-a', metavar='ARCH',
                        choices=ARCH_MODEL_REGISTRY.keys(),
                        help='model architecture')
+    group.add_argument('--initialize-with-watbart', default="0",
+                       help='the path to WatBART with which we initilize the BART weight; default is 0: not using watbart')
     # fmt: on
     return group
 
 
 def add_state_machine_args(parser):
     group = parser.add_argument_group("AMR machine configuration")
     group.add_argument('--machine-config', type=str, default=None,
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/preprocess.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/preprocess_bart.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_bart.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/preprocess_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/preprocess_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/preprocess_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/roberta/binarize_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/binarize_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/roberta/pretrained_embeddings.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/pretrained_embeddings.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/roberta/pretrained_embeddings_bert.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/roberta/pretrained_embeddings_bert.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/sequence_generator.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/sequence_generator_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_bartsv.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/sequence_generator_graph.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_graph.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/sequence_generator_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/sequence_generator_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/__init__.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_bart.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bart.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,14 +274,21 @@
             # training time: pretrained BART needs to be used for initialization
             if 'bart_base' in args.arch:
                 print('-' * 10 + ' loading pretrained bart.base model ' + '-' * 10)
                 bart = torch.hub.load('pytorch/fairseq', 'bart.base')
             elif 'bart_large' in args.arch:
                 print('-' * 10 + 'loading pretrained bart.large model ' + '-' * 10)
                 bart = torch.hub.load('pytorch/fairseq', 'bart.large')
+                if 'initialize_with_watbart' in args.__dict__.keys() and args.initialize_with_watbart is not None:
+                    try:
+                        bart_local = torch.load(args.initialize_with_watbart)
+                        bart.model.load_state_dict(bart_local['model'])
+                    except Exception:
+                        raise ValueError("the specified path at initialize_with_watbart \
+                            is incorrect; please double-check config file.")
             elif 'roberta_base' in args.arch:
                 print('-' * 10 + 'loading pretrained roberta.base model ' + '-' * 10)
                 bart = torch.hub.load('pytorch/fairseq', 'roberta.base')
             elif 'roberta_large' in args.arch:
                 print('-' * 10 + 'loading pretrained roberta.large model ' + '-' * 10)
                 bart = torch.hub.load('pytorch/fairseq', 'roberta.large')
             elif 'apt2_mini' in args.arch:
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bart_dyo.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_bartsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,21 @@
             # training time: pretrained BART needs to be used for initialization
             if 'bart_base' in args.arch or 'bartsv_base' in args.arch:
                 print('-' * 10 + ' loading pretrained bart.base model ' + '-' * 10)
                 bart = torch.hub.load('pytorch/fairseq', 'bart.base')
             elif 'bart_large' in args.arch or 'bartsv_large' in args.arch:
                 print('-' * 10 + 'loading pretrained bart.large model ' + '-' * 10)
                 bart = torch.hub.load('pytorch/fairseq', 'bart.large')
+                if 'initialize_with_watbart' in args.__dict__.keys() and args.initialize_with_watbart is not None:
+                    try:
+                        bart_local = torch.load(args.initialize_with_watbart)
+                        bart.model.load_state_dict(bart_local['model'])
+                    except Exception:
+                        raise ValueError("the specified path at initialize_with_watbart \
+                            is incorrect; please double-check config file.")
             else:
                 raise ValueError
         else:
             # inference time: pretrained BART is only used for dictionary related things; size does not matter
             # NOTE size does matter; update this later in model initialization if model is with "bart.large"
             print('-' * 10 + ' (for bpe vocab and embed size at inference time) loading pretrained bart.base model '
                   + '-' * 10)
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_graphmp.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/tasks/amr_action_pointer_graphmp_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/train.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     stream=sys.stdout,
 )
 logger = logging.getLogger("fairseq_cli.train")
 
 
 def main(args):
 
+    # otherwise we run into problems with support for Half
     if not torch.cuda.is_available():
         args.fp16 = False
 
     import_user_module(args)
 
     assert (
         args.max_tokens is not None or args.batch_size is not None
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/utils.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/utils_font.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/utils_font.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/fairseq_ext/utils_import.py` & `transition_neural_parser-0.5.3.1/src/fairseq_ext/utils_import.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/__init__.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/amr_parser.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/amr_parser.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_data_oracle.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_data_oracle.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_fake_parse.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_fake_parse.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_state_machine.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_reformer.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/o8_state_machine_reformer_amr1.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/parse.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/parse.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/action_pointer/roberta_utils.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/action_pointer/roberta_utils.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/add_id_to_amr.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/add_id_to_amr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/add_sentence_amrs_to_file.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/add_sentence_amrs_to_file.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr_aligner.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_aligner.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr_constituents.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_constituents.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr_latex.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_latex.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/amr_machine.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/amr_machine.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/clbar.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/clbar.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/force_overlap_actions.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/force_overlap_actions.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/gold_subgraph_align.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/gold_subgraph_align.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/io.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/io.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/make_sliding_splits.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/make_sliding_splits.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/merge_sliding_splits.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/merge_sliding_splits.py`

 * *Files identical despite different names*

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/parse.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,27 +39,35 @@
 )
 from transition_amr_parser.force_overlap_actions import force_overlap
 from transition_amr_parser.merge_sliding_splits import (
     merge_actions,
     check_pointers
 )
 from transition_amr_parser.amr_machine import play_all_actions
+from transition_amr_parser.clbar import yellow_font
+from transition_amr_parser.amr_machine import make_eos_force_actions
+
 
 def argument_parsing():
 
     # Argument hanlding
     parser = argparse.ArgumentParser(
         description='Call parser from the command line'
     )
     parser.add_argument(
         '-i', '--in-tokenized-sentences',
         type=str,
         help='File with one __tokenized__ sentence per line'
     )
     parser.add_argument(
+        '--in-doc',
+        type=str,
+        help='File with one __tokenized__ sentence per line and one newline separating each doc (and the end)'
+    )
+    parser.add_argument(
         '--in-amr',
         type=str,
         help='AMR in Penman format to align'
     )
     parser.add_argument(
         '--in-actions',
         type=str,
@@ -204,25 +212,28 @@
         default=False
     )
     args = parser.parse_args()
 
     # sanity checks
     assert (
         bool(args.in_tokenized_sentences) or bool(args.in_amr)
-    ) or bool(args.service), \
-        "Must either specify --in-tokenized-sentences or set --service"
+    ) or bool(args.service) or bool(args.in_doc), \
+        "Must either specify --in-tokenized-sentences or --in-doc or set --service"
 
     if not (bool(args.model_name) ^ bool(args.in_checkpoint)):
         raise Exception("Use either --model-name or --in-checkpoint")
 
     if bool(args.in_actions) and bool(args.tokenize):
         raise Exception(
             "Remove --tokenize option when enabling --force-actions and"
             "provide tokenized input matching the dimensions of force actions."
         )
+    if bool(args.in_actions) and bool(args.in_doc):
+        print(yellow_font(
+            'WARNING: Given force actions will be used superseding the force actions generated by the inhouse force action generator. Make sure it is in the correct format '))
 
     # num samples replaces beam search
     if args.num_samples:
         assert args.nbest == 1
         assert args.beam == 1
 
     if args.sampling_topp != -1:
@@ -288,25 +299,65 @@
             checkpoint_file='model.pt'
         )
     roberta.eval()
     if roberta_use_gpu:
         roberta.cuda()
     return roberta
 
+def read_doc_text(in_file):
+    sents = []
+    docs = []
+    for line in open(in_file, 'r').readlines():
+        if line == '\n':
+            docs.append(sents)
+            sents = []
+        else:
+            sents.append(line.strip('\n'))
+    if len(sents) > 0:
+        docs.append(sents)
+
+    return docs
+
+def get_force_actions(docs, sen_ends=None):
+
+    force_actions_set = []
+    return_docs = []
+    
+    
+    for idx, docsen in enumerate(docs):
+
+        offset = 0
+        if sen_ends is None:
+            ends = []
+            doc_toks = []
+            for sen in docsen:
+                
+                ends.append(offset+len(sen)-1)
+                offset += len(sen)
+                doc_toks.extend(sen)
+
+            force_actions = make_eos_force_actions(doc_toks, ends)
+        else:
+            force_actions = make_eos_force_actions(doc_toks, sen_ends[idx])
+        force_actions_set.append(force_actions)
+        return_docs.append(doc_toks)
+        
+
+    return force_actions_set, return_docs
+
 
 def get_sliding_windows(tok_sentences, window_size, window_overlap,
                         force_actions=None):
     windowed_tok_sentences = []
     windowed_force_actions = []
     windowed_output_actions = []
     all_windows = []
     max_num_windows = 1
 
     for (i, sentence) in enumerate(tok_sentences):
-        print(i)
         # if sentence end markers are availble, windows should respect that
         sentence_ends = []
         if force_actions:
             for (n, actions) in enumerate(force_actions[i]):
                 if 'CLOSE_SENTENCE' in actions:
                     sentence_ends.append(n)
         if len(sentence_ends) == 0:
@@ -340,27 +391,29 @@
         windowed_force_actions,
         windowed_output_actions,
         all_windows,
         max_num_windows
     )
 
 
-def get_sliding_output(args, tok_sentences, parser, gold_amrs=None,
-                       force_actions=None):
+def get_sliding_output(tok_sentences, parser, gold_amrs=None,
+                       force_actions=None, window_size=300, window_overlap=200,
+                       batch_size=128, roberta_batch_size=128,
+                       beam=1, jamr=False, no_isi=False):
 
     (
         windowed_tok_sentences,
         windowed_force_actions,
         windowed_output_actions,
         all_windows,
         max_num_windows
     ) = get_sliding_windows(
         tok_sentences=tok_sentences,
-        window_size=args.window_size,
-        window_overlap=args.window_overlap,
+        window_size=window_size,
+        window_overlap=window_overlap,
         force_actions=force_actions
     )
 
     for widx in range(max_num_windows):
         window_sentences = []
         window_actions = []
         wsidx2sidx = []
@@ -372,21 +425,21 @@
                 window_actions.append(windowed_force_actions[sidx][widx])
 
         # Parse this (widx_th) window of all sentences
         num_window_sent = len(window_sentences)
         print(f'Parsing {num_window_sent} sentences in {widx} window')
         window_result = parser.parse_sentences(
             window_sentences,
-            batch_size=args.batch_size,
-            roberta_batch_size=args.roberta_batch_size,
+            batch_size=batch_size,
+            roberta_batch_size=roberta_batch_size,
             gold_amrs=gold_amrs,
             force_actions=window_actions,
-            beam=args.beam,
-            jamr=args.jamr,
-            no_isi=args.no_isi
+            beam=beam,
+            jamr=jamr,
+            no_isi=no_isi
         )
         # get actions out of window_results
         # save actions in windowed_output_actions[sidx][widx]
         for residx, result in enumerate(window_result[1]):
             windowed_output_actions[wsidx2sidx[residx]
                                     ][widx] = result.action_history
         # change windowed_force_actions[:][widx+1]
@@ -553,25 +606,26 @@
         Raises:
             ValueError: The given model name doesn't match any model in library.
             Exception: _description_
 
         Returns:
             _type_: _description_
         """
-        
+
         MODEL_NAMES = {
             'AMR3-structbart-L-smpl': 'amr3.0-structured-bart-large-neur-al-sampling5-seed42.zip',
             'AMR3-structbart-L': 'amr3.0-structured-bart-large-neur-al-seed42.zip',
             'AMR2-structbart-L': 'amr2.0-structured-bart-large-neur-al-seed42.zip',
             'AMR2-joint-ontowiki-seed42': 'amr2joint_ontowiki2_g2g-structured-bart-large-seed42.zip',
             'AMR2-joint-ontowiki-seed43': 'amr2joint_ontowiki2_g2g-structured-bart-large-seed43.zip',
             'AMR2-joint-ontowiki-seed44': 'amr2joint_ontowiki2_g2g-structured-bart-large-seed44.zip',
             'AMR3-joint-ontowiki-seed42': 'amr3joint_ontowiki2_g2g-structured-bart-large-seed42.zip',
             'AMR3-joint-ontowiki-seed43': 'amr3joint_ontowiki2_g2g-structured-bart-large-seed43.zip',
             'AMR3-joint-ontowiki-seed44': 'amr3joint_ontowiki2_g2g-structured-bart-large-seed44.zip',
+            'doc-sen-conll-amr-seed42': 'both_doc+sen_trainsliding_ws400x100-seed42.zip'
         }
 
         if model_name not in MODEL_NAMES:
             raise ValueError('The model_name provided in not in our library; if you provide a path, \
                              use from_chackpoint() method instead')
 
         # get model class and model names
@@ -579,32 +633,38 @@
         if "ontowiki2" in zip_file:
             model_class = zip_file.split("-structured-bart")[0]
         elif "amr2.0" in zip_file:
             model_class = "AMR2.0"
         else:
             model_class = "AMR3.0"
 
+        if "doc" in model_name:
+            eval_metric = "smatch"
+        else:
+            eval_metric = "wiki.smatch"
+
         model_name = zip_file.split("-seed")[0]
         seed = zip_file.split("-seed")[1][:2]
 
         # get cache storage dir, in which we save the downloaded models
         cache_dir = torch.hub._get_torch_home() + '/'
         cache_save_zip = cache_dir + zip_file
 
         # get checkpoint path
-        model_dir_path = os.path.join(cache_dir, "DATA", model_class, "models", model_name, "seed"+str(seed))
-        checkpoint_path = model_dir_path + "/checkpoint_wiki.smatch_top5-avg.pt"
+        model_dir_path = os.path.join(
+            cache_dir, "DATA", model_class, "models", model_name, "seed"+str(seed))
+        checkpoint_path = model_dir_path + "/checkpoint_"+eval_metric+"_top5-avg.pt"
 
         # get model url to download from
         model_url = "https://github.com/transition-amr-parsing/parser-model-hub/raw/main/models/" + zip_file
 
         if not os.path.isfile(checkpoint_path):
             print('Downloading model from library, and save to cache')
-            # download and save to cache dir 
-            
+            # download and save to cache dir
+
             global pbar
             pbar = None
 
             def show_progress(block_num, block_size, total_size):
                 global pbar
                 if pbar is None:
                     pbar = progressbar.ProgressBar(maxval=total_size)
@@ -613,25 +673,28 @@
                 downloaded = block_num * block_size
                 if downloaded < total_size:
                     pbar.update(downloaded)
                 else:
                     pbar.finish()
                     pbar = None
             if not os.path.isfile(cache_save_zip):
-                urllib.request.urlretrieve(model_url, cache_save_zip, show_progress)
+                urllib.request.urlretrieve(
+                    model_url, cache_save_zip, show_progress)
             else:
                 print("a model zip file is already downloaded")
 
-            if os.path.getsize(cache_save_zip)<1000000:
-                raise Exception("our model download limit is reached; please try downloading  again next week.")
-            
+            if os.path.getsize(cache_save_zip) < 1000000:
+                raise Exception(
+                    "our model download limit is reached; please try downloading  again next week.")
+
             with zipfile.ZipFile(cache_dir + zip_file, 'r') as zip_ref:
                 zip_ref.extractall(torch.hub._get_torch_home())
             print("downloaded model unzipped")
-            assert os.path.isfile(checkpoint_path), 'checkpoint still not available after downloads;'
+            assert os.path.isfile(
+                checkpoint_path), 'checkpoint still not available after downloads;'
         else:
             print('model is already in cache')
         return cls.from_checkpoint(checkpoint_path, dict_dir,
                                    roberta_cache_path, fp16, inspector,
                                    beam, nbest, num_samples, sampling_topp,
                                    temperature)
 
@@ -681,21 +744,21 @@
             pretrained_embed = 'bart.base'
         elif model_args.pretrained_embed_dim == 1024:
             pretrained_embed = 'bart.large'
         else:
             raise ValueError
 
         model_folder = os.path.dirname(checkpoint.split(':')[0])
-        config_data_path = None
-        for dfile in os.listdir(model_folder):
-            if dfile.startswith('config.sh'):
-                config_data_path = os.path.join(model_folder, dfile)
-                break
-        assert config_data_path is not None, \
-            'data configuration file not found'
+        # config_data_path = None
+        # for dfile in os.listdir(model_folder):
+        #     if dfile.startswith('config.sh'):
+        #         config_data_path = os.path.join(model_folder, dfile)
+        #         break
+        # assert config_data_path is not None, \
+        #     'data configuration file not found'
 
         print("pretrained_embed: ", pretrained_embed)
         embeddings = SentenceEncodingBART(name=pretrained_embed)
 
         print("Finished loading models")
 
         # load other args
@@ -821,14 +884,16 @@
             target_tokens = None
 
             sample_predictions = []
             for j, hypo in enumerate(hypos[i][:self.args.nbest]):
                 # args.nbest is default 1, i.e. saving only the top predictions
                 if 'bartsv' in self.model_args.arch:
                     # shared vocabulary BART
+                    print(yellow_font(
+                        'WARNING: If force actions have been provided, they will not be used since this model is a joint vocab model and does not support force actions yet . '))
                     actions_nopos, actions_pos, actions = \
                         post_process_action_pointer_prediction_bartsv(
                             hypo, self.tgt_dict
                         )
 
                     # FIXME: hypo['state_machine'].machine.action_history !=
                     # actions
@@ -944,14 +1009,24 @@
                     m.get_annotation(jamr=jamr, no_isi=no_isi)
                     for m in machine_nbest
                 )
                 machines.append(machine_nbest)
 
         return annotations, machines
 
+    def parse_docs(self, tok_sentences, **kwargs):
+        
+        init_force_actions, doc_sen = get_force_actions(tok_sentences)
+
+            
+        force_actions = [fac+[[]] for fac in init_force_actions]
+
+        annotations, decoding_data = get_sliding_output(tok_sentences=doc_sen,parser=self,force_actions=force_actions,**kwargs)
+
+        return annotations,decoding_data
 
 def simple_inspector(machine):
     '''
     print the first machine
     '''
     os.system('clear')
     print(machine)
@@ -1098,19 +1173,25 @@
         else:
             force_actions = None
 
         if args.sliding:
             gold_amrs = None
 
             result = get_sliding_output(
-                args,
                 tokens,
                 parser,
                 gold_amrs,
-                force_actions
+                force_actions,
+                args.window_size,
+                args.window_overlap,
+                args.batch_size,
+                args.roberta_batch_size,
+                args.beam,
+                args.jamr,
+                args.no_isi
             )
 
         else:
 
             # duplicate if sampling
             assert args.num_samples is None, \
                 "Sampling not supported in --service mode"
@@ -1133,14 +1214,15 @@
 
         else:
             print(''.join(result[0]))
 
 
 def prepare_data(args, parser):
 
+    force_actions = None
     if args.in_amr:
 
         # align mode: read input AMR to be aligned
         gold_amrs = read_amr(args.in_amr)
         if args.tokenize:
             # jamr-like tokenization
             assert all(amr.sentence is not None for amr in gold_amrs), \
@@ -1157,52 +1239,63 @@
             tok_sentences, gold_amrs, parser.tgt_dict
         )
 
     else:
 
         # normal mode
         gold_amrs = None
-        if args.tokenize:
-            # TODO: have tokenized as default
-            # jamr-like tokenization
-            with open(args.in_tok_sentences) as fid:
-                tok_sentences = [
-                    protected_tokenizer(sentence.rstrip())[0]
-                    for sentence in fid.readlines()
-                ]
+
+        if args.in_doc:
+            tok_sentences = []
+            docs = read_doc_text(args.in_doc)
+            for docsen in docs:
+                tok_sen = []
+                for sen in docsen:
+
+                    enc = sen.rstrip().encode("ascii", "ignore")
+
+                    newsen = enc.decode()
+
+                    if args.tokenize:
+                        tok_sen.append(protected_tokenizer(newsen.rstrip())[0])
+                    else:
+                        tok_sen.append(newsen.split())
+                tok_sentences.append(tok_sen)
+
+
+
+
         else:
-            tok_sentences = read_tokenized_sentences(
-                args.in_tokenized_sentences
-            )
+            if args.tokenize:
+                # TODO: have tokenized as default
+                # jamr-like tokenization
+                with open(args.in_tokenized_sentences) as fid:
+                    tok_sentences = [
+                        protected_tokenizer(sentence.rstrip())[0]
+                        for sentence in fid.readlines()
+                    ]
+            else:
+                tok_sentences = read_tokenized_sentences(
+                    args.in_tokenized_sentences
+                )
 
     # check for empty sentences
     assert all(s != [''] for s in tok_sentences), "Empty sentences!"
 
-    # read constrained decoding forced actions if provided
-    if args.in_actions:
-        with open(args.in_actions) as fact:
-            force_actions = [eval(line.strip()) + [[]] for line in fact]
-    else:
-        force_actions = None
-
+    
     # sampling needs copy of sentences N times
     if args.num_samples is not None:
         tok_sentences = [
             tsent
             for tsent in tok_sentences
             for _ in range(args.num_samples)
         ]
-        if args.in_actions:
-            force_actions = [
-                a
-                for a in force_actions
-                for _ in range(args.num_samples)
-            ]
+        
 
-    return tok_sentences, force_actions, gold_amrs
+    return tok_sentences, gold_amrs
 
 
 def save_data(args, annotations, machines):
 
     num_sent = len(machines)
 
     if args.out_amr:
@@ -1254,32 +1347,49 @@
 
         # command line parsing service
         run_service(args, parser)
 
     else:
 
         # offline parsing given files
-        tok_sentences, force_actions, gold_amrs = prepare_data(args, parser)
+        tok_sentences, gold_amrs = prepare_data(args, parser)
+        force_actions = None
+
+        # read constrained decoding forced actions if provided
+        if args.in_actions:
+            with open(args.in_actions) as fact:
+                force_actions = [eval(line.strip()) + [[]] for line in fact]
+            assert len(tok_sentences) == len(
+            force_actions), "Number of force actions doesn't match the number of sentences"
+        
+            # sampling needs copy of force actions N times
+            if args.num_samples is not None:
+                force_actions = [
+                    a
+                    for a in force_actions
+                    for _ in range(args.num_samples)
+                ]
 
         # TODO: max batch sizes could be computed from max sentence length
 
         num_sent = len(tok_sentences)
         print(f'Parsing {num_sent} sentences')
         start = time.time()
 
-        if args.sliding:
-
-            # doc-AMR sliding window parsing
-            annotations, machines = get_sliding_output(
-                args,
-                tok_sentences,
-                parser,
-                gold_amrs,
-                force_actions
-            )
+        if args.in_doc:
+            annotations, machines = parser.parse_docs(tok_sentences, 
+                gold_amrs=gold_amrs,
+                window_size=args.window_size,
+                window_overlap=args.window_overlap,
+                batch_size=args.batch_size,
+                roberta_batch_size=args.roberta_batch_size,
+                beam=args.beam,
+                jamr=args.jamr,
+                no_isi=args.no_isi)
+    
 
         else:
 
             # normal parsing
             annotations, machines = parser.parse_sentences(
                 tok_sentences,
                 batch_size=args.batch_size,
```

### Comparing `transition_neural_parser-0.5.2.dev0/src/transition_amr_parser/plots.py` & `transition_neural_parser-0.5.3.1/src/transition_amr_parser/plots.py`

 * *Files identical despite different names*

