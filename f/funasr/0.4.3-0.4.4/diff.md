# Comparing `tmp/funasr-0.4.3.tar.gz` & `tmp/funasr-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.4.3.tar", last modified: Fri Apr 21 15:36:52 2023, max compression
+gzip compressed data, was "funasr-0.4.4.tar", last modified: Thu Apr 27 09:39:42 2023, max compression
```

## Comparing `funasr-0.4.3.tar` & `funasr-0.4.4.tar`

### file list

```diff
@@ -1,421 +1,413 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.169773 funasr-0.4.3/
--rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.4.3/LICENSE
--rw-r--r--   0 zhifu      (502) staff       (20)     7835 2023-04-21 15:36:52.169437 funasr-0.4.3/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     6813 2023-04-20 17:05:47.000000 funasr-0.4.3/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.022986 funasr-0.4.3/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.043287 funasr-0.4.3/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21327 2023-04-18 11:35:56.000000 funasr-0.4.3/funasr/bin/asr_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11203 2023-04-18 11:14:48.000000 funasr-0.4.3/funasr/bin/asr_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25965 2023-04-18 11:35:56.000000 funasr-0.4.3/funasr/bin/asr_inference_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    37755 2023-04-20 08:05:27.000000 funasr-0.4.3/funasr/bin/asr_inference_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    33456 2023-04-18 11:35:56.000000 funasr-0.4.3/funasr/bin/asr_inference_paraformer_streaming.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19242 2023-04-18 11:35:56.000000 funasr-0.4.3/funasr/bin/asr_inference_paraformer_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32974 2023-04-18 11:35:56.000000 funasr-0.4.3/funasr/bin/asr_inference_paraformer_vad_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25059 2023-04-18 06:44:59.000000 funasr-0.4.3/funasr/bin/asr_inference_rnnt.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23949 2023-04-18 11:28:32.000000 funasr-0.4.3/funasr/bin/asr_inference_uniasr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23931 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/bin/asr_inference_uniasr_vad.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1006 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/bin/asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1027 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/bin/asr_train_paraformer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1036 2023-04-18 06:44:59.000000 funasr-0.4.3/funasr/bin/asr_train_transducer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1024 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/bin/asr_train_uniasr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5309 2023-03-29 08:06:18.000000 funasr-0.4.3/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5327 2023-04-18 11:28:32.000000 funasr-0.4.3/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1010 2023-03-10 07:21:13.000000 funasr-0.4.3/funasr/bin/diar_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14137 2023-04-18 11:28:32.000000 funasr-0.4.3/funasr/bin/eend_ola_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     6814 2023-02-11 09:29:33.000000 funasr-0.4.3/funasr/bin/lm_calc_perplexity.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14544 2023-04-18 11:28:32.000000 funasr-0.4.3/funasr/bin/lm_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3816 2023-04-18 11:28:32.000000 funasr-0.4.3/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1019 2023-02-11 09:29:33.000000 funasr-0.4.3/funasr/bin/lm_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3049 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/bin/modelscope_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3593 2023-04-18 11:28:32.000000 funasr-0.4.3/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-03-10 07:21:13.000000 funasr-0.4.3/funasr/bin/punc_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11940 2023-04-21 03:13:00.000000 funasr-0.4.3/funasr/bin/punctuation_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11121 2023-04-18 11:28:32.000000 funasr-0.4.3/funasr/bin/punctuation_infer_vadrealtime.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20700 2023-04-18 11:28:32.000000 funasr-0.4.3/funasr/bin/sond_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14841 2023-04-18 11:18:21.000000 funasr-0.4.3/funasr/bin/sv_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     4718 2023-04-18 11:18:21.000000 funasr-0.4.3/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.4.3/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12597 2023-04-20 06:52:13.000000 funasr-0.4.3/funasr/bin/tp_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3874 2023-04-18 11:18:21.000000 funasr-0.4.3/funasr/bin/tp_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20030 2023-04-21 15:27:01.000000 funasr-0.4.3/funasr/bin/vad_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4282 2023-04-21 11:09:24.000000 funasr-0.4.3/funasr/bin/vad_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11752 2023-04-18 11:16:41.000000 funasr-0.4.3/funasr/bin/vad_inference_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.045610 funasr-0.4.3/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.4.3/funasr/datasets/iterable_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12671 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/datasets/iterable_dataset_modelscope.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.046962 funasr-0.4.3/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3488 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.048186 funasr-0.4.3/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8055 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.049773 funasr-0.4.3/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1201 2023-03-10 07:21:13.000000 funasr-0.4.3/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2003 2023-04-18 02:01:35.000000 funasr-0.4.3/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    30718 2023-04-18 02:01:35.000000 funasr-0.4.3/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.050182 funasr-0.4.3/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.3/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10833 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.051203 funasr-0.4.3/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5091 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.052091 funasr-0.4.3/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.3/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.4.3/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.4.3/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.053225 funasr-0.4.3/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.3/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.4.3/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.054563 funasr-0.4.3/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.3/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.4.3/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.4.3/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.4.3/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.055155 funasr-0.4.3/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.3/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.4.3/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.057162 funasr-0.4.3/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      966 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.057687 funasr-0.4.3/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.3/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.4.3/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.059393 funasr-0.4.3/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3479 2023-03-29 08:06:18.000000 funasr-0.4.3/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.061998 funasr-0.4.3/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.065801 funasr-0.4.3/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      359 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3503 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      349 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.4.3/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.066646 funasr-0.4.3/funasr/lm/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/lm/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5436 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/lm/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5904 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/lm/seq_rnn_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4243 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/lm/transformer_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.067110 funasr-0.4.3/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2804 2023-03-02 10:32:58.000000 funasr-0.4.3/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.068676 funasr-0.4.3/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5610 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5029 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.077554 funasr-0.4.3/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.4.3/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5298 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.079946 funasr-0.4.3/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7917 2023-04-18 06:44:59.000000 funasr-0.4.3/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    28528 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16707 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11630 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    74061 2023-04-17 07:54:35.000000 funasr-0.4.3/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34689 2023-04-18 06:44:59.000000 funasr-0.4.3/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10238 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20581 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10098 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6710 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51737 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31100 2023-04-21 11:09:24.000000 funasr-0.4.3/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.085025 funasr-0.4.3/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      503 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43611 2023-04-18 06:44:59.000000 funasr-0.4.3/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20993 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.4.3/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.4.3/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.4.3/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17514 2023-02-16 09:30:51.000000 funasr-0.4.3/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.086542 funasr-0.4.3/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.4.3/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.4.3/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.4.3/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41077 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3634 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53339 2023-04-17 07:54:35.000000 funasr-0.4.3/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.088718 funasr-0.4.3/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      400 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8895 2023-02-16 09:30:51.000000 funasr-0.4.3/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5759 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4990 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20471 2023-04-21 15:27:01.000000 funasr-0.4.3/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6322 2023-02-23 03:32:15.000000 funasr-0.4.3/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2817 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.090124 funasr-0.4.3/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-19 10:58:10.000000 funasr-0.4.3/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-18 06:44:59.000000 funasr-0.4.3/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.090592 funasr-0.4.3/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3546 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.091317 funasr-0.4.3/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.091675 funasr-0.4.3/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34651 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.092483 funasr-0.4.3/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/preencoder/sinc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.093001 funasr-0.4.3/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4661 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4715 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.100940 funasr-0.4.3/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    36791 2023-04-18 06:44:59.000000 funasr-0.4.3/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.102650 funasr-0.4.3/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/beam_search/beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-18 06:44:59.000000 funasr-0.4.3/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.105171 funasr-0.4.3/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13504 2023-04-18 06:44:59.000000 funasr-0.4.3/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.105970 funasr-0.4.3/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.4.3/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18008 2023-04-18 06:45:00.000000 funasr-0.4.3/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.107564 funasr-0.4.3/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.4.3/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.4.3/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22115 2023-04-18 06:45:00.000000 funasr-0.4.3/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3649 2023-04-18 06:45:00.000000 funasr-0.4.3/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.109165 funasr-0.4.3/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.110201 funasr-0.4.3/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.111585 funasr-0.4.3/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-18 06:45:00.000000 funasr-0.4.3/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.113209 funasr-0.4.3/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.113733 funasr-0.4.3/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.3/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.114210 funasr-0.4.3/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.3/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.115700 funasr-0.4.3/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.4.3/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.117079 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.120536 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.124836 funasr-0.4.3/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      617 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/demo.py
--rw-r--r--   0 zhifu      (502) staff       (20)      740 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      932 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      383 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      969 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.127215 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7786 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12135 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.131448 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    28927 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-21 11:09:24.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9176 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9707 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1393 2023-04-21 11:10:20.000000 funasr-0.4.3/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.133552 funasr-0.4.3/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.134761 funasr-0.4.3/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.138046 funasr-0.4.3/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    73890 2023-04-18 09:30:37.000000 funasr-0.4.3/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    60627 2023-04-18 06:45:00.000000 funasr-0.4.3/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32463 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6782 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8029 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18814 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12527 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.143691 funasr-0.4.3/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.146785 funasr-0.4.3/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3815 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.150647 funasr-0.4.3/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1764 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/train/abs_espnet_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7280 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.4.3/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    36453 2023-04-20 10:48:18.000000 funasr-0.4.3/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.164680 funasr-0.4.3/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.4.3/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.4.3/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.4.3/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.4.3/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.4.3/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7735 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13178 2023-04-12 07:23:40.000000 funasr-0.4.3/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11759 2023-03-29 08:06:19.000000 funasr-0.4.3/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.4.3/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-04-21 15:27:41.000000 funasr-0.4.3/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.024491 funasr-0.4.3/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     7835 2023-04-21 15:36:51.000000 funasr-0.4.3/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    13238 2023-04-21 15:36:51.000000 funasr-0.4.3/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-21 15:36:51.000000 funasr-0.4.3/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-04-21 15:36:51.000000 funasr-0.4.3/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-04-21 15:36:51.000000 funasr-0.4.3/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-04-21 15:36:52.169828 funasr-0.4.3/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4571 2023-04-17 03:36:48.000000 funasr-0.4.3/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-21 15:36:52.168734 funasr-0.4.3/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    25268 2023-04-17 03:36:48.000000 funasr-0.4.3/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.4.3/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2083 2023-03-29 08:06:19.000000 funasr-0.4.3/tests/test_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.4.3/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.4.3/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.4.3/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2280 2023-04-21 11:09:24.000000 funasr-0.4.3/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.585833 funasr-0.4.4/
+-rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.4.4/LICENSE
+-rw-r--r--   0 zhifu      (502) staff       (20)     8336 2023-04-27 09:39:42.585606 funasr-0.4.4/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7294 2023-04-27 08:40:56.000000 funasr-0.4.4/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.443849 funasr-0.4.4/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.467052 funasr-0.4.4/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21327 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11203 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    25965 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    37755 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    25868 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/bin/asr_inference_paraformer_streaming.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19242 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_paraformer_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32974 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_paraformer_vad_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    25051 2023-04-25 05:58:46.000000 funasr-0.4.4/funasr/bin/asr_inference_rnnt.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23949 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_inference_uniasr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23931 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/bin/asr_inference_uniasr_vad.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1006 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1027 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/asr_train_paraformer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1036 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/asr_train_transducer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1024 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/asr_train_uniasr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5309 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5327 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1010 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/bin/diar_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    14137 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/eend_ola_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     6814 2023-02-11 09:29:33.000000 funasr-0.4.4/funasr/bin/lm_calc_perplexity.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14544 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/lm_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3816 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1019 2023-02-11 09:29:33.000000 funasr-0.4.4/funasr/bin/lm_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3049 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/bin/modelscope_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3593 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/bin/punc_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11940 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/punctuation_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11121 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/punctuation_infer_vadrealtime.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20700 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/sond_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    14841 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/sv_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     4718 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.4.4/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13304 2023-04-25 07:21:40.000000 funasr-0.4.4/funasr/bin/tp_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3874 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/tp_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20030 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/vad_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4282 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/vad_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11752 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/bin/vad_inference_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.471933 funasr-0.4.4/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/datasets/iterable_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12671 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/iterable_dataset_modelscope.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.474213 funasr-0.4.4/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3488 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.476467 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8055 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.484380 funasr-0.4.4/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1201 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2318 2023-04-27 08:40:56.000000 funasr-0.4.4/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.4.4/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.484829 funasr-0.4.4/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10833 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.504385 funasr-0.4.4/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5091 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.505202 funasr-0.4.4/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.4.4/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.506319 funasr-0.4.4/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.507695 funasr-0.4.4/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.4.4/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.508123 funasr-0.4.4/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.4.4/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.509454 funasr-0.4.4/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      966 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.509724 funasr-0.4.4/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.4.4/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.511144 funasr-0.4.4/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3479 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.512455 funasr-0.4.4/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.515723 funasr-0.4.4/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      359 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3503 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      349 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.516370 funasr-0.4.4/funasr/lm/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/lm/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5436 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/lm/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5904 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/lm/seq_rnn_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4243 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/lm/transformer_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.516687 funasr-0.4.4/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2804 2023-03-02 10:32:58.000000 funasr-0.4.4/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.517918 funasr-0.4.4/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5610 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5029 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.525592 funasr-0.4.4/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.4.4/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5298 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.527568 funasr-0.4.4/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7917 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    28528 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16707 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11630 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    74013 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    34815 2023-04-27 08:40:56.000000 funasr-0.4.4/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10238 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20581 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10098 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6710 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51737 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31100 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.531905 funasr-0.4.4/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      503 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43611 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20993 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.4.4/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17514 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.533196 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41077 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3634 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    54425 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.535636 funasr-0.4.4/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      400 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8895 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5759 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4990 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20471 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6322 2023-02-23 03:32:15.000000 funasr-0.4.4/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2817 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.536068 funasr-0.4.4/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.536466 funasr-0.4.4/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3546 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.537483 funasr-0.4.4/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.537815 funasr-0.4.4/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35684 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.538699 funasr-0.4.4/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/preencoder/sinc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.539518 funasr-0.4.4/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4661 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4715 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.544641 funasr-0.4.4/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    36791 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.546829 funasr-0.4.4/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/beam_search/beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.548818 funasr-0.4.4/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.4.4/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.549496 funasr-0.4.4/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.4.4/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.4.4/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.550891 funasr-0.4.4/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.4.4/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22114 2023-04-25 05:58:46.000000 funasr-0.4.4/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3649 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.552209 funasr-0.4.4/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.553080 funasr-0.4.4/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.554434 funasr-0.4.4/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.555370 funasr-0.4.4/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.555678 funasr-0.4.4/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.555856 funasr-0.4.4/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.556472 funasr-0.4.4/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.4.4/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.557013 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.558512 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.560286 funasr-0.4.4/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      617 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      740 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      932 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      383 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      969 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.561196 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8145 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12279 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.563088 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29270 2023-04-25 07:21:40.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9176 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9851 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1393 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.565390 funasr-0.4.4/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.566475 funasr-0.4.4/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.570153 funasr-0.4.4/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    73890 2023-04-23 09:14:57.000000 funasr-0.4.4/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    60627 2023-04-23 09:14:57.000000 funasr-0.4.4/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32463 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6782 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8029 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18814 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12527 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.572918 funasr-0.4.4/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.575595 funasr-0.4.4/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3815 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.578633 funasr-0.4.4/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1764 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/train/abs_espnet_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7280 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.4.4/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    36453 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.585131 funasr-0.4.4/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.4.4/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.4.4/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.4.4/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.4.4/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7735 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13178 2023-04-12 07:23:40.000000 funasr-0.4.4/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.4.4/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.4.4/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-04-27 09:38:41.000000 funasr-0.4.4/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-04-27 09:39:42.444817 funasr-0.4.4/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8336 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    12988 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      838 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-04-27 09:39:42.000000 funasr-0.4.4/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-04-27 09:39:42.585881 funasr-0.4.4/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     4573 2023-04-25 05:58:46.000000 funasr-0.4.4/setup.py
```

### Comparing `funasr-0.4.3/LICENSE` & `funasr-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/PKG-INFO` & `funasr-0.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.4.3
+Version: 0.4.4
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -41,22 +42,20 @@
 | [**Installation**](#installation)
 | [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
 | [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/modelscope_models.md)
 | [**Contact**](#contact)
-|
-[**M2MET2.0 Guidence_CN**](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)
-| [**M2MET2.0 Guidence_EN**](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)
+| [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
-## Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
-We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 ## What's new: 
-
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
+We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
+### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification and Speaker diarization.   
 - We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
 - FunASR supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
@@ -85,15 +84,15 @@
 
 ```shell
 pip install -U modelscope
 # For the users in China, you could install with the command:
 # pip install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
 ```
 
-For more details, please ref to [installation](https://github.com/alibaba-damo-academy/FunASR/wiki)
+For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation.html)
 
 [//]: # ()
 [//]: # (## Usage)
 
 [//]: # (For users who are new to FunASR and ModelScope, please refer to FunASR Docs&#40;[CN]&#40;https://alibaba-damo-academy.github.io/FunASR/cn/index.html&#41; / [EN]&#40;https://alibaba-damo-academy.github.io/FunASR/en/index.html&#41;&#41;)
 
 ## Contact
@@ -104,23 +103,25 @@
 
 |Dingding group |                     Wechat group                      |
 |:---:|:-----------------------------------------------------:|
 |<div align="left"><img src="docs/images/dingding.jpg" width="250"/> | <img src="docs/images/wechat.png" width="232"/></div> |
 
 ## Contributors
 
-| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/DeepScience.png" width="200"/> </div> |
-|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:-----------------------------------------------------------:|
+| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/DeepScience.png" width="200"/> </div> |
+|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|
 
 ## Acknowledge
 
 1. We borrowed a lot of code from [Kaldi](http://kaldi-asr.org/) for data preparation.
 2. We borrowed a lot of code from [ESPnet](https://github.com/espnet/espnet). FunASR follows up the training and finetuning pipelines of ESPnet.
 3. We referred [Wenet](https://github.com/wenet-e2e/wenet) for building dataloader for large scale data training.
-4. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
+4. We acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for contributing the VAD runtime. 
+5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
+6. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 
 ## Citations
 
 ``` bibtex
@@ -139,7 +140,9 @@
 @inproceedings{Shi2023AchievingTP,
   title={Achieving Timestamp Prediction While Recognizing with Non-Autoregressive End-to-End ASR Model},
   author={Xian Shi and Yanni Chen and Shiliang Zhang and Zhijie Yan},
   booktitle={arXiv preprint arXiv:2301.12343}
   year={2023}
 }
 ```
+
+
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.4.3 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.4.4 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
-System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
-Provides-Extra: train Provides-Extra: recipe Provides-Extra: all Provides-
-Extra: test Provides-Extra: doc License-File: LICENSE [//]: # (
+License Platform: UNKNOWN Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
+Research Classifier: Operating System :: POSIX :: Linux Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown Provides-Extra: train Provides-Extra:
+recipe Provides-Extra: all Provides-Extra: test Provides-Extra: doc License-
+File: LICENSE [//]: # (
 [docs/images/funasr_logo.jpg]
 ) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
@@ -27,76 +28,83 @@
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html) |
 [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/
 wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
 github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
 github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
 Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
-modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Guidence_CN**]
-(https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html) |
-[**M2MET2.0 Guidence_EN**](https://alibaba-damo-academy.github.io/FunASR/
-m2met2/index.html) ## Multi-Channel Multi-Party Meeting Transcription 2.0
-(M2MET2.0) Challenge We are pleased to announce that the M2MeT2.0 challenge
-will be held in the near future. The baseline system is conducted on FunASR and
-is provided as a receipe of AliMeeting corpus. For more details you can see the
-guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/
-m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/
-m2met2/index.html)). ## What's new: For the release notes, please ref to [news]
-(https://github.com/alibaba-damo-academy/FunASR/releases) ## Highlights -
-FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity
-Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification
-and Speaker diarization. - We have released large number of academic and
-industrial pretrained models on [ModelScope](https://www.modelscope.cn/
-models?page=1&tasks=auto-speech-recognition) - The pretrained model
-[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best
-performance on many tasks in [SpeechIO leaderboard](https://github.com/
-SpeechColab/Leaderboard) - FunASR supplies a easy-to-use pipeline to finetune
-pretrained models from [ModelScope](https://www.modelscope.cn/
-models?page=1&tasks=auto-speech-recognition) - Compared to [Espnet](https://
-github.com/espnet/espnet) framework, the training speed of large-scale datasets
-in FunASR is much faster owning to the optimized dataloader. ## Installation
-Install from pip ```shell pip install -U funasr # For the users in China, you
-could install with the command: # pip install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
-For the users in China, you could install with the command: # pip install -e ./
--i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip install -U modelscope # For the users in China, you could install with the
-command: # pip install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://github.com/
-alibaba-damo-academy/FunASR/wiki) [//]: # () [//]: # (## Usage) [//]: # (For
-users who are new to FunASR and ModelScope, please refer to FunASR Docs([CN]
-(https://alibaba-damo-academy.github.io/FunASR/cn/index.html) / [EN](https://
-alibaba-damo-academy.github.io/FunASR/en/index.html))) ## Contact If you have
-any questions about FunASR, please contact us by - email: [funasr@list.alibaba-
-inc.com](funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:
------------------------------------------------------:| |
+modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
+(https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
+meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
+Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge We are pleased to
+announce that the M2MeT2.0 challenge will be held in the near future. The
+baseline system is conducted on FunASR and is provided as a receipe of
+AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN]
+(https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN]
+(https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release
+notes For the release notes, please ref to [news](https://github.com/alibaba-
+damo-academy/FunASR/releases) ## Highlights - FunASR supports speech
+recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation
+Restoration, Language Models, Speaker Verification and Speaker diarization. -
+We have released large number of academic and industrial pretrained models on
+[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
+recognition) - The pretrained model [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) obtains the best performance on many tasks in
+[SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard) - FunASR
+supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope]
+(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition) -
+Compared to [Espnet](https://github.com/espnet/espnet) framework, the training
+speed of large-scale datasets in FunASR is much faster owning to the optimized
+dataloader. ## Installation Install from pip ```shell pip install -U funasr #
+For the users in China, you could install with the command: # pip install -
+U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from
+source code ``` sh git clone https://github.com/alibaba/FunASR.git && cd FunASR
+pip install -e ./ # For the users in China, you could install with the command:
+# pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you
+want to use the pretrained models in ModelScope, you should install the
+modelscope: ```shell pip install -U modelscope # For the users in China, you
+could install with the command: # pip install -U modelscope -f https://
+modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/
+installation.html) [//]: # () [//]: # (## Usage) [//]: # (For users who are new
+to FunASR and ModelScope, please refer to FunASR Docs([CN](https://alibaba-
+damo-academy.github.io/FunASR/cn/index.html) / [EN](https://alibaba-damo-
+academy.github.io/FunASR/en/index.html))) ## Contact If you have any questions
+about FunASR, please contact us by - email: [funasr@list.alibaba-inc.com]
+(funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:--------
+---------------------------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
-[docs/images/nwpu.png] | [docs/images/DeepScience.png]
+[docs/images/nwpu.png] | [docs/images/China_Telecom.png]
+| [docs/images/RapidAI.png]
+| [docs/images/DeepScience.png]
 | |:---------------------------------------------------------------:|:---------
 ------------------------------------------------------:|:----------------------
--------------------------------------:| ## Acknowledge 1. We borrowed a lot of
-code from [Kaldi](http://kaldi-asr.org/) for data preparation. 2. We borrowed a
-lot of code from [ESPnet](https://github.com/espnet/espnet). FunASR follows up
-the training and finetuning pipelines of ESPnet. 3. We referred [Wenet](https:/
-/github.com/wenet-e2e/wenet) for building dataloader for large scale data
-training. 4. We acknowledge [DeepScience](https://www.deepscience.cn) for
-contributing the grpc service. ## License This project is licensed under the
-[The MIT License](https://opensource.org/licenses/MIT). FunASR also contains
-various third-party components and some code modified from other repos under
-other open source licenses. ## Citations ``` bibtex @inproceedings
-{gao2022paraformer, title={Paraformer: Fast and Accurate Parallel Transformer
-for Non-autoregressive End-to-End Speech Recognition}, author={Gao, Zhifu and
-Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie}, booktitle={INTERSPEECH},
-year={2022} } @inproceedings{gao2020universal, title={Universal ASR: Unifying
-Streaming and Non-Streaming ASR Using a Single Encoder-Decoder Model}, author=
-{Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin, Ian}, booktitle=
-{arXiv preprint arXiv:2010.14099}, year={2020} } @inproceedings
+----------------------------------------:|:------------------------------------
+-------------------:|:---------------------------------------------------------
+--:| ## Acknowledge 1. We borrowed a lot of code from [Kaldi](http://kaldi-
+asr.org/) for data preparation. 2. We borrowed a lot of code from [ESPnet]
+(https://github.com/espnet/espnet). FunASR follows up the training and
+finetuning pipelines of ESPnet. 3. We referred [Wenet](https://github.com/
+wenet-e2e/wenet) for building dataloader for large scale data training. 4. We
+acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-
+httpserver) for contributing the VAD runtime. 5. We acknowledge [RapidAI]
+(https://github.com/RapidAI) for contributing the Paraformer and
+CT_Transformer-punc runtime. 6. We acknowledge [DeepScience](https://
+www.deepscience.cn) for contributing the grpc service. ## License This project
+is licensed under the [The MIT License](https://opensource.org/licenses/MIT).
+FunASR also contains various third-party components and some code modified from
+other repos under other open source licenses. ## Citations ``` bibtex
+@inproceedings{gao2022paraformer, title={Paraformer: Fast and Accurate Parallel
+Transformer for Non-autoregressive End-to-End Speech Recognition}, author={Gao,
+Zhifu and Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie}, booktitle=
+{INTERSPEECH}, year={2022} } @inproceedings{gao2020universal, title={Universal
+ASR: Unifying Streaming and Non-Streaming ASR Using a Single Encoder-Decoder
+Model}, author={Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin,
+Ian}, booktitle={arXiv preprint arXiv:2010.14099}, year={2020} } @inproceedings
 {Shi2023AchievingTP, title={Achieving Timestamp Prediction While Recognizing
 with Non-Autoregressive End-to-End ASR Model}, author={Xian Shi and Yanni Chen
 and Shiliang Zhang and Zhijie Yan}, booktitle={arXiv preprint arXiv:2301.12343}
 year={2023} } ```
```

### Comparing `funasr-0.4.3/README.md` & `funasr-0.4.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,20 @@
 | [**Installation**](#installation)
 | [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
 | [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/modelscope_models.md)
 | [**Contact**](#contact)
-|
-[**M2MET2.0 Guidence_CN**](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)
-| [**M2MET2.0 Guidence_EN**](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)
+| [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
-## Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
-We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 ## What's new: 
-
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
+We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
+### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification and Speaker diarization.   
 - We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
 - FunASR supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
@@ -58,15 +56,15 @@
 
 ```shell
 pip install -U modelscope
 # For the users in China, you could install with the command:
 # pip install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
 ```
 
-For more details, please ref to [installation](https://github.com/alibaba-damo-academy/FunASR/wiki)
+For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation.html)
 
 [//]: # ()
 [//]: # (## Usage)
 
 [//]: # (For users who are new to FunASR and ModelScope, please refer to FunASR Docs&#40;[CN]&#40;https://alibaba-damo-academy.github.io/FunASR/cn/index.html&#41; / [EN]&#40;https://alibaba-damo-academy.github.io/FunASR/en/index.html&#41;&#41;)
 
 ## Contact
@@ -77,23 +75,25 @@
 
 |Dingding group |                     Wechat group                      |
 |:---:|:-----------------------------------------------------:|
 |<div align="left"><img src="docs/images/dingding.jpg" width="250"/> | <img src="docs/images/wechat.png" width="232"/></div> |
 
 ## Contributors
 
-| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/DeepScience.png" width="200"/> </div> |
-|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:-----------------------------------------------------------:|
+| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/DeepScience.png" width="200"/> </div> |
+|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|
 
 ## Acknowledge
 
 1. We borrowed a lot of code from [Kaldi](http://kaldi-asr.org/) for data preparation.
 2. We borrowed a lot of code from [ESPnet](https://github.com/espnet/espnet). FunASR follows up the training and finetuning pipelines of ESPnet.
 3. We referred [Wenet](https://github.com/wenet-e2e/wenet) for building dataloader for large scale data training.
-4. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
+4. We acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for contributing the VAD runtime. 
+5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
+6. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 
 ## Citations
 
 ``` bibtex
```

#### html2text {}

```diff
@@ -14,76 +14,83 @@
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html) |
 [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/
 wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
 github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
 github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
 Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
-modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Guidence_CN**]
-(https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html) |
-[**M2MET2.0 Guidence_EN**](https://alibaba-damo-academy.github.io/FunASR/
-m2met2/index.html) ## Multi-Channel Multi-Party Meeting Transcription 2.0
-(M2MET2.0) Challenge We are pleased to announce that the M2MeT2.0 challenge
-will be held in the near future. The baseline system is conducted on FunASR and
-is provided as a receipe of AliMeeting corpus. For more details you can see the
-guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/
-m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/
-m2met2/index.html)). ## What's new: For the release notes, please ref to [news]
-(https://github.com/alibaba-damo-academy/FunASR/releases) ## Highlights -
-FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity
-Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification
-and Speaker diarization. - We have released large number of academic and
-industrial pretrained models on [ModelScope](https://www.modelscope.cn/
-models?page=1&tasks=auto-speech-recognition) - The pretrained model
-[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best
-performance on many tasks in [SpeechIO leaderboard](https://github.com/
-SpeechColab/Leaderboard) - FunASR supplies a easy-to-use pipeline to finetune
-pretrained models from [ModelScope](https://www.modelscope.cn/
-models?page=1&tasks=auto-speech-recognition) - Compared to [Espnet](https://
-github.com/espnet/espnet) framework, the training speed of large-scale datasets
-in FunASR is much faster owning to the optimized dataloader. ## Installation
-Install from pip ```shell pip install -U funasr # For the users in China, you
-could install with the command: # pip install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
-For the users in China, you could install with the command: # pip install -e ./
--i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip install -U modelscope # For the users in China, you could install with the
-command: # pip install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://github.com/
-alibaba-damo-academy/FunASR/wiki) [//]: # () [//]: # (## Usage) [//]: # (For
-users who are new to FunASR and ModelScope, please refer to FunASR Docs([CN]
-(https://alibaba-damo-academy.github.io/FunASR/cn/index.html) / [EN](https://
-alibaba-damo-academy.github.io/FunASR/en/index.html))) ## Contact If you have
-any questions about FunASR, please contact us by - email: [funasr@list.alibaba-
-inc.com](funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:
------------------------------------------------------:| |
+modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
+(https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
+meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
+Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge We are pleased to
+announce that the M2MeT2.0 challenge will be held in the near future. The
+baseline system is conducted on FunASR and is provided as a receipe of
+AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN]
+(https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN]
+(https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release
+notes For the release notes, please ref to [news](https://github.com/alibaba-
+damo-academy/FunASR/releases) ## Highlights - FunASR supports speech
+recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation
+Restoration, Language Models, Speaker Verification and Speaker diarization. -
+We have released large number of academic and industrial pretrained models on
+[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
+recognition) - The pretrained model [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) obtains the best performance on many tasks in
+[SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard) - FunASR
+supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope]
+(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition) -
+Compared to [Espnet](https://github.com/espnet/espnet) framework, the training
+speed of large-scale datasets in FunASR is much faster owning to the optimized
+dataloader. ## Installation Install from pip ```shell pip install -U funasr #
+For the users in China, you could install with the command: # pip install -
+U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from
+source code ``` sh git clone https://github.com/alibaba/FunASR.git && cd FunASR
+pip install -e ./ # For the users in China, you could install with the command:
+# pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you
+want to use the pretrained models in ModelScope, you should install the
+modelscope: ```shell pip install -U modelscope # For the users in China, you
+could install with the command: # pip install -U modelscope -f https://
+modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/
+installation.html) [//]: # () [//]: # (## Usage) [//]: # (For users who are new
+to FunASR and ModelScope, please refer to FunASR Docs([CN](https://alibaba-
+damo-academy.github.io/FunASR/cn/index.html) / [EN](https://alibaba-damo-
+academy.github.io/FunASR/en/index.html))) ## Contact If you have any questions
+about FunASR, please contact us by - email: [funasr@list.alibaba-inc.com]
+(funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:--------
+---------------------------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
-[docs/images/nwpu.png] | [docs/images/DeepScience.png]
+[docs/images/nwpu.png] | [docs/images/China_Telecom.png]
+| [docs/images/RapidAI.png]
+| [docs/images/DeepScience.png]
 | |:---------------------------------------------------------------:|:---------
 ------------------------------------------------------:|:----------------------
--------------------------------------:| ## Acknowledge 1. We borrowed a lot of
-code from [Kaldi](http://kaldi-asr.org/) for data preparation. 2. We borrowed a
-lot of code from [ESPnet](https://github.com/espnet/espnet). FunASR follows up
-the training and finetuning pipelines of ESPnet. 3. We referred [Wenet](https:/
-/github.com/wenet-e2e/wenet) for building dataloader for large scale data
-training. 4. We acknowledge [DeepScience](https://www.deepscience.cn) for
-contributing the grpc service. ## License This project is licensed under the
-[The MIT License](https://opensource.org/licenses/MIT). FunASR also contains
-various third-party components and some code modified from other repos under
-other open source licenses. ## Citations ``` bibtex @inproceedings
-{gao2022paraformer, title={Paraformer: Fast and Accurate Parallel Transformer
-for Non-autoregressive End-to-End Speech Recognition}, author={Gao, Zhifu and
-Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie}, booktitle={INTERSPEECH},
-year={2022} } @inproceedings{gao2020universal, title={Universal ASR: Unifying
-Streaming and Non-Streaming ASR Using a Single Encoder-Decoder Model}, author=
-{Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin, Ian}, booktitle=
-{arXiv preprint arXiv:2010.14099}, year={2020} } @inproceedings
+----------------------------------------:|:------------------------------------
+-------------------:|:---------------------------------------------------------
+--:| ## Acknowledge 1. We borrowed a lot of code from [Kaldi](http://kaldi-
+asr.org/) for data preparation. 2. We borrowed a lot of code from [ESPnet]
+(https://github.com/espnet/espnet). FunASR follows up the training and
+finetuning pipelines of ESPnet. 3. We referred [Wenet](https://github.com/
+wenet-e2e/wenet) for building dataloader for large scale data training. 4. We
+acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-
+httpserver) for contributing the VAD runtime. 5. We acknowledge [RapidAI]
+(https://github.com/RapidAI) for contributing the Paraformer and
+CT_Transformer-punc runtime. 6. We acknowledge [DeepScience](https://
+www.deepscience.cn) for contributing the grpc service. ## License This project
+is licensed under the [The MIT License](https://opensource.org/licenses/MIT).
+FunASR also contains various third-party components and some code modified from
+other repos under other open source licenses. ## Citations ``` bibtex
+@inproceedings{gao2022paraformer, title={Paraformer: Fast and Accurate Parallel
+Transformer for Non-autoregressive End-to-End Speech Recognition}, author={Gao,
+Zhifu and Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie}, booktitle=
+{INTERSPEECH}, year={2022} } @inproceedings{gao2020universal, title={Universal
+ASR: Unifying Streaming and Non-Streaming ASR Using a Single Encoder-Decoder
+Model}, author={Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin,
+Ian}, booktitle={arXiv preprint arXiv:2010.14099}, year={2020} } @inproceedings
 {Shi2023AchievingTP, title={Achieving Timestamp Prediction While Recognizing
 with Non-Autoregressive End-to-End ASR Model}, author={Xian Shi and Yanni Chen
 and Shiliang Zhang and Zhijie Yan}, booktitle={arXiv preprint arXiv:2301.12343}
 year={2023} } ```
```

### Comparing `funasr-0.4.3/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.4.4/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_inference.py` & `funasr-0.4.4/funasr/bin/asr_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_inference_launch.py` & `funasr-0.4.4/funasr/bin/asr_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_inference_mfcca.py` & `funasr-0.4.4/funasr/bin/asr_inference_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_inference_paraformer.py` & `funasr-0.4.4/funasr/bin/asr_inference_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_inference_paraformer_streaming.py` & `funasr-0.4.4/funasr/bin/asr_inference_paraformer_vad_punc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!/usr/bin/env python3
+
+import json
 import argparse
 import logging
 import sys
 import time
-import copy
 import os
 import codecs
 import tempfile
 import requests
 from pathlib import Path
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import Dict
 from typing import Any
 from typing import List
-
+import math
+import copy
 import numpy as np
 import torch
-import torchaudio
 from typeguard import check_argument_types
 
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
 from funasr.modules.beam_search.beam_search import Hypothesis
 from funasr.modules.scorers.ctc import CTCPrefixScorer
 from funasr.modules.scorers.length_bonus import LengthBonus
@@ -37,24 +38,31 @@
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
 from funasr.models.frontend.wav_frontend import WavFrontend
+from funasr.tasks.vad import VADTask
+from funasr.bin.vad_inference import Speech2VadSegment
+from funasr.utils.timestamp_tools import time_stamp_sentence, ts_prediction_lfr6_standard
+from funasr.bin.punctuation_infer import Text2Punc
 from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
-from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
-np.set_printoptions(threshold=np.inf)
+
+
+header_colors = '\033[95m'
+end_colors = '\033[0m'
+
 
 class Speech2Text:
     """Speech2Text class
 
     Examples:
             >>> import soundfile
-            >>> speech2text = Speech2Text("asr_config.yml", "asr.pth")
+            >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
             >>> audio, rate = soundfile.read("speech.wav")
             >>> speech2text(audio)
             [(text, token, token_int, hypothesis object), ...]
 
     """
 
     def __init__(
@@ -81,22 +89,22 @@
             **kwargs,
     ):
         assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
+            asr_train_config, asr_model_file, cmvn_file=cmvn_file, device=device
         )
         frontend = None
-        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
+        if asr_model.frontend is not None and asr_train_args.frontend_conf is not None:
             frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
 
-        logging.info("asr_model: {}".format(asr_model))
-        logging.info("asr_train_args: {}".format(asr_train_args))
+        # logging.info("asr_model: {}".format(asr_model))
+        # logging.info("asr_train_args: {}".format(asr_train_args))
         asr_model.to(dtype=getattr(torch, dtype)).eval()
 
         if asr_model.ctc != None:
             ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
             scorers.update(
                 ctc=ctc
             )
@@ -166,34 +174,36 @@
 
         self.asr_model = asr_model
         self.asr_train_args = asr_train_args
         self.converter = converter
         self.tokenizer = tokenizer
 
         # 6. [Optional] Build hotword list from str, local file or url
+        self.hotword_list = None
+        self.hotword_list = self.generate_hotwords_list(hotword_list_or_file)
 
         is_use_lm = lm_weight != 0.0 and lm_file is not None
         if (ctc_weight == 0.0 or asr_model.ctc == None) and not is_use_lm:
             beam_search = None
         self.beam_search = beam_search
         logging.info(f"Beam_search: {self.beam_search}")
         self.beam_search_transducer = beam_search_transducer
         self.maxlenratio = maxlenratio
         self.minlenratio = minlenratio
         self.device = device
         self.dtype = dtype
         self.nbest = nbest
         self.frontend = frontend
         self.encoder_downsampling_factor = 1
-        if asr_train_args.encoder == "data2vec_encoder" or asr_train_args.encoder_conf["input_layer"] == "conv2d":
+        if asr_train_args.encoder_conf["input_layer"] == "conv2d":
             self.encoder_downsampling_factor = 4
 
     @torch.no_grad()
     def __call__(
-            self, cache: dict, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
+            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
             begin_time: int = 0, end_time: int = None,
     ):
         """Inference
 
         Args:
                 speech: Input speech data
         Returns:
@@ -201,46 +211,57 @@
 
         """
         assert check_argument_types()
 
         # Input as audio signal
         if isinstance(speech, np.ndarray):
             speech = torch.tensor(speech)
+
         if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
+            # feats, feats_len = self.frontend.forward(speech, speech_lengths)
+            # fbanks, fbanks_len = self.frontend.forward_fbank(speech, speech_lengths)
+            feats, feats_len = self.frontend.forward_lfr_cmvn(speech, speech_lengths)
             feats = to_device(feats, device=self.device)
             feats_len = feats_len.int()
             self.asr_model.frontend = None
         else:
             feats = speech
             feats_len = speech_lengths
         lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
-        feats_len = cache["encoder"]["stride"] + cache["encoder"]["pad_left"] + cache["encoder"]["pad_right"]
-        feats = feats[:,cache["encoder"]["start_idx"]:cache["encoder"]["start_idx"]+feats_len,:]
-        feats_len = torch.tensor([feats_len])
-        batch = {"speech": feats, "speech_lengths": feats_len, "cache": cache}
+        batch = {"speech": feats, "speech_lengths": feats_len}
 
         # a. To device
         batch = to_device(batch, device=self.device)
 
         # b. Forward Encoder
-        enc, enc_len = self.asr_model.encode_chunk(feats, feats_len, cache)
+        enc, enc_len = self.asr_model.encode(**batch)
         if isinstance(enc, tuple):
             enc = enc[0]
         # assert len(enc) == 1, len(enc)
         enc_len_batch_total = torch.sum(enc_len).item() * self.encoder_downsampling_factor
 
-        predictor_outs = self.asr_model.calc_predictor_chunk(enc, cache)
+        predictor_outs = self.asr_model.calc_predictor(enc, enc_len)
         pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = predictor_outs[0], predictor_outs[1], \
                                                                         predictor_outs[2], predictor_outs[3]
-        pre_token_length = pre_token_length.floor().long()
+        pre_token_length = pre_token_length.round().long()
         if torch.max(pre_token_length) < 1:
             return []
-        decoder_outs = self.asr_model.cal_decoder_with_predictor_chunk(enc, pre_acoustic_embeds, cache)
-        decoder_out = decoder_outs
+
+        if not isinstance(self.asr_model, ContextualParaformer):
+            if self.hotword_list:
+                logging.warning("Hotword is given but asr model is not a ContextualParaformer.")
+            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length)
+            decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
+        else:
+            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length, hw_list=self.hotword_list)
+            decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
+
+        if isinstance(self.asr_model, BiCifParaformer):
+            _, _, us_alphas, us_peaks = self.asr_model.calc_predictor_timestamp(enc, enc_len,
+                                                                                   pre_token_length)  # test no bias cif2
 
         results = []
         b, n, d = decoder_out.size()
         for i in range(b):
             x = enc[i, :enc_len[i], :]
             am_scores = decoder_out[i, :pre_token_length[i], :]
             if self.beam_search is not None:
@@ -267,180 +288,90 @@
                 if isinstance(hyp.yseq, list):
                     token_int = hyp.yseq[1:last_pos]
                 else:
                     token_int = hyp.yseq[1:last_pos].tolist()
 
                 # remove blank symbol id, which is assumed to be 0
                 token_int = list(filter(lambda x: x != 0 and x != 2, token_int))
+                if len(token_int) == 0:
+                    continue
 
                 # Change integer-ids to tokens
                 token = self.converter.ids2tokens(token_int)
 
                 if self.tokenizer is not None:
                     text = self.tokenizer.tokens2text(token)
                 else:
                     text = None
 
-                results.append((text, token, token_int, hyp, enc_len_batch_total, lfr_factor))
+                if isinstance(self.asr_model, BiCifParaformer):
+                    _, timestamp = ts_prediction_lfr6_standard(us_alphas[i], 
+                                                            us_peaks[i], 
+                                                            copy.copy(token), 
+                                                            vad_offset=begin_time)
+                    results.append((text, token, token_int, timestamp, enc_len_batch_total, lfr_factor))
+                else:
+                    results.append((text, token, token_int, enc_len_batch_total, lfr_factor))
 
         # assert check_return_type(results)
         return results
 
-
-class Speech2TextExport:
-    """Speech2TextExport class
-
-    """
-
-    def __init__(
-            self,
-            asr_train_config: Union[Path, str] = None,
-            asr_model_file: Union[Path, str] = None,
-            cmvn_file: Union[Path, str] = None,
-            lm_train_config: Union[Path, str] = None,
-            lm_file: Union[Path, str] = None,
-            token_type: str = None,
-            bpemodel: str = None,
-            device: str = "cpu",
-            maxlenratio: float = 0.0,
-            minlenratio: float = 0.0,
-            dtype: str = "float32",
-            beam_size: int = 20,
-            ctc_weight: float = 0.5,
-            lm_weight: float = 1.0,
-            ngram_weight: float = 0.9,
-            penalty: float = 0.0,
-            nbest: int = 1,
-            frontend_conf: dict = None,
-            hotword_list_or_file: str = None,
-            **kwargs,
-    ):
-
-        # 1. Build ASR model
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file, device
-        )
-        frontend = None
-        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
-
-        logging.info("asr_model: {}".format(asr_model))
-        logging.info("asr_train_args: {}".format(asr_train_args))
-        asr_model.to(dtype=getattr(torch, dtype)).eval()
-
-        token_list = asr_model.token_list
-
-        logging.info(f"Decoding device={device}, dtype={dtype}")
-
-        # 5. [Optional] Build Text converter: e.g. bpe-sym -> Text
-        if token_type is None:
-            token_type = asr_train_args.token_type
-        if bpemodel is None:
-            bpemodel = asr_train_args.bpemodel
-
-        if token_type is None:
-            tokenizer = None
-        elif token_type == "bpe":
-            if bpemodel is not None:
-                tokenizer = build_tokenizer(token_type=token_type, bpemodel=bpemodel)
-            else:
-                tokenizer = None
-        else:
-            tokenizer = build_tokenizer(token_type=token_type)
-        converter = TokenIDConverter(token_list=token_list)
-        logging.info(f"Text tokenizer: {tokenizer}")
-
-        # self.asr_model = asr_model
-        self.asr_train_args = asr_train_args
-        self.converter = converter
-        self.tokenizer = tokenizer
-
-        self.device = device
-        self.dtype = dtype
-        self.nbest = nbest
-        self.frontend = frontend
-
-        model = Paraformer_export(asr_model, onnx=False)
-        self.asr_model = model
-
-    @torch.no_grad()
-    def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None
-    ):
-        """Inference
-
-        Args:
-                speech: Input speech data
-        Returns:
-                text, token, token_int, hyp
-
-        """
-        assert check_argument_types()
-
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-
-        if self.frontend is not None:
-            feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            self.asr_model.frontend = None
+    def generate_hotwords_list(self, hotword_list_or_file):
+        # for None
+        if hotword_list_or_file is None:
+            hotword_list = None
+        # for local txt inputs
+        elif os.path.exists(hotword_list_or_file) and hotword_list_or_file.endswith('.txt'):
+            logging.info("Attempting to parse hotwords from local txt...")
+            hotword_list = []
+            hotword_str_list = []
+            with codecs.open(hotword_list_or_file, 'r') as fin:
+                for line in fin.readlines():
+                    hw = line.strip()
+                    hotword_str_list.append(hw)
+                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
+                hotword_list.append([self.asr_model.sos])
+                hotword_str_list.append('<s>')
+            logging.info("Initialized hotword list from file: {}, hotword list: {}."
+                         .format(hotword_list_or_file, hotword_str_list))
+        # for url, download and generate txt
+        elif hotword_list_or_file.startswith('http'):
+            logging.info("Attempting to parse hotwords from url...")
+            work_dir = tempfile.TemporaryDirectory().name
+            if not os.path.exists(work_dir):
+                os.makedirs(work_dir)
+            text_file_path = os.path.join(work_dir, os.path.basename(hotword_list_or_file))
+            local_file = requests.get(hotword_list_or_file)
+            open(text_file_path, "wb").write(local_file.content)
+            hotword_list_or_file = text_file_path
+            hotword_list = []
+            hotword_str_list = []
+            with codecs.open(hotword_list_or_file, 'r') as fin:
+                for line in fin.readlines():
+                    hw = line.strip()
+                    hotword_str_list.append(hw)
+                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
+                hotword_list.append([self.asr_model.sos])
+                hotword_str_list.append('<s>')
+            logging.info("Initialized hotword list from file: {}, hotword list: {}."
+                         .format(hotword_list_or_file, hotword_str_list))
+        # for text str input
+        elif not hotword_list_or_file.endswith('.txt'):
+            logging.info("Attempting to parse hotwords as str...")
+            hotword_list = []
+            hotword_str_list = []
+            for hw in hotword_list_or_file.strip().split():
+                hotword_str_list.append(hw)
+                hotword_list.append(self.converter.tokens2ids([i for i in hw]))
+            hotword_list.append([self.asr_model.sos])
+            hotword_str_list.append('<s>')
+            logging.info("Hotword list: {}.".format(hotword_str_list))
         else:
-            feats = speech
-            feats_len = speech_lengths
-
-        enc_len_batch_total = feats_len.sum()
-        lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
-        batch = {"speech": feats, "speech_lengths": feats_len}
-
-        # a. To device
-        batch = to_device(batch, device=self.device)
-
-        decoder_outs = self.asr_model(**batch)
-        decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
-
-        results = []
-        b, n, d = decoder_out.size()
-        for i in range(b):
-            am_scores = decoder_out[i, :ys_pad_lens[i], :]
-
-            yseq = am_scores.argmax(dim=-1)
-            score = am_scores.max(dim=-1)[0]
-            score = torch.sum(score, dim=-1)
-            # pad with mask tokens to ensure compatibility with sos/eos tokens
-            yseq = torch.tensor(
-                yseq.tolist(), device=yseq.device
-            )
-            nbest_hyps = [Hypothesis(yseq=yseq, score=score)]
-
-            for hyp in nbest_hyps:
-                assert isinstance(hyp, (Hypothesis)), type(hyp)
-
-                # remove sos/eos and get results
-                last_pos = -1
-                if isinstance(hyp.yseq, list):
-                    token_int = hyp.yseq[1:last_pos]
-                else:
-                    token_int = hyp.yseq[1:last_pos].tolist()
-
-                # remove blank symbol id, which is assumed to be 0
-                token_int = list(filter(lambda x: x != 0 and x != 2, token_int))
-
-                # Change integer-ids to tokens
-                token = self.converter.ids2tokens(token_int)
-
-                if self.tokenizer is not None:
-                    text = self.tokenizer.tokens2text(token)
-                else:
-                    text = None
-
-                results.append((text, token, token_int, hyp, enc_len_batch_total, lfr_factor))
-
-        return results
+            hotword_list = None
+        return hotword_list
 
 
 def inference(
         maxlenratio: float,
         minlenratio: float,
         batch_size: int,
         beam_size: int,
@@ -464,15 +395,20 @@
         streaming: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
-
+        vad_infer_config: Optional[str] = None,
+        vad_model_file: Optional[str] = None,
+        vad_cmvn_file: Optional[str] = None,
+        time_stamp_writer: bool = False,
+        punc_infer_config: Optional[str] = None,
+        punc_model_file: Optional[str] = None,
         **kwargs,
 ):
     inference_pipeline = inference_modelscope(
         maxlenratio=maxlenratio,
         minlenratio=minlenratio,
         batch_size=batch_size,
         beam_size=beam_size,
@@ -495,15 +431,20 @@
         streaming=streaming,
         output_dir=output_dir,
         dtype=dtype,
         seed=seed,
         ngram_weight=ngram_weight,
         nbest=nbest,
         num_workers=num_workers,
-
+        vad_infer_config=vad_infer_config,
+        vad_model_file=vad_model_file,
+        vad_cmvn_file=vad_cmvn_file,
+        time_stamp_writer=time_stamp_writer,
+        punc_infer_config=punc_infer_config,
+        punc_model_file=punc_model_file,
         **kwargs,
     )
     return inference_pipeline(data_path_and_name_and_type, raw_inputs)
 
 
 def inference_modelscope(
         maxlenratio: float,
@@ -522,20 +463,27 @@
         lm_train_config: Optional[str] = None,
         lm_file: Optional[str] = None,
         token_type: Optional[str] = None,
         key_file: Optional[str] = None,
         word_lm_train_config: Optional[str] = None,
         bpemodel: Optional[str] = None,
         allow_variable_data_keys: bool = False,
+        output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
-        output_dir: Optional[str] = None,
+        vad_infer_config: Optional[str] = None,
+        vad_model_file: Optional[str] = None,
+        vad_cmvn_file: Optional[str] = None,
+        time_stamp_writer: bool = True,
+        punc_infer_config: Optional[str] = None,
+        punc_model_file: Optional[str] = None,
+        outputs_dict: Optional[bool] = True,
         param_dict: dict = None,
         **kwargs,
 ):
     assert check_argument_types()
     ncpu = kwargs.get("ncpu", 1)
     torch.set_num_threads(ncpu)
 
@@ -545,26 +493,39 @@
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
-    export_mode = False
+    if param_dict is not None:
+        hotword_list_or_file = param_dict.get('hotword')
+    else:
+        hotword_list_or_file = None
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
-        batch_size = 1
 
     # 1. Set random-seed
     set_all_random_seed(seed)
 
-    # 2. Build speech2text
+    # 2. Build speech2vadsegment
+    speech2vadsegment_kwargs = dict(
+        vad_infer_config=vad_infer_config,
+        vad_model_file=vad_model_file,
+        vad_cmvn_file=vad_cmvn_file,
+        device=device,
+        dtype=dtype,
+    )
+    # logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
+    speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
+
+    # 3. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
         token_type=token_type,
@@ -575,162 +536,152 @@
         dtype=dtype,
         beam_size=beam_size,
         ctc_weight=ctc_weight,
         lm_weight=lm_weight,
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
+        hotword_list_or_file=hotword_list_or_file,
     )
-    if export_mode:
-        speech2text = Speech2TextExport(**speech2text_kwargs)
-    else:
-        speech2text = Speech2Text(**speech2text_kwargs)
-        
-    def _load_bytes(input):
-        middle_data = np.frombuffer(input, dtype=np.int16)
-        middle_data = np.asarray(middle_data)
-        if middle_data.dtype.kind not in 'iu':
-            raise TypeError("'middle_data' must be an array of integers")
-        dtype = np.dtype('float32')
-        if dtype.kind != 'f':
-            raise TypeError("'dtype' must be a floating point type")
-
-        i = np.iinfo(middle_data.dtype)
-        abs_max = 2 ** (i.bits - 1)
-        offset = i.min + abs_max
-        array = np.frombuffer((middle_data.astype(dtype) - offset) / abs_max, dtype=np.float32)
-        return array
-    
-    def _forward(
-            data_path_and_name_and_type,
-            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-            output_dir_v2: Optional[str] = None,
-            fs: dict = None,
-            param_dict: dict = None,
-            **kwargs,
-    ):
+    speech2text = Speech2Text(**speech2text_kwargs)
+    text2punc = None
+    if punc_model_file is not None:
+        text2punc = Text2Punc(punc_infer_config, punc_model_file, device=device, dtype=dtype)
+
+    if output_dir is not None:
+        writer = DatadirWriter(output_dir)
+        ibest_writer = writer[f"1best_recog"]
+        ibest_writer["token_list"][""] = " ".join(speech2text.asr_train_args.token_list)
+
+    def _forward(data_path_and_name_and_type,
+                 raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+                 output_dir_v2: Optional[str] = None,
+                 fs: dict = None,
+                 param_dict: dict = None,
+                 **kwargs,
+                 ):
+
+        hotword_list_or_file = None
+        if param_dict is not None:
+            hotword_list_or_file = param_dict.get('hotword')
+
+        if 'hotword' in kwargs:
+            hotword_list_or_file = kwargs['hotword']
+
+        if speech2text.hotword_list is None:
+            speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
 
         # 3. Build data-iterator
-        is_final = False
-        cache = {}
-        if param_dict is not None and "cache" in param_dict:
-            cache = param_dict["cache"]
-        if param_dict is not None and "is_final" in param_dict:
-            is_final = param_dict["is_final"]
-
-        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "bytes":
-            raw_inputs = _load_bytes(data_path_and_name_and_type[0])
-            raw_inputs = torch.tensor(raw_inputs)
-        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "sound":
-            raw_inputs = torchaudio.load(data_path_and_name_and_type[0])[0][0]
-            is_final = True
         if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, np.ndarray):
-                raw_inputs = torch.tensor(raw_inputs)
+            if isinstance(raw_inputs, torch.Tensor):
+                raw_inputs = raw_inputs.numpy()
+            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
+        loader = ASRTask.build_streaming_iterator(
+            data_path_and_name_and_type,
+            dtype=dtype,
+            fs=fs,
+            batch_size=1,
+            key_file=key_file,
+            num_workers=num_workers,
+            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
+            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
+            allow_variable_data_keys=allow_variable_data_keys,
+            inference=True,
+        )
+
+        if param_dict is not None:
+            use_timestamp = param_dict.get('use_timestamp', True)
+        else:
+            use_timestamp = True
+
+        finish_count = 0
+        file_count = 1
+        lfr_factor = 6
         # 7 .Start for-loop
-        # FIXME(kamo): The output format should be discussed about
         asr_result_list = []
-        results = []
-        asr_result = ""
-        wait = True
-        if len(cache) == 0:
-            cache["encoder"] = {"start_idx": 0, "pad_left": 0, "stride": 10, "pad_right": 5, "cif_hidden": None, "cif_alphas": None, "is_final": is_final, "left": 0, "right": 0}
-            cache_de = {"decode_fsmn": None}
-            cache["decoder"] = cache_de
-            cache["first_chunk"] = True
-            cache["speech"] = []
-            cache["accum_speech"] = 0
-
-        if raw_inputs is not None:
-            if len(cache["speech"]) == 0:
-                cache["speech"] = raw_inputs
-            else:
-                cache["speech"] = torch.cat([cache["speech"], raw_inputs], dim=0)
-            cache["accum_speech"] += len(raw_inputs)
-            while cache["accum_speech"] >= 960:
-                if cache["first_chunk"]:
-                    if cache["accum_speech"] >= 14400:
-                        speech = torch.unsqueeze(cache["speech"], axis=0)
-                        speech_length = torch.tensor([len(cache["speech"])])
-                        cache["encoder"]["pad_left"] = 5 
-                        cache["encoder"]["pad_right"] = 5 
-                        cache["encoder"]["stride"] = 10
-                        cache["encoder"]["left"] = 5
-                        cache["encoder"]["right"] = 0
-                        results = speech2text(cache, speech, speech_length)
-                        cache["accum_speech"] -= 4800
-                        cache["first_chunk"] = False
-                        cache["encoder"]["start_idx"] = -5
-                        cache["encoder"]["is_final"] = False
-                        wait = False
+        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
+        writer = None
+        if output_path is not None:
+            writer = DatadirWriter(output_path)
+            ibest_writer = writer[f"1best_recog"]
+
+        for keys, batch in loader:
+            assert isinstance(batch, dict), type(batch)
+            assert all(isinstance(s, str) for s in keys), keys
+            _bs = len(next(iter(batch.values())))
+            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
+
+            vad_results = speech2vadsegment(**batch)
+            fbanks, vadsegments = vad_results[0], vad_results[1]
+            for i, segments in enumerate(vadsegments):
+                result_segments = [["", [], [], []]]
+                for j, segment_idx in enumerate(segments):
+                    bed_idx, end_idx = int(segment_idx[0] / 10), int(segment_idx[1] / 10)
+                    segment = fbanks[:, bed_idx:end_idx, :].to(device)
+                    speech_lengths = torch.Tensor([end_idx - bed_idx]).int().to(device)
+                    batch = {"speech": segment, "speech_lengths": speech_lengths, "begin_time": vadsegments[i][j][0],
+                             "end_time": vadsegments[i][j][1]}
+                    results = speech2text(**batch)
+                    if len(results) < 1:
+                        continue
+
+                    result_cur = [results[0][:-2]]
+                    if j == 0:
+                        result_segments = result_cur
                     else:
-                        if is_final:
-                            cache["encoder"]["stride"] = len(cache["speech"]) // 960
-                            cache["encoder"]["pad_left"] = 0
-                            cache["encoder"]["pad_right"] = 0
-                            speech = torch.unsqueeze(cache["speech"], axis=0)
-                            speech_length = torch.tensor([len(cache["speech"])])
-                            results = speech2text(cache, speech, speech_length)
-                            cache["accum_speech"] = 0
-                            wait = False
-                        else:
-                            break
+                        result_segments = [
+                            [result_segments[0][i] + result_cur[0][i] for i in range(len(result_cur[0]))]]
+
+                key = keys[0]
+                result = result_segments[0]
+                text, token, token_int = result[0], result[1], result[2]
+                time_stamp = None if len(result) < 4 else result[3]
+
+
+                if use_timestamp and time_stamp is not None: 
+                    postprocessed_result = postprocess_utils.sentence_postprocess(token, time_stamp)
                 else:
-                    if cache["accum_speech"] >= 19200:
-                        cache["encoder"]["start_idx"] += 10
-                        cache["encoder"]["stride"] = 10
-                        cache["encoder"]["pad_left"] = 5
-                        cache["encoder"]["pad_right"] = 5
-                        cache["encoder"]["left"] = 0
-                        cache["encoder"]["right"] = 0
-                        speech = torch.unsqueeze(cache["speech"], axis=0)
-                        speech_length = torch.tensor([len(cache["speech"])])
-                        results = speech2text(cache, speech, speech_length)
-                        cache["accum_speech"] -= 9600
-                        wait = False
-                    else:
-                        if is_final:
-                            cache["encoder"]["is_final"] = True
-                            if cache["accum_speech"] >= 14400:
-                                cache["encoder"]["start_idx"] += 10
-                                cache["encoder"]["stride"] = 10
-                                cache["encoder"]["pad_left"] = 5
-                                cache["encoder"]["pad_right"] = 5
-                                cache["encoder"]["left"] = 0
-                                cache["encoder"]["right"] = cache["accum_speech"] // 960 - 15
-                                speech = torch.unsqueeze(cache["speech"], axis=0)
-                                speech_length = torch.tensor([len(cache["speech"])])
-                                results = speech2text(cache, speech, speech_length)
-                                cache["accum_speech"] -= 9600
-                                wait = False
-                            else:
-                                cache["encoder"]["start_idx"] += 10
-                                cache["encoder"]["stride"] = cache["accum_speech"] // 960 - 5
-                                cache["encoder"]["pad_left"] = 5
-                                cache["encoder"]["pad_right"] = 0
-                                cache["encoder"]["left"] = 0
-                                cache["encoder"]["right"] = 0
-                                speech = torch.unsqueeze(cache["speech"], axis=0)
-                                speech_length = torch.tensor([len(cache["speech"])])
-                                results = speech2text(cache, speech, speech_length)
-                                cache["accum_speech"] = 0
-                                wait = False
-                        else:
-                            break
-                
-                if len(results) >= 1:
-                    asr_result += results[0][0]
-            if asr_result == "":
-                asr_result = "sil"
-            if wait:
-                asr_result = "waiting_for_more_voice"
-            item = {'key': "utt", 'value': asr_result}
-            asr_result_list.append(item)
-        else:
-            return []
+                    postprocessed_result = postprocess_utils.sentence_postprocess(token)
+                text_postprocessed = ""
+                time_stamp_postprocessed = ""
+                text_postprocessed_punc = postprocessed_result
+                if len(postprocessed_result) == 3:
+                    text_postprocessed, time_stamp_postprocessed, word_lists = postprocessed_result[0], \
+                                                                               postprocessed_result[1], \
+                                                                               postprocessed_result[2]
+                else:
+                    text_postprocessed, word_lists = postprocessed_result[0], postprocessed_result[1]
+
+                text_postprocessed_punc = text_postprocessed
+                punc_id_list = []
+                if len(word_lists) > 0 and text2punc is not None:
+                    text_postprocessed_punc, punc_id_list = text2punc(word_lists, 20)
+
+                item = {'key': key, 'value': text_postprocessed_punc}
+                if text_postprocessed != "":
+                    item['text_postprocessed'] = text_postprocessed
+                if time_stamp_postprocessed != "":
+                    item['time_stamp'] = time_stamp_postprocessed
+
+                item['sentences'] = time_stamp_sentence(punc_id_list, time_stamp_postprocessed, text_postprocessed)
+
+                asr_result_list.append(item)
+                finish_count += 1
+                # asr_utils.print_progress(finish_count / file_count)
+                if writer is not None:
+                    # Write the result to each file
+                    ibest_writer["token"][key] = " ".join(token)
+                    ibest_writer["token_int"][key] = " ".join(map(str, token_int))
+                    ibest_writer["vad"][key] = "{}".format(vadsegments)
+                    ibest_writer["text"][key] = " ".join(word_lists)
+                    ibest_writer["text_with_punc"][key] = text_postprocessed_punc
+                    if time_stamp_postprocessed is not None:
+                        ibest_writer["time_stamp"][key] = "{}".format(time_stamp_postprocessed)
+
+                logging.info("decoding, utt: {}, predictions: {}".format(key, text_postprocessed_punc))
         return asr_result_list
 
     return _forward
 
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
@@ -764,20 +715,15 @@
     )
     parser.add_argument(
         "--num_workers",
         type=int,
         default=1,
         help="The number of workers used for DataLoader",
     )
-    parser.add_argument(
-        "--hotword",
-        type=str_or_none,
-        default=None,
-        help="hotword file path or hotwords seperated by space"
-    )
+
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
         required=False,
         action="append",
     )
@@ -864,14 +810,15 @@
         type=float,
         default=0.5,
         help="CTC weight in joint decoding",
     )
     group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
     group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
     group.add_argument("--streaming", type=str2bool, default=False)
+    group.add_argument("--time_stamp_writer", type=str2bool, default=False)
 
     group.add_argument(
         "--frontend_conf",
         default=None,
         help="",
     )
     group.add_argument("--raw_inputs", type=list, default=None)
@@ -889,36 +836,46 @@
     group.add_argument(
         "--bpemodel",
         type=str_or_none,
         default=None,
         help="The model path of sentencepiece. "
              "If not given, refers from the training args",
     )
-
+    group.add_argument(
+        "--vad_infer_config",
+        type=str,
+        help="VAD infer configuration",
+    )
+    group.add_argument(
+        "--vad_model_file",
+        type=str,
+        help="VAD model parameter file",
+    )
+    group.add_argument(
+        "--vad_cmvn_file",
+        type=str,
+        help="vad, Global cmvn file",
+    )
+    group.add_argument(
+        "--punc_infer_config",
+        type=str,
+        help="VAD infer configuration",
+    )
+    group.add_argument(
+        "--punc_model_file",
+        type=str,
+        help="VAD model parameter file",
+    )
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
     args = parser.parse_args(cmd)
-    param_dict = {'hotword': args.hotword}
     kwargs = vars(args)
     kwargs.pop("config", None)
-    kwargs['param_dict'] = param_dict
     inference(**kwargs)
 
 
 if __name__ == "__main__":
     main()
-
-    # from modelscope.pipelines import pipeline
-    # from modelscope.utils.constant import Tasks
-    #
-    # inference_16k_pipline = pipeline(
-    #     task=Tasks.auto_speech_recognition,
-    #     model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch')
-    #
-    # rec_result = inference_16k_pipline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
-    # print(rec_result)
-
-
```

### Comparing `funasr-0.4.3/funasr/bin/asr_inference_paraformer_vad.py` & `funasr-0.4.4/funasr/bin/asr_inference_paraformer_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_inference_paraformer_vad_punc.py` & `funasr-0.4.4/funasr/bin/asr_inference_paraformer_streaming.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python3
-
-import json
 import argparse
 import logging
 import sys
 import time
+import copy
 import os
 import codecs
 import tempfile
 import requests
+import yaml
 from pathlib import Path
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import Dict
 from typing import Any
 from typing import List
-import math
-import copy
+
 import numpy as np
 import torch
 from typeguard import check_argument_types
 
 from funasr.fileio.datadir_writer import DatadirWriter
 from funasr.modules.beam_search.beam_search import BeamSearchPara as BeamSearch
 from funasr.modules.beam_search.beam_search import Hypothesis
@@ -37,32 +36,26 @@
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils import config_argparse
 from funasr.utils.cli_utils import get_commandline_args
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_none
 from funasr.utils import asr_utils, wav_utils, postprocess_utils
-from funasr.models.frontend.wav_frontend import WavFrontend
-from funasr.tasks.vad import VADTask
-from funasr.bin.vad_inference import Speech2VadSegment
-from funasr.utils.timestamp_tools import time_stamp_sentence, ts_prediction_lfr6_standard
-from funasr.bin.punctuation_infer import Text2Punc
-from funasr.models.e2e_asr_paraformer import BiCifParaformer, ContextualParaformer
-
+from funasr.models.frontend.wav_frontend import WavFrontend, WavFrontendOnline
+from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
 
-header_colors = '\033[95m'
-end_colors = '\033[0m'
+np.set_printoptions(threshold=np.inf)
 
 
 class Speech2Text:
     """Speech2Text class
 
     Examples:
             >>> import soundfile
-            >>> speech2text = Speech2Text("asr_config.yml", "asr.pb")
+            >>> speech2text = Speech2Text("asr_config.yml", "asr.pth")
             >>> audio, rate = soundfile.read("speech.wav")
             >>> speech2text(audio)
             [(text, token, token_int, hypothesis object), ...]
 
     """
 
     def __init__(
@@ -89,22 +82,22 @@
             **kwargs,
     ):
         assert check_argument_types()
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = ASRTask.build_model_from_file(
-            asr_train_config, asr_model_file, cmvn_file=cmvn_file, device=device
+            asr_train_config, asr_model_file, cmvn_file, device
         )
         frontend = None
-        if asr_model.frontend is not None and asr_train_args.frontend_conf is not None:
-            frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
+        if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
+            frontend = WavFrontendOnline(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
 
-        # logging.info("asr_model: {}".format(asr_model))
-        # logging.info("asr_train_args: {}".format(asr_train_args))
+        logging.info("asr_model: {}".format(asr_model))
+        logging.info("asr_train_args: {}".format(asr_train_args))
         asr_model.to(dtype=getattr(torch, dtype)).eval()
 
         if asr_model.ctc != None:
             ctc = CTCPrefixScorer(ctc=asr_model.ctc, eos=asr_model.eos)
             scorers.update(
                 ctc=ctc
             )
@@ -174,94 +167,101 @@
 
         self.asr_model = asr_model
         self.asr_train_args = asr_train_args
         self.converter = converter
         self.tokenizer = tokenizer
 
         # 6. [Optional] Build hotword list from str, local file or url
-        self.hotword_list = None
-        self.hotword_list = self.generate_hotwords_list(hotword_list_or_file)
 
         is_use_lm = lm_weight != 0.0 and lm_file is not None
         if (ctc_weight == 0.0 or asr_model.ctc == None) and not is_use_lm:
             beam_search = None
         self.beam_search = beam_search
         logging.info(f"Beam_search: {self.beam_search}")
         self.beam_search_transducer = beam_search_transducer
         self.maxlenratio = maxlenratio
         self.minlenratio = minlenratio
         self.device = device
         self.dtype = dtype
         self.nbest = nbest
         self.frontend = frontend
         self.encoder_downsampling_factor = 1
-        if asr_train_args.encoder_conf["input_layer"] == "conv2d":
+        if asr_train_args.encoder == "data2vec_encoder" or asr_train_args.encoder_conf["input_layer"] == "conv2d":
             self.encoder_downsampling_factor = 4
 
     @torch.no_grad()
     def __call__(
-            self, speech: Union[torch.Tensor, np.ndarray], speech_lengths: Union[torch.Tensor, np.ndarray] = None,
-            begin_time: int = 0, end_time: int = None,
+            self, cache: dict, speech: Union[torch.Tensor], speech_lengths: Union[torch.Tensor] = None
     ):
         """Inference
 
         Args:
                 speech: Input speech data
         Returns:
                 text, token, token_int, hyp
 
         """
         assert check_argument_types()
-
-        # Input as audio signal
-        if isinstance(speech, np.ndarray):
-            speech = torch.tensor(speech)
-
-        if self.frontend is not None:
-            # feats, feats_len = self.frontend.forward(speech, speech_lengths)
-            # fbanks, fbanks_len = self.frontend.forward_fbank(speech, speech_lengths)
-            feats, feats_len = self.frontend.forward_lfr_cmvn(speech, speech_lengths)
-            feats = to_device(feats, device=self.device)
-            feats_len = feats_len.int()
-            self.asr_model.frontend = None
+        results = []
+        cache_en = cache["encoder"]
+        if speech.shape[1] < 16 * 60 and cache_en["is_final"]:
+            cache_en["tail_chunk"] = True
+            feats = cache_en["feats"]
+            feats_len = torch.tensor([feats.shape[1]])
+            results = self.infer(feats, feats_len, cache)
+            return results
         else:
-            feats = speech
-            feats_len = speech_lengths
-        lfr_factor = max(1, (feats.size()[-1] // 80) - 1)
-        batch = {"speech": feats, "speech_lengths": feats_len}
+            if self.frontend is not None:
+                feats, feats_len = self.frontend.forward(speech, speech_lengths, cache_en["is_final"])
+                feats = to_device(feats, device=self.device)
+                feats_len = feats_len.int()
+                self.asr_model.frontend = None
+            else:
+                feats = speech
+                feats_len = speech_lengths
 
-        # a. To device
-        batch = to_device(batch, device=self.device)
+            if feats.shape[1] != 0:
+                if cache_en["is_final"]:
+                    if feats.shape[1] + cache_en["chunk_size"][2] < cache_en["chunk_size"][1]:
+                        cache_en["last_chunk"] = True
+                    else:
+                        # first chunk
+                        feats_chunk1 = feats[:, :cache_en["chunk_size"][1], :]
+                        feats_len = torch.tensor([feats_chunk1.shape[1]])
+                        results_chunk1 = self.infer(feats_chunk1, feats_len, cache)
+
+                        # last chunk
+                        cache_en["last_chunk"] = True
+                        feats_chunk2 = feats[:, -(feats.shape[1] + cache_en["chunk_size"][2] - cache_en["chunk_size"][1]):, :]
+                        feats_len = torch.tensor([feats_chunk2.shape[1]])
+                        results_chunk2 = self.infer(feats_chunk2, feats_len, cache)
+
+                        return ["".join(results_chunk1 + results_chunk2)]
+
+                results = self.infer(feats, feats_len, cache)
+
+        return results
 
+    @torch.no_grad()
+    def infer(self, feats: Union[torch.Tensor], feats_len: Union[torch.Tensor], cache: List = None):
+        batch = {"speech": feats, "speech_lengths": feats_len}
+        batch = to_device(batch, device=self.device)
         # b. Forward Encoder
-        enc, enc_len = self.asr_model.encode(**batch)
+        enc, enc_len = self.asr_model.encode_chunk(feats, feats_len, cache=cache)
         if isinstance(enc, tuple):
             enc = enc[0]
         # assert len(enc) == 1, len(enc)
         enc_len_batch_total = torch.sum(enc_len).item() * self.encoder_downsampling_factor
 
-        predictor_outs = self.asr_model.calc_predictor(enc, enc_len)
-        pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = predictor_outs[0], predictor_outs[1], \
-                                                                        predictor_outs[2], predictor_outs[3]
-        pre_token_length = pre_token_length.round().long()
+        predictor_outs = self.asr_model.calc_predictor_chunk(enc, cache)
+        pre_acoustic_embeds, pre_token_length= predictor_outs[0], predictor_outs[1]
         if torch.max(pre_token_length) < 1:
             return []
-
-        if not isinstance(self.asr_model, ContextualParaformer):
-            if self.hotword_list:
-                logging.warning("Hotword is given but asr model is not a ContextualParaformer.")
-            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length)
-            decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
-        else:
-            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds, pre_token_length, hw_list=self.hotword_list)
-            decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
-
-        if isinstance(self.asr_model, BiCifParaformer):
-            _, _, us_alphas, us_peaks = self.asr_model.calc_predictor_timestamp(enc, enc_len,
-                                                                                   pre_token_length)  # test no bias cif2
+        decoder_outs = self.asr_model.cal_decoder_with_predictor_chunk(enc, pre_acoustic_embeds, cache)
+        decoder_out = decoder_outs
 
         results = []
         b, n, d = decoder_out.size()
         for i in range(b):
             x = enc[i, :enc_len[i], :]
             am_scores = decoder_out[i, :pre_token_length[i], :]
             if self.beam_search is not None:
@@ -288,91 +288,27 @@
                 if isinstance(hyp.yseq, list):
                     token_int = hyp.yseq[1:last_pos]
                 else:
                     token_int = hyp.yseq[1:last_pos].tolist()
 
                 # remove blank symbol id, which is assumed to be 0
                 token_int = list(filter(lambda x: x != 0 and x != 2, token_int))
-                if len(token_int) == 0:
-                    continue
 
                 # Change integer-ids to tokens
                 token = self.converter.ids2tokens(token_int)
 
                 if self.tokenizer is not None:
                     text = self.tokenizer.tokens2text(token)
                 else:
                     text = None
-
-                if isinstance(self.asr_model, BiCifParaformer):
-                    _, timestamp = ts_prediction_lfr6_standard(us_alphas[i], 
-                                                            us_peaks[i], 
-                                                            copy.copy(token), 
-                                                            vad_offset=begin_time)
-                    results.append((text, token, token_int, timestamp, enc_len_batch_total, lfr_factor))
-                else:
-                    results.append((text, token, token_int, enc_len_batch_total, lfr_factor))
+                results.append(text)
 
         # assert check_return_type(results)
         return results
 
-    def generate_hotwords_list(self, hotword_list_or_file):
-        # for None
-        if hotword_list_or_file is None:
-            hotword_list = None
-        # for local txt inputs
-        elif os.path.exists(hotword_list_or_file) and hotword_list_or_file.endswith('.txt'):
-            logging.info("Attempting to parse hotwords from local txt...")
-            hotword_list = []
-            hotword_str_list = []
-            with codecs.open(hotword_list_or_file, 'r') as fin:
-                for line in fin.readlines():
-                    hw = line.strip()
-                    hotword_str_list.append(hw)
-                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
-                hotword_list.append([self.asr_model.sos])
-                hotword_str_list.append('<s>')
-            logging.info("Initialized hotword list from file: {}, hotword list: {}."
-                         .format(hotword_list_or_file, hotword_str_list))
-        # for url, download and generate txt
-        elif hotword_list_or_file.startswith('http'):
-            logging.info("Attempting to parse hotwords from url...")
-            work_dir = tempfile.TemporaryDirectory().name
-            if not os.path.exists(work_dir):
-                os.makedirs(work_dir)
-            text_file_path = os.path.join(work_dir, os.path.basename(hotword_list_or_file))
-            local_file = requests.get(hotword_list_or_file)
-            open(text_file_path, "wb").write(local_file.content)
-            hotword_list_or_file = text_file_path
-            hotword_list = []
-            hotword_str_list = []
-            with codecs.open(hotword_list_or_file, 'r') as fin:
-                for line in fin.readlines():
-                    hw = line.strip()
-                    hotword_str_list.append(hw)
-                    hotword_list.append(self.converter.tokens2ids([i for i in hw]))
-                hotword_list.append([self.asr_model.sos])
-                hotword_str_list.append('<s>')
-            logging.info("Initialized hotword list from file: {}, hotword list: {}."
-                         .format(hotword_list_or_file, hotword_str_list))
-        # for text str input
-        elif not hotword_list_or_file.endswith('.txt'):
-            logging.info("Attempting to parse hotwords as str...")
-            hotword_list = []
-            hotword_str_list = []
-            for hw in hotword_list_or_file.strip().split():
-                hotword_str_list.append(hw)
-                hotword_list.append(self.converter.tokens2ids([i for i in hw]))
-            hotword_list.append([self.asr_model.sos])
-            hotword_str_list.append('<s>')
-            logging.info("Hotword list: {}.".format(hotword_str_list))
-        else:
-            hotword_list = None
-        return hotword_list
-
 
 def inference(
         maxlenratio: float,
         minlenratio: float,
         batch_size: int,
         beam_size: int,
         ngpu: int,
@@ -395,20 +331,15 @@
         streaming: bool = False,
         output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
-        vad_infer_config: Optional[str] = None,
-        vad_model_file: Optional[str] = None,
-        vad_cmvn_file: Optional[str] = None,
-        time_stamp_writer: bool = False,
-        punc_infer_config: Optional[str] = None,
-        punc_model_file: Optional[str] = None,
+
         **kwargs,
 ):
     inference_pipeline = inference_modelscope(
         maxlenratio=maxlenratio,
         minlenratio=minlenratio,
         batch_size=batch_size,
         beam_size=beam_size,
@@ -431,20 +362,15 @@
         streaming=streaming,
         output_dir=output_dir,
         dtype=dtype,
         seed=seed,
         ngram_weight=ngram_weight,
         nbest=nbest,
         num_workers=num_workers,
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        time_stamp_writer=time_stamp_writer,
-        punc_infer_config=punc_infer_config,
-        punc_model_file=punc_model_file,
+
         **kwargs,
     )
     return inference_pipeline(data_path_and_name_and_type, raw_inputs)
 
 
 def inference_modelscope(
         maxlenratio: float,
@@ -463,69 +389,47 @@
         lm_train_config: Optional[str] = None,
         lm_file: Optional[str] = None,
         token_type: Optional[str] = None,
         key_file: Optional[str] = None,
         word_lm_train_config: Optional[str] = None,
         bpemodel: Optional[str] = None,
         allow_variable_data_keys: bool = False,
-        output_dir: Optional[str] = None,
         dtype: str = "float32",
         seed: int = 0,
         ngram_weight: float = 0.9,
         nbest: int = 1,
         num_workers: int = 1,
-        vad_infer_config: Optional[str] = None,
-        vad_model_file: Optional[str] = None,
-        vad_cmvn_file: Optional[str] = None,
-        time_stamp_writer: bool = True,
-        punc_infer_config: Optional[str] = None,
-        punc_model_file: Optional[str] = None,
-        outputs_dict: Optional[bool] = True,
+        output_dir: Optional[str] = None,
         param_dict: dict = None,
         **kwargs,
 ):
     assert check_argument_types()
-    ncpu = kwargs.get("ncpu", 1)
-    torch.set_num_threads(ncpu)
 
     if word_lm_train_config is not None:
         raise NotImplementedError("Word LM is not implemented")
     if ngpu > 1:
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
-    if param_dict is not None:
-        hotword_list_or_file = param_dict.get('hotword')
-    else:
-        hotword_list_or_file = None
+    export_mode = False
 
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
+        batch_size = 1
 
     # 1. Set random-seed
     set_all_random_seed(seed)
 
-    # 2. Build speech2vadsegment
-    speech2vadsegment_kwargs = dict(
-        vad_infer_config=vad_infer_config,
-        vad_model_file=vad_model_file,
-        vad_cmvn_file=vad_cmvn_file,
-        device=device,
-        dtype=dtype,
-    )
-    # logging.info("speech2vadsegment_kwargs: {}".format(speech2vadsegment_kwargs))
-    speech2vadsegment = Speech2VadSegment(**speech2vadsegment_kwargs)
-
-    # 3. Build speech2text
+    # 2. Build speech2text
     speech2text_kwargs = dict(
         asr_train_config=asr_train_config,
         asr_model_file=asr_model_file,
         cmvn_file=cmvn_file,
         lm_train_config=lm_train_config,
         lm_file=lm_file,
         token_type=token_type,
@@ -536,152 +440,111 @@
         dtype=dtype,
         beam_size=beam_size,
         ctc_weight=ctc_weight,
         lm_weight=lm_weight,
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
-        hotword_list_or_file=hotword_list_or_file,
     )
+
     speech2text = Speech2Text(**speech2text_kwargs)
-    text2punc = None
-    if punc_model_file is not None:
-        text2punc = Text2Punc(punc_infer_config, punc_model_file, device=device, dtype=dtype)
-
-    if output_dir is not None:
-        writer = DatadirWriter(output_dir)
-        ibest_writer = writer[f"1best_recog"]
-        ibest_writer["token_list"][""] = " ".join(speech2text.asr_train_args.token_list)
-
-    def _forward(data_path_and_name_and_type,
-                 raw_inputs: Union[np.ndarray, torch.Tensor] = None,
-                 output_dir_v2: Optional[str] = None,
-                 fs: dict = None,
-                 param_dict: dict = None,
-                 **kwargs,
-                 ):
-
-        hotword_list_or_file = None
-        if param_dict is not None:
-            hotword_list_or_file = param_dict.get('hotword')
 
-        if 'hotword' in kwargs:
-            hotword_list_or_file = kwargs['hotword']
+    def _load_bytes(input):
+        middle_data = np.frombuffer(input, dtype=np.int16)
+        middle_data = np.asarray(middle_data)
+        if middle_data.dtype.kind not in 'iu':
+            raise TypeError("'middle_data' must be an array of integers")
+        dtype = np.dtype('float32')
+        if dtype.kind != 'f':
+            raise TypeError("'dtype' must be a floating point type")
+
+        i = np.iinfo(middle_data.dtype)
+        abs_max = 2 ** (i.bits - 1)
+        offset = i.min + abs_max
+        array = np.frombuffer((middle_data.astype(dtype) - offset) / abs_max, dtype=np.float32)
+        return array
+
+    def _read_yaml(yaml_path: Union[str, Path]) -> Dict:
+        if not Path(yaml_path).exists():
+            raise FileExistsError(f'The {yaml_path} does not exist.')
+
+        with open(str(yaml_path), 'rb') as f:
+            data = yaml.load(f, Loader=yaml.Loader)
+        return data
+
+    def _prepare_cache(cache: dict = {}, chunk_size=[5,10,5], batch_size=1):
+        if len(cache) > 0:
+            return cache
+        config = _read_yaml(asr_train_config)
+        enc_output_size = config["encoder_conf"]["output_size"]
+        feats_dims = config["frontend_conf"]["n_mels"] * config["frontend_conf"]["lfr_m"]
+        cache_en = {"start_idx": 0, "cif_hidden": torch.zeros((batch_size, 1, enc_output_size)),
+                    "cif_alphas": torch.zeros((batch_size, 1)), "chunk_size": chunk_size, "last_chunk": False,
+                    "feats": torch.zeros((batch_size, chunk_size[0] + chunk_size[2], feats_dims)), "tail_chunk": False}
+        cache["encoder"] = cache_en
+
+        cache_de = {"decode_fsmn": None}
+        cache["decoder"] = cache_de
+
+        return cache
+
+    def _cache_reset(cache: dict = {}, chunk_size=[5,10,5], batch_size=1):
+        if len(cache) > 0:
+            config = _read_yaml(asr_train_config)
+            enc_output_size = config["encoder_conf"]["output_size"]
+            feats_dims = config["frontend_conf"]["n_mels"] * config["frontend_conf"]["lfr_m"]
+            cache_en = {"start_idx": 0, "cif_hidden": torch.zeros((batch_size, 1, enc_output_size)),
+                        "cif_alphas": torch.zeros((batch_size, 1)), "chunk_size": chunk_size, "last_chunk": False,
+                        "feats": torch.zeros((batch_size, chunk_size[0] + chunk_size[2], feats_dims)), "tail_chunk": False}
+            cache["encoder"] = cache_en
 
-        if speech2text.hotword_list is None:
-            speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
+            cache_de = {"decode_fsmn": None}
+            cache["decoder"] = cache_de
 
-        # 3. Build data-iterator
-        if data_path_and_name_and_type is None and raw_inputs is not None:
-            if isinstance(raw_inputs, torch.Tensor):
-                raw_inputs = raw_inputs.numpy()
-            data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
-        loader = ASRTask.build_streaming_iterator(
+        return cache
+
+    def _forward(
             data_path_and_name_and_type,
-            dtype=dtype,
-            fs=fs,
-            batch_size=1,
-            key_file=key_file,
-            num_workers=num_workers,
-            preprocess_fn=VADTask.build_preprocess_fn(speech2vadsegment.vad_infer_args, False),
-            collate_fn=VADTask.build_collate_fn(speech2vadsegment.vad_infer_args, False),
-            allow_variable_data_keys=allow_variable_data_keys,
-            inference=True,
-        )
+            raw_inputs: Union[np.ndarray, torch.Tensor] = None,
+            output_dir_v2: Optional[str] = None,
+            fs: dict = None,
+            param_dict: dict = None,
+            **kwargs,
+    ):
 
-        if param_dict is not None:
-            use_timestamp = param_dict.get('use_timestamp', True)
-        else:
-            use_timestamp = True
+        # 3. Build data-iterator
+        if data_path_and_name_and_type is not None and data_path_and_name_and_type[2] == "bytes":
+            raw_inputs = _load_bytes(data_path_and_name_and_type[0])
+            raw_inputs = torch.tensor(raw_inputs)
+        if data_path_and_name_and_type is None and raw_inputs is not None:
+            if isinstance(raw_inputs, np.ndarray):
+                raw_inputs = torch.tensor(raw_inputs)
+        is_final = False
+        cache = {}
+        chunk_size = [5, 10, 5]
+        if param_dict is not None and "cache" in param_dict:
+            cache = param_dict["cache"]
+        if param_dict is not None and "is_final" in param_dict:
+            is_final = param_dict["is_final"]
+        if param_dict is not None and "chunk_size" in param_dict:
+            chunk_size = param_dict["chunk_size"]
 
-        finish_count = 0
-        file_count = 1
-        lfr_factor = 6
         # 7 .Start for-loop
+        # FIXME(kamo): The output format should be discussed about
+        raw_inputs = torch.unsqueeze(raw_inputs, axis=0)
+        input_lens = torch.tensor([raw_inputs.shape[1]])
         asr_result_list = []
-        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
-        writer = None
-        if output_path is not None:
-            writer = DatadirWriter(output_path)
-            ibest_writer = writer[f"1best_recog"]
-
-        for keys, batch in loader:
-            assert isinstance(batch, dict), type(batch)
-            assert all(isinstance(s, str) for s in keys), keys
-            _bs = len(next(iter(batch.values())))
-            assert len(keys) == _bs, f"{len(keys)} != {_bs}"
-
-            vad_results = speech2vadsegment(**batch)
-            fbanks, vadsegments = vad_results[0], vad_results[1]
-            for i, segments in enumerate(vadsegments):
-                result_segments = [["", [], [], []]]
-                for j, segment_idx in enumerate(segments):
-                    bed_idx, end_idx = int(segment_idx[0] / 10), int(segment_idx[1] / 10)
-                    segment = fbanks[:, bed_idx:end_idx, :].to(device)
-                    speech_lengths = torch.Tensor([end_idx - bed_idx]).int().to(device)
-                    batch = {"speech": segment, "speech_lengths": speech_lengths, "begin_time": vadsegments[i][j][0],
-                             "end_time": vadsegments[i][j][1]}
-                    results = speech2text(**batch)
-                    if len(results) < 1:
-                        continue
-
-                    result_cur = [results[0][:-2]]
-                    if j == 0:
-                        result_segments = result_cur
-                    else:
-                        result_segments = [
-                            [result_segments[0][i] + result_cur[0][i] for i in range(len(result_cur[0]))]]
-
-                key = keys[0]
-                result = result_segments[0]
-                text, token, token_int = result[0], result[1], result[2]
-                time_stamp = None if len(result) < 4 else result[3]
 
-
-                if use_timestamp and time_stamp is not None: 
-                    postprocessed_result = postprocess_utils.sentence_postprocess(token, time_stamp)
-                else:
-                    postprocessed_result = postprocess_utils.sentence_postprocess(token)
-                text_postprocessed = ""
-                time_stamp_postprocessed = ""
-                text_postprocessed_punc = postprocessed_result
-                if len(postprocessed_result) == 3:
-                    text_postprocessed, time_stamp_postprocessed, word_lists = postprocessed_result[0], \
-                                                                               postprocessed_result[1], \
-                                                                               postprocessed_result[2]
-                else:
-                    text_postprocessed, word_lists = postprocessed_result[0], postprocessed_result[1]
-
-                text_postprocessed_punc = text_postprocessed
-                punc_id_list = []
-                if len(word_lists) > 0 and text2punc is not None:
-                    text_postprocessed_punc, punc_id_list = text2punc(word_lists, 20)
-
-                item = {'key': key, 'value': text_postprocessed_punc}
-                if text_postprocessed != "":
-                    item['text_postprocessed'] = text_postprocessed
-                if time_stamp_postprocessed != "":
-                    item['time_stamp'] = time_stamp_postprocessed
-
-                item['sentences'] = time_stamp_sentence(punc_id_list, time_stamp_postprocessed, text_postprocessed)
-
-                asr_result_list.append(item)
-                finish_count += 1
-                # asr_utils.print_progress(finish_count / file_count)
-                if writer is not None:
-                    # Write the result to each file
-                    ibest_writer["token"][key] = " ".join(token)
-                    ibest_writer["token_int"][key] = " ".join(map(str, token_int))
-                    ibest_writer["vad"][key] = "{}".format(vadsegments)
-                    ibest_writer["text"][key] = " ".join(word_lists)
-                    ibest_writer["text_with_punc"][key] = text_postprocessed_punc
-                    if time_stamp_postprocessed is not None:
-                        ibest_writer["time_stamp"][key] = "{}".format(time_stamp_postprocessed)
-
-                logging.info("decoding, utt: {}, predictions: {}".format(key, text_postprocessed_punc))
+        cache = _prepare_cache(cache, chunk_size=chunk_size, batch_size=1)
+        cache["encoder"]["is_final"] = is_final
+        asr_result = speech2text(cache, raw_inputs, input_lens)
+        item = {'key': "utt", 'value': asr_result}
+        asr_result_list.append(item)
+        if is_final:
+            cache = _cache_reset(cache, chunk_size=chunk_size, batch_size=1)
         return asr_result_list
 
     return _forward
 
 
 def get_parser():
     parser = config_argparse.ArgumentParser(
@@ -715,15 +578,20 @@
     )
     parser.add_argument(
         "--num_workers",
         type=int,
         default=1,
         help="The number of workers used for DataLoader",
     )
-
+    parser.add_argument(
+        "--hotword",
+        type=str_or_none,
+        default=None,
+        help="hotword file path or hotwords seperated by space"
+    )
     group = parser.add_argument_group("Input data related")
     group.add_argument(
         "--data_path_and_name_and_type",
         type=str2triple_str,
         required=False,
         action="append",
     )
@@ -810,15 +678,14 @@
         type=float,
         default=0.5,
         help="CTC weight in joint decoding",
     )
     group.add_argument("--lm_weight", type=float, default=1.0, help="RNNLM weight")
     group.add_argument("--ngram_weight", type=float, default=0.9, help="ngram weight")
     group.add_argument("--streaming", type=str2bool, default=False)
-    group.add_argument("--time_stamp_writer", type=str2bool, default=False)
 
     group.add_argument(
         "--frontend_conf",
         default=None,
         help="",
     )
     group.add_argument("--raw_inputs", type=list, default=None)
@@ -836,46 +703,34 @@
     group.add_argument(
         "--bpemodel",
         type=str_or_none,
         default=None,
         help="The model path of sentencepiece. "
              "If not given, refers from the training args",
     )
-    group.add_argument(
-        "--vad_infer_config",
-        type=str,
-        help="VAD infer configuration",
-    )
-    group.add_argument(
-        "--vad_model_file",
-        type=str,
-        help="VAD model parameter file",
-    )
-    group.add_argument(
-        "--vad_cmvn_file",
-        type=str,
-        help="vad, Global cmvn file",
-    )
-    group.add_argument(
-        "--punc_infer_config",
-        type=str,
-        help="VAD infer configuration",
-    )
-    group.add_argument(
-        "--punc_model_file",
-        type=str,
-        help="VAD model parameter file",
-    )
+
     return parser
 
 
 def main(cmd=None):
     print(get_commandline_args(), file=sys.stderr)
     parser = get_parser()
     args = parser.parse_args(cmd)
+    param_dict = {'hotword': args.hotword}
     kwargs = vars(args)
     kwargs.pop("config", None)
+    kwargs['param_dict'] = param_dict
     inference(**kwargs)
 
 
 if __name__ == "__main__":
     main()
+
+    # from modelscope.pipelines import pipeline
+    # from modelscope.utils.constant import Tasks
+    #
+    # inference_16k_pipline = pipeline(
+    #     task=Tasks.auto_speech_recognition,
+    #     model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch')
+    #
+    # rec_result = inference_16k_pipline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
+    # print(rec_result)
```

### Comparing `funasr-0.4.3/funasr/bin/asr_inference_rnnt.py` & `funasr-0.4.4/funasr/bin/asr_inference_rnnt.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         self.converter = converter
         self.tokenizer = tokenizer
 
         self.beam_search = beam_search
         self.streaming = streaming
         self.simu_streaming = simu_streaming
         self.chunk_size = max(chunk_size, 0)
-        self.left_context = max(left_context, 0)
+        self.left_context = left_context
         self.right_context = max(right_context, 0)
 
         if not streaming or chunk_size == 0:
             self.streaming = False
             self.asr_model.encoder.dynamic_chunk_training = False
         
         if not simu_streaming or chunk_size == 0:
```

### Comparing `funasr-0.4.3/funasr/bin/asr_inference_uniasr.py` & `funasr-0.4.4/funasr/bin/asr_inference_uniasr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_inference_uniasr_vad.py` & `funasr-0.4.4/funasr/bin/asr_inference_uniasr_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_train.py` & `funasr-0.4.4/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_train_paraformer.py` & `funasr-0.4.4/funasr/bin/asr_train_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_train_transducer.py` & `funasr-0.4.4/funasr/bin/asr_train_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/asr_train_uniasr.py` & `funasr-0.4.4/funasr/bin/asr_train_uniasr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/build_trainer.py` & `funasr-0.4.4/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/data2vec_train.py` & `funasr-0.4.4/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/diar_inference_launch.py` & `funasr-0.4.4/funasr/bin/diar_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/diar_train.py` & `funasr-0.4.4/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/eend_ola_inference.py` & `funasr-0.4.4/funasr/bin/eend_ola_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/lm_calc_perplexity.py` & `funasr-0.4.4/funasr/bin/lm_calc_perplexity.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/lm_inference.py` & `funasr-0.4.4/funasr/bin/lm_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/lm_inference_launch.py` & `funasr-0.4.4/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/lm_train.py` & `funasr-0.4.4/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/modelscope_infer.py` & `funasr-0.4.4/funasr/bin/modelscope_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/punc_inference_launch.py` & `funasr-0.4.4/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/punc_train.py` & `funasr-0.4.4/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/punctuation_infer.py` & `funasr-0.4.4/funasr/bin/punctuation_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/punctuation_infer_vadrealtime.py` & `funasr-0.4.4/funasr/bin/punctuation_infer_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/sond_inference.py` & `funasr-0.4.4/funasr/bin/sond_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/sv_inference.py` & `funasr-0.4.4/funasr/bin/sv_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/sv_inference_launch.py` & `funasr-0.4.4/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/tokenize_text.py` & `funasr-0.4.4/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/tp_inference.py` & `funasr-0.4.4/funasr/bin/tp_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -218,23 +218,37 @@
         text_cleaner=None,
         g2p_type=None,
         text_name="text",
         non_linguistic_symbols=speechtext2timestamp.tp_train_args.non_linguistic_symbols,
         split_with_space=split_with_space,
         seg_dict_file=seg_dict_file,
     )
+
+    if output_dir is not None:
+        writer = DatadirWriter(output_dir)
+        tp_writer = writer[f"timestamp_prediction"]
+        # ibest_writer["token_list"][""] = " ".join(speech2text.asr_train_args.token_list)
+    else:
+        tp_writer = None
     
     def _forward(
             data_path_and_name_and_type,
             raw_inputs: Union[np.ndarray, torch.Tensor] = None,
             output_dir_v2: Optional[str] = None,
             fs: dict = None,
             param_dict: dict = None,
             **kwargs
-    ):
+    ):  
+        output_path = output_dir_v2 if output_dir_v2 is not None else output_dir
+        writer = None
+        if output_path is not None:
+            writer = DatadirWriter(output_path)
+            tp_writer = writer[f"timestamp_prediction"]
+        else:
+            tp_writer = None
         # 3. Build data-iterator
         if data_path_and_name_and_type is None and raw_inputs is not None:
             if isinstance(raw_inputs, torch.Tensor):
                 raw_inputs = raw_inputs.numpy()
             data_path_and_name_and_type = [raw_inputs, "speech", "waveform"]
         
         loader = ASRTask.build_streaming_iterator(
@@ -264,14 +278,17 @@
 
             for batch_id in range(_bs):
                 key = keys[batch_id]
                 token = speechtext2timestamp.converter.ids2tokens(batch['text'][batch_id])
                 ts_str, ts_list = ts_prediction_lfr6_standard(us_alphas[batch_id], us_cif_peak[batch_id], token, force_time_shift=-3.0)
                 logging.warning(ts_str)
                 item = {'key': key, 'value': ts_str, 'timestamp':ts_list}
+                if tp_writer is not None:
+                    tp_writer["tp_sync"][key+'#'] = ts_str
+                    tp_writer["tp_time"][key+'#'] = str(ts_list)
                 tp_result_list.append(item)
         return tp_result_list
 
     return _forward
 
 
 def get_parser():
```

### Comparing `funasr-0.4.3/funasr/bin/tp_inference_launch.py` & `funasr-0.4.4/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/vad_inference.py` & `funasr-0.4.4/funasr/bin/vad_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/vad_inference_launch.py` & `funasr-0.4.4/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/bin/vad_inference_online.py` & `funasr-0.4.4/funasr/bin/vad_inference_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/collate_fn.py` & `funasr-0.4.4/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/dataset.py` & `funasr-0.4.4/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/iterable_dataset.py` & `funasr-0.4.4/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/iterable_dataset_modelscope.py` & `funasr-0.4.4/funasr/datasets/iterable_dataset_modelscope.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.4.4/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.4.4/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.4.4/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/large_datasets/dataset.py` & `funasr-0.4.4/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.4.4/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.4.4/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.4.4/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.4.4/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.4.4/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,29 @@
                 if len(word) > len(longest_word):
                     longest_word = word
         word_list.append(longest_word)
         i += len(longest_word)
     return word_list
 
 def seg_tokenize(txt, seg_dict):
+    pattern = re.compile(r'^[\u4E00-\u9FA50-9]+$')
     out_txt = ""
     for word in txt:
         word = word.lower()
         if word in seg_dict:
             out_txt += seg_dict[word] + " "
         else:
-            out_txt += "<unk>" + " "
+            if pattern.match(word):
+                for char in word:
+                    if char in seg_dict:
+                        out_txt += seg_dict[char] + " "
+                    else:
+                        out_txt += "<unk>" + " "
+            else:
+                out_txt += "<unk>" + " "
     return out_txt.strip().split()
 
 def tokenize(data,
              vocab=None,
              seg_dict=None,
              punc_dict=None,
              bpe_tokenizer=None):
```

### Comparing `funasr-0.4.3/funasr/datasets/ms_dataset.py` & `funasr-0.4.4/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/datasets/preprocessor.py` & `funasr-0.4.4/funasr/datasets/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,30 @@
             if word in dic:
                 if len(word) > len(longest_word):
                     longest_word = word
         word_list.append(longest_word)
         i += len(longest_word)
     return word_list
 
-
 def seg_tokenize(txt, seg_dict):
+    pattern = re.compile(r'^[\u4E00-\u9FA50-9]+$')
     out_txt = ""
     for word in txt:
         word = word.lower()
         if word in seg_dict:
             out_txt += seg_dict[word] + " "
         else:
-            out_txt += "<unk>" + " "
+            if pattern.match(word):
+                for char in word:
+                    if char in seg_dict:
+                        out_txt += seg_dict[char] + " "
+                    else:
+                        out_txt += "<unk>" + " "
+            else:
+                out_txt += "<unk>" + " "
     return out_txt.strip().split()
 
 def seg_tokenize_wo_pattern(txt, seg_dict):
     out_txt = ""
     for word in txt:
         if word in seg_dict:
             out_txt += seg_dict[word] + " "
```

### Comparing `funasr-0.4.3/funasr/export/export_model.py` & `funasr-0.4.4/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/CT_Transformer.py` & `funasr-0.4.4/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/__init__.py` & `funasr-0.4.4/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.4.4/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.4.4/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.4.4/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/e2e_vad.py` & `funasr-0.4.4/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.4.4/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.4.4/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.4.4/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/modules/decoder_layer.py` & `funasr-0.4.4/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/modules/encoder_layer.py` & `funasr-0.4.4/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/modules/feedforward.py` & `funasr-0.4.4/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/modules/multihead_att.py` & `funasr-0.4.4/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/models/predictor/cif.py` & `funasr-0.4.4/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/test/test_onnx.py` & `funasr-0.4.4/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/test/test_onnx_punc.py` & `funasr-0.4.4/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.4.4/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/test/test_onnx_vad.py` & `funasr-0.4.4/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/export/utils/torch_function.py` & `funasr-0.4.4/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/fileio/datadir_writer.py` & `funasr-0.4.4/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/fileio/npy_scp.py` & `funasr-0.4.4/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/fileio/rand_gen_dataset.py` & `funasr-0.4.4/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/fileio/read_text.py` & `funasr-0.4.4/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/fileio/sound_scp.py` & `funasr-0.4.4/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/iterators/chunk_iter_factory.py` & `funasr-0.4.4/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/iterators/multiple_iter_factory.py` & `funasr-0.4.4/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/iterators/sequence_iter_factory.py` & `funasr-0.4.4/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/layers/complex_utils.py` & `funasr-0.4.4/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/layers/global_mvn.py` & `funasr-0.4.4/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/layers/label_aggregation.py` & `funasr-0.4.4/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/layers/log_mel.py` & `funasr-0.4.4/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/layers/mask_along_axis.py` & `funasr-0.4.4/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/layers/sinc_conv.py` & `funasr-0.4.4/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/layers/stft.py` & `funasr-0.4.4/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/layers/time_warp.py` & `funasr-0.4.4/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/layers/utterance_mvn.py` & `funasr-0.4.4/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/lm/abs_model.py` & `funasr-0.4.4/funasr/lm/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/lm/seq_rnn_lm.py` & `funasr-0.4.4/funasr/lm/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/lm/transformer_lm.py` & `funasr-0.4.4/funasr/lm/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/losses/label_smoothing_loss.py` & `funasr-0.4.4/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/main_funcs/average_nbest_models.py` & `funasr-0.4.4/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.4.4/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/main_funcs/collect_stats.py` & `funasr-0.4.4/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/main_funcs/pack_funcs.py` & `funasr-0.4.4/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/ctc.py` & `funasr-0.4.4/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/data2vec.py` & `funasr-0.4.4/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/decoder/contextual_decoder.py` & `funasr-0.4.4/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/decoder/rnn_decoder.py` & `funasr-0.4.4/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.4.4/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/decoder/sanm_decoder.py` & `funasr-0.4.4/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/decoder/sv_decoder.py` & `funasr-0.4.4/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/decoder/transformer_decoder.py` & `funasr-0.4.4/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/e2e_asr.py` & `funasr-0.4.4/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/e2e_asr_common.py` & `funasr-0.4.4/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/e2e_asr_mfcca.py` & `funasr-0.4.4/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/e2e_asr_paraformer.py` & `funasr-0.4.4/funasr/models/e2e_asr_paraformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,17 +708,17 @@
         if intermediate_outs is not None:
             return (encoder_out, intermediate_outs), encoder_out_lens
 
         return encoder_out, torch.tensor([encoder_out.size(1)])
 
     def calc_predictor_chunk(self, encoder_out, cache=None):
 
-        pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = \
+        pre_acoustic_embeds, pre_token_length = \
             self.predictor.forward_chunk(encoder_out, cache["encoder"])
-        return pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index
+        return pre_acoustic_embeds, pre_token_length
 
     def cal_decoder_with_predictor_chunk(self, encoder_out, sematic_embeds, cache=None):
         decoder_outs = self.decoder.forward_chunk(
             encoder_out, sematic_embeds, cache["decoder"]
         )
         decoder_out = decoder_outs
         decoder_out = torch.log_softmax(decoder_out, dim=-1)
```

### Comparing `funasr-0.4.3/funasr/models/e2e_asr_transducer.py` & `funasr-0.4.4/funasr/models/e2e_asr_transducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,27 +382,27 @@
                 blank=self.blank_id,
                 fastemit_lambda=self.fastemit_lambda,
                 gather=True,
         )
 
         if not self.training and (self.report_cer or self.report_wer):
             if self.error_calculator is None:
-                from espnet2.asr_transducer.error_calculator import ErrorCalculator
+                from funasr.modules.e2e_asr_common import ErrorCalculatorTransducer as ErrorCalculator
 
                 self.error_calculator = ErrorCalculator(
                     self.decoder,
                     self.joint_network,
                     self.token_list,
                     self.sym_space,
                     self.sym_blank,
                     report_cer=self.report_cer,
                     report_wer=self.report_wer,
                 )
 
-            cer_transducer, wer_transducer = self.error_calculator(encoder_out, target)
+            cer_transducer, wer_transducer = self.error_calculator(encoder_out, target, t_len)
 
             return loss_transducer, cer_transducer, wer_transducer
 
         return loss_transducer, None, None
 
     def _calc_ctc_loss(
         self,
@@ -527,16 +527,16 @@
         auxiliary_lm_loss_weight: float = 0.0,
         auxiliary_lm_loss_smoothing: float = 0.0,
         ignore_id: int = -1,
         sym_space: str = "<space>",
         sym_blank: str = "<blank>",
         report_cer: bool = True,
         report_wer: bool = True,
-        sym_sos: str = "<sos/eos>",
-        sym_eos: str = "<sos/eos>",
+        sym_sos: str = "<s>",
+        sym_eos: str = "</s>",
         extract_feats_in_collect_stats: bool = True,
         lsm_weight: float = 0.0,
         length_normalized_loss: bool = False,
     ) -> None:
         """Construct an ESPnetASRTransducerModel object."""
         super().__init__()
 
@@ -885,25 +885,27 @@
                 blank=self.blank_id,
                 fastemit_lambda=self.fastemit_lambda,
                 gather=True,
         )
 
         if not self.training and (self.report_cer or self.report_wer):
             if self.error_calculator is None:
+                from funasr.modules.e2e_asr_common import ErrorCalculatorTransducer as ErrorCalculator
+
                 self.error_calculator = ErrorCalculator(
                     self.decoder,
                     self.joint_network,
                     self.token_list,
                     self.sym_space,
                     self.sym_blank,
                     report_cer=self.report_cer,
                     report_wer=self.report_wer,
                 )
 
-            cer_transducer, wer_transducer = self.error_calculator(encoder_out, target)
+            cer_transducer, wer_transducer = self.error_calculator(encoder_out, target, t_len)
             return loss_transducer, cer_transducer, wer_transducer
 
         return loss_transducer, None, None
 
     def _calc_ctc_loss(
         self,
         encoder_out: torch.Tensor,
```

### Comparing `funasr-0.4.3/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.4.4/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/e2e_diar_sond.py` & `funasr-0.4.4/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/e2e_sv.py` & `funasr-0.4.4/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/e2e_tp.py` & `funasr-0.4.4/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/e2e_uni_asr.py` & `funasr-0.4.4/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/e2e_vad.py` & `funasr-0.4.4/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/conformer_encoder.py` & `funasr-0.4.4/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.4.4/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.4.4/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.4.4/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.4.4/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.4.4/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.4.4/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.4.4/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.4.4/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.4.4/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.4.4/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/rnn_encoder.py` & `funasr-0.4.4/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/encoder/sanm_encoder.py` & `funasr-0.4.4/funasr/models/encoder/sanm_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 import logging
 import torch
 import torch.nn as nn
+import torch.nn.functional as F
 from funasr.modules.streaming_utils.chunk_utilis import overlap_chunk
 from typeguard import check_argument_types
 import numpy as np
+from funasr.torch_utils.device_funcs import to_device
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.attention import MultiHeadedAttention, MultiHeadedAttentionSANM, MultiHeadedAttentionSANMwithMask
 from funasr.modules.embedding import SinusoidalPositionEncoder, StreamSinusoidalPositionEncoder
 from funasr.modules.layer_norm import LayerNorm
 from funasr.modules.multi_layer_conv import Conv1dLinear
 from funasr.modules.multi_layer_conv import MultiLayeredConv1d
 from funasr.modules.positionwise_feed_forward import (
@@ -345,26 +347,46 @@
             xs_pad = self.after_norm(xs_pad)
 
         olens = masks.squeeze(1).sum(1)
         if len(intermediate_outs) > 0:
             return (xs_pad, intermediate_outs), olens, None
         return xs_pad, olens, None
 
+    def _add_overlap_chunk(self, feats: np.ndarray, cache: dict = {}):
+        if len(cache) == 0:
+            return feats
+        # process last chunk
+        cache["feats"] = to_device(cache["feats"], device=feats.device)
+        overlap_feats = torch.cat((cache["feats"], feats), dim=1)
+        if cache["is_final"]:
+            cache["feats"] = overlap_feats[:, -cache["chunk_size"][0]:, :]
+            if not cache["last_chunk"]:
+               padding_length = sum(cache["chunk_size"]) - overlap_feats.shape[1]
+               overlap_feats = overlap_feats.transpose(1, 2)
+               overlap_feats = F.pad(overlap_feats, (0, padding_length))
+               overlap_feats = overlap_feats.transpose(1, 2)
+        else:
+            cache["feats"] = overlap_feats[:, -(cache["chunk_size"][0] + cache["chunk_size"][2]):, :]
+        return overlap_feats
+
     def forward_chunk(self,
                       xs_pad: torch.Tensor,
                       ilens: torch.Tensor,
                       cache: dict = None,
                       ctc: CTC = None,
                       ):
         xs_pad *= self.output_size() ** 0.5
         if self.embed is None:
             xs_pad = xs_pad
         else:
             xs_pad = self.embed(xs_pad, cache)
-
+        if cache["tail_chunk"]:
+            xs_pad = cache["feats"]
+        else:
+            xs_pad = self._add_overlap_chunk(xs_pad, cache)
         encoder_outs = self.encoders0(xs_pad, None, None, None, None)
         xs_pad, masks = encoder_outs[0], encoder_outs[1]
         intermediate_outs = []
         if len(self.interctc_layer_idx) == 0:
             encoder_outs = self.encoders(xs_pad, None, None, None, None)
             xs_pad, masks = encoder_outs[0], encoder_outs[1]
         else:
```

### Comparing `funasr-0.4.3/funasr/models/encoder/transformer_encoder.py` & `funasr-0.4.4/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/frontend/default.py` & `funasr-0.4.4/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.4.4/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/frontend/fused.py` & `funasr-0.4.4/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/frontend/s3prl.py` & `funasr-0.4.4/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/frontend/wav_frontend.py` & `funasr-0.4.4/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.4.4/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/frontend/windowing.py` & `funasr-0.4.4/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/joint_net/joint_network.py` & `funasr-0.4.4/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/pooling/statistic_pooling.py` & `funasr-0.4.4/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.4.4/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/predictor/cif.py` & `funasr-0.4.4/funasr/models/predictor/cif.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch
 from torch import nn
 import logging
 import numpy as np
+from funasr.torch_utils.device_funcs import to_device
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.streaming_utils.utils import sequence_mask
 
 class CifPredictor(nn.Module):
     def __init__(self, idim, l_order, r_order, threshold=1.0, dropout=0.1, smooth_factor=1.0, noise_threshold=0, tail_threshold=0.45):
         super(CifPredictor, self).__init__()
 
@@ -196,77 +197,100 @@
         if target_length is None and self.tail_threshold > 0.0:
             token_num_int = torch.max(token_num).type(torch.int32).item()
             acoustic_embeds = acoustic_embeds[:, :token_num_int, :]
 
         return acoustic_embeds, token_num, alphas, cif_peak
 
     def forward_chunk(self, hidden, cache=None):
-        b, t, d = hidden.size()
+        batch_size, len_time, hidden_size = hidden.shape
         h = hidden
         context = h.transpose(1, 2)
         queries = self.pad(context)
         output = torch.relu(self.cif_conv1d(queries))
         output = output.transpose(1, 2)
         output = self.cif_output(output)
         alphas = torch.sigmoid(output)
         alphas = torch.nn.functional.relu(alphas * self.smooth_factor - self.noise_threshold)
 
         alphas = alphas.squeeze(-1)
-        mask_chunk_predictor = None
-        if cache is not None:
-            mask_chunk_predictor = None
-            mask_chunk_predictor = torch.zeros_like(alphas)
-            mask_chunk_predictor[:, cache["pad_left"]:cache["stride"] + cache["pad_left"]] = 1.0
-       
-        if mask_chunk_predictor is not None:
-            alphas = alphas * mask_chunk_predictor
-      
-        if cache is not None:
-            if cache["is_final"]:
-                alphas[:, cache["stride"] + cache["pad_left"] - 1] += 0.45
-            if cache["cif_hidden"] is not None:
-                hidden = torch.cat((cache["cif_hidden"], hidden), 1)
-            if cache["cif_alphas"] is not None:
-                alphas = torch.cat((cache["cif_alphas"], alphas), -1)
 
-        token_num = alphas.sum(-1)
-        acoustic_embeds, cif_peak = cif(hidden, alphas, self.threshold)
-        len_time = alphas.size(-1)
-        last_fire_place = len_time - 1
-        last_fire_remainds = 0.0
-        pre_alphas_length = 0
-        last_fire = False
- 
-        mask_chunk_peak_predictor = None
-        if cache is not None:
-            mask_chunk_peak_predictor = None
-            mask_chunk_peak_predictor = torch.zeros_like(cif_peak)
-            if cache["cif_alphas"] is not None:
-                pre_alphas_length = cache["cif_alphas"].size(-1)
-                mask_chunk_peak_predictor[:, :pre_alphas_length] = 1.0
-            mask_chunk_peak_predictor[:, pre_alphas_length + cache["pad_left"]:pre_alphas_length + cache["stride"] + cache["pad_left"]] = 1.0
-            
-        if mask_chunk_peak_predictor is not None:
-            cif_peak = cif_peak * mask_chunk_peak_predictor.squeeze(-1)
-        
-        for i in range(len_time):
-            if cif_peak[0][len_time - 1 - i] > self.threshold or cif_peak[0][len_time - 1 - i] == self.threshold:
-                last_fire_place = len_time - 1 - i
-                last_fire_remainds = cif_peak[0][len_time - 1 - i] - self.threshold
-                last_fire = True
-                break
-        if last_fire:
-           last_fire_remainds = torch.tensor([last_fire_remainds], dtype=alphas.dtype).to(alphas.device)
-           cache["cif_hidden"] = hidden[:, last_fire_place:, :]
-           cache["cif_alphas"] = torch.cat((last_fire_remainds.unsqueeze(0), alphas[:, last_fire_place+1:]), -1)
-        else:
-           cache["cif_hidden"] = hidden
-           cache["cif_alphas"] = alphas
-        token_num_int = token_num.floor().type(torch.int32).item()
-        return acoustic_embeds[:, 0:token_num_int, :], token_num, alphas, cif_peak
+        token_length = []
+        list_fires = []
+        list_frames = []
+        cache_alphas = []
+        cache_hiddens = []
+
+        if cache is not None and "chunk_size" in cache:
+            alphas[:, :cache["chunk_size"][0]] = 0.0
+            alphas[:, sum(cache["chunk_size"][:2]):] = 0.0
+        if cache is not None and "cif_alphas" in cache and "cif_hidden" in cache:
+            cache["cif_hidden"] = to_device(cache["cif_hidden"], device=hidden.device)
+            cache["cif_alphas"] = to_device(cache["cif_alphas"], device=alphas.device)
+            hidden = torch.cat((cache["cif_hidden"], hidden), dim=1)
+            alphas = torch.cat((cache["cif_alphas"], alphas), dim=1)
+        if cache is not None and "last_chunk" in cache and cache["last_chunk"]:
+            tail_hidden = torch.zeros((batch_size, 1, hidden_size), device=hidden.device)
+            tail_alphas = torch.tensor([[self.tail_threshold]], device=alphas.device)
+            tail_alphas = torch.tile(tail_alphas, (batch_size, 1))
+            hidden = torch.cat((hidden, tail_hidden), dim=1)
+            alphas = torch.cat((alphas, tail_alphas), dim=1)
+
+        len_time = alphas.shape[1]
+        for b in range(batch_size):
+            integrate = 0.0
+            frames = torch.zeros((hidden_size), device=hidden.device)
+            list_frame = []
+            list_fire = []
+            for t in range(len_time):
+                alpha = alphas[b][t]
+                if alpha + integrate < self.threshold:
+                    integrate += alpha
+                    list_fire.append(integrate)
+                    frames += alpha * hidden[b][t]
+                else:
+                    frames += (self.threshold - integrate) * hidden[b][t]
+                    list_frame.append(frames)
+                    integrate += alpha
+                    list_fire.append(integrate)
+                    integrate -= self.threshold
+                    frames = integrate * hidden[b][t]
+
+            cache_alphas.append(integrate)
+            if integrate > 0.0:
+                cache_hiddens.append(frames / integrate)
+            else:
+                cache_hiddens.append(frames)
+
+            token_length.append(torch.tensor(len(list_frame), device=alphas.device))
+            list_fires.append(list_fire)
+            list_frames.append(list_frame)
+
+        cache["cif_alphas"] = torch.stack(cache_alphas, axis=0)
+        cache["cif_alphas"] = torch.unsqueeze(cache["cif_alphas"], axis=0)
+        cache["cif_hidden"] = torch.stack(cache_hiddens, axis=0)
+        cache["cif_hidden"] = torch.unsqueeze(cache["cif_hidden"], axis=0)
+
+        max_token_len = max(token_length)
+        if max_token_len == 0:
+             return hidden, torch.stack(token_length, 0)
+        list_ls = []
+        for b in range(batch_size):
+            pad_frames = torch.zeros((max_token_len - token_length[b], hidden_size), device=alphas.device)
+            if token_length[b] == 0:
+                list_ls.append(pad_frames)
+            else:
+                list_frames[b] = torch.stack(list_frames[b])
+                list_ls.append(torch.cat((list_frames[b], pad_frames), dim=0))
+
+        cache["cif_alphas"] = torch.stack(cache_alphas, axis=0)
+        cache["cif_alphas"] = torch.unsqueeze(cache["cif_alphas"], axis=0)
+        cache["cif_hidden"] = torch.stack(cache_hiddens, axis=0)
+        cache["cif_hidden"] = torch.unsqueeze(cache["cif_hidden"], axis=0)
+        return torch.stack(list_ls, 0), torch.stack(token_length, 0)
+
 
     def tail_process_fn(self, hidden, alphas, token_num=None, mask=None):
         b, t, d = hidden.size()
         tail_threshold = self.tail_threshold
         if mask is not None:
             zeros_t = torch.zeros((b, 1), dtype=torch.float32, device=alphas.device)
             ones_t = torch.ones_like(zeros_t)
```

### Comparing `funasr-0.4.3/funasr/models/preencoder/linear.py` & `funasr-0.4.4/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/preencoder/sinc.py` & `funasr-0.4.4/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/specaug/specaug.py` & `funasr-0.4.4/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/target_delay_transformer.py` & `funasr-0.4.4/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/models/vad_realtime_transformer.py` & `funasr-0.4.4/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/add_sos_eos.py` & `funasr-0.4.4/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/attention.py` & `funasr-0.4.4/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.4.4/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.4.4/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/beam_search/beam_search.py` & `funasr-0.4.4/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.4.4/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/data2vec/data_utils.py` & `funasr-0.4.4/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/data2vec/ema_module.py` & `funasr-0.4.4/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.4.4/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/data2vec/quant_noise.py` & `funasr-0.4.4/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/data2vec/utils.py` & `funasr-0.4.4/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.4.4/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/dynamic_conv.py` & `funasr-0.4.4/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/dynamic_conv2d.py` & `funasr-0.4.4/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/e2e_asr_common.py` & `funasr-0.4.4/funasr/modules/e2e_asr_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,31 +292,35 @@
         self.space = sym_space
         self.blank = sym_blank
 
         self.report_cer = report_cer
         self.report_wer = report_wer
 
     def __call__(
-        self, encoder_out: torch.Tensor, target: torch.Tensor
+        self, encoder_out: torch.Tensor, target: torch.Tensor, encoder_out_lens: torch.Tensor,
     ) -> Tuple[Optional[float], Optional[float]]:
         """Calculate sentence-level WER or/and CER score for Transducer model.
         Args:
             encoder_out: Encoder output sequences. (B, T, D_enc)
             target: Target label ID sequences. (B, L)
+            encoder_out_lens: Encoder output sequences length. (B,)
         Returns:
             : Sentence-level CER score.
             : Sentence-level WER score.
         """
         cer, wer = None, None
 
         batchsize = int(encoder_out.size(0))
 
         encoder_out = encoder_out.to(next(self.decoder.parameters()).device)
 
-        batch_nbest = [self.beam_search(encoder_out[b]) for b in range(batchsize)]
+        batch_nbest = [
+            self.beam_search(encoder_out[b][: encoder_out_lens[b]])
+            for b in range(batchsize)
+        ]
         pred = [nbest_hyp[0].yseq[1:] for nbest_hyp in batch_nbest]
 
         char_pred, char_target = self.convert_to_char(pred, target)
 
         if self.report_cer:
             cer = self.calculate_cer(char_pred, char_target)
```

### Comparing `funasr-0.4.3/funasr/modules/eend_ola/encoder.py` & `funasr-0.4.4/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.4.4/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/embedding.py` & `funasr-0.4.4/funasr/modules/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,29 +421,22 @@
         inv_timescales = torch.exp(torch.arange(depth / 2).type(dtype) * (-log_timescale_increment))
         inv_timescales = torch.reshape(inv_timescales, [batch_size, -1])
         scaled_time = torch.reshape(positions, [1, -1, 1]) * torch.reshape(inv_timescales, [1, 1, -1])
         encoding = torch.cat([torch.sin(scaled_time), torch.cos(scaled_time)], dim=2)
         return encoding.type(dtype)
 
     def forward(self, x, cache=None):
-        start_idx = 0
-        pad_left = 0
-        pad_right = 0
         batch_size, timesteps, input_dim = x.size()
+        start_idx = 0
         if cache is not None:
             start_idx = cache["start_idx"]
-            pad_left = cache["left"]
-            pad_right = cache["right"]
+            cache["start_idx"] += timesteps
         positions = torch.arange(1, timesteps+start_idx+1)[None, :]
         position_encoding = self.encode(positions, input_dim, x.dtype).to(x.device)
-        outputs = x + position_encoding[:, start_idx: start_idx + timesteps]
-        outputs = outputs.transpose(1, 2)
-        outputs = F.pad(outputs, (pad_left, pad_right))
-        outputs = outputs.transpose(1, 2)
-        return outputs
+        return x + position_encoding[:, start_idx: start_idx + timesteps]
 
 class StreamingRelPositionalEncoding(torch.nn.Module):
     """Relative positional encoding.
     Args:
         size: Module size.
         max_len: Maximum input length.
         dropout_rate: Dropout rate.
```

### Comparing `funasr-0.4.3/funasr/modules/frontends/beamformer.py` & `funasr-0.4.4/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.4.4/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.4.4/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/frontends/feature_transform.py` & `funasr-0.4.4/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/frontends/frontend.py` & `funasr-0.4.4/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/frontends/mask_estimator.py` & `funasr-0.4.4/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/layer_norm.py` & `funasr-0.4.4/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/lightconv.py` & `funasr-0.4.4/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/lightconv2d.py` & `funasr-0.4.4/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/mask.py` & `funasr-0.4.4/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/multi_layer_conv.py` & `funasr-0.4.4/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/nets_utils.py` & `funasr-0.4.4/funasr/modules/nets_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,15 +591,15 @@
     Returns:
         mask: Chunk mask. (size, size)
 
     """
     mask = torch.zeros(size, size, device=device, dtype=torch.bool)
 
     for i in range(size):
-        if left_chunk_size <= 0:
+        if left_chunk_size < 0:
             start = 0
         else:
             start = max((i // chunk_size - left_chunk_size) * chunk_size, 0)
 
         end = min((i // chunk_size + 1) * chunk_size, size)
         mask[i, start:end] = True
```

### Comparing `funasr-0.4.3/funasr/modules/positionwise_feed_forward.py` & `funasr-0.4.4/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/repeat.py` & `funasr-0.4.4/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/rnn/argument.py` & `funasr-0.4.4/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/rnn/attentions.py` & `funasr-0.4.4/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/rnn/decoders.py` & `funasr-0.4.4/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/rnn/encoders.py` & `funasr-0.4.4/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/scorers/ctc.py` & `funasr-0.4.4/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.4.4/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/scorers/length_bonus.py` & `funasr-0.4.4/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/scorers/scorer_interface.py` & `funasr-0.4.4/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.4.4/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.4.4/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/streaming_utils/utils.py` & `funasr-0.4.4/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/subsampling.py` & `funasr-0.4.4/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/modules/subsampling_without_posenc.py` & `funasr-0.4.4/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/optimizers/fairseq_adam.py` & `funasr-0.4.4/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/optimizers/sgd.py` & `funasr-0.4.4/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/libtorch/demo.py` & `funasr-0.4.4/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.4.4/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/libtorch/setup.py` & `funasr-0.4.4/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/demo.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import os.path
 from pathlib import Path
 from typing import List, Union, Tuple
 
 import copy
 import librosa
@@ -15,14 +17,19 @@
 from .utils.frontend import WavFrontend
 from .utils.timestamp_utils import time_stamp_lfr6_onnx
 
 logging = get_logger()
 
 
 class Paraformer():
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    Paraformer: Fast and Accurate Parallel Transformer for Non-autoregressive End-to-End Speech Recognition
+    https://arxiv.org/abs/2206.08317
+    """
     def __init__(self, model_dir: Union[str, Path] = None,
                  batch_size: int = 1,
                  device_id: Union[str, int] = "-1",
                  plot_timestamp_to: str = "",
                  quantize: bool = False,
                  intra_op_num_threads: int = 4,
                  ):
```

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import os.path
 from pathlib import Path
 from typing import List, Union, Tuple
 import numpy as np
 
 from .utils.utils import (ONNXRuntimeError,
```

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
+
 from enum import Enum
 from typing import List, Tuple, Dict, Any
 
 import math
 import numpy as np
 
 class VadStateMachine(Enum):
@@ -185,14 +189,19 @@
         return AudioChangeState.kChangeStateInvalid
 
     def FrameSizeMs(self) -> int:
         return int(self.frame_size_ms)
 
 
 class E2EVadModel():
+    """
+    Author: Speech Lab of DAMO Academy, Alibaba Group
+    Deep-FSMN for Large Vocabulary Continuous Speech Recognition
+    https://arxiv.org/abs/1803.05030
+    """
     def __init__(self, vad_post_args: Dict[str, Any]):
         super(E2EVadModel, self).__init__()
         self.vad_opts = VADXOptions(**vad_post_args)
         self.windows_detector = WindowDetector(self.vad_opts.window_size_ms,
                                                self.vad_opts.sil_to_speech_time_thres,
                                                self.vad_opts.speech_to_sil_time_thres,
                                                self.vad_opts.frame_in_ms)
```

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Copyright (c) Alibaba, Inc. and its affiliates.
+# -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import string
 import logging
 from typing import Any, List, Union
 
 
 def isChinese(ch: str):
```

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
+
 import numpy as np
 
 
 def time_stamp_lfr6_onnx(us_cif_peak, char_list, begin_time=0.0, total_offset=-1.5):
     if not len(char_list):
         return []
     START_END_THRESHOLD = 5
```

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- encoding: utf-8 -*-
+# Copyright FunASR (https://github.com/alibaba-damo-academy/FunASR). All Rights Reserved.
+#  MIT License  (https://opensource.org/licenses/MIT)
 
 import os.path
 from pathlib import Path
 from typing import List, Union, Tuple
 
 import copy
 import librosa
```

### Comparing `funasr-0.4.3/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.4.4/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/samplers/build_batch_sampler.py` & `funasr-0.4.4/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/samplers/folded_batch_sampler.py` & `funasr-0.4.4/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/samplers/length_batch_sampler.py` & `funasr-0.4.4/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.4.4/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.4.4/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.4.4/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/schedulers/abs_scheduler.py` & `funasr-0.4.4/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/schedulers/noam_lr.py` & `funasr-0.4.4/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.4.4/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/schedulers/warmup_lr.py` & `funasr-0.4.4/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/tasks/abs_task.py` & `funasr-0.4.4/funasr/tasks/abs_task.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/tasks/asr.py` & `funasr-0.4.4/funasr/tasks/asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/tasks/data2vec.py` & `funasr-0.4.4/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/tasks/diar.py` & `funasr-0.4.4/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/tasks/lm.py` & `funasr-0.4.4/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/tasks/punctuation.py` & `funasr-0.4.4/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/tasks/sv.py` & `funasr-0.4.4/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/tasks/vad.py` & `funasr-0.4.4/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/text/build_tokenizer.py` & `funasr-0.4.4/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/text/char_tokenizer.py` & `funasr-0.4.4/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/text/cleaner.py` & `funasr-0.4.4/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/text/korean_cleaner.py` & `funasr-0.4.4/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/text/phoneme_tokenizer.py` & `funasr-0.4.4/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.4.4/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/text/token_id_converter.py` & `funasr-0.4.4/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/text/word_tokenizer.py` & `funasr-0.4.4/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.4.4/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/torch_utils/device_funcs.py` & `funasr-0.4.4/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/torch_utils/forward_adaptor.py` & `funasr-0.4.4/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/torch_utils/initialize.py` & `funasr-0.4.4/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.4.4/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/torch_utils/model_summary.py` & `funasr-0.4.4/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/torch_utils/recursive_op.py` & `funasr-0.4.4/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/train/abs_espnet_model.py` & `funasr-0.4.4/funasr/train/abs_espnet_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/train/abs_model.py` & `funasr-0.4.4/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/train/class_choices.py` & `funasr-0.4.4/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/train/distributed_utils.py` & `funasr-0.4.4/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/train/reporter.py` & `funasr-0.4.4/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/train/trainer.py` & `funasr-0.4.4/funasr/train/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/asr_env_checking.py` & `funasr-0.4.4/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/asr_utils.py` & `funasr-0.4.4/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/build_dataclass.py` & `funasr-0.4.4/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/cli_utils.py` & `funasr-0.4.4/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/compute_eer.py` & `funasr-0.4.4/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/compute_min_dcf.py` & `funasr-0.4.4/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/compute_wer.py` & `funasr-0.4.4/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/config_argparse.py` & `funasr-0.4.4/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/get_default_kwargs.py` & `funasr-0.4.4/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/griffin_lim.py` & `funasr-0.4.4/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/job_runner.py` & `funasr-0.4.4/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/misc.py` & `funasr-0.4.4/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/modelscope_param.py` & `funasr-0.4.4/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/nested_dict_action.py` & `funasr-0.4.4/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/postprocess_utils.py` & `funasr-0.4.4/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/sized_dict.py` & `funasr-0.4.4/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/timestamp_tools.py` & `funasr-0.4.4/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/types.py` & `funasr-0.4.4/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.4.3/funasr/utils/wav_utils.py` & `funasr-0.4.4/funasr/utils/wav_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         wav_lines = f_wav.readlines()
         text_lines = f_text.readlines()
     os.rename(wav_file, "{}.bak".format(wav_file))
     os.rename(text_file, "{}.bak".format(text_file))
     wav_dict = {}
     for line in wav_lines:
         parts = line.strip().split()
-        if len(parts) < 2:
+        if len(parts) != 2:
             continue
         sample_name, wav_path = parts
         wav_dict[sample_name] = wav_path
     text_dict = {}
     for line in text_lines:
         parts = line.strip().split()
         if len(parts) < 2:
```

### Comparing `funasr-0.4.3/funasr.egg-info/PKG-INFO` & `funasr-0.4.4/funasr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.4.3
+Version: 0.4.4
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -41,22 +42,20 @@
 | [**Installation**](#installation)
 | [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html)
 | [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C)
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/modelscope_models.md)
 | [**Contact**](#contact)
-|
-[**M2MET2.0 Guidence_CN**](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)
-| [**M2MET2.0 Guidence_EN**](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)
+| [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
-## Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
-We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
 ## What's new: 
-
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge
+We are pleased to announce that the M2MeT2.0 challenge will be held in the near future. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
+### Release notes
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification and Speaker diarization.   
 - We have released large number of academic and industrial pretrained models on [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
 - The pretrained model [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best performance on many tasks in [SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard)
 - FunASR supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition)
@@ -85,15 +84,15 @@
 
 ```shell
 pip install -U modelscope
 # For the users in China, you could install with the command:
 # pip install -U modelscope -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/simple
 ```
 
-For more details, please ref to [installation](https://github.com/alibaba-damo-academy/FunASR/wiki)
+For more details, please ref to [installation](https://alibaba-damo-academy.github.io/FunASR/en/installation.html)
 
 [//]: # ()
 [//]: # (## Usage)
 
 [//]: # (For users who are new to FunASR and ModelScope, please refer to FunASR Docs&#40;[CN]&#40;https://alibaba-damo-academy.github.io/FunASR/cn/index.html&#41; / [EN]&#40;https://alibaba-damo-academy.github.io/FunASR/en/index.html&#41;&#41;)
 
 ## Contact
@@ -104,23 +103,25 @@
 
 |Dingding group |                     Wechat group                      |
 |:---:|:-----------------------------------------------------:|
 |<div align="left"><img src="docs/images/dingding.jpg" width="250"/> | <img src="docs/images/wechat.png" width="232"/></div> |
 
 ## Contributors
 
-| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/DeepScience.png" width="200"/> </div> |
-|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:-----------------------------------------------------------:|
+| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/DeepScience.png" width="200"/> </div> |
+|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|
 
 ## Acknowledge
 
 1. We borrowed a lot of code from [Kaldi](http://kaldi-asr.org/) for data preparation.
 2. We borrowed a lot of code from [ESPnet](https://github.com/espnet/espnet). FunASR follows up the training and finetuning pipelines of ESPnet.
 3. We referred [Wenet](https://github.com/wenet-e2e/wenet) for building dataloader for large scale data training.
-4. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
+4. We acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for contributing the VAD runtime. 
+5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
+6. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 
 ## Citations
 
 ``` bibtex
@@ -139,7 +140,9 @@
 @inproceedings{Shi2023AchievingTP,
   title={Achieving Timestamp Prediction While Recognizing with Non-Autoregressive End-to-End ASR Model},
   author={Xian Shi and Yanni Chen and Shiliang Zhang and Zhijie Yan},
   booktitle={arXiv preprint arXiv:2301.12343}
   year={2023}
 }
 ```
+
+
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.4.3 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.4.4 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
-System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
-Provides-Extra: train Provides-Extra: recipe Provides-Extra: all Provides-
-Extra: test Provides-Extra: doc License-File: LICENSE [//]: # (
+License Platform: UNKNOWN Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Science/
+Research Classifier: Operating System :: POSIX :: Linux Classifier: License ::
+OSI Approved :: Apache Software License Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown Provides-Extra: train Provides-Extra:
+recipe Provides-Extra: all Provides-Extra: test Provides-Extra: doc License-
+File: LICENSE [//]: # (
 [docs/images/funasr_logo.jpg]
 ) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
@@ -27,76 +28,83 @@
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Docs**](https://alibaba-damo-academy.github.io/FunASR/en/index.html) |
 [**Tutorial**](https://github.com/alibaba-damo-academy/FunASR/
 wiki#funasr%E7%94%A8%E6%88%B7%E6%89%8B%E5%86%8C) | [**Papers**](https://
 github.com/alibaba-damo-academy/FunASR#citations) | [**Runtime**](https://
 github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime) | [**Model
 Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/
-modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Guidence_CN**]
-(https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html) |
-[**M2MET2.0 Guidence_EN**](https://alibaba-damo-academy.github.io/FunASR/
-m2met2/index.html) ## Multi-Channel Multi-Party Meeting Transcription 2.0
-(M2MET2.0) Challenge We are pleased to announce that the M2MeT2.0 challenge
-will be held in the near future. The baseline system is conducted on FunASR and
-is provided as a receipe of AliMeeting corpus. For more details you can see the
-guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/
-m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/
-m2met2/index.html)). ## What's new: For the release notes, please ref to [news]
-(https://github.com/alibaba-damo-academy/FunASR/releases) ## Highlights -
-FunASR supports speech recognition(ASR), Multi-talker ASR, Voice Activity
-Detection(VAD), Punctuation Restoration, Language Models, Speaker Verification
-and Speaker diarization. - We have released large number of academic and
-industrial pretrained models on [ModelScope](https://www.modelscope.cn/
-models?page=1&tasks=auto-speech-recognition) - The pretrained model
-[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) obtains the best
-performance on many tasks in [SpeechIO leaderboard](https://github.com/
-SpeechColab/Leaderboard) - FunASR supplies a easy-to-use pipeline to finetune
-pretrained models from [ModelScope](https://www.modelscope.cn/
-models?page=1&tasks=auto-speech-recognition) - Compared to [Espnet](https://
-github.com/espnet/espnet) framework, the training speed of large-scale datasets
-in FunASR is much faster owning to the optimized dataloader. ## Installation
-Install from pip ```shell pip install -U funasr # For the users in China, you
-could install with the command: # pip install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip install -e ./ #
-For the users in China, you could install with the command: # pip install -e ./
--i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip install -U modelscope # For the users in China, you could install with the
-command: # pip install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://github.com/
-alibaba-damo-academy/FunASR/wiki) [//]: # () [//]: # (## Usage) [//]: # (For
-users who are new to FunASR and ModelScope, please refer to FunASR Docs([CN]
-(https://alibaba-damo-academy.github.io/FunASR/cn/index.html) / [EN](https://
-alibaba-damo-academy.github.io/FunASR/en/index.html))) ## Contact If you have
-any questions about FunASR, please contact us by - email: [funasr@list.alibaba-
-inc.com](funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:
------------------------------------------------------:| |
+modelscope_models.md) | [**Contact**](#contact) | [**M2MET2.0 Challenge**]
+(https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-
+meeting-transcription-20-m2met20-challenge) ## What's new: ### Multi-Channel
+Multi-Party Meeting Transcription 2.0 (M2MET2.0) Challenge We are pleased to
+announce that the M2MeT2.0 challenge will be held in the near future. The
+baseline system is conducted on FunASR and is provided as a receipe of
+AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN]
+(https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN]
+(https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release
+notes For the release notes, please ref to [news](https://github.com/alibaba-
+damo-academy/FunASR/releases) ## Highlights - FunASR supports speech
+recognition(ASR), Multi-talker ASR, Voice Activity Detection(VAD), Punctuation
+Restoration, Language Models, Speaker Verification and Speaker diarization. -
+We have released large number of academic and industrial pretrained models on
+[ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-
+recognition) - The pretrained model [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) obtains the best performance on many tasks in
+[SpeechIO leaderboard](https://github.com/SpeechColab/Leaderboard) - FunASR
+supplies a easy-to-use pipeline to finetune pretrained models from [ModelScope]
+(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition) -
+Compared to [Espnet](https://github.com/espnet/espnet) framework, the training
+speed of large-scale datasets in FunASR is much faster owning to the optimized
+dataloader. ## Installation Install from pip ```shell pip install -U funasr #
+For the users in China, you could install with the command: # pip install -
+U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from
+source code ``` sh git clone https://github.com/alibaba/FunASR.git && cd FunASR
+pip install -e ./ # For the users in China, you could install with the command:
+# pip install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you
+want to use the pretrained models in ModelScope, you should install the
+modelscope: ```shell pip install -U modelscope # For the users in China, you
+could install with the command: # pip install -U modelscope -f https://
+modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/
+installation.html) [//]: # () [//]: # (## Usage) [//]: # (For users who are new
+to FunASR and ModelScope, please refer to FunASR Docs([CN](https://alibaba-
+damo-academy.github.io/FunASR/cn/index.html) / [EN](https://alibaba-damo-
+academy.github.io/FunASR/en/index.html))) ## Contact If you have any questions
+about FunASR, please contact us by - email: [funasr@list.alibaba-inc.com]
+(funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:--------
+---------------------------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
-[docs/images/nwpu.png] | [docs/images/DeepScience.png]
+[docs/images/nwpu.png] | [docs/images/China_Telecom.png]
+| [docs/images/RapidAI.png]
+| [docs/images/DeepScience.png]
 | |:---------------------------------------------------------------:|:---------
 ------------------------------------------------------:|:----------------------
--------------------------------------:| ## Acknowledge 1. We borrowed a lot of
-code from [Kaldi](http://kaldi-asr.org/) for data preparation. 2. We borrowed a
-lot of code from [ESPnet](https://github.com/espnet/espnet). FunASR follows up
-the training and finetuning pipelines of ESPnet. 3. We referred [Wenet](https:/
-/github.com/wenet-e2e/wenet) for building dataloader for large scale data
-training. 4. We acknowledge [DeepScience](https://www.deepscience.cn) for
-contributing the grpc service. ## License This project is licensed under the
-[The MIT License](https://opensource.org/licenses/MIT). FunASR also contains
-various third-party components and some code modified from other repos under
-other open source licenses. ## Citations ``` bibtex @inproceedings
-{gao2022paraformer, title={Paraformer: Fast and Accurate Parallel Transformer
-for Non-autoregressive End-to-End Speech Recognition}, author={Gao, Zhifu and
-Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie}, booktitle={INTERSPEECH},
-year={2022} } @inproceedings{gao2020universal, title={Universal ASR: Unifying
-Streaming and Non-Streaming ASR Using a Single Encoder-Decoder Model}, author=
-{Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin, Ian}, booktitle=
-{arXiv preprint arXiv:2010.14099}, year={2020} } @inproceedings
+----------------------------------------:|:------------------------------------
+-------------------:|:---------------------------------------------------------
+--:| ## Acknowledge 1. We borrowed a lot of code from [Kaldi](http://kaldi-
+asr.org/) for data preparation. 2. We borrowed a lot of code from [ESPnet]
+(https://github.com/espnet/espnet). FunASR follows up the training and
+finetuning pipelines of ESPnet. 3. We referred [Wenet](https://github.com/
+wenet-e2e/wenet) for building dataloader for large scale data training. 4. We
+acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-
+httpserver) for contributing the VAD runtime. 5. We acknowledge [RapidAI]
+(https://github.com/RapidAI) for contributing the Paraformer and
+CT_Transformer-punc runtime. 6. We acknowledge [DeepScience](https://
+www.deepscience.cn) for contributing the grpc service. ## License This project
+is licensed under the [The MIT License](https://opensource.org/licenses/MIT).
+FunASR also contains various third-party components and some code modified from
+other repos under other open source licenses. ## Citations ``` bibtex
+@inproceedings{gao2022paraformer, title={Paraformer: Fast and Accurate Parallel
+Transformer for Non-autoregressive End-to-End Speech Recognition}, author={Gao,
+Zhifu and Zhang, Shiliang and McLoughlin, Ian and Yan, Zhijie}, booktitle=
+{INTERSPEECH}, year={2022} } @inproceedings{gao2020universal, title={Universal
+ASR: Unifying Streaming and Non-Streaming ASR Using a Single Encoder-Decoder
+Model}, author={Gao, Zhifu and Zhang, Shiliang and Lei, Ming and McLoughlin,
+Ian}, booktitle={arXiv preprint arXiv:2010.14099}, year={2020} } @inproceedings
 {Shi2023AchievingTP, title={Achieving Timestamp Prediction While Recognizing
 with Non-Autoregressive End-to-End ASR Model}, author={Xian Shi and Yanni Chen
 and Shiliang Zhang and Zhijie Yan}, booktitle={arXiv preprint arXiv:2301.12343}
 year={2023} } ```
```

### Comparing `funasr-0.4.3/funasr.egg-info/SOURCES.txt` & `funasr-0.4.4/funasr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -347,15 +347,8 @@
 funasr/utils/modelscope_param.py
 funasr/utils/nested_dict_action.py
 funasr/utils/postprocess_utils.py
 funasr/utils/sized_dict.py
 funasr/utils/timestamp_tools.py
 funasr/utils/types.py
 funasr/utils/wav_utils.py
-funasr/utils/yaml_no_alias_safe_dump.py
-tests/test_asr_inference_pipeline.py
-tests/test_asr_vad_punc_inference_pipeline.py
-tests/test_inference_pipeline.py
-tests/test_lm_pipeline.py
-tests/test_punctuation_pipeline.py
-tests/test_sv_inference_pipeline.py
-tests/test_vad_inference_pipeline.py
+funasr/utils/yaml_no_alias_safe_dump.py
```

### Comparing `funasr-0.4.3/funasr.egg-info/requires.txt` & `funasr-0.4.4/funasr.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 pypinyin<=0.44.0
 espnet_tts_frontend
 pytorch_wpe
 editdistance==0.5.2
 tensorboard==1.15
 g2p
 oss2
-kaldi-native-fbank
 edit-distance
 
 [all]
 torch_optimizer
 fairscale
 transformers
 editdistance==0.5.2
```

### Comparing `funasr-0.4.3/setup.py` & `funasr-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         # "ci_sdr",
         "pytorch_wpe",
         "editdistance==0.5.2",
         "tensorboard==1.15",
         "g2p",
         # PAI
         "oss2",
-        "kaldi-native-fbank",
+        # "kaldi-native-fbank",
         # timestamp
         "edit-distance"
     ],
     # train: The modules invoked when training only.
     "train": [
         # "pillow>=6.1.0",
         "editdistance==0.5.2",
```

