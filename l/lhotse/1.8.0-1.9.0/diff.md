# Comparing `tmp/lhotse-1.8.0.tar.gz` & `tmp/lhotse-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lhotse-1.8.0.tar", last modified: Fri Sep 30 13:10:52 2022, max compression
+gzip compressed data, was "lhotse-1.9.0.tar", last modified: Thu Oct 20 18:24:59 2022, max compression
```

## Comparing `lhotse-1.8.0.tar` & `lhotse-1.9.0.tar`

### file list

```diff
@@ -1,246 +1,250 @@
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.964168 lhotse-1.8.0/
--rw-r--r--   0 pzelasko   (501) staff       (20)    11357 2022-02-08 02:21:04.000000 lhotse-1.8.0/LICENSE
--rw-r--r--   0 pzelasko   (501) staff       (20)      179 2022-02-08 02:21:04.000000 lhotse-1.8.0/MANIFEST.in
--rw-r--r--   0 pzelasko   (501) staff       (20)    10554 2022-09-30 13:10:52.963979 lhotse-1.8.0/PKG-INFO
--rw-r--r--   0 pzelasko   (501) staff       (20)     9304 2022-09-12 21:16:34.000000 lhotse-1.8.0/README.md
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.918366 lhotse-1.8.0/docs/
--rw-r--r--   0 pzelasko   (501) staff       (20)       98 2022-09-12 21:16:34.000000 lhotse-1.8.0/docs/requirements.txt
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.922120 lhotse-1.8.0/lhotse/
--rw-r--r--   0 pzelasko   (501) staff       (20)     1473 2022-09-30 13:10:14.000000 lhotse-1.8.0/lhotse/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    14043 2022-03-23 16:15:21.000000 lhotse-1.8.0/lhotse/array.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    87180 2022-09-28 01:01:50.000000 lhotse-1.8.0/lhotse/audio.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.924095 lhotse-1.8.0/lhotse/augmentation/
--rw-r--r--   0 pzelasko   (501) staff       (20)      199 2022-09-12 20:03:21.000000 lhotse-1.8.0/lhotse/augmentation/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      171 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/augmentation/common.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    16632 2022-09-12 20:03:21.000000 lhotse-1.8.0/lhotse/augmentation/torchaudio.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2865 2022-04-12 12:35:14.000000 lhotse-1.8.0/lhotse/augmentation/transform.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     8071 2022-09-12 20:03:21.000000 lhotse-1.8.0/lhotse/augmentation/utils.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2096 2022-04-12 12:35:14.000000 lhotse-1.8.0/lhotse/augmentation/wpe.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.924444 lhotse-1.8.0/lhotse/bin/
--rw-r--r--   0 pzelasko   (501) staff       (20)       31 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/__init__.py
--rwxr-xr-x   0 pzelasko   (501) staff       (20)     1033 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/lhotse.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.926436 lhotse-1.8.0/lhotse/bin/modes/
--rw-r--r--   0 pzelasko   (501) staff       (20)      217 2022-09-28 01:01:50.000000 lhotse-1.8.0/lhotse/bin/modes/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      678 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/cli_base.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    13855 2022-07-06 22:39:25.000000 lhotse-1.8.0/lhotse/bin/modes/cut.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     9443 2022-06-11 03:29:54.000000 lhotse-1.8.0/lhotse/bin/modes/features.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      848 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/install_tools.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     3825 2022-06-11 03:29:54.000000 lhotse-1.8.0/lhotse/bin/modes/kaldi.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    11387 2022-06-11 03:29:54.000000 lhotse-1.8.0/lhotse/bin/modes/manipulation.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.935672 lhotse-1.8.0/lhotse/bin/modes/recipes/
--rw-r--r--   0 pzelasko   (501) staff       (20)     1426 2022-07-06 22:39:25.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      768 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/adept.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1115 2022-02-22 14:07:11.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/aidatatang_200zh.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      731 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/aishell.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      689 2022-06-23 03:07:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/aishell2.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      739 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/aishell4.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      974 2022-03-12 20:34:34.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/ali_meeting.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2529 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/ami.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      586 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/aspire.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1002 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/babel.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      997 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/broadcast_news.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1420 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/bvcc.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1771 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/callhome_egyptian.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2616 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/callhome_english.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      677 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/cmu_arctic.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      642 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/cmu_indic.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      777 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/cmu_kids.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1445 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/commonvoice.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1012 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/cslu_kids.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      933 2022-07-06 22:39:25.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/daily_talk.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1003 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/dihard3.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      895 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/earnings21.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      820 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/earnings22.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1013 2022-05-16 17:50:29.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/eval2000.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1897 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/fisher_english.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1206 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/fisher_spanish.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1277 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/gale_arabic.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1487 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/gale_mandarin.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1954 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/gigaspeech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      849 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/heroico.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      892 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/hifitts.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2086 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/icsi.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      464 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/l2_arctic.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      967 2022-07-06 22:39:25.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/libricss.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1542 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/librimix.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1646 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/librispeech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1476 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/libritts.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      761 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/ljspeech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      751 2022-06-23 03:07:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/magicdata.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1207 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/mgb2.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1165 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/mls.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1536 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/mtedx.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      795 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/musan.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      752 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/nsc.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      551 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/peoples_speech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      761 2022-06-23 03:07:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/primewords.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      951 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/rir_noise.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1150 2022-03-12 20:34:34.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/spgispeech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      721 2022-06-23 03:07:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/stcmds.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1879 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/switchboard.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      496 2022-06-23 03:07:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/tal_asr.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      695 2022-06-23 03:07:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/tal_csasr.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      726 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/tedlium.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      741 2022-06-23 03:07:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/thchs_30.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1328 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/timit.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      760 2022-08-08 19:33:14.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/vctk.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1992 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/voxceleb.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1073 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/wenet_speech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      696 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/bin/modes/recipes/yesno.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2658 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/bin/modes/validate.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4742 2022-09-30 13:09:33.000000 lhotse-1.8.0/lhotse/bin/modes/workflows.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2648 2022-03-21 20:49:37.000000 lhotse-1.8.0/lhotse/caching.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.937029 lhotse-1.8.0/lhotse/cut/
--rw-r--r--   0 pzelasko   (501) staff       (20)     3213 2022-09-26 19:49:40.000000 lhotse-1.8.0/lhotse/cut/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    33030 2022-09-30 13:09:33.000000 lhotse-1.8.0/lhotse/cut/base.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    49432 2022-09-26 19:49:40.000000 lhotse-1.8.0/lhotse/cut/mixed.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    46676 2022-09-26 19:49:40.000000 lhotse-1.8.0/lhotse/cut/mono.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    16185 2022-09-26 19:49:40.000000 lhotse-1.8.0/lhotse/cut/padding.py
--rw-r--r--   0 pzelasko   (501) staff       (20)   118486 2022-09-26 19:49:40.000000 lhotse-1.8.0/lhotse/cut/set.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.940269 lhotse-1.8.0/lhotse/dataset/
--rw-r--r--   0 pzelasko   (501) staff       (20)      950 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/dataset/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    20786 2022-05-16 17:50:29.000000 lhotse-1.8.0/lhotse/dataset/collation.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.942019 lhotse-1.8.0/lhotse/dataset/cut_transforms/
--rw-r--r--   0 pzelasko   (501) staff       (20)      455 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/dataset/cut_transforms/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2947 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/dataset/cut_transforms/concatenate.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4687 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/dataset/cut_transforms/extra_padding.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2690 2022-03-14 20:27:31.000000 lhotse-1.8.0/lhotse/dataset/cut_transforms/mix.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1139 2022-03-23 16:15:21.000000 lhotse-1.8.0/lhotse/dataset/cut_transforms/perturb_speed.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1139 2022-03-23 16:15:21.000000 lhotse-1.8.0/lhotse/dataset/cut_transforms/perturb_tempo.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1191 2022-03-23 16:15:21.000000 lhotse-1.8.0/lhotse/dataset/cut_transforms/perturb_volume.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1861 2022-09-12 20:03:21.000000 lhotse-1.8.0/lhotse/dataset/cut_transforms/reverberate.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1936 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/dataset/dataloading.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4649 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/dataset/diarization.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    19260 2022-08-26 19:42:48.000000 lhotse-1.8.0/lhotse/dataset/input_strategies.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4169 2022-05-13 16:34:54.000000 lhotse-1.8.0/lhotse/dataset/iterable_dataset.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.944867 lhotse-1.8.0/lhotse/dataset/sampling/
--rw-r--r--   0 pzelasko   (501) staff       (20)      374 2022-03-30 16:14:53.000000 lhotse-1.8.0/lhotse/dataset/sampling/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    25443 2022-08-08 19:33:14.000000 lhotse-1.8.0/lhotse/dataset/sampling/base.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    18920 2022-09-13 19:11:49.000000 lhotse-1.8.0/lhotse/dataset/sampling/bucketing.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    12570 2022-08-08 19:33:14.000000 lhotse-1.8.0/lhotse/dataset/sampling/cut_pairs.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     3289 2022-03-18 15:11:44.000000 lhotse-1.8.0/lhotse/dataset/sampling/data_source.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    14861 2022-08-08 19:33:14.000000 lhotse-1.8.0/lhotse/dataset/sampling/dynamic.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    17132 2022-06-23 13:24:05.000000 lhotse-1.8.0/lhotse/dataset/sampling/dynamic_bucketing.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     8600 2022-08-08 19:33:14.000000 lhotse-1.8.0/lhotse/dataset/sampling/round_robin.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    10232 2022-08-08 19:33:14.000000 lhotse-1.8.0/lhotse/dataset/sampling/simple.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6405 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/dataset/sampling/utils.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     8758 2022-08-08 19:33:14.000000 lhotse-1.8.0/lhotse/dataset/sampling/zip.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    17421 2022-07-06 22:39:25.000000 lhotse-1.8.0/lhotse/dataset/signal_transforms.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6643 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/dataset/source_separation.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     8974 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/dataset/speech_recognition.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2696 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/dataset/speech_synthesis.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     3927 2022-05-16 17:50:29.000000 lhotse-1.8.0/lhotse/dataset/unsupervised.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1550 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/dataset/vad.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2315 2022-03-14 20:27:31.000000 lhotse-1.8.0/lhotse/dataset/vis.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    23174 2022-06-11 03:29:54.000000 lhotse-1.8.0/lhotse/dataset/webdataset.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.947560 lhotse-1.8.0/lhotse/features/
--rw-r--r--   0 pzelasko   (501) staff       (20)     1103 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/features/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    38822 2022-09-26 19:49:40.000000 lhotse-1.8.0/lhotse/features/base.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      618 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/features/compression.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2184 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/features/fbank.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    38623 2022-06-11 03:29:54.000000 lhotse-1.8.0/lhotse/features/io.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.947936 lhotse-1.8.0/lhotse/features/kaldi/
--rw-r--r--   0 pzelasko   (501) staff       (20)      150 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/features/kaldi/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5779 2022-09-26 19:49:40.000000 lhotse-1.8.0/lhotse/features/kaldi/extractors.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    33637 2022-09-12 20:03:21.000000 lhotse-1.8.0/lhotse/features/kaldi/layers.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     8905 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/features/kaldifeat.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5260 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/features/librosa_fbank.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1632 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/features/mfcc.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     7603 2022-02-09 19:10:13.000000 lhotse-1.8.0/lhotse/features/mixer.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6307 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/features/opensmile.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2538 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/features/spectrogram.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    14423 2022-08-25 18:33:43.000000 lhotse-1.8.0/lhotse/kaldi.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    16764 2022-09-26 19:49:40.000000 lhotse-1.8.0/lhotse/lazy.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5316 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/manifest.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     3865 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/manipulation.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     2663 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/parallel.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    20353 2022-09-28 01:01:50.000000 lhotse-1.8.0/lhotse/qa.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.962225 lhotse-1.8.0/lhotse/recipes/
--rw-r--r--   0 pzelasko   (501) staff       (20)     2670 2022-07-06 22:39:25.000000 lhotse-1.8.0/lhotse/recipes/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6210 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/adept.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5636 2022-08-25 18:33:43.000000 lhotse-1.8.0/lhotse/recipes/aidatatang_200zh.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5954 2022-08-25 18:33:43.000000 lhotse-1.8.0/lhotse/recipes/aishell.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6011 2022-08-27 21:07:52.000000 lhotse-1.8.0/lhotse/recipes/aishell2.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6574 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/aishell4.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     7628 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/ali_meeting.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    27027 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/ami.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     7096 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/aspire.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     8976 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/babel.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     9237 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/broadcast_news.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     9185 2022-09-12 20:03:21.000000 lhotse-1.8.0/lhotse/recipes/bvcc.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4352 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/callhome_egyptian.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    10235 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/callhome_english.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6443 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/cmu_arctic.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     7492 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/cmu_indic.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6228 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/cmu_kids.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    12796 2022-06-11 03:29:54.000000 lhotse-1.8.0/lhotse/recipes/commonvoice.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5834 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/cslu_kids.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5421 2022-07-06 22:39:25.000000 lhotse-1.8.0/lhotse/recipes/daily_talk.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5995 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/dihard3.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6394 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/earnings21.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5936 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/earnings22.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5551 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/eval2000.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     9831 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/fisher_english.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5212 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/fisher_spanish.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     9077 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/gale_arabic.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     8698 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/gale_mandarin.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     7431 2022-03-14 20:27:31.000000 lhotse-1.8.0/lhotse/recipes/gigaspeech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    11008 2022-06-05 13:17:46.000000 lhotse-1.8.0/lhotse/recipes/heroico.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     7156 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/hifitts.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    23438 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/icsi.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     8641 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/l2_arctic.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    15121 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/libricss.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6162 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/librimix.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    10370 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/librispeech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     9609 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/libritts.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4680 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/ljspeech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     7553 2022-08-25 18:33:43.000000 lhotse-1.8.0/lhotse/recipes/magicdata.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    11196 2022-06-05 13:17:46.000000 lhotse-1.8.0/lhotse/recipes/mgb2.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5297 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/mls.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6227 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/mobvoihotwords.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    12798 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/mtedx.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4548 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/musan.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     7910 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/nsc.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5629 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/peoples_speech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5201 2022-06-23 03:07:04.000000 lhotse-1.8.0/lhotse/recipes/primewords.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6910 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/rir_noise.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     6904 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/spgispeech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5352 2022-08-25 18:33:43.000000 lhotse-1.8.0/lhotse/recipes/stcmds.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     7084 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/switchboard.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     3977 2022-08-25 18:33:43.000000 lhotse-1.8.0/lhotse/recipes/tal_asr.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5047 2022-08-25 18:33:43.000000 lhotse-1.8.0/lhotse/recipes/tal_csasr.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5676 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/tedlium.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5909 2022-08-25 18:33:43.000000 lhotse-1.8.0/lhotse/recipes/thchs_30.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    12425 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/timit.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     3217 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/utils.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    11295 2022-08-08 19:33:14.000000 lhotse-1.8.0/lhotse/recipes/vctk.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    19399 2022-08-25 18:33:43.000000 lhotse-1.8.0/lhotse/recipes/voxceleb.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5278 2022-06-02 21:58:11.000000 lhotse-1.8.0/lhotse/recipes/wenet_speech.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     5706 2022-05-27 00:31:12.000000 lhotse-1.8.0/lhotse/recipes/yesno.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    20785 2022-09-16 23:47:21.000000 lhotse-1.8.0/lhotse/serialization.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    35245 2022-09-30 13:09:33.000000 lhotse-1.8.0/lhotse/supervision.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.962560 lhotse-1.8.0/lhotse/testing/
--rw-r--r--   0 pzelasko   (501) staff       (20)        0 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/testing/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4642 2022-09-30 13:09:33.000000 lhotse-1.8.0/lhotse/testing/dummies.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4931 2022-06-09 17:23:44.000000 lhotse-1.8.0/lhotse/testing/fixtures.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.963385 lhotse-1.8.0/lhotse/tools/
--rw-r--r--   0 pzelasko   (501) staff       (20)       39 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/tools/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)      381 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/tools/env.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     1557 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/tools/sph2pipe.py
--rw-r--r--   0 pzelasko   (501) staff       (20)    25841 2022-09-29 15:37:03.000000 lhotse-1.8.0/lhotse/utils.py
--rw-r--r--   0 pzelasko   (501) staff       (20)       21 2022-09-30 13:10:52.000000 lhotse-1.8.0/lhotse/version.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     4127 2022-02-08 02:21:04.000000 lhotse-1.8.0/lhotse/workarounds.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.963771 lhotse-1.8.0/lhotse/workflows/
--rw-r--r--   0 pzelasko   (501) staff       (20)       95 2022-09-30 13:09:33.000000 lhotse-1.8.0/lhotse/workflows/__init__.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     8932 2022-09-30 13:09:33.000000 lhotse-1.8.0/lhotse/workflows/forced_alignment.py
--rw-r--r--   0 pzelasko   (501) staff       (20)     3400 2022-09-28 01:38:51.000000 lhotse-1.8.0/lhotse/workflows/whisper.py
-drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-09-30 13:10:52.922880 lhotse-1.8.0/lhotse.egg-info/
--rw-r--r--   0 pzelasko   (501) staff       (20)    10554 2022-09-30 13:10:52.000000 lhotse-1.8.0/lhotse.egg-info/PKG-INFO
--rw-r--r--   0 pzelasko   (501) staff       (20)     6883 2022-09-30 13:10:52.000000 lhotse-1.8.0/lhotse.egg-info/SOURCES.txt
--rw-r--r--   0 pzelasko   (501) staff       (20)        1 2022-09-30 13:10:52.000000 lhotse-1.8.0/lhotse.egg-info/dependency_links.txt
--rw-r--r--   0 pzelasko   (501) staff       (20)       49 2022-09-30 13:10:52.000000 lhotse-1.8.0/lhotse.egg-info/entry_points.txt
--rw-r--r--   0 pzelasko   (501) staff       (20)     1245 2022-09-30 13:10:52.000000 lhotse-1.8.0/lhotse.egg-info/requires.txt
--rw-r--r--   0 pzelasko   (501) staff       (20)        7 2022-09-30 13:10:52.000000 lhotse-1.8.0/lhotse.egg-info/top_level.txt
--rw-r--r--   0 pzelasko   (501) staff       (20)      128 2022-05-27 00:31:12.000000 lhotse-1.8.0/pyproject.toml
--rw-r--r--   0 pzelasko   (501) staff       (20)       38 2022-09-30 13:10:52.964208 lhotse-1.8.0/setup.cfg
--rw-r--r--   0 pzelasko   (501) staff       (20)    10719 2022-09-30 13:10:01.000000 lhotse-1.8.0/setup.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.087600 lhotse-1.9.0/
+-rw-r--r--   0 pzelasko   (501) staff       (20)    11357 2022-02-08 02:21:04.000000 lhotse-1.9.0/LICENSE
+-rw-r--r--   0 pzelasko   (501) staff       (20)      179 2022-02-08 02:21:04.000000 lhotse-1.9.0/MANIFEST.in
+-rw-r--r--   0 pzelasko   (501) staff       (20)    10554 2022-10-20 18:24:59.087433 lhotse-1.9.0/PKG-INFO
+-rw-r--r--   0 pzelasko   (501) staff       (20)     9304 2022-09-12 21:16:34.000000 lhotse-1.9.0/README.md
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.039813 lhotse-1.9.0/docs/
+-rw-r--r--   0 pzelasko   (501) staff       (20)       98 2022-09-12 21:16:34.000000 lhotse-1.9.0/docs/requirements.txt
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.043327 lhotse-1.9.0/lhotse/
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1483 2022-10-20 18:24:22.000000 lhotse-1.9.0/lhotse/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    14043 2022-03-23 16:15:21.000000 lhotse-1.9.0/lhotse/array.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    89531 2022-10-20 18:23:41.000000 lhotse-1.9.0/lhotse/audio.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.045417 lhotse-1.9.0/lhotse/augmentation/
+-rw-r--r--   0 pzelasko   (501) staff       (20)      199 2022-09-12 20:03:21.000000 lhotse-1.9.0/lhotse/augmentation/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      171 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/augmentation/common.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    18110 2022-10-07 18:43:43.000000 lhotse-1.9.0/lhotse/augmentation/torchaudio.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2865 2022-04-12 12:35:14.000000 lhotse-1.9.0/lhotse/augmentation/transform.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     8071 2022-09-12 20:03:21.000000 lhotse-1.9.0/lhotse/augmentation/utils.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2096 2022-04-12 12:35:14.000000 lhotse-1.9.0/lhotse/augmentation/wpe.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.045889 lhotse-1.9.0/lhotse/bin/
+-rw-r--r--   0 pzelasko   (501) staff       (20)       31 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/__init__.py
+-rwxr-xr-x   0 pzelasko   (501) staff       (20)     1033 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/lhotse.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.047822 lhotse-1.9.0/lhotse/bin/modes/
+-rw-r--r--   0 pzelasko   (501) staff       (20)      217 2022-09-28 01:01:50.000000 lhotse-1.9.0/lhotse/bin/modes/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      678 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/cli_base.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    13855 2022-07-06 22:39:25.000000 lhotse-1.9.0/lhotse/bin/modes/cut.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     9443 2022-06-11 03:29:54.000000 lhotse-1.9.0/lhotse/bin/modes/features.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      848 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/install_tools.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     4114 2022-10-05 00:26:07.000000 lhotse-1.9.0/lhotse/bin/modes/kaldi.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    11387 2022-06-11 03:29:54.000000 lhotse-1.9.0/lhotse/bin/modes/manipulation.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.057629 lhotse-1.9.0/lhotse/bin/modes/recipes/
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1445 2022-10-17 20:53:51.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      768 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/adept.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1115 2022-02-22 14:07:11.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/aidatatang_200zh.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      731 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/aishell.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      689 2022-06-23 03:07:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/aishell2.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      739 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/aishell4.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      974 2022-03-12 20:34:34.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/ali_meeting.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2529 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/ami.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      586 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/aspire.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1002 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/babel.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      997 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/broadcast_news.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1420 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/bvcc.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1771 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/callhome_egyptian.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2616 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/callhome_english.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      677 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/cmu_arctic.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      642 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/cmu_indic.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      777 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/cmu_kids.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1445 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/commonvoice.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1846 2022-10-17 20:53:51.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/csj.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1012 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/cslu_kids.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      933 2022-07-06 22:39:25.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/daily_talk.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1003 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/dihard3.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      895 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/earnings21.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      820 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/earnings22.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1013 2022-05-16 17:50:29.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/eval2000.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1897 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/fisher_english.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1206 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/fisher_spanish.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1277 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/gale_arabic.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1487 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/gale_mandarin.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1954 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/gigaspeech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      849 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/heroico.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      892 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/hifitts.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2086 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/icsi.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      464 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/l2_arctic.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      967 2022-07-06 22:39:25.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/libricss.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1542 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/librimix.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1646 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/librispeech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1476 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/libritts.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      761 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/ljspeech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      751 2022-06-23 03:07:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/magicdata.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1207 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/mgb2.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1165 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/mls.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1536 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/mtedx.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      795 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/musan.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      752 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/nsc.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      551 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/peoples_speech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      761 2022-06-23 03:07:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/primewords.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      951 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/rir_noise.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1150 2022-03-12 20:34:34.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/spgispeech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      721 2022-06-23 03:07:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/stcmds.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1879 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/switchboard.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      496 2022-06-23 03:07:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/tal_asr.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      695 2022-06-23 03:07:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/tal_csasr.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      726 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/tedlium.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      741 2022-06-23 03:07:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/thchs_30.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1328 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/timit.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      760 2022-08-08 19:33:14.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/vctk.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1992 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/voxceleb.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1073 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/wenet_speech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      696 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/bin/modes/recipes/yesno.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2658 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/bin/modes/validate.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5262 2022-10-07 18:43:43.000000 lhotse-1.9.0/lhotse/bin/modes/workflows.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2648 2022-03-21 20:49:37.000000 lhotse-1.9.0/lhotse/caching.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.059201 lhotse-1.9.0/lhotse/cut/
+-rw-r--r--   0 pzelasko   (501) staff       (20)     3711 2022-10-20 18:23:41.000000 lhotse-1.9.0/lhotse/cut/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    35109 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/cut/base.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    39866 2022-10-07 18:43:43.000000 lhotse-1.9.0/lhotse/cut/data.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    55091 2022-10-17 20:53:51.000000 lhotse-1.9.0/lhotse/cut/mixed.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    11536 2022-10-07 18:43:43.000000 lhotse-1.9.0/lhotse/cut/mono.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    18957 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/cut/multi.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    16314 2022-10-17 20:53:51.000000 lhotse-1.9.0/lhotse/cut/padding.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)   118672 2022-10-17 20:53:51.000000 lhotse-1.9.0/lhotse/cut/set.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.063654 lhotse-1.9.0/lhotse/dataset/
+-rw-r--r--   0 pzelasko   (501) staff       (20)      950 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/dataset/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    20786 2022-05-16 17:50:29.000000 lhotse-1.9.0/lhotse/dataset/collation.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.065647 lhotse-1.9.0/lhotse/dataset/cut_transforms/
+-rw-r--r--   0 pzelasko   (501) staff       (20)      455 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/dataset/cut_transforms/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2947 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/dataset/cut_transforms/concatenate.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     4687 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/dataset/cut_transforms/extra_padding.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2690 2022-03-14 20:27:31.000000 lhotse-1.9.0/lhotse/dataset/cut_transforms/mix.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1139 2022-03-23 16:15:21.000000 lhotse-1.9.0/lhotse/dataset/cut_transforms/perturb_speed.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1139 2022-03-23 16:15:21.000000 lhotse-1.9.0/lhotse/dataset/cut_transforms/perturb_tempo.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1191 2022-03-23 16:15:21.000000 lhotse-1.9.0/lhotse/dataset/cut_transforms/perturb_volume.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1861 2022-09-12 20:03:21.000000 lhotse-1.9.0/lhotse/dataset/cut_transforms/reverberate.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1936 2022-10-10 20:12:48.000000 lhotse-1.9.0/lhotse/dataset/dataloading.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     4649 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/dataset/diarization.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    19260 2022-08-26 19:42:48.000000 lhotse-1.9.0/lhotse/dataset/input_strategies.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     4169 2022-05-13 16:34:54.000000 lhotse-1.9.0/lhotse/dataset/iterable_dataset.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.067398 lhotse-1.9.0/lhotse/dataset/sampling/
+-rw-r--r--   0 pzelasko   (501) staff       (20)      374 2022-03-30 16:14:53.000000 lhotse-1.9.0/lhotse/dataset/sampling/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    25575 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/dataset/sampling/base.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    19266 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/dataset/sampling/bucketing.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    12916 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/dataset/sampling/cut_pairs.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     3289 2022-03-18 15:11:44.000000 lhotse-1.9.0/lhotse/dataset/sampling/data_source.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    15207 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/dataset/sampling/dynamic.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    17478 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/dataset/sampling/dynamic_bucketing.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     8600 2022-08-08 19:33:14.000000 lhotse-1.9.0/lhotse/dataset/sampling/round_robin.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    10578 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/dataset/sampling/simple.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6405 2022-10-17 19:25:56.000000 lhotse-1.9.0/lhotse/dataset/sampling/utils.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     8758 2022-08-08 19:33:14.000000 lhotse-1.9.0/lhotse/dataset/sampling/zip.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    17421 2022-07-06 22:39:25.000000 lhotse-1.9.0/lhotse/dataset/signal_transforms.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6643 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/dataset/source_separation.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     8974 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/dataset/speech_recognition.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2696 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/dataset/speech_synthesis.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     3927 2022-05-16 17:50:29.000000 lhotse-1.9.0/lhotse/dataset/unsupervised.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1550 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/dataset/vad.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2315 2022-03-14 20:27:31.000000 lhotse-1.9.0/lhotse/dataset/vis.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    23174 2022-06-11 03:29:54.000000 lhotse-1.9.0/lhotse/dataset/webdataset.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.069489 lhotse-1.9.0/lhotse/features/
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1103 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/features/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    38879 2022-10-07 18:43:43.000000 lhotse-1.9.0/lhotse/features/base.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      618 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/features/compression.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2184 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/features/fbank.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    38623 2022-10-20 18:23:41.000000 lhotse-1.9.0/lhotse/features/io.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.069959 lhotse-1.9.0/lhotse/features/kaldi/
+-rw-r--r--   0 pzelasko   (501) staff       (20)      150 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/features/kaldi/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5779 2022-09-26 19:49:40.000000 lhotse-1.9.0/lhotse/features/kaldi/extractors.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    33637 2022-09-12 20:03:21.000000 lhotse-1.9.0/lhotse/features/kaldi/layers.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     8905 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/features/kaldifeat.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5260 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/features/librosa_fbank.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1632 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/features/mfcc.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     7834 2022-10-07 18:43:43.000000 lhotse-1.9.0/lhotse/features/mixer.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6307 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/features/opensmile.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2538 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/features/spectrogram.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    15149 2022-10-05 00:26:07.000000 lhotse-1.9.0/lhotse/kaldi.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    17845 2022-10-20 18:23:41.000000 lhotse-1.9.0/lhotse/lazy.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5316 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/manifest.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     3865 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/manipulation.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2663 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/parallel.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    20737 2022-10-12 19:17:30.000000 lhotse-1.9.0/lhotse/qa.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.085233 lhotse-1.9.0/lhotse/recipes/
+-rw-r--r--   0 pzelasko   (501) staff       (20)     2699 2022-10-17 20:53:51.000000 lhotse-1.9.0/lhotse/recipes/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6210 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/adept.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5636 2022-08-25 18:33:43.000000 lhotse-1.9.0/lhotse/recipes/aidatatang_200zh.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5954 2022-08-25 18:33:43.000000 lhotse-1.9.0/lhotse/recipes/aishell.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6011 2022-08-27 21:07:52.000000 lhotse-1.9.0/lhotse/recipes/aishell2.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6594 2022-10-12 19:17:30.000000 lhotse-1.9.0/lhotse/recipes/aishell4.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     7665 2022-10-12 19:17:30.000000 lhotse-1.9.0/lhotse/recipes/ali_meeting.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    27048 2022-10-12 19:17:30.000000 lhotse-1.9.0/lhotse/recipes/ami.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     7226 2022-10-12 19:17:30.000000 lhotse-1.9.0/lhotse/recipes/aspire.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     8976 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/babel.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     9237 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/broadcast_news.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     9185 2022-09-12 20:03:21.000000 lhotse-1.9.0/lhotse/recipes/bvcc.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     4352 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/callhome_egyptian.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    10235 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/callhome_english.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6443 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/cmu_arctic.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     7492 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/cmu_indic.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6228 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/cmu_kids.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    12796 2022-06-11 03:29:54.000000 lhotse-1.9.0/lhotse/recipes/commonvoice.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    43512 2022-10-17 20:53:51.000000 lhotse-1.9.0/lhotse/recipes/csj.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5834 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/cslu_kids.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5421 2022-07-06 22:39:25.000000 lhotse-1.9.0/lhotse/recipes/daily_talk.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5995 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/dihard3.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6394 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/earnings21.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5936 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/earnings22.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5551 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/eval2000.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     9830 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/recipes/fisher_english.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5212 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/fisher_spanish.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     9077 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/gale_arabic.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     8698 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/gale_mandarin.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     7431 2022-03-14 20:27:31.000000 lhotse-1.9.0/lhotse/recipes/gigaspeech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    11008 2022-06-05 13:17:46.000000 lhotse-1.9.0/lhotse/recipes/heroico.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     7156 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/hifitts.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    23441 2022-10-12 19:17:30.000000 lhotse-1.9.0/lhotse/recipes/icsi.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     8641 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/l2_arctic.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    15404 2022-10-12 19:17:30.000000 lhotse-1.9.0/lhotse/recipes/libricss.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6162 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/librimix.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    10370 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/librispeech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     9609 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/libritts.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     4680 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/ljspeech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     7553 2022-10-10 01:55:27.000000 lhotse-1.9.0/lhotse/recipes/magicdata.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    11198 2022-10-10 01:55:27.000000 lhotse-1.9.0/lhotse/recipes/mgb2.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5297 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/mls.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6227 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/mobvoihotwords.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    12798 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/mtedx.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     4548 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/musan.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     7910 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/nsc.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5629 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/peoples_speech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5201 2022-06-23 03:07:04.000000 lhotse-1.9.0/lhotse/recipes/primewords.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6910 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/rir_noise.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6904 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/spgispeech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5352 2022-08-25 18:33:43.000000 lhotse-1.9.0/lhotse/recipes/stcmds.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     7084 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/switchboard.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     3977 2022-08-25 18:33:43.000000 lhotse-1.9.0/lhotse/recipes/tal_asr.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5047 2022-08-25 18:33:43.000000 lhotse-1.9.0/lhotse/recipes/tal_csasr.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5676 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/tedlium.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5909 2022-08-25 18:33:43.000000 lhotse-1.9.0/lhotse/recipes/thchs_30.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    12425 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/timit.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     3217 2022-05-27 00:31:12.000000 lhotse-1.9.0/lhotse/recipes/utils.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    11295 2022-08-08 19:33:14.000000 lhotse-1.9.0/lhotse/recipes/vctk.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    19399 2022-08-25 18:33:43.000000 lhotse-1.9.0/lhotse/recipes/voxceleb.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5278 2022-06-02 21:58:11.000000 lhotse-1.9.0/lhotse/recipes/wenet_speech.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5717 2022-10-10 17:49:23.000000 lhotse-1.9.0/lhotse/recipes/yesno.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    20866 2022-10-20 18:23:41.000000 lhotse-1.9.0/lhotse/serialization.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    36230 2022-10-10 01:54:11.000000 lhotse-1.9.0/lhotse/supervision.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.085627 lhotse-1.9.0/lhotse/testing/
+-rw-r--r--   0 pzelasko   (501) staff       (20)        0 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/testing/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6595 2022-10-20 18:23:41.000000 lhotse-1.9.0/lhotse/testing/dummies.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     4931 2022-06-09 17:23:44.000000 lhotse-1.9.0/lhotse/testing/fixtures.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.086591 lhotse-1.9.0/lhotse/tools/
+-rw-r--r--   0 pzelasko   (501) staff       (20)       39 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/tools/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)      381 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/tools/env.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1557 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/tools/sph2pipe.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)    26615 2022-10-20 18:23:43.000000 lhotse-1.9.0/lhotse/utils.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)       21 2022-10-20 18:24:57.000000 lhotse-1.9.0/lhotse/version.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     4127 2022-02-08 02:21:04.000000 lhotse-1.9.0/lhotse/workarounds.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.087195 lhotse-1.9.0/lhotse/workflows/
+-rw-r--r--   0 pzelasko   (501) staff       (20)       95 2022-09-30 13:09:33.000000 lhotse-1.9.0/lhotse/workflows/__init__.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     9247 2022-10-17 20:53:51.000000 lhotse-1.9.0/lhotse/workflows/forced_alignment.py
+-rw-r--r--   0 pzelasko   (501) staff       (20)     5582 2022-10-12 19:17:30.000000 lhotse-1.9.0/lhotse/workflows/whisper.py
+drwxr-xr-x   0 pzelasko   (501) staff       (20)        0 2022-10-20 18:24:59.044041 lhotse-1.9.0/lhotse.egg-info/
+-rw-r--r--   0 pzelasko   (501) staff       (20)    10554 2022-10-20 18:24:58.000000 lhotse-1.9.0/lhotse.egg-info/PKG-INFO
+-rw-r--r--   0 pzelasko   (501) staff       (20)     6976 2022-10-20 18:24:59.000000 lhotse-1.9.0/lhotse.egg-info/SOURCES.txt
+-rw-r--r--   0 pzelasko   (501) staff       (20)        1 2022-10-20 18:24:58.000000 lhotse-1.9.0/lhotse.egg-info/dependency_links.txt
+-rw-r--r--   0 pzelasko   (501) staff       (20)       49 2022-10-20 18:24:58.000000 lhotse-1.9.0/lhotse.egg-info/entry_points.txt
+-rw-r--r--   0 pzelasko   (501) staff       (20)     1245 2022-10-20 18:24:58.000000 lhotse-1.9.0/lhotse.egg-info/requires.txt
+-rw-r--r--   0 pzelasko   (501) staff       (20)        7 2022-10-20 18:24:58.000000 lhotse-1.9.0/lhotse.egg-info/top_level.txt
+-rw-r--r--   0 pzelasko   (501) staff       (20)      128 2022-05-27 00:31:12.000000 lhotse-1.9.0/pyproject.toml
+-rw-r--r--   0 pzelasko   (501) staff       (20)       38 2022-10-20 18:24:59.087634 lhotse-1.9.0/setup.cfg
+-rw-r--r--   0 pzelasko   (501) staff       (20)    10719 2022-10-20 18:24:11.000000 lhotse-1.9.0/setup.py
```

### Comparing `lhotse-1.8.0/LICENSE` & `lhotse-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/PKG-INFO` & `lhotse-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lhotse
-Version: 1.8.0
+Version: 1.9.0
 Summary: Data preparation for speech processing models training.
 Author: The Lhotse Development Team
 Author-email: pzelasko@jhu.edu
 License: Apache-2.0 License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lhotse-1.8.0/README.md` & `lhotse-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/__init__.py` & `lhotse-1.9.0/lhotse/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .audio import (
     AudioSource,
     Recording,
     RecordingSet,
     set_audio_duration_mismatch_tolerance,
 )
 from .caching import is_caching_enabled, set_caching_enabled
-from .cut import CutSet, MonoCut, create_cut_set_eager, create_cut_set_lazy
+from .cut import CutSet, MonoCut, MultiCut, create_cut_set_eager, create_cut_set_lazy
 from .features import *
 from .kaldi import load_kaldi_data_dir
 from .manipulation import combine, split_parallelize_combine, to_manifest
 from .qa import fix_manifests, validate, validate_recordings_and_supervisions
 from .serialization import load_manifest, load_manifest_lazy, store_manifest
 from .supervision import SupervisionSegment, SupervisionSet
 from .tools.env import add_tools_to_path as _add_tools_to_path
@@ -30,12 +30,12 @@
     # Try to get Lhotse's version (should be created during running pip install / python setup.py ...)
     from .version import __version__
 except:
     # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! #
     # NOTE: REMEMBER TO UPDATE THE ACTUAL VERSION IN setup.py WHEN RELEASING #
     # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! #
     # Use a default placeholder when the version is unavailable...
-    __version__ = "1.8.0+missing.version.file"
+    __version__ = "1.9.0+missing.version.file"
 
 from . import augmentation, dataset, features, recipes
 
 _add_tools_to_path()
```

### Comparing `lhotse-1.8.0/lhotse/array.py` & `lhotse-1.9.0/lhotse/array.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/audio.py` & `lhotse-1.9.0/lhotse/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,16 +311,27 @@
     """
 
     id: str
     sources: List[AudioSource]
     sampling_rate: int
     num_samples: int
     duration: Seconds
+    channel_ids: Optional[List[int]] = None
     transforms: Optional[List[Dict]] = None
 
+    def __post_init__(self):
+        if self.channel_ids is None:
+            self.channel_ids = sorted(
+                cid for source in self.sources for cid in source.channels
+            )
+
+    @property
+    def num_channels(self):
+        return len(self.channel_ids)
+
     @staticmethod
     def from_file(
         path: Pathlike,
         recording_id: Optional[Union[str, Callable[[Path], str]]] = None,
         relative_path_depth: Optional[int] = None,
         force_opus_sampling_rate: Optional[int] = None,
         force_read_audio: bool = False,
@@ -495,56 +506,27 @@
         )
 
     def to_dict(self) -> dict:
         return asdict_nonull(self)
 
     def to_cut(self):
         """
-        Create a Cut out of this recording.
-
-        For single-channel recordings, we return a :class:`MonoCut`.
-        For multi-channel recordings, we return a :class:`MixedCut` with as
-        many tracks as the number of channels.
-        The implementation of the multi-channel case may change in the future...
-        """
-        from lhotse.cut import MixedCut, MixTrack, MonoCut
-
-        if self.num_channels == 1:
-            return MonoCut(
-                id=self.id,
-                start=0.0,
-                duration=self.duration,
-                channel=self.channel_ids[0],
-                recording=self,
-            )
-        else:
-            # TODO: if we ever have "MultiCut" we may replace this implementation
-            return MixedCut(
-                id=self.id,
-                tracks=[
-                    MixTrack(
-                        cut=MonoCut(
-                            id=f"{self.id}_ch{cidx}",
-                            start=0.0,
-                            duration=self.duration,
-                            channel=cidx,
-                            recording=self,
-                        )
-                    )
-                    for cidx in self.channel_ids
-                ],
-            )
-
-    @property
-    def num_channels(self):
-        return sum(len(source.channels) for source in self.sources)
+        Create a Cut out of this recording --- MonoCut or MultiCut, depending on the
+        number of channels.
+        """
+        from lhotse.cut import MonoCut, MultiCut
 
-    @property
-    def channel_ids(self):
-        return sorted(cid for source in self.sources for cid in source.channels)
+        cls = MonoCut if self.num_channels == 1 else MultiCut
+        return cls(
+            id=self.id,
+            start=0.0,
+            duration=self.duration,
+            channel=self.channel_ids[0] if self.num_channels == 1 else self.channel_ids,
+            recording=self,
+        )
 
     @rich_exception_info
     def load_audio(
         self,
         channels: Optional[Channels] = None,
         offset: Seconds = 0.0,
         duration: Optional[Seconds] = None,
@@ -752,26 +734,44 @@
         :param affix_id: When true, we will modify the ``Recording.id`` field
             by affixing it with "_rvb".
         :param rir_channels: The channels of the impulse response to be used (in case of multi-channel
             impulse responses). By default, only the first channel is used. If no RIR is
             provided, we will generate one with as many channels as this argument specifies.
         :return: the perturbed ``Recording``.
         """
+
+        # We may need to change the `channel_ids` field according to whether we are convolving
+        # with a multi-channel RIR or not.
+        # The following cases are possible:
+        # Case 1: input is mono, rir is mono -> mono output, no need to change
+        # Case 2: input is mono, rir is multi-channel -> multi-channel output, change channel_ids
+        # Case 3: input is multi-channel, rir is mono -> multi-channel output, no need to change
+        # Case 4: input is multi-channel, rir is multi-channel -> multi-channel output,
+        #   no need to change (since we assume that the RIR has the same number of channels as the input)
+
+        if self.num_channels > 1 or rir_channels is None or len(rir_channels) == 1:
+            # Case 1, 3 or 4
+            new_channel_ids = self.channel_ids
+        else:
+            # Case 2
+            new_channel_ids = list(range(len(rir_channels)))
+
         transforms = self.transforms.copy() if self.transforms is not None else []
         transforms.append(
             ReverbWithImpulseResponse(
                 rir=rir_recording,
                 normalize_output=normalize_output,
                 early_only=early_only,
                 rir_channels=rir_channels if rir_channels is not None else [0],
             ).to_dict()
         )
         return fastcopy(
             self,
             id=f"{self.id}_rvb" if affix_id else self.id,
+            channel_ids=new_channel_ids,
             transforms=transforms,
         )
 
     def resample(self, sampling_rate: int) -> "Recording":
         """
         Return a new ``Recording`` that will be lazily resampled while loading audio.
         :param sampling_rate: The new sampling rate.
@@ -1191,14 +1191,24 @@
     It is initialized with a numpy array of audio samples (typically float32 in [-1, 1] range)
     that represents the "reference" signal for the mix.
     Other signals can be mixed to it with different time offsets and SNRs using the
     ``add_to_mix`` method.
     The time offset is relative to the start of the reference signal
     (only positive values are supported).
     The SNR is relative to the energy of the signal used to initialize the ``AudioMixer``.
+
+    .. note:: Both single-channel and multi-channel signals are supported as reference
+        and added signals. The only requirement is that the when mixing 2 multi-channel
+        signals, they must have the same number of channels.
+
+    .. note:: When the AudioMixer contains multi-channel tracks, 2 types of mixed signals
+        can be generated:
+        - `mixed_audio` mixes each channel independently, and returns a multi-channel signal.
+          If there is a mono track, it is added to all the channels.
+        - `mixed_mono_audio` mixes all channels together, and returns a single-channel signal.
     """
 
     def __init__(
         self,
         base_audio: np.ndarray,
         sampling_rate: int,
         reference_energy: Optional[float] = None,
@@ -1211,14 +1221,15 @@
         :param sampling_rate: Sampling rate of the audio.
         :param reference_energy: Optionally pass a reference energy value to compute SNRs against.
             This might be required when ``base_audio`` corresponds to zero-padding.
         """
         self.tracks = [base_audio]
         self.offsets = [0]
         self.sampling_rate = sampling_rate
+        self.num_channels = base_audio.shape[0]
         self.dtype = self.tracks[0].dtype
 
         # Keep a pre-computed energy value of the audio that we initialize the Mixer with;
         # it is required to compute gain ratios that satisfy SNR during the mix.
         if reference_energy is None:
             self.reference_energy = audio_energy(base_audio)
         else:
@@ -1248,54 +1259,74 @@
         for offset, audio in zip(self.offsets, self.tracks):
             longest = max(longest, offset + audio.shape[1])
         return longest
 
     @property
     def unmixed_audio(self) -> List[np.ndarray]:
         """
-        Return a list of numpy arrays with the shape (1, num_samples), where each track is
+        Return a list of numpy arrays with the shape (C, num_samples), where each track is
         zero padded and scaled adequately to the offsets and SNR used in ``add_to_mix`` call.
         """
         total = self.num_samples_total
         return [
             self._pad_track(track, offset=offset, total=total)
             for offset, track in zip(self.offsets, self.tracks)
         ]
 
     @property
     def mixed_audio(self) -> np.ndarray:
         """
-        Return a numpy ndarray with the shape (1, num_samples) - a mono mix of the tracks
+        Return a numpy ndarray with the shape (num_channels, num_samples) - a mix of the tracks
+        supplied with ``add_to_mix`` calls.
+        """
+        total = self.num_samples_total
+        mixed = np.zeros((self.num_channels, total), dtype=self.dtype)
+        for offset, track in zip(self.offsets, self.tracks):
+            # Only two cases are possible here: either the track is mono, or it has the same
+            # number of channels as the mixer. For the latter case, we don't need to do anything
+            # special, as we can just add the track to the mix. For the former case, we need to
+            # add the mono track to all channels by repeating it.
+            if track.shape[0] == 1 and self.num_channels > 1:
+                track = np.tile(track, (self.num_channels, 1))
+            mixed[:, offset : offset + track.shape[1]] += track
+        return mixed
+
+    @property
+    def mixed_mono_audio(self) -> np.ndarray:
+        """
+        Return a numpy ndarray with the shape (1, num_samples) - a mix of the tracks
         supplied with ``add_to_mix`` calls.
         """
         total = self.num_samples_total
         mixed = np.zeros((1, total), dtype=self.dtype)
         for offset, track in zip(self.offsets, self.tracks):
+            if track.shape[0] > 1:
+                # Sum all channels of the track
+                track = np.sum(track, axis=0, keepdims=True)
             mixed[:, offset : offset + track.shape[1]] += track
         return mixed
 
     def add_to_mix(
         self,
         audio: np.ndarray,
         snr: Optional[Decibels] = None,
         offset: Seconds = 0.0,
     ):
         """
-        Add audio (only support mono-channel) of a new track into the mix.
+        Add audio of a new track into the mix.
         :param audio: An array of audio samples to be mixed in.
         :param snr: Signal-to-noise ratio, assuming `audio` represents noise (positive SNR - lower `audio` energy,
         negative SNR - higher `audio` energy)
         :param offset: How many seconds to shift `audio` in time. For mixing, the signal will be padded before
         the start with low energy values.
         :return:
         """
-        if len(audio) == 0:
+        if audio.size == 0:
             return  # do nothing for empty arrays
 
-        assert audio.shape[0] == 1  # TODO: support multi-channels
         assert offset >= 0.0, "Negative offset in mixing is not supported."
 
         num_samples_offset = compute_num_samples(offset, self.sampling_rate)
 
         # When SNR is requested, find what gain is needed to satisfy the SNR
         gain = 1.0
         if snr is not None:
@@ -1308,14 +1339,24 @@
             # When mixing time-domain signals, we are working with root-power (field) quantities,
             # whereas the energy ratio applies to power quantities. To compute the gain correctly,
             # we need to take a square root of the energy ratio.
             gain = sqrt(target_energy / added_audio_energy)
 
         self.tracks.append(gain * audio)
         self.offsets.append(num_samples_offset)
+        # We cannot mix 2 multi-channel audios with different number of channels.
+        if (
+            audio.shape[0] != self.num_channels
+            and self.num_channels != 1
+            and audio.shape[0] != 1
+        ):
+            raise ValueError(
+                f"Cannot mix audios with {audio.shape[0]} and {self.num_channels} channels."
+            )
+        self.num_channels = max(self.num_channels, audio.shape[0])
 
 
 def audio_energy(audio: np.ndarray) -> float:
     return float(np.average(audio**2))
 
 
 FileObject = Any  # Alias for file-like objects
```

### Comparing `lhotse-1.8.0/lhotse/augmentation/torchaudio.py` & `lhotse-1.9.0/lhotse/augmentation/torchaudio.py`

 * *Files 19% similar despite different names*

```diff
@@ -353,55 +353,80 @@
 
     def __call__(
         self,
         samples: np.ndarray,
         sampling_rate: int,
     ) -> np.ndarray:
         """
-        :param samples: The audio samples to reverberate (must be single-channel).
+        :param samples: The audio samples to reverberate.
         :param sampling_rate: The sampling rate of the audio samples.
         """
-        assert samples.shape[0] == 1, "The input audio must be single-channel."
         sampling_rate = int(sampling_rate)  # paranoia mode
 
-        if self.rir is None:
-            rir_ = generate_fast_random_rir(
-                nsource=len(self.rir_channels), sr=sampling_rate
+        D_in, N_in = samples.shape
+        input_is_mono = D_in == 1
+
+        # The following cases are possible:
+        # Case 1: input is mono, rir is mono -> mono output
+        #   We will generate a random mono rir if not provided explicitly.
+        # Case 2: input is mono, rir is multi-channel -> multi-channel output
+        #   This requires a user-provided rir, since we cannot simulate array microphone.
+        # Case 3: input is multi-channel, rir is mono -> multi-channel output
+        #   This does not make much sense, but we will apply the same rir to all channels.
+        # 4. input is multi-channel, rir is multi-channel -> multi-channel output
+        #   This also requires a user-provided rir. Also, the number of channels in the rir
+        #   must match the number of channels in the input.
+
+        # Let us make some assertions based on the above.
+        if input_is_mono:
+            assert (
+                self.rir is not None or len(self.rir_channels) == 1
+            ), "For mono input, either provide an RIR explicitly or set rir_channels to [0]."
+        else:
+            assert len(self.rir_channels) == 1 or len(self.rir_channels) == D_in, (
+                "For multi-channel input, we only support mono RIR or RIR with the same number "
+                "of channels as the input."
             )
+
+        # Generate a random RIR if not provided.
+        if self.rir is None:
+            rir_ = generate_fast_random_rir(nsource=1, sr=sampling_rate)
         else:
             rir_ = (
                 self.rir.load_audio(channels=self.rir_channels)
                 if not self.early_only
-                else self.rir.load_audio(duration=0.05)
+                else self.rir.load_audio(channels=self.rir_channels, duration=0.05)
             )
 
-        # Determine output length.
-        _, N_in = samples.shape
-        D, N_rir = rir_.shape
+        D_rir, N_rir = rir_.shape
         N_out = N_in  # Enforce shift output
+        # output is multi-channel if either input or rir is multi-channel
+        D_out = D_rir if input_is_mono else D_in
+
+        # if RIR is mono, repeat it to match the number of channels in the input
+        rir_ = rir_.repeat(D_out, axis=0) if D_rir == 1 else rir_
 
         # Initialize output matrix with the specified input channel.
-        augmented = np.zeros((D, N_out), dtype=samples.dtype)
-        power_before_reverb = np.sum(np.abs(samples) ** 2) / samples.shape[1]
+        augmented = np.zeros((D_out, N_out), dtype=samples.dtype)
 
-        for d in range(D):
-            augmented[d, :N_in] = samples
+        for d in range(D_out):
+            d_in = 0 if input_is_mono else d
+            augmented[d, :N_in] = samples[d_in]
+            power_before_reverb = np.sum(np.abs(samples[d_in]) ** 2) / N_in
             rir_d = rir_[d, :] * self.RIR_SCALING_FACTOR
 
             # Convolve the signal with impulse response.
             aug_d = convolve1d(
-                torch.from_numpy(samples[0]), torch.from_numpy(rir_d)
+                torch.from_numpy(samples[d_in]), torch.from_numpy(rir_d)
             ).numpy()
             shift_index = np.argmax(rir_d)
             augmented[d, :] = aug_d[shift_index : shift_index + N_out]
 
             if self.normalize_output:
-                power_after_reverb = (
-                    np.sum(np.abs(augmented[d, :]) ** 2) / augmented.shape[1]
-                )
+                power_after_reverb = np.sum(np.abs(augmented[d, :]) ** 2) / N_out
                 if power_after_reverb > 0:
                     augmented[d, :] *= np.sqrt(power_before_reverb / power_after_reverb)
 
         return augmented
 
     def reverse_timestamps(
         self,
```

### Comparing `lhotse-1.8.0/lhotse/augmentation/transform.py` & `lhotse-1.9.0/lhotse/augmentation/transform.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/augmentation/utils.py` & `lhotse-1.9.0/lhotse/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/augmentation/wpe.py` & `lhotse-1.9.0/lhotse/augmentation/wpe.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/lhotse.py` & `lhotse-1.9.0/lhotse/bin/lhotse.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/cli_base.py` & `lhotse-1.9.0/lhotse/bin/modes/cli_base.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/cut.py` & `lhotse-1.9.0/lhotse/bin/modes/cut.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/features.py` & `lhotse-1.9.0/lhotse/bin/modes/features.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/install_tools.py` & `lhotse-1.9.0/lhotse/bin/modes/install_tools.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/kaldi.py` & `lhotse-1.9.0/lhotse/bin/modes/kaldi.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,34 +35,45 @@
 @click.option(
     "-j",
     "--num-jobs",
     default=1,
     type=int,
     help="Number of jobs for computing recording durations.",
 )
+@click.option(
+    "-d",
+    "--compute-durations",
+    default=False,
+    is_flag=True,
+    show_default=True,
+    type=bool,
+    help="Compute durations by reading the whole file instead of using reco2dur file",
+)
 def import_(
     data_dir: Pathlike,
     sampling_rate: int,
     manifest_dir: Pathlike,
     frame_shift: float,
     map_string_to_underscores: Optional[str],
     num_jobs: int,
+    compute_durations: bool,
 ):
     """
     Convert a Kaldi data dir DATA_DIR into a directory MANIFEST_DIR of lhotse manifests. Ignores feats.scp.
     The SAMPLING_RATE has to be explicitly specified as it is not available to read from DATA_DIR.
     """
     from lhotse.kaldi import load_kaldi_data_dir
 
     recording_set, maybe_supervision_set, maybe_feature_set = load_kaldi_data_dir(
         path=data_dir,
         sampling_rate=sampling_rate,
         frame_shift=frame_shift,
         map_string_to_underscores=map_string_to_underscores,
         num_jobs=num_jobs,
+        use_reco2dur=not compute_durations,
     )
     manifest_dir = Path(manifest_dir)
     manifest_dir.mkdir(parents=True, exist_ok=True)
     recording_set.to_file(manifest_dir / "recordings.jsonl.gz")
     if maybe_supervision_set is not None:
         maybe_supervision_set.to_file(manifest_dir / "supervisions.jsonl.gz")
     if maybe_feature_set is not None:
```

### Comparing `lhotse-1.8.0/lhotse/bin/modes/manipulation.py` & `lhotse-1.9.0/lhotse/bin/modes/manipulation.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/__init__.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .bvcc import *
 from .callhome_egyptian import *
 from .callhome_english import *
 from .cmu_arctic import *
 from .cmu_indic import *
 from .cmu_kids import *
 from .commonvoice import *
+from .csj import *
 from .cslu_kids import *
 from .daily_talk import *
 from .dihard3 import *
 from .earnings21 import *
 from .earnings22 import *
 from .eval2000 import *
 from .fisher_english import *
```

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/adept.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/adept.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/aidatatang_200zh.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/aidatatang_200zh.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/aishell.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/aishell.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/aishell2.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/aishell2.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/aishell4.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/aishell4.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/ali_meeting.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/ali_meeting.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/ami.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/ami.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/aspire.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/aspire.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/babel.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/babel.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/broadcast_news.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/broadcast_news.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/bvcc.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/bvcc.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/callhome_egyptian.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/callhome_egyptian.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/callhome_english.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/callhome_english.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/cmu_arctic.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/cmu_arctic.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/cmu_indic.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/cmu_indic.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/cmu_kids.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/cmu_kids.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/commonvoice.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/commonvoice.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/cslu_kids.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/cslu_kids.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/daily_talk.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/daily_talk.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/dihard3.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/dihard3.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/earnings21.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/earnings21.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/earnings22.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/earnings22.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/eval2000.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/eval2000.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/fisher_english.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/fisher_english.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/fisher_spanish.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/fisher_spanish.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/gale_arabic.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/gale_arabic.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/gale_mandarin.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/gale_mandarin.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/gigaspeech.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/gigaspeech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/heroico.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/heroico.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/hifitts.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/hifitts.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/icsi.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/icsi.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/libricss.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/libricss.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/librimix.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/librimix.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/librispeech.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/librispeech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/libritts.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/libritts.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/ljspeech.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/ljspeech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/magicdata.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/magicdata.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/mgb2.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/mgb2.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/mls.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/mls.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/mtedx.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/mtedx.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/musan.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/musan.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/nsc.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/nsc.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/peoples_speech.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/peoples_speech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/primewords.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/primewords.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/rir_noise.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/rir_noise.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/spgispeech.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/spgispeech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/stcmds.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/stcmds.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/switchboard.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/switchboard.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/tal_csasr.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/tal_csasr.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/tedlium.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/tedlium.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/thchs_30.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/thchs_30.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/timit.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/timit.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/vctk.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/vctk.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/voxceleb.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/voxceleb.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/wenet_speech.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/wenet_speech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/recipes/yesno.py` & `lhotse-1.9.0/lhotse/bin/modes/recipes/yesno.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/validate.py` & `lhotse-1.9.0/lhotse/bin/modes/validate.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/bin/modes/workflows.py` & `lhotse-1.9.0/lhotse/bin/modes/workflows.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 @click.option(
     "-r",
     "--recordings-dir",
     type=click.Path(exists=True, file_okay=False),
     help="Directory with recordings. We will create a RecordingSet for it automatically.",
 )
 @click.option(
+    "-c",
+    "--cuts-manifest",
+    type=click.Path(exists=True, dir_okay=False, allow_dash=True),
+    help="Path to an existing cuts manifest.",
+)
+@click.option(
     "-e",
     "--extension",
     default="wav",
     help="Audio file extension to search for. Used with RECORDINGS_DIR.",
 )
 @click.option(
     "-n",
@@ -51,50 +57,57 @@
     "-d", "--device", default="cpu", help="Device on which to run the inference."
 )
 @click.option("-j", "--jobs", default=1, help="Number of jobs for audio scanning.")
 def annotate_with_whisper(
     out_cuts: str,
     recordings_manifest: Optional[str],
     recordings_dir: Optional[str],
+    cuts_manifest: Optional[str],
     extension: str,
     model_name: str,
     language: Optional[str],
     device: str,
     jobs: int,
 ):
     """
-    Use OpenAI Whisper model to annotate either RECORDINGS_MANIFEST or RECORDINGS_DIR.
+    Use OpenAI Whisper model to annotate either RECORDINGS_MANIFEST, RECORDINGS_DIR, or CUTS_MANIFEST.
     It will perform automatic segmentation, transcription, and language identification.
 
-    RECORDINGS_MANIFEST and RECORDINGS_DIR are mutually exclusive.
+    RECORDINGS_MANIFEST, RECORDINGS_DIR, and CUTS_MANIFEST are mutually exclusive. If CUTS_MANIFEST
+    is provided, its supervisions will be overwritten with the results of the inference.
 
     Note: this is an experimental feature of Lhotse, and is not guaranteed to yield
     high quality of data.
     """
     from lhotse import annotate_with_whisper as annotate_with_whisper_
 
-    assert exactly_one_not_null(recordings_manifest, recordings_dir), (
-        "Options RECORDINGS_MANIFEST and RECORDINGS_DIR are mutually exclusive "
+    assert exactly_one_not_null(recordings_manifest, recordings_dir, cuts_manifest), (
+        "Options RECORDINGS_MANIFEST, RECORDINGS_DIR, and CUTS_MANIFEST are mutually exclusive "
         "and at least one is required."
     )
 
     if recordings_manifest is not None:
-        recordings = RecordingSet.from_file(recordings_manifest)
-    else:
-        recordings = RecordingSet.from_dir(
+        manifest = RecordingSet.from_file(recordings_manifest)
+    elif recordings_dir is not None:
+        manifest = RecordingSet.from_dir(
             recordings_dir, pattern=f"*.{extension}", num_jobs=jobs
         )
+    else:
+        manifest = CutSet.from_file(cuts_manifest).to_eager()
 
     with CutSet.open_writer(out_cuts) as writer:
         for cut in tqdm(
             annotate_with_whisper_(
-                recordings, language=language, model_name=model_name, device=device
+                manifest,
+                language=language,
+                model_name=model_name,
+                device=device,
             ),
-            total=len(recordings),
-            desc="Recordings",
+            total=len(manifest),
+            desc="Annotating with Whisper",
         ):
             writer.write(cut, flush=True)
 
 
 @workflows.command()
 @click.argument(
     "in_cuts", type=click.Path(exists=True, dir_okay=False, allow_dash=True)
```

### Comparing `lhotse-1.8.0/lhotse/caching.py` & `lhotse-1.9.0/lhotse/caching.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/cut/__init__.py` & `lhotse-1.9.0/lhotse/cut/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-from .base import Cut
-from .mixed import MixedCut, MixTrack
-from .mono import MonoCut
-from .padding import PaddingCut
-from .set import CutSet
-
 """
 The following is the hierarchy of imports in this module (to avoid circular imports):
+
       ┌─────────────┐
-      │ __init__.py │─────────────────────────────────┬────────────────────┐
-      └─────────────┘                                 │                    │
-             │                                        ▼                    │
-             │                               ┌────────────────┐            │
-             ├──────────────────────┬───────▶│  mono.MonoCut  │────────────┤
-             │                      │        └────────────────┘            │
-             │                      │                                      │
-             │                      │                                      │
-             │           ┌────────────────────┐                            ▼
-             │           │   mixed.MixTrack   │                     ┌─────────────┐
-             ├──────────▶│   mixed.MixedCut   │────────────────────▶│  base.Cut   │
-             │           └────────────────────┘                     └─────────────┘
-             │                      │                                      ▲
-             │                      │                                      │
-             │                      │                                      │
-             │                      │        ┌────────────────────┐        │
-             ├──────────────────────┴───────▶│ padding.PaddingCut │────────┤
-             │                               └────────────────────┘        │
-    ┌────────────────┐                                  ▲                  │
-    │   set.CutSet   │──────────────────────────────────┴──────────────────┘
+      │ __init__.py │─────────────┬────────────────────────────────────────────┐
+      └─────────────┘             │                                            │
+             │                    │                                            │
+             │                    ▼                                            │
+             │           ┌────────────────┐                                    │
+             ├──────────▶│  mono.MonoCut  │────────────────────┐               │
+             │           └────────────────┘                    │               │
+             │                                                 ▼               │
+             │           ┌────────────────┐           ┌────────────────┐       │
+             ├──────────▶│ multi.MultiCut │──────────▶│  data.DataCut  │───────┤
+             │           └────────────────┘           └────────────────┘       │
+             │                                                 ▲               ▼
+             │           ┌────────────────────┐                │        ┌─────────────┐
+             ├──────────▶│   mixed.MixedCut   │────────────────┴───────▶│  base.Cut   │
+             │           └────────────────────┘                         └─────────────┘
+             │                      │                                          ▲
+             │                      │                                          │
+             │                      │         ┌────────────────────┐           │
+             ├──────────────────────┴────────▶│ padding.PaddingCut │───────────┤
+             │                                └────────────────────┘           │
+    ┌────────────────┐                                   ▲                     │
+    │   set.CutSet   │───────────────────────────────────┴─────────────────────┘
     └────────────────┘
+
 """
 
+from .base import Cut
+from .mixed import MixedCut, MixTrack
+from .mono import MonoCut
+from .multi import MultiCut
+from .padding import PaddingCut
+from .set import CutSet
+
 # The following functions are imported in other modules, so we need to import them here.
 __all__ = [
     "create_cut_set_eager",
     "create_cut_set_lazy",
     "compute_supervisions_frame_mask",
     "append_cuts",
     "mix_cuts",
```

### Comparing `lhotse-1.8.0/lhotse/cut/base.py` & `lhotse-1.9.0/lhotse/cut/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -390,14 +390,15 @@
         plt.show()
 
     def trim_to_supervisions(
         self,
         keep_overlapping: bool = True,
         min_duration: Optional[Seconds] = None,
         context_direction: Literal["center", "left", "right", "random"] = "center",
+        keep_all_channels: bool = False,
     ) -> "CutSet":  # noqa: F821
         """
         Splits the current :class:`.Cut` into as many cuts as there are supervisions (:class:`.SupervisionSegment`).
         These cuts have identical start times and durations as the supervisions.
         When there are overlapping supervisions, they can be kept or discarded via ``keep_overlapping`` flag.
 
         For example, the following cut::
@@ -419,27 +420,43 @@
                     Cut2
                |-----------|
                Sup1
                |-|
                     Sup2
                |-----------|
 
+        For the case of a multi-channel cut with multiple supervisions, we can either trim
+        while respecting the supervision channels (in which case output cut has the same channels
+        as the supervision) or ignore the channels (in which case output cut has the same channels
+        as the input cut).
+
+        .. hint:: If the resulting trimmed cut contains a single supervision, we set the cut id to
+            the ``id`` of this supervision, for better compatibility with downstream tools, e.g.
+            comparing the hypothesis of ASR with the reference in icefall.
+
+        .. hint:: If a MultiCut is trimmed and the resulting trimmed cut contains a single channel,
+            we convert it to a MonoCut.
+
         :param keep_overlapping: when ``False``, it will discard parts of other supervisions that overlap with the
             main supervision. In the illustration above, it would discard ``Sup2`` in ``Cut1`` and ``Sup1`` in ``Cut2``.
             In this mode, we guarantee that there will always be exactly one supervision per cut.
         :param min_duration: An optional duration in seconds; specifying this argument will extend the cuts
             that would have been shorter than ``min_duration`` with actual acoustic context in the recording/features.
             If there are supervisions present in the context, they are kept when ``keep_overlapping`` is true.
             If there is not enough context, the returned cut will be shorter than ``min_duration``.
             If the supervision segment is longer than ``min_duration``, the return cut will be longer.
         :param context_direction: Which direction should the cut be expanded towards to include context.
             The value of "center" implies equal expansion to left and right;
             random uniformly samples a value between "left" and "right".
+        :param keep_all_channels: If ``True``, the output cut will have the same channels as the input cut. By default,
+            the trimmed cut will have the same channels as the supervision.
         :return: a list of cuts.
         """
+        from .mixed import MixedCut
+        from .multi import MultiCut
         from .set import CutSet
 
         cuts = []
         supervisions_index = self.index_supervisions(index_mixed_tracks=True)
         for segment in self.supervisions:
             if min_duration is None:
                 # Cut boundaries are equal to the supervision segment boundaries.
@@ -454,17 +471,39 @@
                 )
             trimmed = self.truncate(
                 offset=new_start,
                 duration=new_duration,
                 keep_excessive_supervisions=keep_overlapping,
                 _supervisions_index=supervisions_index,
             )
+
             if not keep_overlapping:
                 # Ensure that there is exactly one supervision per cut.
                 trimmed = trimmed.filter_supervisions(lambda s: s.id == segment.id)
+
+            if not keep_all_channels and not isinstance(trimmed, MixedCut):
+                # For MixedCut, we can't change the channels since it is defined by the
+                # number of channels in underlying tracks.
+
+                # Ensure that all supervisions have the same channel.
+                assert len(set(s.channel for s in trimmed.supervisions)) == 1, (
+                    "Trimmed cut has supervisions with different channels. Either set "
+                    "`ignore_channel=True` to keep original channels or `keep_overlapping=False` "
+                    "to retain only 1 supervision per trimmed cut."
+                )
+                trimmed.channel = trimmed.supervisions[0].channel
+
+                # If we have a single-channel MultiCut, we will convert it into a MonoCut.
+                if isinstance(trimmed, MultiCut) and trimmed.num_channels == 1:
+                    trimmed = trimmed.to_mono()[0]
+
+            if len(trimmed.supervisions) == 1:
+                # If the trimmed cut contains a single supervision, we set the cut id to
+                # the id of this supervision.
+                trimmed.id = segment.id
             cuts.append(trimmed)
         return CutSet.from_cuts(cuts)
 
     def cut_into_windows(
         self,
         duration: Seconds,
         hop: Optional[Seconds] = None,
@@ -565,20 +604,18 @@
 
         :param storage_path: The path to location where we will store the audio recordings.
         :param augment_fn: an optional callable used for audio augmentation.
             Be careful with the types of augmentations used: if they modify
             the start/end/duration times of the cut and its supervisions,
             you will end up with incorrect supervision information when using this API.
             E.g. for speed perturbation, use ``CutSet.perturb_speed()`` instead.
-        :return: a new MonoCut instance.
+        :return: a new Cut instance.
         """
         import torchaudio
 
-        from .mono import MonoCut
-
         storage_path = Path(storage_path)
         samples = self.load_audio()
         if augment_fn is not None:
             samples = augment_fn(samples, self.sampling_rate)
 
         torchaudio.save(
             str(storage_path), torch.as_tensor(samples), sample_rate=self.sampling_rate
@@ -587,26 +624,22 @@
             id=storage_path.stem,
             sampling_rate=self.sampling_rate,
             num_samples=samples.shape[1],
             duration=samples.shape[1] / self.sampling_rate,
             sources=[
                 AudioSource(
                     type="file",
-                    channels=[0],
+                    channels=list(range(self.num_channels)),
                     source=str(storage_path),
                 )
             ],
         )
-        return MonoCut(
-            id=self.id,
-            start=0,
-            duration=recording.duration,
-            channel=0,
+        return fastcopy(
+            recording.to_cut(),
             supervisions=self.supervisions,
-            recording=recording,
             custom=self.custom if hasattr(self, "custom") else None,
         )
 
     def speakers_feature_mask(
         self,
         min_speaker_dim: Optional[int] = None,
         speaker_to_idx_map: Optional[Dict[str, int]] = None,
```

### Comparing `lhotse-1.8.0/lhotse/cut/mixed.py` & `lhotse-1.9.0/lhotse/cut/mixed.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
+import warnings
 from dataclasses import dataclass
-from functools import partial
+from functools import partial, reduce
+from operator import add
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 from intervaltree import IntervalTree
 
 from lhotse.audio import AudioMixer, Recording, audio_energy
 from lhotse.augmentation import AugmentFn
 from lhotse.cut.base import Cut
-from lhotse.cut.mono import MonoCut
+from lhotse.cut.data import DataCut
 from lhotse.cut.padding import PaddingCut
 from lhotse.features import (
     FeatureExtractor,
     FeatureMixer,
     create_default_feature_extractor,
 )
 from lhotse.features.io import FeaturesWriter
@@ -25,48 +27,53 @@
     NonPositiveEnergyError,
     Pathlike,
     Seconds,
     add_durations,
     compute_num_frames,
     compute_num_samples,
     fastcopy,
+    merge_items_with_delimiter,
+    overlaps,
     perturb_num_samples,
     rich_exception_info,
     uuid4,
 )
 
 
 @dataclass
 class MixTrack:
     """
-    Represents a single track in a mix of Cuts. Points to a specific MonoCut and holds information on
+    Represents a single track in a mix of Cuts. Points to a specific DataCut or PaddingCut and holds information on
     how to mix it with other Cuts, relative to the first track in a mix.
     """
 
-    cut: Union[MonoCut, PaddingCut]
+    cut: Union[DataCut, PaddingCut]
+    type: str = None
     offset: Seconds = 0.0
     snr: Optional[Decibels] = None
 
+    def __post_init__(self):
+        self.type = type(self.cut).__name__
+
     @staticmethod
     def from_dict(data: dict):
-        raw_cut = data.pop("cut")
-        try:
-            cut = MonoCut.from_dict(raw_cut)
-        except TypeError:
-            cut = PaddingCut.from_dict(raw_cut)
-        return MixTrack(cut, **data)
+        from .set import deserialize_cut
+
+        # Take out `type` from data dict and put it into the `cut` dict.
+        cut_dict = data.pop("cut")
+        cut_dict["type"] = data.pop("type")
+        return MixTrack(deserialize_cut(cut_dict), **data)
 
 
 @dataclass
 class MixedCut(Cut):
     """
     :class:`~lhotse.cut.MixedCut` is a :class:`~lhotse.cut.Cut` that actually consists of multiple other cuts.
-    It can be interpreted as a multi-channel cut, but its primary purpose is to allow
-    time-domain and feature-domain augmentation via mixing the training cuts with noise, music, and babble cuts.
-    The actual mixing operations are performed on-the-fly.
+    Its primary purpose is to allow time-domain and feature-domain augmentation via mixing the training cuts
+    with noise, music, and babble cuts. The actual mixing operations are performed on-the-fly.
 
     Internally, :class:`~lhotse.cut.MixedCut` holds other cuts in multiple trakcs (:class:`~lhotse.cut.MixTrack`),
     each with its own offset and SNR that is relative to the first track.
 
     Please refer to the documentation of :class:`~lhotse.cut.Cut` to learn more about using cuts.
 
     In addition to methods available in :class:`~lhotse.cut.Cut`, :class:`~lhotse.cut.MixedCut` provides the methods to
@@ -75,18 +82,24 @@
         >>> cut = MixedCut(...)
         >>> mono_features = cut.load_features()
         >>> assert len(mono_features.shape) == 2
         >>> multi_features = cut.load_features(mixed=False)
         >>> # Now, the first dimension is the channel.
         >>> assert len(multi_features.shape) == 3
 
+    .. note:: MixedCut is different from MultiCut, which is intended to represent multi-channel recordings
+        that share the same supervisions.
+
+    .. note:: Each track in a MixedCut can be either a MonoCut, MultiCut, or PaddingCut.
+
     See also:
 
         - :class:`lhotse.cut.Cut`
         - :class:`lhotse.cut.MonoCut`
+        - :class:`lhotse.cut.MultiCut`
         - :class:`lhotse.cut.CutSet`
     """
 
     id: str
     tracks: List[MixTrack]
 
     @property
@@ -107,14 +120,19 @@
 
     @property
     def duration(self) -> Seconds:
         track_durations = (track.offset + track.cut.duration for track in self.tracks)
         return round(max(track_durations), ndigits=8)
 
     @property
+    def channel(self) -> Union[int, List[int]]:
+        num_channels = self.num_channels
+        return list(range(num_channels)) if num_channels > 1 else 0
+
+    @property
     def has_features(self) -> bool:
         return self._first_non_padding_cut.has_features
 
     @property
     def has_recording(self) -> bool:
         return self._first_non_padding_cut.has_recording
 
@@ -144,14 +162,19 @@
         return compute_num_samples(self.duration, self.sampling_rate)
 
     @property
     def num_features(self) -> Optional[int]:
         return self.tracks[0].cut.num_features
 
     @property
+    def num_channels(self) -> Optional[int]:
+        # PaddingCut and MonoCut have 1 channel each, MultiCut has N. We don't support MixedCut with MixedCut tracks.
+        return max(track.cut.num_channels for track in self.tracks)
+
+    @property
     def features_type(self) -> Optional[str]:
         return self._first_non_padding_cut.features.type if self.has_features else None
 
     def __getattr__(self, name: str) -> Any:
         """
         This magic function is called when the user tries to access an attribute
         of :class:`.MixedCut` that doesn't exist. It is used for accessing the custom
@@ -186,15 +209,15 @@
 
         # Returning the contents of "mono_cut.custom[name]",
         # or raising AttributeError.
         try:
             (
                 non_padding_idx,
                 mono_cut,
-            ) = self._assert_one_mono_cut_with_attr_and_return_it_with_track_index(name)
+            ) = self._assert_one_data_cut_with_attr_and_return_it_with_track_index(name)
             return getattr(mono_cut, name)
         except AssertionError:
             raise AttributeError(
                 f"No such attribute: '{name}' (note: custom attributes are not supported "
                 f"when a MixedCut consists of more than one MonoCut with that attribute)."
             )
 
@@ -217,15 +240,15 @@
         """
 
         from lhotse.array import Array, pad_array
 
         (
             non_padding_idx,
             mono_cut,
-        ) = self._assert_one_mono_cut_with_attr_and_return_it_with_track_index(name)
+        ) = self._assert_one_data_cut_with_attr_and_return_it_with_track_index(name)
 
         # Use getattr to propagate AttributeError if "name" is not defined.
         manifest = getattr(mono_cut, name)
 
         # Check if the corresponding manifest for 'load_something' is of type
         # Array; if yes, just return the loaded data.
         # This is likely an embedding without a temporal dimension.
@@ -263,34 +286,34 @@
             temporal_dim=manifest.temporal_dim,
             frame_shift=manifest.frame_shift,
             offset=left_padding,
             padded_duration=padded_duration,
             pad_value=pad_value,
         )
 
-    def _assert_one_mono_cut_with_attr_and_return_it_with_track_index(
+    def _assert_one_data_cut_with_attr_and_return_it_with_track_index(
         self,
         attr_name: str,
-    ) -> Tuple[int, MonoCut]:
+    ) -> Tuple[int, DataCut]:
         # TODO(pzelasko): consider relaxing this condition to
         #                 supporting mixed cuts that are not overlapping
         non_padding_cuts = [
             (idx, t.cut)
             for idx, t in enumerate(self.tracks)
-            if isinstance(t.cut, MonoCut)
+            if isinstance(t.cut, DataCut)
         ]
         non_padding_cuts_with_custom_attr = [
             (idx, cut)
             for idx, cut in non_padding_cuts
             if cut.custom is not None and attr_name in cut.custom
         ]
         assert len(non_padding_cuts_with_custom_attr) == 1, (
             f"This MixedCut has {len(non_padding_cuts_with_custom_attr)} non-padding cuts "
             f"with a custom attribute '{attr_name}'. We currently don't support mixing custom attributes. "
-            f"Consider dropping the attribute on all but one of MonoCuts. Problematic cut:\n{self}"
+            f"Consider dropping the attribute on all but one of DataCuts. Problematic cut:\n{self}"
         )
         non_padding_idx, mono_cut = non_padding_cuts_with_custom_attr[0]
         return non_padding_idx, mono_cut
 
     def truncate(
         self,
         *,
@@ -345,37 +368,37 @@
             # 'track_end' is expressed relative to the beginning of the mix
             # (not to be confused with the 'start' of the underlying MonoCut)
             track_end = add_durations(
                 track.offset, track.cut.duration, sampling_rate=self.sampling_rate
             )
 
             if track_end < offset:
-                # Omit a MonoCut that ends before the truncation offset.
+                # Omit a Cut that ends before the truncation offset.
                 continue
 
             cut_duration_decrease = 0
             if track_end > new_mix_end:
                 if duration is not None:
                     cut_duration_decrease = add_durations(
                         track_end, -new_mix_end, sampling_rate=self.sampling_rate
                     )
                 else:
                     cut_duration_decrease = add_durations(
                         track_end, -old_duration, sampling_rate=self.sampling_rate
                     )
 
-            # Compute the new MonoCut's duration after trimming the start and the end.
+            # Compute the new Cut's duration after trimming the start and the end.
             new_duration = add_durations(
                 track.cut.duration,
                 -cut_offset,
                 -cut_duration_decrease,
                 sampling_rate=self.sampling_rate,
             )
             if new_duration <= 0:
-                # Omit a MonoCut that is completely outside the time span of the new truncated MixedCut.
+                # Omit a Cut that is completely outside the time span of the new truncated MixedCut.
                 continue
 
             new_tracks.append(
                 MixTrack(
                     cut=track.cut.truncate(
                         offset=cut_offset,
                         duration=new_duration,
@@ -509,37 +532,37 @@
             by affixing it with "_sp{factor}".
         :return: a modified copy of the current ``MixedCut``.
         """
         # TODO(pzelasko): test most extensively for edge cases
         # Pre-conditions
         assert (
             self.has_recording
-        ), "Cannot perturb speed on a MonoCut without Recording."
+        ), "Cannot perturb speed on a MixedCut without Recording."
         if self.has_features:
             logging.warning(
                 "Attempting to perturb speed on a MixedCut that references pre-computed features. "
                 "The feature manifest(s) will be detached, as we do not support feature-domain "
                 "speed perturbation."
             )
         return MixedCut(
             id=f"{self.id}_sp{factor}" if affix_id else self.id,
             tracks=[
-                MixTrack(
+                fastcopy(
+                    track,
                     cut=track.cut.perturb_speed(factor=factor, affix_id=affix_id),
                     offset=round(
                         perturb_num_samples(
                             num_samples=compute_num_samples(
                                 track.offset, self.sampling_rate
                             ),
                             factor=factor,
                         )
                         / self.sampling_rate,
                         ndigits=8,
                     ),
-                    snr=track.snr,
                 )
                 for track in self.tracks
             ],
         )
 
     def perturb_tempo(self, factor: float, affix_id: bool = True) -> "MixedCut":
         """
@@ -556,37 +579,37 @@
             by affixing it with "_tp{factor}".
         :return: a modified copy of the current ``MixedCut``.
         """
         # TODO(pzelasko): test most extensively for edge cases
         # Pre-conditions
         assert (
             self.has_recording
-        ), "Cannot perturb tempo on a MonoCut without Recording."
+        ), "Cannot perturb tempo on a MixedCut without Recording."
         if self.has_features:
             logging.warning(
                 "Attempting to perturb tempo on a MixedCut that references pre-computed features. "
                 "The feature manifest(s) will be detached, as we do not support feature-domain "
                 "tempo perturbation."
             )
         return MixedCut(
             id=f"{self.id}_tp{factor}" if affix_id else self.id,
             tracks=[
-                MixTrack(
+                fastcopy(
+                    track,
                     cut=track.cut.perturb_tempo(factor=factor, affix_id=affix_id),
                     offset=round(
                         perturb_num_samples(
                             num_samples=compute_num_samples(
                                 track.offset, self.sampling_rate
                             ),
                             factor=factor,
                         )
                         / self.sampling_rate,
                         ndigits=8,
                     ),
-                    snr=track.snr,
                 )
                 for track in self.tracks
             ],
         )
 
     def perturb_volume(self, factor: float, affix_id: bool = True) -> "MixedCut":
         """
@@ -597,15 +620,15 @@
         :param affix_id: When true, we will modify the ``MixedCut.id`` field
             by affixing it with "_vp{factor}".
         :return: a modified copy of the current ``MixedCut``.
         """
         # Pre-conditions
         assert (
             self.has_recording
-        ), "Cannot perturb volume on a MonoCut without Recording."
+        ), "Cannot perturb volume on a MixedCut without Recording."
         if self.has_features:
             logging.warning(
                 "Attempting to perturb volume on a MixedCut that references pre-computed features. "
                 "The feature manifest(s) will be detached, as we do not support feature-domain "
                 "volume perturbation."
             )
         return MixedCut(
@@ -653,17 +676,18 @@
                 "The feature manifest(s) will be detached, as we do not support feature-domain "
                 "reverberation."
             )
 
         assert rir_recording is None or all(
             c < rir_recording.num_channels for c in rir_channels
         ), "Invalid channel index in `rir_channels`."
+
         assert len(rir_channels) == 1 or len(rir_channels) == len(
             self.tracks
-        ), "Invalid number of channels in `rir_channels`. Must be 1 or equal to number of tracks."
+        ), "Invalid number of channels in `rir_channels`, must be either 1 or equal to the number of tracks."
 
         if len(rir_channels) == 1:
             rir_channels = rir_channels * len(self.tracks)
 
         # NOTE: Currently, if no RIR is provided, this method will generate a
         # random one for each track in the MixedCut. This is not ideal since the room
         # configuration for all the RIRs should be the same. But we ignore this for now
@@ -687,32 +711,47 @@
         )
 
     @rich_exception_info
     def load_features(self, mixed: bool = True) -> Optional[np.ndarray]:
         """
         Loads the features of the source cuts and mixes them on-the-fly.
 
-        :param mixed: when True (default), returns a 2D array of features mixed in the feature domain.
-            Otherwise returns a 3D array with the first dimension equal to the number of tracks.
+        :param mixed: when True (default), the features are mixed together (as defined in
+            the mixing function for the extractor). This could result in either a 2D or 3D
+            array. For example, if all underlying tracks are single-channel, the output
+            will be a 2D array of shape (num_frames, num_features). If any of the tracks
+            are multi-channel, the output may be a 3D array of shape (num_frames, num_features,
+            num_channels).
         :return: A numpy ndarray with features and with shape ``(num_frames, num_features)``,
             or ``(num_tracks, num_frames, num_features)``
         """
         if not self.has_features:
             return None
         first_cut = self.tracks[0].cut
 
         # First, check for a simple scenario: just a single cut with padding.
         # When that is the case, we don't have to instantiate a feature extractor,
         # because we are not performing any actual mixing.
         # That makes life simpler for the users who have a custom feature extractor,
         # but don't actually care about feature-domain mixing; just want to pad.
         if mixed and all(isinstance(t.cut, PaddingCut) for t in self.tracks[1:]):
             padding_val = self.tracks[1].cut.feat_value
-            feats = np.ones((self.num_frames, self.num_features)) * padding_val
-            feats[: first_cut.num_frames, :] = first_cut.load_features()
+            first_cut_feats = first_cut.load_features()
+            if first_cut_feats.ndim == 2:
+                # 2D features
+                feats = np.ones((self.num_frames, self.num_features)) * padding_val
+            else:
+                # 3D features
+                feats = (
+                    np.ones(
+                        (self.num_frames, self.num_features, first_cut_feats.shape[-1])
+                    )
+                    * padding_val
+                )
+            feats[: first_cut.num_frames, ...] = first_cut_feats
             return feats
 
         # When there is more than one "regular" cut, we will perform an actual mix.
 
         # First, we have to make sure that the reference energy levels are appropriate.
         # They might not be if the first track is a padding track.
         reference_feats = None
@@ -748,15 +787,16 @@
                     feats=feats,
                     snr=track.snr,
                     offset=track.offset,
                     sampling_rate=track.cut.sampling_rate,
                 )
             except NonPositiveEnergyError as e:
                 logging.warning(
-                    str(e) + f' MonoCut with id "{track.cut.id}" will not be mixed in.'
+                    str(e)
+                    + f' {type(track.cut).__name__} with id "{track.cut.id}" will not be mixed in.'
                 )
 
         if mixed:
             # Checking for some edge cases below.
             feats = mixer.mixed_feats
             # Note: The slicing below is a work-around for an edge-case
             #  when two cuts have durations that ended with 0.005 (e.g. 10.125 and 5.715)
@@ -778,20 +818,30 @@
                 "load_features() was called."
             )
             return feats
         else:
             return mixer.unmixed_feats
 
     @rich_exception_info
-    def load_audio(self, mixed: bool = True) -> Optional[np.ndarray]:
+    def load_audio(
+        self, mixed: bool = True, mono_downmix: bool = False
+    ) -> Optional[np.ndarray]:
         """
         Loads the audios of the source cuts and mix them on-the-fly.
 
-        :param mixed: When True (default), returns a mono mix of the underlying tracks.
-            Otherwise returns a numpy array with the number of channels equal to the number of tracks.
+        :param mixed: When True (default), returns a mix of the underlying tracks. This will
+            return a numpy array with shape ``(num_channels, num_samples)``, where ``num_channels``
+            is determined by the ``num_channels`` property of the MixedCut. Otherwise returns a
+            numpy array with the number of channels equal to the total number of channels
+            across all tracks in the MixedCut. For example, if it contains a MultiCut with 2
+            channels and a MonoCut with 1 channel, the returned array will have shape
+            ``(3, num_samples)``.
+        :param mono_downmix: If the MixedCut contains > 1 channels (for e.g. when one of its tracks
+            is a MultiCut), this parameter controls whether the returned array will be down-mixed
+            to a single channel. This down-mixing is done by summing the channels together.
         :return: A numpy ndarray with audio samples and with shape ``(num_channels, num_samples)``
         """
         if not self.has_recording:
             return None
         first_cut = self.tracks[0].cut
 
         # First, we have to make sure that the reference energy levels are appropriate.
@@ -829,21 +879,29 @@
                 mixer.add_to_mix(
                     audio=audio,
                     snr=track.snr,
                     offset=track.offset,
                 )
             except NonPositiveEnergyError as e:
                 logging.warning(
-                    f'{e} MonoCut with id "{track.cut.id}" will not be mixed in.'
+                    f'{e} {type(track.cut).__name__} with id "{track.cut.id}" will not be mixed in.'
                 )
 
+        # Flattening a MixedCut without MultiCut tracks has no effect
+        mono_downmix = mono_downmix and any(
+            track.type == "MultiCut" for track in self.tracks
+        )
+
+        # Flattening a MixedCut without mixed=True has no effect
+        mono_downmix = mono_downmix and mixed
+
         if mixed:
             # Off-by-one errors can happen during mixing due to imperfect float arithmetic and rounding;
             # we will fix them on-the-fly so that the manifest does not lie about the num_samples.
-            audio = mixer.mixed_audio
+            audio = mixer.mixed_mono_audio if mono_downmix else mixer.mixed_audio
             if audio.shape[1] - self.num_samples == 1:
                 audio = audio[:, : self.num_samples]
             if audio.shape[1] - self.num_samples == -1:
                 audio = np.concatenate((audio, audio[:, -1:]), axis=1)
             assert audio.shape[1] == self.num_samples, (
                 f"Inconsistent number of samples in a MixedCut: please report "
                 f"this issue at https://github.com/lhotse-speech/lhotse/issues "
@@ -915,15 +973,15 @@
 
     def compute_and_store_features(
         self,
         extractor: FeatureExtractor,
         storage: FeaturesWriter,
         augment_fn: Optional[AugmentFn] = None,
         mix_eagerly: bool = True,
-    ) -> Cut:
+    ) -> DataCut:
         """
         Compute the features from this cut, store them on disk, and create a new `MonoCut` object with the
         feature manifest attached. This cut has to be able to load audio.
 
         :param extractor: a ``FeatureExtractor`` instance used to compute the features.
         :param storage: a ``FeaturesWriter`` instance used to store the features.
         :param augment_fn: an optional callable used for audio augmentation.
@@ -931,14 +989,16 @@
             and mix them dynamically when loading the features.
             When True, mix the audio first and store the mixed features, returning a new ``MonoCut`` instance
             with the same ID. The returned ``MonoCut`` will not have a ``Recording`` attached.
         :return: a new ``MonoCut`` instance if ``mix_eagerly`` is True, or returns ``self``
             with each of the tracks containing the ``Features`` manifests.
         """
         if mix_eagerly:
+            from .mono import MonoCut
+
             features_info = extractor.extract_from_samples_and_store(
                 samples=self.load_audio(),
                 storage=storage,
                 sampling_rate=self.sampling_rate,
                 offset=0,
                 channel=0,
                 augment_fn=augment_fn,
@@ -994,15 +1054,15 @@
             of calling this method.
         """
         n_sups = len(self.supervisions)
         if n_sups == 0:
             if not add_empty:
                 return self
             first_non_padding_idx = [
-                idx for idx, t in enumerate(self.tracks) if isinstance(t.cut, MonoCut)
+                idx for idx, t in enumerate(self.tracks) if isinstance(t.cut, DataCut)
             ][0]
             new_tracks = [
                 fastcopy(
                     t,
                     cut=fastcopy(
                         t.cut,
                         supervisions=[
@@ -1086,39 +1146,112 @@
 
         The text fields are concatenated with a whitespace, and all other string fields
         (including IDs) are prefixed with "cat#" and concatenated with a hash symbol "#".
         This is also applied to ``custom`` fields. Fields with a ``None`` value are omitted.
 
         .. note:: If you're using individual tracks of a mixed cut, note that this transform
              drops all the supervisions in individual tracks and assigns the merged supervision
-             in the first :class:`.MonoCut` found in ``self.tracks``.
+             in the first :class:`.DataCut` found in ``self.tracks``.
 
         :param custom_merge_fn: a function that will be called to merge custom fields values.
             We expect ``custom_merge_fn`` to handle all possible custom keys.
             When not provided, we will treat all custom values as strings.
             It will be called roughly like:
             ``custom_merge_fn(custom_key, [s.custom[custom_key] for s in sups])``
         """
-        from .set import merge_supervisions
+        # "m" stands for merged in variable names below
+
+        if custom_merge_fn is not None:
+            # Merge custom fields with the user-provided function.
+            merge_custom = custom_merge_fn
+        else:
+            # Merge the string representations of custom fields.
+            merge_custom = lambda k, vs: merge_items_with_delimiter(map(str, vs))
+
+        sups = sorted(self.supervisions, key=lambda s: s.start)
+
+        if len(sups) <= 1:
+            return self
+
+        # the sampling rate is arbitrary, ensures there are no float precision errors
+        mstart = sups[0].start
+        mend = sups[-1].end
+        mduration = add_durations(mend, -mstart, sampling_rate=self.sampling_rate)
+
+        custom_keys = set(
+            k for s in sups if s.custom is not None for k in s.custom.keys()
+        )
+        alignment_keys = set(
+            k for s in sups if s.alignment is not None for k in s.alignment.keys()
+        )
+
+        if any(overlaps(s1, s2) for s1, s2 in zip(sups, sups[1:])) and any(
+            s.text is not None for s in sups
+        ):
+            warnings.warn(
+                "You are merging overlapping supervisions that have text transcripts. "
+                "The result is likely to be unusable if you are going to train speech "
+                f"recognition models (cut id: {self.id})."
+            )
 
-        return merge_supervisions(self, custom_merge_fn=custom_merge_fn)
+        msup = SupervisionSegment(
+            id=merge_items_with_delimiter(s.id for s in sups),
+            # Make merged recording_id is a mix of recording_ids.
+            recording_id=merge_items_with_delimiter(s.recording_id for s in sups),
+            start=mstart,
+            duration=mduration,
+            # Hardcode -1 to indicate no specific channel, as the supervisions might have
+            # come from different channels in their original recordings.
+            channel=-1,
+            text=" ".join(s.text for s in sups if s.text),
+            speaker=merge_items_with_delimiter(s.speaker for s in sups if s.speaker),
+            language=merge_items_with_delimiter(s.language for s in sups if s.language),
+            gender=merge_items_with_delimiter(s.gender for s in sups if s.gender),
+            custom={
+                k: merge_custom(
+                    k,
+                    (
+                        s.custom[k]
+                        for s in sups
+                        if s.custom is not None and k in s.custom
+                    ),
+                )
+                for k in custom_keys
+            },
+            alignment={
+                # Concatenate the lists of alignment units.
+                k: reduce(
+                    add,
+                    (
+                        s.alignment[k]
+                        for s in sups
+                        if s.alignment is not None and k in s.alignment
+                    ),
+                )
+                for k in alignment_keys
+            },
+        )
+
+        new_cut = self.drop_supervisions()
+        new_cut._first_non_padding_cut.supervisions = [msup]
+        return new_cut
 
     def filter_supervisions(
         self, predicate: Callable[[SupervisionSegment], bool]
     ) -> Cut:
         """
         Modify cut to store only supervisions accepted by `predicate`
 
         Example:
             >>> cut = cut.filter_supervisions(lambda s: s.id in supervision_ids)
             >>> cut = cut.filter_supervisions(lambda s: s.duration < 5.0)
             >>> cut = cut.filter_supervisions(lambda s: s.text is not None)
 
         :param predicate: A callable that accepts `SupervisionSegment` and returns bool
-        :return: a modified MonoCut
+        :return: a modified MixedCut
         """
         new_mixed_cut = fastcopy(
             self,
             tracks=[
                 fastcopy(track, cut=track.cut.filter_supervisions(predicate))
                 for track in self.tracks
             ],
@@ -1153,13 +1286,13 @@
             tracks=[
                 fastcopy(t, cut=t.cut.with_recording_path_prefix(path))
                 for t in self.tracks
             ],
         )
 
     @property
-    def _first_non_padding_cut(self) -> MonoCut:
+    def _first_non_padding_cut(self) -> DataCut:
         return self._first_non_padding_track.cut
 
     @property
     def _first_non_padding_track(self) -> MixTrack:
         return [t for t in self.tracks if not isinstance(t.cut, PaddingCut)][0]
```

### Comparing `lhotse-1.8.0/lhotse/cut/mono.py` & `lhotse-1.9.0/lhotse/cut/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass, field
 from functools import partial
 from math import isclose
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 import numpy as np
 import torch
@@ -30,34 +31,33 @@
     perturb_num_samples,
     rich_exception_info,
     uuid4,
 )
 
 
 @dataclass
-class MonoCut(Cut):
+class DataCut(Cut, metaclass=ABCMeta):
     """
-    :class:`~lhotse.cut.MonoCut` is a :class:`~lhotse.cut.Cut` of a single channel of
-    a :class:`~lhotse.audio.Recording`. In addition to Cut, it has a specified channel attribute. This is the most commonly used type of cut.
-
-    Please refer to the documentation of :class:`~lhotse.cut.Cut` to learn more about using cuts.
+    :class:`~lhotse.cut.DataCut` is a base class for cuts that point to actual audio data.
+    It can be either a :class:`~lhotse.cut.MonoCut` or a :class:`~lhotse.cut.MultiCut`.
+    This is as opposed to :class:`~lhotse.cut.MixedCut`, which is simply an operation on
+    a collection of cuts.
 
     See also:
 
-        - :class:`lhotse.cut.Cut`
-        - :class:`lhotse.cut.MixedCut`
-        - :class:`lhotse.cut.CutSet`
+        - :class:`lhotse.cut.MonoCut`
+        - :class:`lhotse.cut.MultiCut`
     """
 
     id: str
 
     # Begin and duration are needed to specify which chunk of features/recording to load.
     start: Seconds
     duration: Seconds
-    channel: int
+    channel: Union[int, List[int]]
 
     # Supervisions that will be used as targets for model training later on. They don't have to cover the whole
     # cut duration. They also might overlap.
     supervisions: List[SupervisionSegment] = field(default_factory=list)
 
     # The features can span longer than the actual cut - the Features object "knows" its start and end time
     # within the underlying recording. We can expect the interval [begin, begin + duration] to be a subset of the
@@ -195,67 +195,47 @@
         )
 
     @property
     def num_features(self) -> Optional[int]:
         return self.features.num_features if self.has_features else None
 
     @property
+    @abstractmethod
+    def num_channels(self) -> Optional[int]:
+        ...
+
+    @property
     def features_type(self) -> Optional[str]:
         return self.features.type if self.has_features else None
 
     @property
     def sampling_rate(self) -> int:
         return (
             self.features.sampling_rate
             if self.has_features
             else self.recording.sampling_rate
         )
 
     @rich_exception_info
-    def load_features(self) -> Optional[np.ndarray]:
-        """
-        Load the features from the underlying storage and cut them to the relevant
-        [begin, duration] region of the current MonoCut.
-        """
-        if self.has_features:
-            feats = self.features.load(start=self.start, duration=self.duration)
-            # Note: we forgive off-by-one errors in the feature matrix frames
-            #       due to various hard-to-predict floating point arithmetic issues.
-            #       If needed, we will remove or duplicate the last frame to be
-            #       consistent with the manifests declared "num_frames".
-            if feats.shape[0] - self.num_frames == 1:
-                feats = feats[: self.num_frames, :]
-            elif feats.shape[0] - self.num_frames == -1:
-                feats = np.concatenate((feats, feats[-1:, :]), axis=0)
-            return feats
-        return None
+    @abstractmethod
+    def load_features(self, **kwargs) -> Optional[np.ndarray]:
+        ...
 
     @rich_exception_info
-    def load_audio(self) -> Optional[np.ndarray]:
-        """
-        Load the audio by locating the appropriate recording in the supplied RecordingSet.
-        The audio is trimmed to the [begin, end] range specified by the MonoCut.
-
-        :return: a numpy ndarray with audio samples, with shape (1 <channel>, N <samples>)
-        """
-        if self.has_recording:
-            return self.recording.load_audio(
-                channels=self.channel,
-                offset=self.start,
-                duration=self.duration,
-            )
-        return None
+    @abstractmethod
+    def load_audio(self, **kwargs) -> Optional[np.ndarray]:
+        ...
 
     def move_to_memory(
         self,
         audio_format: str = "flac",
         load_audio: bool = True,
         load_features: bool = True,
         load_custom: bool = True,
-    ) -> "MonoCut":
+    ) -> "Cut":
         """
         Load data (audio, features, or custom arrays) into memory and attach them
         to a copy of the manifest. This is useful when you want to store cuts together
         with the actual data in some binary format that enables sequential data reads.
 
         Audio is encoded with ``audio_format`` (compatible with ``torchaudio.save``),
         floating point features are encoded with lilcom, and other arrays are pickled.
@@ -312,15 +292,15 @@
     def attach_tensor(
         self,
         name: str,
         data: Union[np.ndarray, torch.Tensor],
         frame_shift: Optional[Seconds] = None,
         temporal_dim: Optional[int] = None,
         compressed: bool = False,
-    ) -> "MonoCut":
+    ) -> "Cut":
         """
         Attach a tensor to this MonoCut, described with an :class:`~lhotse.array.Array` manifest.
         The attached data is stored in-memory for later use, and can be accessed by
         calling ``cut.load_<name>()`` or :meth:`cut.load_custom`.
 
         This is useful if you want actions such as truncate/pad to propagate to the tensor, e.g.::
 
@@ -364,35 +344,35 @@
                     frame_shift=frame_shift,
                     temporal_dim=temporal_dim,
                     start=cpy.start,
                 ),
             )
         return cpy
 
-    def drop_features(self) -> "MonoCut":
-        """Return a copy of the current :class:`.MonoCut`, detached from ``features``."""
+    def drop_features(self) -> "DataCut":
+        """Return a copy of the current :class:`.DataCut`, detached from ``features``."""
         assert (
             self.has_recording
-        ), f"Cannot detach features from a MonoCut with no Recording (cut ID = {self.id})."
+        ), f"Cannot detach features from a DataCut with no Recording (cut ID = {self.id})."
         return fastcopy(self, features=None)
 
-    def drop_recording(self) -> "MonoCut":
-        """Return a copy of the current :class:`.MonoCut`, detached from ``recording``."""
+    def drop_recording(self) -> "DataCut":
+        """Return a copy of the current :class:`.DataCut`, detached from ``recording``."""
         assert (
             self.has_features
-        ), f"Cannot detach recording from a MonoCut with no Features (cut ID = {self.id})."
+        ), f"Cannot detach recording from a DataCut with no Features (cut ID = {self.id})."
         return fastcopy(self, recording=None)
 
-    def drop_supervisions(self) -> "MonoCut":
-        """Return a copy of the current :class:`.MonoCut`, detached from ``supervisions``."""
+    def drop_supervisions(self) -> "DataCut":
+        """Return a copy of the current :class:`.DataCut`, detached from ``supervisions``."""
         return fastcopy(self, supervisions=[])
 
     def fill_supervision(
         self, add_empty: bool = True, shrink_ok: bool = False
-    ) -> "MonoCut":
+    ) -> "DataCut":
         """
         Fills the whole duration of a cut with a supervision segment.
 
         If the cut has one supervision, its start is set to 0 and duration is set to ``cut.duration``.
         Note: this may either expand a supervision that was shorter than a cut, or shrink a supervision
         that exceeds the cut.
 
@@ -440,15 +420,15 @@
     def compute_and_store_features(
         self,
         extractor: FeatureExtractor,
         storage: FeaturesWriter,
         augment_fn: Optional[AugmentFn] = None,
         *args,
         **kwargs,
-    ) -> Cut:
+    ) -> "DataCut":
         """
         Compute the features from this cut, store them on disk, and attach a feature manifest to this cut.
         This cut has to be able to load audio.
 
         :param extractor: a ``FeatureExtractor`` instance used to compute the features.
         :param storage: a ``FeaturesWriter`` instance used to write the features to a storage.
         :param augment_fn: an optional callable used for audio augmentation.
@@ -469,36 +449,36 @@
         self,
         *,
         offset: Seconds = 0.0,
         duration: Optional[Seconds] = None,
         keep_excessive_supervisions: bool = True,
         preserve_id: bool = False,
         _supervisions_index: Optional[Dict[str, IntervalTree]] = None,
-    ) -> "MonoCut":
+    ) -> "DataCut":
         """
-        Returns a new MonoCut that is a sub-region of the current MonoCut.
+        Returns a new MonoCut that is a sub-region of the current DataCut.
 
         Note that no operation is done on the actual features or recording -
-        it's only during the call to :meth:`MonoCut.load_features` / :meth:`MonoCut.load_audio`
+        it's only during the call to :meth:`DataCut.load_features` / :meth:`DataCut.load_audio`
         when the actual changes happen (a subset of features/audio is loaded).
 
         .. hint::
 
-            To extend a cut by a fixed duration, use the :meth:`MonoCut.extend_by` method.
+            To extend a cut by a fixed duration, use the :meth:`DataCut.extend_by` method.
 
-        :param offset: float (seconds), controls the start of the new cut relative to the current MonoCut's start.
-            E.g., if the current MonoCut starts at 10.0, and offset is 2.0, the new start is 12.0.
-        :param duration: optional float (seconds), controls the duration of the resulting MonoCut.
+        :param offset: float (seconds), controls the start of the new cut relative to the current DataCut's start.
+            E.g., if the current DataCut starts at 10.0, and offset is 2.0, the new start is 12.0.
+        :param duration: optional float (seconds), controls the duration of the resulting DataCut.
             By default, the duration is (end of the cut before truncation) - (offset).
         :param keep_excessive_supervisions: bool. Since trimming may happen inside a SupervisionSegment,
             the caller has an option to either keep or discard such supervisions.
         :param preserve_id: bool. Should the truncated cut keep the same ID or get a new, random one.
         :param _supervisions_index: an IntervalTree; when passed, allows to speed up processing of Cuts with a very
             large number of supervisions. Intended as an internal parameter.
-        :return: a new MonoCut instance. If the current MonoCut is shorter than the duration, return None.
+        :return: a new MonoCut instance. If the current DataCut is shorter than the duration, return None.
         """
         assert (
             offset >= 0
         ), f"Offset for truncate must be non-negative (provided {offset})."
         new_start = max(
             add_durations(self.start, offset, sampling_rate=self.sampling_rate), 0
         )
@@ -570,33 +550,33 @@
     def extend_by(
         self,
         *,
         duration: Seconds,
         direction: str = "both",
         preserve_id: bool = False,
         pad_silence: bool = True,
-    ) -> "MonoCut":
+    ) -> Cut:
         """
-        Returns a new MonoCut that is an extended region of the current MonoCut by extending
+        Returns a new Cut (DataCut or MixedCut) that is an extended region of the current DataCut by extending
         the cut by a fixed duration in the specified direction.
 
         Note that no operation is done on the actual features or recording -
-        it's only during the call to :meth:`MonoCut.load_features` / :meth:`MonoCut.load_audio`
+        it's only during the call to :meth:`DataCut.load_features` / :meth:`DataCut.load_audio`
         when the actual changes happen (an extended version of features/audio is loaded).
 
         .. hint::
 
             This method extends a cut by a given duration, either to the left or to the right (or both), using
-            the "real" content of the recording that the cut is part of. For example, a MonoCut spanning
+            the "real" content of the recording that the cut is part of. For example, a DataCut spanning
             the region from 2s to 5s in a recording, when extended by 2s to the right, will now span
             the region from 2s to 7s in the same recording (provided the recording length exceeds 7s).
             If the recording is shorter, additional silence will be padded to achieve the desired duration
             by default. This behavior can be changed by setting ``pad_silence=False``.
-            Also see :meth:`MonoCut.pad` which pads a cut "to" a specified length.
-            To "truncate" a cut, use :meth:`MonoCut.truncate`.
+            Also see :meth:`DataCut.pad` which pads a cut "to" a specified length.
+            To "truncate" a cut, use :meth:`DataCut.truncate`.
 
         .. hint::
 
             If `pad_silence` is set to False, then the cut will be extended only as much as allowed
             within the recording's boundary.
 
         .. hint::
@@ -741,26 +721,26 @@
             num_samples=num_samples,
             pad_feat_value=pad_feat_value,
             direction=direction,
             preserve_id=preserve_id,
             pad_value_dict=pad_value_dict,
         )
 
-    def resample(self, sampling_rate: int, affix_id: bool = False) -> "MonoCut":
+    def resample(self, sampling_rate: int, affix_id: bool = False) -> "DataCut":
         """
-        Return a new ``MonoCut`` that will lazily resample the audio while reading it.
+        Return a new ``DataCut`` that will lazily resample the audio while reading it.
         This operation will drop the feature manifest, if attached.
         It does not affect the supervision.
 
         :param sampling_rate: The new sampling rate.
         :param affix_id: Should we modify the ID (useful if both versions of the same
             cut are going to be present in a single manifest).
-        :return: a modified copy of the current ``MonoCut``.
+        :return: a modified copy of the current ``DataCut``.
         """
-        assert self.has_recording, "Cannot resample a MonoCut without Recording."
+        assert self.has_recording, "Cannot resample a DataCut without Recording."
         custom = self.custom
         if isinstance(custom, dict) and any(
             isinstance(v, Recording) for v in custom.values()
         ):
             custom = {
                 k: v.resample(sampling_rate) if isinstance(v, Recording) else v
                 for k, v in custom.items()
@@ -770,33 +750,33 @@
             self,
             id=f"{self.id}_rs{sampling_rate}" if affix_id else self.id,
             recording=self.recording.resample(sampling_rate),
             features=None,
             custom=custom,
         )
 
-    def perturb_speed(self, factor: float, affix_id: bool = True) -> "MonoCut":
+    def perturb_speed(self, factor: float, affix_id: bool = True) -> "DataCut":
         """
-        Return a new ``MonoCut`` that will lazily perturb the speed while loading audio.
+        Return a new ``DataCut`` that will lazily perturb the speed while loading audio.
         The ``num_samples``, ``start`` and ``duration`` fields are updated to reflect the
         shrinking/extending effect of speed.
         We are also updating the time markers of the underlying ``Recording`` and the supervisions.
 
         :param factor: The speed will be adjusted this many times (e.g. factor=1.1 means 1.1x faster).
         :param affix_id: When true, we will modify the ``MonoCut.id`` field
             by affixing it with "_sp{factor}".
-        :return: a modified copy of the current ``MonoCut``.
+        :return: a modified copy of the current ``DataCut``.
         """
         # Pre-conditions
         assert (
             self.has_recording
-        ), "Cannot perturb speed on a MonoCut without Recording."
+        ), "Cannot perturb speed on a DataCut without Recording."
         if self.has_features:
             logging.warning(
-                "Attempting to perturb speed on a MonoCut that references pre-computed features. "
+                "Attempting to perturb speed on a DataCut that references pre-computed features. "
                 "The feature manifest will be detached, as we do not support feature-domain "
                 "speed perturbation."
             )
             self.features = None
         # Actual audio perturbation.
         recording_sp = self.recording.perturb_speed(factor=factor, affix_id=affix_id)
         # Match the supervision's start and duration to the perturbed audio.
@@ -820,43 +800,43 @@
             id=f"{self.id}_sp{factor}" if affix_id else self.id,
             recording=recording_sp,
             supervisions=supervisions_sp,
             duration=new_duration,
             start=new_start,
         )
 
-    def perturb_tempo(self, factor: float, affix_id: bool = True) -> "MonoCut":
+    def perturb_tempo(self, factor: float, affix_id: bool = True) -> "DataCut":
         """
-        Return a new ``MonoCut`` that will lazily perturb the tempo while loading audio.
+        Return a new ``DataCut`` that will lazily perturb the tempo while loading audio.
 
         Compared to speed perturbation, tempo preserves pitch.
         The ``num_samples``, ``start`` and ``duration`` fields are updated to reflect the
         shrinking/extending effect of speed.
         We are also updating the time markers of the underlying ``Recording`` and the supervisions.
 
         :param factor: The tempo will be adjusted this many times (e.g. factor=1.1 means 1.1x faster).
         :param affix_id: When true, we will modify the ``MonoCut.id`` field
             by affixing it with "_tp{factor}".
-        :return: a modified copy of the current ``MonoCut``.
+        :return: a modified copy of the current ``DataCut``.
         """
         # Pre-conditions
         assert (
             self.has_recording
-        ), "Cannot perturb speed on a MonoCut without Recording."
+        ), "Cannot perturb speed on a DataCut without Recording."
         if self.has_features:
             logging.warning(
-                "Attempting to perturb tempo on a MonoCut that references pre-computed features. "
+                "Attempting to perturb tempo on a DataCut that references pre-computed features. "
                 "The feature manifest will be detached, as we do not support feature-domain "
                 "speed perturbation."
             )
             self.features = None
         # Actual audio perturbation.
         recording_sp = self.recording.perturb_tempo(factor=factor, affix_id=affix_id)
         # Match the supervision's start and duration to the perturbed audio.
-        # Since SupervisionSegment "start" is relative to the MonoCut's, it's okay (and necessary)
+        # Since SupervisionSegment "start" is relative to the DataCut's, it's okay (and necessary)
         # to perturb it as well.
         supervisions_sp = [
             s.perturb_tempo(
                 factor=factor, sampling_rate=self.sampling_rate, affix_id=affix_id
             )
             for s in self.supervisions
         ]
@@ -872,30 +852,30 @@
             id=f"{self.id}_tp{factor}" if affix_id else self.id,
             recording=recording_sp,
             supervisions=supervisions_sp,
             duration=new_duration,
             start=new_start,
         )
 
-    def perturb_volume(self, factor: float, affix_id: bool = True) -> "MonoCut":
+    def perturb_volume(self, factor: float, affix_id: bool = True) -> "DataCut":
         """
-        Return a new ``MonoCut`` that will lazily perturb the volume while loading audio.
+        Return a new ``DataCut`` that will lazily perturb the volume while loading audio.
 
         :param factor: The volume will be adjusted this many times (e.g. factor=1.1 means 1.1x louder).
-        :param affix_id: When true, we will modify the ``MonoCut.id`` field
+        :param affix_id: When true, we will modify the ``DataCut.id`` field
             by affixing it with "_vp{factor}".
-        :return: a modified copy of the current ``MonoCut``.
+        :return: a modified copy of the current ``DataCut``.
         """
         # Pre-conditions
         assert (
             self.has_recording
-        ), "Cannot perturb volume on a MonoCut without Recording."
+        ), "Cannot perturb volume on a DataCut without Recording."
         if self.has_features:
             logging.warning(
-                "Attempting to perturb volume on a MonoCut that references pre-computed features. "
+                "Attempting to perturb volume on a DataCut that references pre-computed features. "
                 "The feature manifest will be detached, as we do not support feature-domain "
                 "volume perturbation."
             )
             self.features = None
         # Actual audio perturbation.
         recording_vp = self.recording.perturb_volume(factor=factor, affix_id=affix_id)
         # Match the supervision's id (and it's underlying recording id).
@@ -907,127 +887,42 @@
         return fastcopy(
             self,
             id=f"{self.id}_vp{factor}" if affix_id else self.id,
             recording=recording_vp,
             supervisions=supervisions_vp,
         )
 
+    @abstractmethod
     def reverb_rir(
         self,
         rir_recording: Optional["Recording"] = None,
         normalize_output: bool = True,
         early_only: bool = False,
         affix_id: bool = True,
         rir_channels: List[int] = [0],
-    ) -> Cut:
-        """
-        Return a new ``MonoCut`` that will convolve the audio with the provided impulse response.
-        If the `rir_recording` is multi-channel, the `rir_channels` argument determines which channels
-        will be used. By default, we use the first channel and return a MonoCut.
-
-        If no ``rir_recording`` is provided, we will generate an impulse response using a fast random
-        generator (https://arxiv.org/abs/2208.04101).
-
-        :param rir_recording: The impulse response to use for convolving.
-        :param normalize_output: When true, output will be normalized to have energy as input.
-        :param early_only: When true, only the early reflections (first 50 ms) will be used.
-        :param affix_id: When true, we will modify the ``MonoCut.id`` field
-            by affixing it with "_rvb".
-        :param rir_channels: The channels of the impulse response to use. First channel is used by default.
-            If multiple channels are specified, this will produce a MixedCut instead of a MonoCut.
-        :return: a modified copy of the current ``MonoCut``.
-        """
-        # Pre-conditions
-        assert (
-            self.has_recording
-        ), "Cannot apply reverberation on a MonoCut without Recording."
-        if self.has_features:
-            logging.warning(
-                "Attempting to reverberate a MonoCut that references pre-computed features. "
-                "The feature manifest will be detached, as we do not support feature-domain "
-                "reverberation."
-            )
-            self.features = None
-
-        assert rir_recording is None or all(
-            c < rir_recording.num_channels for c in rir_channels
-        ), "Invalid channel index in `rir_channels`."
-        if len(rir_channels) == 1 or (
-            rir_recording is not None and rir_recording.num_channels == 1
-        ):
-            # reverberation will return a MonoCut
-            recording_rvb = self.recording.reverb_rir(
-                rir_recording=rir_recording,
-                normalize_output=normalize_output,
-                early_only=early_only,
-                affix_id=affix_id,
-                rir_channels=rir_channels,
-            )
-            # Match the supervision's id (and it's underlying recording id).
-            supervisions_rvb = [
-                s.reverb_rir(
-                    affix_id=affix_id,
-                )
-                for s in self.supervisions
-            ]
-
-            return fastcopy(
-                self,
-                id=f"{self.id}_rvb" if affix_id else self.id,
-                recording=recording_rvb,
-                supervisions=supervisions_rvb,
-            )
-        else:
-            from .mixed import MixedCut, MixTrack
-
-            # we will return a MixedCut where each track represents the MonoCut convolved
-            # with a single channel of the RIR
-            new_tracks = [
-                MixTrack(
-                    cut=fastcopy(
-                        self,
-                        recording=self.recording.reverb_rir(
-                            rir_recording=rir_recording,
-                            normalize_output=normalize_output,
-                            early_only=early_only,
-                            affix_id=affix_id,
-                            rir_channels=[channel],
-                        ),
-                        supervisions=[
-                            s.reverb_rir(
-                                affix_id=affix_id,
-                            )
-                            for s in self.supervisions
-                        ],
-                    ),
-                    offset=0,
-                )
-                for channel in rir_channels
-            ]
-            return MixedCut(
-                id=f"{self.id}_rvb" if affix_id else self.id, tracks=new_tracks
-            )
+    ) -> "DataCut":
+        ...
 
     def map_supervisions(
         self, transform_fn: Callable[[SupervisionSegment], SupervisionSegment]
-    ) -> "MonoCut":
+    ) -> "DataCut":
         """
         Return a copy of the cut that has its supervisions transformed by ``transform_fn``.
 
         :param transform_fn: a function that modifies a supervision as an argument.
         :return: a modified MonoCut.
         """
         new_cut = fastcopy(
             self, supervisions=[s.map(transform_fn) for s in self.supervisions]
         )
         return new_cut
 
     def filter_supervisions(
         self, predicate: Callable[[SupervisionSegment], bool]
-    ) -> "MonoCut":
+    ) -> "DataCut":
         """
         Return a copy of the cut that only has supervisions accepted by ``predicate``.
 
         Example::
 
             >>> cut = cut.filter_supervisions(lambda s: s.id in supervision_ids)
             >>> cut = cut.filter_supervisions(lambda s: s.duration < 5.0)
@@ -1037,69 +932,29 @@
         :return: a modified MonoCut
         """
         new_cut = fastcopy(
             self, supervisions=[s for s in self.supervisions if predicate(s)]
         )
         return new_cut
 
+    @abstractmethod
     def merge_supervisions(
-        self, custom_merge_fn: Optional[Callable[[str, Iterable[Any]], Any]] = None
-    ) -> "MonoCut":
-        """
-        Return a copy of the cut that has all of its supervisions merged into
-        a single segment.
-
-        The new start is the start of the earliest superivion, and the new duration
-        is a minimum spanning duration for all the supervisions.
-
-        The text fields are concatenated with a whitespace, and all other string fields
-        (including IDs) are prefixed with "cat#" and concatenated with a hash symbol "#".
-        This is also applied to ``custom`` fields. Fields with a ``None`` value are omitted.
-
-        :param custom_merge_fn: a function that will be called to merge custom fields values.
-            We expect ``custom_merge_fn`` to handle all possible custom keys.
-            When not provided, we will treat all custom values as strings.
-            It will be called roughly like:
-            ``custom_merge_fn(custom_key, [s.custom[custom_key] for s in sups])``
-        """
-        from .set import merge_supervisions
-
-        # "m" stands for merged in variable names below
-        return merge_supervisions(self, custom_merge_fn=custom_merge_fn)
+        self,
+        custom_merge_fn: Optional[Callable[[str, Iterable[Any]], Any]] = None,
+        **kwargs,
+    ) -> "DataCut":
+        ...
 
     @staticmethod
-    def from_dict(data: dict) -> "MonoCut":
-        from lhotse.serialization import deserialize_custom_field
-
-        # Remove "type" field if exists.
-        data.pop("type", None)
-
-        features = (
-            Features.from_dict(data.pop("features")) if "features" in data else None
-        )
-        recording = (
-            Recording.from_dict(data.pop("recording")) if "recording" in data else None
-        )
-        supervision_infos = data.pop("supervisions") if "supervisions" in data else []
-
-        if "custom" in data:
-            deserialize_custom_field(data["custom"])
-
-        if "type" in data:
-            data.pop("type")
-
-        return MonoCut(
-            **data,
-            features=features,
-            recording=recording,
-            supervisions=[SupervisionSegment.from_dict(s) for s in supervision_infos],
-        )
+    @abstractmethod
+    def from_dict(data: dict) -> "DataCut":
+        ...
 
-    def with_features_path_prefix(self, path: Pathlike) -> "MonoCut":
+    def with_features_path_prefix(self, path: Pathlike) -> "DataCut":
         if not self.has_features:
             return self
         return fastcopy(self, features=self.features.with_path_prefix(path))
 
-    def with_recording_path_prefix(self, path: Pathlike) -> "MonoCut":
+    def with_recording_path_prefix(self, path: Pathlike) -> "DataCut":
         if not self.has_recording:
             return self
         return fastcopy(self, recording=self.recording.with_path_prefix(path))
```

### Comparing `lhotse-1.8.0/lhotse/cut/padding.py` & `lhotse-1.9.0/lhotse/cut/padding.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,21 +59,29 @@
         return 0
 
     @property
     def supervisions(self):
         return []
 
     @property
+    def channel(self) -> int:
+        return 0
+
+    @property
     def has_features(self) -> bool:
         return self.num_frames is not None
 
     @property
     def has_recording(self) -> bool:
         return self.num_samples is not None
 
+    @property
+    def num_channels(self) -> int:
+        return 1
+
     def has(self, field: str) -> bool:
         if field == "recording":
             return self.has_recording
         elif field == "features":
             return self.has_features
         else:
             return self.custom is not None and field in self.custom
```

### Comparing `lhotse-1.8.0/lhotse/cut/set.py` & `lhotse-1.9.0/lhotse/cut/set.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import random
 import warnings
 from collections import Counter, defaultdict
 from concurrent.futures import Executor, ProcessPoolExecutor
 from functools import partial, reduce
 from itertools import chain, islice
 from math import ceil
-from operator import add
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     FrozenSet,
     Iterable,
@@ -32,16 +31,18 @@
 from intervaltree import IntervalTree
 from tqdm.auto import tqdm
 from typing_extensions import Literal
 
 from lhotse.audio import RecordingSet, null_result_on_audio_loading_error
 from lhotse.augmentation import AugmentFn
 from lhotse.cut.base import Cut
+from lhotse.cut.data import DataCut
 from lhotse.cut.mixed import MixedCut, MixTrack
 from lhotse.cut.mono import MonoCut
+from lhotse.cut.multi import MultiCut
 from lhotse.cut.padding import PaddingCut
 from lhotse.features import FeatureExtractor, Features, FeatureSet
 from lhotse.features.base import StatsAccumulator, compute_global_stats
 from lhotse.features.io import FeaturesWriter, LilcomChunkyWriter
 from lhotse.lazy import AlgorithmMixin
 from lhotse.serialization import Serializable
 from lhotse.supervision import SupervisionSegment, SupervisionSet
@@ -252,14 +253,18 @@
         return {id_: cut for id_, cut in self.cuts.items() if isinstance(cut, MixedCut)}
 
     @property
     def simple_cuts(self) -> Dict[str, MonoCut]:
         return {id_: cut for id_, cut in self.cuts.items() if isinstance(cut, MonoCut)}
 
     @property
+    def multi_cuts(self) -> Dict[str, MultiCut]:
+        return {id_: cut for id_, cut in self.cuts.items() if isinstance(cut, MultiCut)}
+
+    @property
     def ids(self) -> Iterable[str]:
         return self.cuts.keys()
 
     @property
     def speakers(self) -> FrozenSet[str]:
         return frozenset(
             supervision.speaker for cut in self for supervision in cut.supervisions
@@ -315,32 +320,15 @@
                 features=features,
                 output_path=output_path,
                 random_ids=random_ids,
             )
 
     @staticmethod
     def from_dicts(data: Iterable[dict]) -> "CutSet":
-        def deserialize_one(raw_cut: dict) -> Cut:
-            cut_type = raw_cut.pop("type")
-            if cut_type == "MonoCut":
-                return MonoCut.from_dict(raw_cut)
-            if cut_type == "Cut":
-                warnings.warn(
-                    "Your manifest was created with Lhotse version earlier than v0.8, when MonoCut was called Cut. "
-                    "Please re-generate it with Lhotse v0.8 as it might stop working in a future version "
-                    "(using manifest.from_file() and then manifest.to_file() should be sufficient)."
-                )
-                return MonoCut.from_dict(raw_cut)
-            if cut_type == "MixedCut":
-                return MixedCut.from_dict(raw_cut)
-            raise ValueError(
-                f"Unexpected cut type during deserialization: '{cut_type}'"
-            )
-
-        return CutSet.from_cuts(deserialize_one(cut) for cut in data)
+        return CutSet.from_cuts(deserialize_cut(cut) for cut in data)
 
     @staticmethod
     def from_webdataset(
         path: Union[Pathlike, Sequence[Pathlike]], **wds_kwargs
     ) -> "CutSet":
         """
         Provides the ability to read Lhotse objects from a WebDataset tarball (or a
@@ -417,35 +405,35 @@
             output_dir / "recordings.jsonl.gz" if output_dir is not None else None
         ) as rw, SupervisionSet.open_writer(
             output_dir / "supervisions.jsonl.gz" if output_dir is not None else None
         ) as sw, FeatureSet.open_writer(
             output_dir / "features.jsonl.gz" if output_dir is not None else None
         ) as fw:
 
-            def save(mono_cut: MonoCut):
-                if mono_cut.has_recording and mono_cut.recording_id not in stored_rids:
-                    rw.write(mono_cut.recording)
-                    stored_rids.add(mono_cut.recording_id)
-                if mono_cut.has_features:
+            def save(cut: DataCut):
+                if cut.has_recording and cut.recording_id not in stored_rids:
+                    rw.write(cut.recording)
+                    stored_rids.add(cut.recording_id)
+                if cut.has_features:
                     # Note: we have no way of saying if features are unique,
                     #       so we will always write them.
-                    fw.write(mono_cut.features)
-                for sup in mono_cut.supervisions:
+                    fw.write(cut.features)
+                for sup in cut.supervisions:
                     if sup.id not in stored_sids:
                         # Supervisions inside cuts are relative to cuts start,
                         # so we correct the offset.
-                        sw.write(sup.with_offset(mono_cut.start))
+                        sw.write(sup.with_offset(cut.start))
                         stored_sids.add(sup.id)
 
             for cut in tqdm(self, desc="Decomposing cuts") if verbose else self:
-                if isinstance(cut, MonoCut):
+                if isinstance(cut, DataCut):
                     save(cut)
                 elif isinstance(cut, MixedCut):
                     for track in cut.tracks:
-                        if isinstance(track.cut, MonoCut):
+                        if isinstance(track.cut, DataCut):
                             save(track.cut)
 
         return rw.open_manifest(), sw.open_manifest(), fw.open_manifest()
 
     def describe(self) -> None:
         """
         Print a message describing details about the ``CutSet`` - the number of cuts and the
@@ -677,14 +665,15 @@
         )
 
     def trim_to_supervisions(
         self,
         keep_overlapping: bool = True,
         min_duration: Optional[Seconds] = None,
         context_direction: Literal["center", "left", "right", "random"] = "center",
+        keep_all_channels: bool = False,
         num_jobs: int = 1,
     ) -> "CutSet":
         """
         Return a new CutSet with Cuts that have identical spans as their supervisions.
 
         For example, the following cut::
 
@@ -705,25 +694,32 @@
                     Cut2
                |-----------|
                Sup1
                |-|
                     Sup2
                |-----------|
 
+        For the case of a multi-channel cut with multiple supervisions, we can either trim
+        while respecting the supervision channels (in which case output cut has the same channels
+        as the supervision) or ignore the channels (in which case output cut has the same channels
+        as the input cut).
+
         :param keep_overlapping: when ``False``, it will discard parts of other supervisions that overlap with the
             main supervision. In the illustration above, it would discard ``Sup2`` in ``Cut1`` and ``Sup1`` in ``Cut2``.
             In this mode, we guarantee that there will always be exactly one supervision per cut.
         :param min_duration: An optional duration in seconds; specifying this argument will extend the cuts
             that would have been shorter than ``min_duration`` with actual acoustic context in the recording/features.
             If there are supervisions present in the context, they are kept when ``keep_overlapping`` is true.
             If there is not enough context, the returned cut will be shorter than ``min_duration``.
             If the supervision segment is longer than ``min_duration``, the return cut will be longer.
         :param context_direction: Which direction should the cut be expanded towards to include context.
             The value of "center" implies equal expansion to left and right;
             random uniformly samples a value between "left" and "right".
+        :param keep_all_channels: If ``True``, the output cut will have the same channels as the input cut. By default,
+            the trimmed cut will have the same channels as the supervision.
         :param num_jobs: Number of parallel workers to process the cuts.
         :return: a ``CutSet``.
         """
 
         if num_jobs == 1:
             from lhotse.lazy import LazyFlattener, LazyMapper
 
@@ -732,28 +728,30 @@
                     LazyMapper(
                         self,
                         partial(
                             _trim_to_supervisions_single,
                             keep_overlapping=keep_overlapping,
                             min_duration=min_duration,
                             context_direction=context_direction,
+                            keep_all_channels=keep_all_channels,
                         ),
                     )
                 )
             )
 
         from lhotse.manipulation import split_parallelize_combine
 
         result = split_parallelize_combine(
             num_jobs,
             self,
             _trim_to_supervisions_single,
             keep_overlapping=keep_overlapping,
             min_duration=min_duration,
             context_direction=context_direction,
+            keep_all_channels=keep_all_channels,
         )
         return result
 
     def trim_to_unsupervised_segments(self) -> "CutSet":
         """
         Return a new CutSet with Cuts created from segments that have no supervisions (likely
         silence or noise).
@@ -780,14 +778,18 @@
             if supervisions[-1].end < cut.duration:
                 segments.append((supervisions[-1].end, cut.duration))
             # Create cuts from all found unsupervised segments.
             for start, end in segments:
                 cuts.append(cut.truncate(offset=start, duration=end - start))
         return CutSet.from_cuts(cuts)
 
+    @deprecated(
+        "Cut.mix_same_recording_channels will be removed in a future release. Please use "
+        "`combine_same_recording_channels()` instead."
+    )
     def mix_same_recording_channels(self) -> "CutSet":
         """
         Find cuts that come from the same recording and have matching start and end times, but
         represent different channels. Then, mix them together (in matching groups) and return
         a new ``CutSet`` that contains their mixes. This is useful for processing microphone array
         recordings.
 
@@ -807,14 +809,43 @@
                 "This operation is not applicable to CutSet's containing MixedCut's."
             )
         from cytoolz.itertoolz import groupby
 
         groups = groupby(lambda cut: (cut.recording.id, cut.start, cut.end), self)
         return CutSet.from_cuts(mix_cuts(cuts) for cuts in groups.values())
 
+    def combine_same_recording_channels(self) -> "CutSet":
+        """
+        Find cuts that come from the same recording and have matching start and end times, but
+        represent different channels. Then, combine them together to form MultiCut's and return
+        a new ``CutSet`` containing these MultiCut's. This is useful for processing microphone array
+        recordings.
+
+        It is intended to be used as the first operation after creating a new ``CutSet`` (but
+        might also work in other circumstances, e.g. if it was cut to windows first).
+
+        Example:
+            >>> ami = prepare_ami('path/to/ami')
+            >>> cut_set = CutSet.from_manifests(recordings=ami['train']['recordings'])
+            >>> multi_channel_cut_set = cut_set.combine_same_recording_channels()
+
+        In the AMI example, the ``multi_channel_cut_set`` will yield MultiCuts that hold all single-channel
+        Cuts together.
+
+        .. note:: See also :func:`CutSet.mix_same_recording_channels`, which is now deprecated.
+        """
+        if self.mixed_cuts or self.multi_cuts:
+            raise ValueError(
+                "This operation is not applicable to CutSet's containing MixedCut's or MultiCut's."
+            )
+        from cytoolz.itertoolz import groupby
+
+        groups = groupby(lambda cut: (cut.recording.id, cut.start, cut.end), self)
+        return CutSet.from_cuts(MultiCut.from_mono(cuts) for cuts in groups.values())
+
     def sort_by_duration(self, ascending: bool = False) -> "CutSet":
         """
         Sort the CutSet according to cuts duration and return the result. Descending by default.
         """
         return CutSet.from_cuts(
             sorted(self, key=(lambda cut: cut.duration), reverse=not ascending)
         )
@@ -837,15 +868,15 @@
 
         The interval tree can be efficiently queried for overlapping and/or enveloping segments.
         It helps speed up some operations on Cuts of very long recordings (1h+) that contain many
         supervisions.
 
         :param index_mixed_tracks: Should the tracks of MixedCut's be indexed as additional, separate entries.
         :param keep_ids: If specified, we will only index the supervisions with the specified IDs.
-        :return: a mapping from MonoCut ID to an interval tree of SupervisionSegments.
+        :return: a mapping from Cut ID to an interval tree of SupervisionSegments.
         """
         indexed = {}
         for cut in self:
             indexed.update(
                 cut.index_supervisions(
                     index_mixed_tracks=index_mixed_tracks, keep_ids=keep_ids
                 )
@@ -991,16 +1022,16 @@
         self,
         duration: Seconds,
         hop: Optional[Seconds] = None,
         keep_excessive_supervisions: bool = True,
         num_jobs: int = 1,
     ) -> "CutSet":
         """
-        Return a new ``CutSet``, made by traversing each ``MonoCut`` in windows of ``duration`` seconds by ``hop`` seconds and
-        creating new ``MonoCut`` out of them.
+        Return a new ``CutSet``, made by traversing each ``DataCut`` in windows of ``duration`` seconds by ``hop`` seconds and
+        creating new ``DataCut`` out of them.
 
         The last window might have a shorter duration if there was not enough audio, so you might want to
         use either ``.filter()`` or ``.pad()`` afterwards to obtain a uniform duration ``CutSet``.
 
         :param duration: Desired duration of the new cuts in seconds.
         :param hop: Shift between the windows in the new cuts in seconds.
         :param keep_excessive_supervisions: bool. When a cut is truncated in the middle of a supervision segment,
@@ -1378,28 +1409,27 @@
             Learn more about the ``Executor`` API at
             https://lhotse.readthedocs.io/en/latest/parallelism.html
         :param mix_eagerly: Related to how the features are extracted for ``MixedCut``
             instances, if any are present.
             When False, extract and store the features for each track separately,
             and mix them dynamically when loading the features.
             When True, mix the audio first and store the mixed features,
-            returning a new ``MonoCut`` instance with the same ID.
-            The returned ``MonoCut`` will not have a ``Recording`` attached.
+            returning a new ``DataCut`` instance with the same ID.
+            The returned ``DataCut`` will not have a ``Recording`` attached.
         :param progress_bar: Should a progress bar be displayed (automatically turned off
             for parallel computation).
         :return: Returns a new ``CutSet`` with ``Features`` manifests attached to the cuts.
         """
-        from cytoolz import identity
-
+        from lhotse.lazy import LazySlicer
         from lhotse.manipulation import combine
 
         # Pre-conditions and args setup
         progress = (
-            identity  # does nothing, unless we overwrite it with an actual prog bar
-        )
+            lambda x: x
+        )  # does nothing, unless we overwrite it with an actual prog bar
         if num_jobs is None:
             num_jobs = 1
         if num_jobs == 1 and executor is not None:
             logging.warning(
                 "Executor argument was passed but num_jobs set to 1: "
                 "we will ignore the executor and use non-parallel execution."
             )
@@ -1448,15 +1478,17 @@
             storage_path = Path(storage_path)
             storage_path.mkdir(parents=True, exist_ok=True)
 
             def sub_storage_path(idx: int) -> str:
                 return storage_path / f"feats-{idx}"
 
         # Parallel execution: prepare the CutSet splits
-        cut_sets = self.split(num_jobs, shuffle=True)
+        # We use LazySlicer to pick every k element out of n
+        # (e.g. with 2 jobs, job 1 picks every 0th elem, job 2 picks every 1st elem)
+        cut_sets = [CutSet(LazySlicer(self, k=i, n=num_jobs)) for i in range(num_jobs)]
 
         # Initialize the default executor if None was given
         if executor is None:
             executor = ProcessPoolExecutor(num_jobs)
 
         # Submit the chunked tasks to parallel workers.
         # Each worker runs the non-parallel version of this function inside.
@@ -1620,23 +1652,23 @@
                         start=cut.start,
                         duration=cut.duration,
                         type=extractor.name,
                         num_frames=feat_mat.shape[0],
                         num_features=feat_mat.shape[1],
                         frame_shift=frame_shift,
                         sampling_rate=cut.sampling_rate,
-                        channels=0,
+                        channels=cut.channel,
                         storage_type=feats_writer.name,
                         storage_path=str(feats_writer.storage_path),
                         storage_key=storage_key,
                     )
                     validate_features(feat_manifest, feats_data=feat_mat)
 
                     # Update the cut manifest.
-                    if isinstance(cut, MonoCut):
+                    if isinstance(cut, DataCut):
                         feat_manifest.recording_id = cut.recording_id
                         cut = fastcopy(cut, features=feat_manifest)
                     if isinstance(cut, MixedCut):
                         # If this was a mixed cut, we will just discard its
                         # recordings and create a new mono cut that has just
                         # the features attached.
                         feat_manifest.recording_id = cut.id
@@ -1889,19 +1921,19 @@
                 if not item.has_features or isinstance(item, PaddingCut):
                     manifest_writer.write(item)
                     continue
 
                 if isinstance(item, MixedCut):
                     cpy = fastcopy(item)
                     for t in cpy.tracks:
-                        if isinstance(t.cut, MonoCut):
+                        if isinstance(t.cut, DataCut):
                             t.cut.features = t.cut.features.copy_feats(writer=writer)
                     manifest_writer.write(cpy)
 
-                elif isinstance(item, MonoCut):
+                elif isinstance(item, DataCut):
                     cpy = fastcopy(item)
                     cpy.features = cpy.features.copy_feats(writer=writer)
                     manifest_writer.write(cpy)
 
                 else:
                     manifest_writer.write(item)
 
@@ -2039,14 +2071,35 @@
     assert reference_cut.sampling_rate == mixed_in_cut.sampling_rate, (
         f"Cannot mix cuts with different sampling rates "
         f"({reference_cut.sampling_rate} vs. "
         f"{mixed_in_cut.sampling_rate}). "
         f"Please resample the recordings first."
     )
 
+    # If either of the cuts is a MultiCut, we need to further check a few things.
+    if isinstance(reference_cut, MultiCut) or isinstance(mixed_in_cut, MultiCut):
+        # If both are MultiCuts, we need to check that they point to the same channels
+        if isinstance(reference_cut, MultiCut) and isinstance(mixed_in_cut, MultiCut):
+            assert (
+                reference_cut.channel == mixed_in_cut.channel
+            ), "Cannot mix MultiCuts with different channel ids."
+        # If only one of them is a MultiCut and the other is a MixedCut, we need to check
+        # all the tracks of the MixedCut to make sure they point to the same channels.
+        if isinstance(reference_cut, MixedCut) or isinstance(mixed_in_cut, MixedCut):
+            if isinstance(reference_cut, MixedCut):
+                mixed_cut = reference_cut
+                multi_cut = mixed_in_cut
+            else:
+                mixed_cut = mixed_in_cut
+                multi_cut = reference_cut
+            assert all(
+                track.type != "MultiCut" or track.cut.channel == multi_cut.channel
+                for track in mixed_cut.tracks
+            ), "Cannot mix a MultiCut with a MixedCut that contains MultiCuts with different channel ids."
+
     # Determine the ID of the result.
     if preserve_id is None:
         mixed_cut_id = str(uuid4())
     elif preserve_id == "left":
         mixed_cut_id = reference_cut.id
     elif preserve_id == "right":
         mixed_cut_id = mixed_in_cut.id
@@ -2059,15 +2112,15 @@
     # If the offset is larger than the left_cut duration, pad it.
     if offset > reference_cut.duration:
         reference_cut = reference_cut.pad(duration=offset)
 
     # When the left_cut is a MixedCut, take its existing tracks, otherwise create a new track.
     if isinstance(reference_cut, MixedCut):
         old_tracks = reference_cut.tracks
-    elif isinstance(reference_cut, (MonoCut, PaddingCut)):
+    elif isinstance(reference_cut, (DataCut, PaddingCut)):
         old_tracks = [MixTrack(cut=reference_cut)]
     else:
         raise ValueError(f"Unsupported type of cut in mix(): {type(reference_cut)}")
 
     # When the right_cut is a MixedCut, adapt its existing tracks with the new offset and snr,
     # otherwise create a new track.
     if isinstance(mixed_in_cut, MixedCut):
@@ -2088,15 +2141,15 @@
                     if snr is not None and track is not None
                     # When no SNR was specified whatsoever, use none.
                     else None
                 ),
             )
             for track in mixed_in_cut.tracks
         ]
-    elif isinstance(mixed_in_cut, (MonoCut, PaddingCut)):
+    elif isinstance(mixed_in_cut, (DataCut, PaddingCut)):
         new_tracks = [MixTrack(cut=mixed_in_cut, offset=offset, snr=snr)]
     else:
         raise ValueError(f"Unsupported type of cut in mix(): {type(reference_cut)}")
 
     return MixedCut(id=mixed_cut_id, tracks=old_tracks + new_tracks)
 
 
@@ -2112,15 +2165,15 @@
 ) -> Cut:
     """
     Return a new MixedCut, padded with zeros in the recording, and ``pad_feat_value`` in each feature bin.
 
     The user can choose to pad either to a specific `duration`; a specific number of frames `max_frames`;
     or a specific number of samples `num_samples`. The three arguments are mutually exclusive.
 
-    :param cut: MonoCut to be padded.
+    :param cut: DataCut to be padded.
     :param duration: The cut's minimal duration after padding.
     :param num_frames: The cut's total number of frames after padding.
     :param num_samples: The cut's total number of samples after padding.
     :param pad_feat_value: A float value that's used for padding the features.
         By default we assume a log-energy floor of approx. -23 (1e-10 after exp).
     :param direction: string, 'left', 'right' or 'both'. Determines whether the padding is added before or after
         the cut.
@@ -2331,16 +2384,16 @@
     output_path: Optional[Pathlike] = None,
     random_ids: bool = False,
 ) -> CutSet:
     """
     Create a :class:`.CutSet` from any combination of supervision, feature and recording manifests.
     At least one of ``recordings`` or ``features`` is required.
 
-    The created cuts will be of type :class:`.MonoCut`, even when the recordings have multiple channels.
-    The :class:`.MonoCut` boundaries correspond to those found in the ``features``, when available,
+    The created cuts will be of type :class:`.DataCut` (MonoCut for single-channel and MultiCut for multi-channel).
+    The :class:`.DataCut` boundaries correspond to those found in the ``features``, when available,
     otherwise to those found in the ``recordings``.
 
     When ``supervisions`` are provided, we'll be searching them for matching recording IDs
     and attaching to created cuts, assuming they are fully within the cut's time span.
 
     :param recordings: an optional :class:`~lhotse.audio.RecordingSet` manifest.
     :param supervisions: an optional :class:`~lhotse.supervision.SupervisionSet` manifest.
@@ -2361,60 +2414,77 @@
     if sup_ok:
         supervisions = supervisions.to_eager()  # must be eager to use .find()
     if feat_ok:
         # Case I: Features are provided.
         # Use features to determine the cut boundaries and attach recordings and supervisions as available.
         if rec_ok:
             recordings = recordings.to_eager()  # ensure it can be indexed with cut.id
-        cuts = CutSet.from_cuts(
-            MonoCut(
-                id=str(uuid4())
-                if random_ids
-                else f"{feats.recording_id}-{idx}-{feats.channels}",
-                start=feats.start,
-                duration=feats.duration,
-                channel=feats.channels,
-                features=feats,
-                recording=recordings[feats.recording_id] if rec_ok else None,
-                # The supervisions' start times are adjusted if the features object starts at time other than 0s.
-                supervisions=list(
-                    supervisions.find(
-                        recording_id=feats.recording_id,
-                        channel=feats.channels,
-                        start_after=feats.start,
-                        end_before=feats.end,
-                        adjust_offset=True,
+        cuts = []
+        for idx, feats in enumerate(features):
+            is_mono = (
+                feats.channels is None
+                or isinstance(feats.channels, int)
+                or len(feats.channels) == 1
+            )
+            if is_mono:
+                cls = MonoCut
+                channel = feats.channels if feats.channels is not None else 0
+            else:
+                cls = MultiCut
+                channel = list(feats.channels)
+            cuts.append(
+                cls(
+                    id=str(uuid4()) if random_ids else f"{feats.recording_id}-{idx}",
+                    start=feats.start,
+                    duration=feats.duration,
+                    channel=channel,
+                    features=feats,
+                    recording=recordings[feats.recording_id] if rec_ok else None,
+                    # The supervisions' start times are adjusted if the features object starts at time other than 0s.
+                    supervisions=list(
+                        supervisions.find(
+                            recording_id=feats.recording_id,
+                            channel=channel,
+                            start_after=feats.start,
+                            end_before=feats.end,
+                            adjust_offset=True,
+                        )
                     )
+                    if sup_ok
+                    else [],
                 )
-                if sup_ok
-                else [],
             )
-            for idx, feats in enumerate(features)
-        )
     else:
         # Case II: Recordings are provided (and features are not).
         # Use recordings to determine the cut boundaries.
-        cuts = CutSet.from_cuts(
-            MonoCut(
-                id=str(uuid4()) if random_ids else f"{recording.id}-{ridx}-{cidx}",
-                start=0,
-                duration=recording.duration,
-                channel=channel,
-                recording=recording,
-                supervisions=list(
-                    supervisions.find(recording_id=recording.id, channel=channel)
+        cuts = []
+        for ridx, recording in enumerate(recordings):
+            if recording.num_channels == 1:
+                cls = MonoCut
+                channel = recording.channel_ids[0]
+            else:
+                cls = MultiCut
+                channel = recording.channel_ids
+            cuts.append(
+                cls(
+                    id=str(uuid4()) if random_ids else f"{recording.id}-{ridx}",
+                    start=0,
+                    duration=recording.duration,
+                    channel=channel,
+                    recording=recording,
+                    supervisions=list(
+                        supervisions.find(
+                            recording_id=recording.id,
+                        )
+                    )
+                    if sup_ok
+                    else [],
                 )
-                if sup_ok
-                else [],
             )
-            for ridx, recording in enumerate(recordings)
-            # A single cut always represents a single channel. When a recording has multiple channels,
-            # we create a new cut for each channel separately.
-            for cidx, channel in enumerate(recording.channel_ids)
-        )
+    cuts = CutSet.from_cuts(cuts)
     if output_path is not None:
         cuts.to_file(output_path)
     return cuts
 
 
 def create_cut_set_lazy(
     output_path: Pathlike,
@@ -2494,28 +2564,39 @@
                     f"Mismatched recording_id: Features.recording_id == {feats.recording_id}, "
                     f"but Recording.id == '{rec.id}'"
                 )
                 sups, supervisions = _takewhile(
                     supervisions, lambda s: s.recording_id == feats.recording_id
                 )
                 sups = SupervisionSet.from_segments(sups)
-                cut = MonoCut(
-                    id=str(uuid4())
-                    if random_ids
-                    else f"{feats.recording_id}-{idx}-{feats.channels}",
+
+                is_mono = (
+                    feats.channels is None
+                    or isinstance(feats.channels, int)
+                    or len(feats.channels) == 1
+                )
+                if is_mono:
+                    cls = MonoCut
+                    channel = feats.channels if feats.channels is not None else 0
+                else:
+                    cls = MultiCut
+                    channel = list(feats.channels)
+
+                cut = cls(
+                    id=str(uuid4()) if random_ids else f"{feats.recording_id}-{idx}",
                     start=feats.start,
                     duration=feats.duration,
-                    channel=feats.channels,
+                    channel=channel,
                     features=feats,
                     recording=rec,
                     # The supervisions' start times are adjusted if the features object starts at time other than 0s.
                     supervisions=list(
                         sups.find(
                             recording_id=feats.recording_id,
-                            channel=feats.channels,
+                            channel=channel,
                             start_after=feats.start,
                             end_before=feats.end,
                             adjust_offset=True,
                         )
                     )
                     if sup_ok
                     else [],
@@ -2535,30 +2616,31 @@
             # because there might simply be no supervisions with that ID.
             # It's up to the user to make sure it's sorted properly.
             sups, supervisions = _takewhile(
                 supervisions, lambda s: s.recording_id == recording.id
             )
             sups = SupervisionSet.from_segments(sups)
 
-            # A single cut always represents a single channel. When a recording has multiple channels,
-            # we create a new cut for each channel separately.
-            for cidx, channel in enumerate(recording.channel_ids):
-                cut = MonoCut(
-                    id=str(uuid4()) if random_ids else f"{recording.id}-{ridx}-{cidx}",
-                    start=0,
-                    duration=recording.duration,
-                    channel=channel,
-                    recording=recording,
-                    supervisions=list(
-                        sups.find(recording_id=recording.id, channel=channel)
-                    )
-                    if sup_ok
-                    else [],
-                )
-                writer.write(cut)
+            if recording.num_channels == 1:
+                cls = MonoCut
+                channel = recording.channel_ids[0]
+            else:
+                cls = MultiCut
+                channel = recording.channel_ids
+            cut = cls(
+                id=str(uuid4()) if random_ids else f"{recording.id}-{ridx}",
+                start=0,
+                duration=recording.duration,
+                channel=channel,
+                recording=recording,
+                supervisions=list(sups.find(recording_id=recording.id))
+                if sup_ok
+                else [],
+            )
+            writer.write(cut)
 
     return CutSet.from_jsonl_lazy(output_path)
 
 
 T = TypeVar("T")
 
 
@@ -2582,150 +2664,56 @@
                 break
 
     except StopIteration:
         pass
     return collected, iterable
 
 
-def merge_supervisions(
-    cut: Cut, custom_merge_fn: Optional[Callable[[str, Iterable[Any]], Any]] = None
-) -> Cut:
-    """
-    Return a copy of the cut that has all of its supervisions merged into
-    a single segment.
-
-    The new start is the start of the earliest superivion, and the new duration
-    is a minimum spanning duration for all the supervisions.
-
-    The text fields are concatenated with a whitespace, and all other string fields
-    (including IDs) are prefixed with "cat#" and concatenated with a hash symbol "#".
-    This is also applied to ``custom`` fields. Fields with a ``None`` value are omitted.
-
-    .. note:: If you're using individual tracks of a :class:`MixedCut`, note that this transform
-         drops all the supervisions in individual tracks and assigns the merged supervision
-         in the first :class:`.MonoCut` found in ``self.tracks``.
-
-    :param custom_merge_fn: a function that will be called to merge custom fields values.
-        We expect ``custom_merge_fn`` to handle all possible custom keys.
-        When not provided, we will treat all custom values as strings.
-        It will be called roughly like:
-        ``custom_merge_fn(custom_key, [s.custom[custom_key] for s in sups])``
-    """
-    # "m" stands for merged in variable names below
-
-    def merge(values: Iterable[str]) -> Optional[str]:
-        # e.g.
-        # values = ["1125-76840-0001", "1125-53670-0003"]
-        # return "cat#1125-76840-0001#1125-53670-0003"
-        values = list(values)
-        if len(values) == 0:
-            return None
-        if len(values) == 1:
-            return values[0]
-        return "#".join(chain(["cat"], values))
-
-    if custom_merge_fn is not None:
-        # Merge custom fields with the user-provided function.
-        merge_custom = custom_merge_fn
-    else:
-        # Merge the string representations of custom fields.
-        merge_custom = lambda k, vs: merge(map(str, vs))
-
-    if isinstance(cut, PaddingCut):
-        return cut
-
-    sups = sorted(cut.supervisions, key=lambda s: s.start)
-
-    if len(sups) <= 1:
-        return cut
-
-    # the sampling rate is arbitrary, ensures there are no float precision errors
-    mstart = sups[0].start
-    mend = sups[-1].end
-    mduration = add_durations(mend, -mstart, sampling_rate=cut.sampling_rate)
-
-    custom_keys = set(k for s in sups if s.custom is not None for k in s.custom.keys())
-    alignment_keys = set(
-        k for s in sups if s.alignment is not None for k in s.alignment.keys()
-    )
-
-    if any(overlaps(s1, s2) for s1, s2 in zip(sups, sups[1:])) and any(
-        s.text is not None for s in sups
-    ):
+def deserialize_cut(raw_cut: dict) -> Cut:
+    cut_type = raw_cut.pop("type")
+    if cut_type == "MonoCut":
+        return MonoCut.from_dict(raw_cut)
+    if cut_type == "MultiCut":
+        return MultiCut.from_dict(raw_cut)
+    if cut_type == "PaddingCut":
+        return PaddingCut.from_dict(raw_cut)
+    if cut_type == "Cut":
         warnings.warn(
-            "You are merging overlapping supervisions that have text transcripts. "
-            "The result is likely to be unusable if you are going to train speech "
-            f"recognition models (cut id: {cut.id})."
-        )
-
-    is_mixed = isinstance(cut, MixedCut)
-
-    msup = SupervisionSegment(
-        id=merge(s.id for s in sups),
-        # For MixedCut, make merged recording_id is a mix of recording_ids.
-        # For MonoCut, the recording_id is always the same.
-        recording_id=merge(s.recording_id for s in sups)
-        if is_mixed
-        else sups[0].recording_id,
-        start=mstart,
-        duration=mduration,
-        # For MixedCut, hardcode -1 to indicate no specific channel,
-        # as the supervisions might have come from different channels
-        # in their original recordings.
-        # For MonoCut, the channel is always the same.
-        channel=-1 if is_mixed else sups[0].channel,
-        text=" ".join(s.text for s in sups if s.text),
-        speaker=merge(s.speaker for s in sups if s.speaker),
-        language=merge(s.language for s in sups if s.language),
-        gender=merge(s.gender for s in sups if s.gender),
-        custom={
-            k: merge_custom(
-                k, (s.custom[k] for s in sups if s.custom is not None and k in s.custom)
-            )
-            for k in custom_keys
-        },
-        alignment={
-            # Concatenate the lists of alignment units.
-            k: reduce(
-                add,
-                (
-                    s.alignment[k]
-                    for s in sups
-                    if s.alignment is not None and k in s.alignment
-                ),
-            )
-            for k in alignment_keys
-        },
-    )
-
-    if is_mixed:
-        new_cut = cut.drop_supervisions()
-        new_cut._first_non_padding_cut.supervisions = [msup]
-        return new_cut
-    else:
-        return fastcopy(cut, supervisions=[msup])
+            "Your manifest was created with Lhotse version earlier than v0.8, when MonoCut was called Cut. "
+            "Please re-generate it with Lhotse v0.8 as it might stop working in a future version "
+            "(using manifest.from_file() and then manifest.to_file() should be sufficient)."
+        )
+        return MonoCut.from_dict(raw_cut)
+    if cut_type == "MixedCut":
+        return MixedCut.from_dict(raw_cut)
+    raise ValueError(f"Unexpected cut type during deserialization: '{cut_type}'")
 
 
 def _cut_into_windows_single(
     cuts: CutSet, duration, hop, keep_excessive_supervisions
 ) -> CutSet:
     return cuts.cut_into_windows(
         duration=duration,
         hop=hop,
         keep_excessive_supervisions=keep_excessive_supervisions,
     ).to_eager()
 
 
 def _trim_to_supervisions_single(
-    cuts: CutSet, keep_overlapping, min_duration, context_direction
+    cuts: CutSet,
+    keep_overlapping,
+    min_duration,
+    context_direction,
+    keep_all_channels,
 ) -> CutSet:
     return cuts.trim_to_supervisions(
         keep_overlapping=keep_overlapping,
         min_duration=min_duration,
         context_direction=context_direction,
+        keep_all_channels=keep_all_channels,
     ).to_eager()
 
 
 def _add_recording_path_prefix_single(cut, path):
     return cut.with_recording_path_prefix(path)
```

### Comparing `lhotse-1.8.0/lhotse/dataset/__init__.py` & `lhotse-1.9.0/lhotse/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/collation.py` & `lhotse-1.9.0/lhotse/dataset/collation.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/cut_transforms/concatenate.py` & `lhotse-1.9.0/lhotse/dataset/cut_transforms/concatenate.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/cut_transforms/extra_padding.py` & `lhotse-1.9.0/lhotse/dataset/cut_transforms/extra_padding.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/cut_transforms/mix.py` & `lhotse-1.9.0/lhotse/dataset/cut_transforms/mix.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/cut_transforms/perturb_speed.py` & `lhotse-1.9.0/lhotse/dataset/cut_transforms/perturb_speed.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/cut_transforms/perturb_tempo.py` & `lhotse-1.9.0/lhotse/dataset/cut_transforms/perturb_tempo.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/cut_transforms/perturb_volume.py` & `lhotse-1.9.0/lhotse/dataset/cut_transforms/perturb_volume.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/cut_transforms/reverberate.py` & `lhotse-1.9.0/lhotse/dataset/cut_transforms/reverberate.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/dataloading.py` & `lhotse-1.9.0/lhotse/dataset/dataloading.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/diarization.py` & `lhotse-1.9.0/lhotse/dataset/diarization.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/input_strategies.py` & `lhotse-1.9.0/lhotse/dataset/input_strategies.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/iterable_dataset.py` & `lhotse-1.9.0/lhotse/dataset/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/base.py` & `lhotse-1.9.0/lhotse/dataset/sampling/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,14 +507,17 @@
     stats_per_epoch: Dict[int, EpochDiagnostics] = None
 
     def __post_init__(self):
         if self.stats_per_epoch is None:
             self.stats_per_epoch = {}
             self.set_epoch(self.current_epoch)
 
+    def reset_current_epoch(self) -> None:
+        self.stats_per_epoch[self.current_epoch] = EpochDiagnostics(self.current_epoch)
+
     def set_epoch(self, epoch: int) -> None:
         self.current_epoch = epoch
         if epoch not in self.stats_per_epoch:
             self.stats_per_epoch[epoch] = EpochDiagnostics(epoch=epoch)
 
     def advance_epoch(self) -> None:
         self.set_epoch(self.current_epoch + 1)
```

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/bucketing.py` & `lhotse-1.9.0/lhotse/dataset/sampling/bucketing.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,19 @@
 
         super().load_state_dict(state_dict)
 
     def __iter__(self) -> "BucketingSampler":
         # Restored state with load_state_dict()? Skip resetting.
         if self._just_restored_state:
             return self
+        # Why reset the current epoch?
+        # Either we are iterating the epoch for the first time and it's a no-op,
+        # or we are iterating the same epoch again, in which case setting more steps
+        # than are actually available per epoch would have broken the checkpoint restoration.
+        self.diagnostics.reset_current_epoch()
         # Reset the state to the beginning of the epoch.
         self.bucket_rng.seed(self.seed + self.epoch)
         for b in self.bucket_samplers:
             iter(b)
         self.depleted = [False] * self.num_buckets
         return self
```

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/cut_pairs.py` & `lhotse-1.9.0/lhotse/dataset/sampling/cut_pairs.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,19 @@
     def __iter__(self) -> "CutPairsSampler":
         """
         Prepare the dataset for iterating over a new epoch. Will shuffle the data if requested.
         """
         # Restored state with load_state_dict()? Skip resetting only this once.
         if self._just_restored_state:
             return self
+        # Why reset the current epoch?
+        # Either we are iterating the epoch for the first time and it's a no-op,
+        # or we are iterating the same epoch again, in which case setting more steps
+        # than are actually available per epoch would have broken the checkpoint restoration.
+        self.diagnostics.reset_current_epoch()
         # Reset the state to the beginning of the epoch.
         if self.shuffle:
             self.source_cuts.shuffle(self.seed + self.epoch)
             self.target_cuts.shuffle(self.seed + self.epoch)
         iter(self.source_cuts)
         iter(self.target_cuts)
         return self
```

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/data_source.py` & `lhotse-1.9.0/lhotse/dataset/sampling/data_source.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/dynamic.py` & `lhotse-1.9.0/lhotse/dataset/sampling/dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,14 +164,19 @@
         for _ in range(num_batches_to_iter):
             next(self)
         self._just_restored_state = True
 
     def __iter__(self) -> "DynamicCutSampler":
         if self._just_restored_state:
             return self
+        # Why reset the current epoch?
+        # Either we are iterating the epoch for the first time and it's a no-op,
+        # or we are iterating the same epoch again, in which case setting more steps
+        # than are actually available per epoch would have broken the checkpoint restoration.
+        self.diagnostics.reset_current_epoch()
         self.rng = random.Random(self.seed + self.epoch)
         # Initiate iteration
         self.cuts_iter = [iter(cs) for cs in self.cuts]
         # Optionally shuffle
         if self.shuffle:
             self.cuts_iter = [
                 # Important -- every shuffler has a copy of RNG seeded in the same way,
```

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/dynamic_bucketing.py` & `lhotse-1.9.0/lhotse/dataset/sampling/dynamic_bucketing.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,14 +190,19 @@
             next(self)
         self._just_restored_state = True
 
     def __iter__(self) -> "DynamicBucketingSampler":
         if self._just_restored_state:
             return self
         self.rng = random.Random(self.seed + self.epoch)
+        # Why reset the current epoch?
+        # Either we are iterating the epoch for the first time and it's a no-op,
+        # or we are iterating the same epoch again, in which case setting more steps
+        # than are actually available per epoch would have broken the checkpoint restoration.
+        self.diagnostics.reset_current_epoch()
         # Initiate iteration
         self.cuts_iter = [iter(cs) for cs in self.cuts]
         # Optionally shuffle
         if self.shuffle:
             self.cuts_iter = [
                 # Important -- every shuffler has a copy of RNG seeded in the same way,
                 # so that they are reproducible.
```

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/round_robin.py` & `lhotse-1.9.0/lhotse/dataset/sampling/round_robin.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/simple.py` & `lhotse-1.9.0/lhotse/dataset/sampling/simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,19 @@
     def __iter__(self) -> "SimpleCutSampler":
         """
         Prepare the dataset for iterating over a new epoch. Will shuffle the data if requested.
         """
         # Restored state with load_state_dict()? Skip resetting only this once.
         if self._just_restored_state:
             return self
+        # Why reset the current epoch?
+        # Either we are iterating the epoch for the first time and it's a no-op,
+        # or we are iterating the same epoch again, in which case setting more steps
+        # than are actually available per epoch would have broken the checkpoint restoration.
+        self.diagnostics.reset_current_epoch()
         # Reset the state to the beginning of the epoch.
         if self.shuffle:
             self.data_source.shuffle(self.seed + self.epoch)
         iter(self.data_source)
         return self
 
     def _next_batch(self) -> CutSet:
```

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/utils.py` & `lhotse-1.9.0/lhotse/dataset/sampling/utils.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/sampling/zip.py` & `lhotse-1.9.0/lhotse/dataset/sampling/zip.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/signal_transforms.py` & `lhotse-1.9.0/lhotse/dataset/signal_transforms.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/source_separation.py` & `lhotse-1.9.0/lhotse/dataset/source_separation.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/speech_recognition.py` & `lhotse-1.9.0/lhotse/dataset/speech_recognition.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/speech_synthesis.py` & `lhotse-1.9.0/lhotse/dataset/speech_synthesis.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/unsupervised.py` & `lhotse-1.9.0/lhotse/dataset/unsupervised.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/vad.py` & `lhotse-1.9.0/lhotse/dataset/vad.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/vis.py` & `lhotse-1.9.0/lhotse/dataset/vis.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/dataset/webdataset.py` & `lhotse-1.9.0/lhotse/dataset/webdataset.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/__init__.py` & `lhotse-1.9.0/lhotse/features/__init__.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/base.py` & `lhotse-1.9.0/lhotse/features/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
     def extract_from_samples_and_store(
         self,
         samples: np.ndarray,
         storage: FeaturesWriter,
         sampling_rate: int,
         offset: Seconds = 0,
-        channel: Optional[int] = None,
+        channel: Optional[Union[int, List[int]]] = None,
         augment_fn: Optional[AugmentFn] = None,
     ) -> "Features":
         """
         Extract the features from an array of audio samples in a full pipeline:
 
         * optional audio augmentation;
         * extract the features;
@@ -213,15 +213,15 @@
         ``MixedCut`` instances, which may be created from multiple recordings and channels.
 
         :param samples: a numpy ndarray with the audio samples.
         :param sampling_rate: integer sampling rate of ``samples``.
         :param storage: a ``FeaturesWriter`` object that will handle storing the feature matrices.
         :param offset: an offset in seconds for where to start reading the recording - when used for
             ``Cut`` feature extraction, must be equal to ``Cut.start``.
-        :param channel: an optional channel number to insert into ``Features`` manifest.
+        :param channel: an optional channel number(s) to insert into ``Features`` manifest.
         :param augment_fn: an optional ``WavAugmenter`` instance to modify the waveform before feature extraction.
         :return: a ``Features`` manifest item for the extracted feature matrix (it is not written to disk).
         """
         from lhotse.qa import validate_features
 
         if augment_fn is not None:
             samples = augment_fn(samples, sampling_rate)
@@ -696,15 +696,15 @@
                 )
                 return self
             return FeatureSet.from_features(self.features[-last:])
 
     def find(
         self,
         recording_id: str,
-        channel_id: int = 0,
+        channel_id: Union[int, List[int]] = 0,
         start: Seconds = 0.0,
         duration: Optional[Seconds] = None,
         leeway: Seconds = 0.05,
     ) -> Features:
         """
         Find and return a Features object that best satisfies the search criteria.
         Raise a KeyError when no such object is available.
@@ -763,15 +763,15 @@
                 lambda feat: feat.recording_id, self
             )
         return self._features_by_recording_id
 
     def load(
         self,
         recording_id: str,
-        channel_id: int = 0,
+        channel_id: Union[int, List[int]] = 0,
         start: Seconds = 0.0,
         duration: Optional[Seconds] = None,
     ) -> np.ndarray:
         """
         Find a Features object that best satisfies the search criteria and load the features as a numpy ndarray.
         Raise a KeyError when no such object is available.
         """
```

### Comparing `lhotse-1.8.0/lhotse/features/compression.py` & `lhotse-1.9.0/lhotse/features/compression.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/fbank.py` & `lhotse-1.9.0/lhotse/features/fbank.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/io.py` & `lhotse-1.9.0/lhotse/features/io.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/kaldi/extractors.py` & `lhotse-1.9.0/lhotse/features/kaldi/extractors.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/kaldi/layers.py` & `lhotse-1.9.0/lhotse/features/kaldi/layers.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/kaldifeat.py` & `lhotse-1.9.0/lhotse/features/kaldifeat.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/librosa_fbank.py` & `lhotse-1.9.0/lhotse/features/librosa_fbank.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/mfcc.py` & `lhotse-1.9.0/lhotse/features/mfcc.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/mixer.py` & `lhotse-1.9.0/lhotse/features/mixer.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             This value is adequate only for log space features. For non-log space features,
             e.g. energies, use either 0 or a small positive value like 1e-5.
         :param reference_energy: Optionally pass a reference energy value to compute SNRs against.
             This might be required when ``base_feats`` correspond to padding energies.
         """
         self.feature_extractor = feature_extractor
         self.tracks = [base_feats]
+        self.num_channels = 1 if base_feats.ndim == 2 else base_feats.shape[-1]
         self.gains = []
         self.frame_shift = frame_shift
         self.padding_value = padding_value
         self.dtype = self.tracks[0].dtype
 
         # Keep a pre-computed energy value of the features that we initialize the Mixer with;
         # it is required to compute gain ratios that satisfy SNR during the mix.
@@ -82,14 +83,27 @@
         result = self.tracks[0]
         for feats_to_add, gain in zip(self.tracks[1:], self.gains):
             result = self.feature_extractor.mix(
                 features_a=result, features_b=feats_to_add, energy_scaling_factor_b=gain
             )
         return result
 
+    def _get_dummy_array(self, num_frames: int) -> np.ndarray:
+        return np.full(
+            shape=(num_frames, self.num_features)
+            if self.num_channels == 1
+            else (
+                num_frames,
+                self.num_features,
+                self.num_channels,
+            ),
+            fill_value=self.padding_value,
+            dtype=self.dtype,
+        )
+
     def add_to_mix(
         self,
         feats: np.ndarray,
         sampling_rate: int,
         snr: Optional[Decibels] = None,
         offset: Seconds = 0.0,
     ):
@@ -103,14 +117,18 @@
         the start with low energy values.
         """
         if len(feats) == 0:
             return  # do nothing for empty arrays
 
         assert offset >= 0.0, "Negative offset in mixing is not supported."
 
+        assert (
+            self.tracks[0].ndim == feats.ndim
+        ), f"Feature dimensions mismatch in mixing"
+
         reference_feats = self.tracks[0]
         num_frames_offset = compute_num_frames(
             duration=offset, frame_shift=self.frame_shift, sampling_rate=sampling_rate
         )
         current_num_frames = reference_feats.shape[0]
         incoming_num_frames = feats.shape[0] + num_frames_offset
         mix_num_frames = max(current_num_frames, incoming_num_frames)
@@ -120,46 +138,37 @@
         # When the existing frames are less than what we anticipate after the mix,
         # we need to pad after the end of the existing features mixed so far.
         if current_num_frames < mix_num_frames:
             for idx in range(len(self.tracks)):
                 padded_track = np.vstack(
                     [
                         self.tracks[idx],
-                        self.padding_value
-                        * np.ones(
-                            (mix_num_frames - current_num_frames, self.num_features),
-                            dtype=self.dtype,
-                        ),
+                        self._get_dummy_array(mix_num_frames - current_num_frames),
                     ]
                 )
                 self.tracks[idx] = padded_track
 
         # When there is an offset, we need to pad before the start of the features we're adding.
         if offset > 0:
             feats_to_add = np.vstack(
                 [
-                    self.padding_value
-                    * np.ones((num_frames_offset, self.num_features), dtype=self.dtype),
+                    self._get_dummy_array(num_frames_offset),
                     feats_to_add,
                 ]
             )
 
         # When the features we're mixing in are shorter that the anticipated mix length,
         # we need to pad after their end.
         # Note: we're doing that inefficiently, as we potentially re-allocate numpy arrays twice,
         # during this padding and the offset padding before. If that's a bottleneck, we'll optimize.
         if incoming_num_frames < mix_num_frames:
             feats_to_add = np.vstack(
                 [
                     feats_to_add,
-                    self.padding_value
-                    * np.ones(
-                        (mix_num_frames - incoming_num_frames, self.num_features),
-                        dtype=self.dtype,
-                    ),
+                    self._get_dummy_array(mix_num_frames - incoming_num_frames),
                 ]
             )
 
         # When SNR is requested, find what gain is needed to satisfy the SNR
         gain = 1.0
         if snr is not None:
             # Compute the added signal energy before it was padded
```

### Comparing `lhotse-1.8.0/lhotse/features/opensmile.py` & `lhotse-1.9.0/lhotse/features/opensmile.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/features/spectrogram.py` & `lhotse-1.9.0/lhotse/features/spectrogram.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/kaldi.py` & `lhotse-1.9.0/lhotse/kaldi.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,23 @@
 
 
 def load_kaldi_data_dir(
     path: Pathlike,
     sampling_rate: int,
     frame_shift: Optional[Seconds] = None,
     map_string_to_underscores: Optional[str] = None,
+    use_reco2dur: bool = True,
     num_jobs: int = 1,
 ) -> Tuple[RecordingSet, Optional[SupervisionSet], Optional[FeatureSet]]:
     """
     Load a Kaldi data directory and convert it to a Lhotse RecordingSet and
     SupervisionSet manifests. For this to work, at least the wav.scp file must exist.
-    SupervisionSet is created only when a segments file exists.
+    SupervisionSet is created only when a segments file exists. reco2dur is used by
+    default when exists (to enforce reading the duration from the audio files
+    themselves, please set use_reco2dur = False.
     All the other files (text, utt2spk, etc.) are optional, and some of them might
     not be handled yet. In particular, feats.scp files are ignored.
 
     :param map_string_to_underscores: optional string, when specified, we will replace
         all instances of this string in SupervisonSegment IDs to underscores.
         This is to help with handling underscores in Kaldi
         (see :func:`.export_to_kaldi`). This is also done for speaker IDs.
@@ -75,18 +78,25 @@
     def fix_id(t: str) -> str:
         if map_string_to_underscores is None:
             return t
         return t.replace(map_string_to_underscores, "_")
 
     # must exist for RecordingSet
     recordings = load_kaldi_text_mapping(path / "wav.scp", must_exist=True)
-
-    with ProcessPoolExecutor(num_jobs) as ex:
-        dur_vals = ex.map(get_duration, recordings.values())
-    durations = dict(zip(recordings.keys(), dur_vals))
+    reco2dur = path / "reco2dur"
+    if use_reco2dur and reco2dur.is_file():
+        durations = load_kaldi_text_mapping(reco2dur, float_vals=True)
+        assert len(durations) == len(recordings), (
+            "The duration file reco2dur does not "
+            "have the same length as the  wav.scp file"
+        )
+    else:
+        with ProcessPoolExecutor(num_jobs) as ex:
+            dur_vals = ex.map(get_duration, recordings.values())
+        durations = dict(zip(recordings.keys(), dur_vals))
 
     recording_set = RecordingSet.from_recordings(
         Recording(
             id=recording_id,
             sources=[
                 AudioSource(
                     type="command" if path_or_cmd.endswith("|") else "file",
@@ -279,15 +289,15 @@
                 for channel in source.channels
             },
             path=output_dir / "wav.scp",
         )
         # segments
         save_kaldi_text_mapping(
             data={
-                sup.id: f"{sup.recording_id} {sup.start} {sup.end}"
+                sup.id: f"{sup.recording_id}_{sup.channel} {sup.start} {sup.end}"
                 for sup in supervisions
             },
             path=output_dir / "segments",
         )
         # reco2dur
         save_kaldi_text_mapping(
             data={
@@ -323,21 +333,23 @@
         save_kaldi_text_mapping(
             data={sup.id: sup.gender for sup in supervisions},
             path=output_dir / "utt2gender",
         )
 
 
 def load_kaldi_text_mapping(
-    path: Path, must_exist: bool = False
+    path: Path, must_exist: bool = False, float_vals: bool = False
 ) -> Dict[str, Optional[str]]:
     """Load Kaldi files such as utt2spk, spk2gender, text, etc. as a dict."""
     mapping = defaultdict(lambda: None)
     if path.is_file():
         with path.open() as f:
             mapping = dict(line.strip().split(maxsplit=1) for line in f)
+        if float_vals:
+            mapping = {key: float(val) for key, val in mapping.items()}
     elif must_exist:
         raise ValueError(f"No such file: {path}")
     return mapping
 
 
 def save_kaldi_text_mapping(data: Dict[str, Any], path: Path):
     """Save flat dicts to Kaldi files such as utt2spk, spk2gender, text, etc."""
@@ -367,23 +379,26 @@
             return audios
         elif Path(source.source).suffix == ".sph":
             # we will do this specifically using the sph2pipe because
             # ffmpeg does not support shorten compression, which is sometimes
             # used in the sph files
             audios = dict()
             for channel in source.channels:
-                audios[
-                    channel
-                ] = f"sph2pipe {source.source} -f wav -c {channel+1} -p | ffmpeg -threads 1 -i pipe:0 -ar {sampling_rate} -f wav -threads 1 pipe:1 |"
+                audios[channel] = (
+                    f"sph2pipe {source.source} -f wav -c {channel+1} -p | "
+                    "ffmpeg -threads 1"
+                    f" -i pipe:0 -ar {sampling_rate} -f wav -threads 1 pipe:1 |"
+                )
 
             return audios
         else:
             # Handles non-WAVE audio formats and multi-channel WAVEs.
             audios = dict()
             for channel in source.channels:
-                audios[
-                    channel
-                ] = f"ffmpeg -threads 1 -i {source.source} -ar {sampling_rate} -map_channel 0.0.{channel}  -f wav -threads 1 pipe:1 |"
+                audios[channel] = (
+                    f"ffmpeg -threads 1 -i {source.source} -ar {sampling_rate} "
+                    f"-map_channel 0.0.{channel}  -f wav -threads 1 pipe:1 |"
+                )
             return audios
 
     else:
         raise ValueError(f"Unknown AudioSource type: {source.type}")
```

### Comparing `lhotse-1.8.0/lhotse/lazy.py` & `lhotse-1.9.0/lhotse/lazy.py`

 * *Files 3% similar despite different names*

```diff
@@ -467,14 +467,44 @@
             raise AttributeError()
         return len(self.iterator) * self.times
 
     def __add__(self, other) -> "LazyIteratorChain":
         return LazyIteratorChain(self, other)
 
 
+class LazySlicer(ImitatesDict):
+    """
+    A wrapper over an iterable that enables selecting k-th element every n elements.
+    """
+
+    def __init__(self, iterator: Iterable, k: int, n: int) -> None:
+        self.iterator = iterator
+        assert (
+            k < n
+        ), f"When selecting k-th element every n elements, k must be less than n (got k={k} n={n})."
+        self.k = k
+        self.n = n
+
+    def __iter__(self):
+        for idx, item in enumerate(self.iterator):
+            if idx % self.n == self.k:
+                yield item
+
+    def __add__(self, other) -> "LazyIteratorChain":
+        return LazyIteratorChain(self, other)
+
+    def __len__(self) -> int:
+        raise NotImplementedError(
+            "LazySlicer does not support __len__ because it would require "
+            "iterating over the whole iterator, which is not possible in a lazy fashion. "
+            "If you really need to know the length, convert to eager mode first using "
+            "`.to_eager()`. Note that this will require loading the whole iterator into memory."
+        )
+
+
 def attach_repeat_idx_to_id(item: Any, idx: int) -> Any:
     if not hasattr(item, "id"):
         return item
     return fastcopy(item, id=f"{item.id}_repeat{idx}")
 
 
 def count_newlines_fast(path: Pathlike):
```

### Comparing `lhotse-1.8.0/lhotse/manifest.py` & `lhotse-1.9.0/lhotse/manifest.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/manipulation.py` & `lhotse-1.9.0/lhotse/manipulation.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/parallel.py` & `lhotse-1.9.0/lhotse/parallel.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/qa.py` & `lhotse-1.9.0/lhotse/qa.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     LHOTSE_AUDIO_DURATION_MISMATCH_TOLERANCE,
     Recording,
     RecordingSet,
 )
 from lhotse.cut import Cut, CutSet, MixedCut, MonoCut, PaddingCut
 from lhotse.features import Features, FeatureSet
 from lhotse.supervision import SupervisionSegment, SupervisionSet
-from lhotse.utils import compute_num_frames, overlaps
+from lhotse.utils import compute_num_frames, is_equal_or_contains, overlaps
 
 _VALIDATORS: Dict[str, Callable] = {}
 
 
 def validate(obj: Any, read_data: bool = False) -> None:
     """
     Validate a Lhotse manifest object.
@@ -61,21 +61,24 @@
     :param supervisions: a corresponding :class:`~lhotse.supervision.SupervisionSet` instance.
     :return: a pair of ``recordings`` and ``supervisions`` that were fixed:
         the original manifests are not modified.
     """
     recordings, supervisions = remove_missing_recordings_and_supervisions(
         recordings, supervisions
     )
-    if len(recordings) == 0 or len(supervisions) == 0:
-        raise ValueError(
-            "There are no matching recordings and supervisions in the input manifests."
-        )
+    # We don't use len(recordings) or len(supervisions) here because recordings and supervisions can be lazy.
+    assert (
+        len(frozenset(r.id for r in recordings)) > 0
+    ), "No recordings left after fixing the manifests."
+
     supervisions = trim_supervisions_to_recordings(recordings, supervisions)
-    if len(supervisions) == 0:
-        raise ValueError("All supervisions exceed the recordings duration.")
+    assert (
+        len(frozenset(s.id for s in supervisions)) > 0
+    ), "No supervisions left after fixing the manifests."
+
     return recordings, supervisions
 
 
 def validate_recordings_and_supervisions(
     recordings: Union[RecordingSet, Recording],
     supervisions: Union[SupervisionSet, SupervisionSegment],
     read_data: bool = False,
@@ -103,15 +106,15 @@
     # Errors
     for s in supervisions:
         r = recordings[s.recording_id]
         assert -1e-3 <= s.start <= s.end <= r.duration + 1e-3, (
             f"Supervision {s.id}: exceeded the bounds of its corresponding recording "
             f"(supervision spans [{s.start}, {s.end}]; recording spans [0, {r.duration}])"
         )
-        assert s.channel in r.channel_ids, (
+        assert is_equal_or_contains(r.channel_ids, s.channel), (
             f"Supervision {s.id}: channel {s.channel} does not exist in its corresponding Recording "
             f"(recording channels: {r.channel_ids})"
         )
     # Warnings
     recording_ids = frozenset(r.id for r in recordings)
     recording_ids_in_sups = frozenset(s.recording_id for s in supervisions)
     only_in_recordings = recording_ids - recording_ids_in_sups
@@ -146,19 +149,20 @@
     if only_in_recordings:
         recordings = recordings.filter(lambda r: r.id not in only_in_recordings)
         logging.warning(
             f"Removed {len(only_in_recordings)} recordings with no corresponding supervisions."
         )
     only_in_supervisions = recording_ids_in_sups - recording_ids
     if only_in_supervisions:
-        n_orig_sups = len(supervisions)
+        supervision_ids = frozenset(s.id for s in supervisions)
         supervisions = supervisions.filter(
             lambda s: s.recording_id not in only_in_supervisions
         )
-        n_removed_sups = n_orig_sups - len(supervisions)
+        supervision_ids_after = frozenset(s.id for s in supervisions)
+        n_removed_sups = len(supervision_ids) - len(supervision_ids_after)
         logging.warning(
             f"Removed {n_removed_sups} supervisions with no corresponding recordings "
             f"(for a total of {len(only_in_supervisions)} recording IDs)."
         )
     return recordings, supervisions
 
 
@@ -449,15 +453,17 @@
 
     # Catch errors in data preparation:
     # - more than one supervision for a given recording starts at 0 (in a given channel)
     supervisions._index_by_recording_id_and_cache()
     for rid, sups in supervisions._segments_by_recording_id.items():
         cntr_per_channel = defaultdict(int)
         for s in sups:
-            cntr_per_channel[s.channel] += int(s.start == 0)
+            # channel can be an int or a list (in which case we convert it to a tuple)
+            c = s.channel if isinstance(s.channel, int) else tuple(s.channel)
+            cntr_per_channel[c] += int(s.start == 0)
         for channel, count in cntr_per_channel.items():
             if count > 1:
                 logging.warning(
                     f"SupervisionSet contains {count} supervisions that start at 0 for recording {rid} "
                     f"(channel {channel}). Did you forget to set supervision start times?"
                 )
```

### Comparing `lhotse-1.8.0/lhotse/recipes/__init__.py` & `lhotse-1.9.0/lhotse/recipes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .bvcc import download_bvcc, prepare_bvcc
 from .callhome_egyptian import prepare_callhome_egyptian
 from .callhome_english import prepare_callhome_english
 from .cmu_arctic import download_cmu_arctic, prepare_cmu_arctic
 from .cmu_indic import download_cmu_indic, prepare_cmu_indic
 from .cmu_kids import prepare_cmu_kids
 from .commonvoice import prepare_commonvoice
+from .csj import prepare_csj
 from .cslu_kids import prepare_cslu_kids
 from .daily_talk import download_daily_talk, prepare_daily_talk
 from .dihard3 import prepare_dihard3
 from .eval2000 import prepare_eval2000
 from .fisher_english import prepare_fisher_english
 from .fisher_spanish import prepare_fisher_spanish
 from .gale_arabic import prepare_gale_arabic
```

### Comparing `lhotse-1.8.0/lhotse/recipes/adept.py` & `lhotse-1.9.0/lhotse/recipes/adept.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/aidatatang_200zh.py` & `lhotse-1.9.0/lhotse/recipes/aidatatang_200zh.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/aishell.py` & `lhotse-1.9.0/lhotse/recipes/aishell.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/aishell2.py` & `lhotse-1.9.0/lhotse/recipes/aishell2.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/aishell4.py` & `lhotse-1.9.0/lhotse/recipes/aishell4.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                         end = interval.maxTime
                         text = interval.mark
                         segment = SupervisionSegment(
                             id=f"{idx}-{spk_id}-{j}",
                             recording_id=idx,
                             start=start,
                             duration=round(end - start, 4),
-                            channel=0,
+                            channel=recording.channel_ids,
                             language="Chinese",
                             speaker=spk_id,
                             text=text.strip(),
                         )
                         supervisions.append(segment)
 
         recording_set = RecordingSet.from_recordings(recordings)
```

### Comparing `lhotse-1.8.0/lhotse/recipes/ali_meeting.py` & `lhotse-1.9.0/lhotse/recipes/ali_meeting.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                         end = interval.maxTime
                         text = interval.mark
                         segment = SupervisionSegment(
                             id=f"{session_id}-{spk_id}-{i}",
                             recording_id=recording.id,
                             start=start,
                             duration=round(end - start, 4),
-                            channel=0,
+                            channel=0 if mic == "near" else list(range(8)),
                             language="Chinese",
                             speaker=spk_id,
                             gender=gender,
                             text=text.strip(),
                         )
                         supervisions.append(segment)
```

### Comparing `lhotse-1.8.0/lhotse/recipes/ami.py` & `lhotse-1.9.0/lhotse/recipes/ami.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
         text = re.sub(r"[^A-Z0-9']+", " ", text)
         # remove multiple spaces
         text = re.sub(r"\s+", " ", text)
         # apply few exception for dashed phrases, Mm-Hmm, Uh-Huh, OK etc. those are frequent in AMI
         # and will be added to dictionary
         text = re.sub(r"MM HMM", "MM-HMM", text)
         text = re.sub(r"UH HUH", "UH-HUH", text)
-        text = re.sub(r"(\b)O K(\b)", "\g<1>OK\g<2>", text)
+        text = re.sub(r"(\b)O K(\b)", r"\g<1>OK\g<2>", text)
         return text
 
 
 # IHM and MDM audio requires grouping multiple channels of AudioSource into
 # one Recording.
 
 
@@ -546,15 +546,15 @@
             if duration > 0:
                 segments.append(
                     SupervisionSegment(
                         id=f"{recording.id}-{seg_idx}",
                         recording_id=recording.id,
                         start=seg_info.start_time,
                         duration=duration,
-                        channel=0,
+                        channel=recording.channel_ids,
                         language="English",
                         speaker=seg_info.speaker,
                         gender=seg_info.gender,
                         text=seg_info.text,
                     )
                 )
     return SupervisionSet.from_segments(segments)
```

### Comparing `lhotse-1.8.0/lhotse/recipes/aspire.py` & `lhotse-1.9.0/lhotse/recipes/aspire.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,14 +154,17 @@
                     id=f"{session}-{speaker}-{i:03d}",
                     recording_id=session,
                     start=seg.start,
                     duration=round(seg.end - seg.start, 4),
                     speaker=speaker,
                     text=seg.text,
                     language="English",
+                    channel=0
+                    if mic == "single"
+                    else recording_set[session].channel_ids,
                 )
                 for i, seg in enumerate(segs)
             ]
         supervision_set = SupervisionSet.from_segments(supervisions)
 
         recording_set, supervision_set = fix_manifests(recording_set, supervision_set)
         validate_recordings_and_supervisions(recording_set, supervision_set)
```

### Comparing `lhotse-1.8.0/lhotse/recipes/babel.py` & `lhotse-1.9.0/lhotse/recipes/babel.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/broadcast_news.py` & `lhotse-1.9.0/lhotse/recipes/broadcast_news.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/bvcc.py` & `lhotse-1.9.0/lhotse/recipes/bvcc.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/callhome_egyptian.py` & `lhotse-1.9.0/lhotse/recipes/callhome_egyptian.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/callhome_english.py` & `lhotse-1.9.0/lhotse/recipes/callhome_english.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/cmu_arctic.py` & `lhotse-1.9.0/lhotse/recipes/cmu_arctic.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/cmu_indic.py` & `lhotse-1.9.0/lhotse/recipes/cmu_indic.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/cmu_kids.py` & `lhotse-1.9.0/lhotse/recipes/cmu_kids.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/commonvoice.py` & `lhotse-1.9.0/lhotse/recipes/commonvoice.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/cslu_kids.py` & `lhotse-1.9.0/lhotse/recipes/cslu_kids.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/daily_talk.py` & `lhotse-1.9.0/lhotse/recipes/daily_talk.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/dihard3.py` & `lhotse-1.9.0/lhotse/recipes/dihard3.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/earnings21.py` & `lhotse-1.9.0/lhotse/recipes/earnings21.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/earnings22.py` & `lhotse-1.9.0/lhotse/recipes/earnings22.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/eval2000.py` & `lhotse-1.9.0/lhotse/recipes/eval2000.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/fisher_english.py` & `lhotse-1.9.0/lhotse/recipes/fisher_english.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
                 ):
                     if not tmp_supervisions:
                         err_sups += 1
                     for s in tmp_supervisions:
                         writer.write(s)
                     pbar.update()
         supervisions = writer.open_manifest()
-        if err_recos:
+        if err_sups:
             warnings.warn(
                 f"Out of {len(create_supervisions_input)} transcript files, "
                 f"{err_sups} had errors and were omitted."
             )
 
     recordings, supervisions = fix_manifests(recordings, supervisions)
     validate_recordings_and_supervisions(recordings, supervisions)
```

### Comparing `lhotse-1.8.0/lhotse/recipes/fisher_spanish.py` & `lhotse-1.9.0/lhotse/recipes/fisher_spanish.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/gale_arabic.py` & `lhotse-1.9.0/lhotse/recipes/gale_arabic.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/gale_mandarin.py` & `lhotse-1.9.0/lhotse/recipes/gale_mandarin.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/gigaspeech.py` & `lhotse-1.9.0/lhotse/recipes/gigaspeech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/heroico.py` & `lhotse-1.9.0/lhotse/recipes/heroico.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/hifitts.py` & `lhotse-1.9.0/lhotse/recipes/hifitts.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/icsi.py` & `lhotse-1.9.0/lhotse/recipes/icsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,15 +465,15 @@
             if duration > 0:
                 segments.append(
                     SupervisionSegment(
                         id=f"{recording.id}-{seg_idx}",
                         recording_id=recording.id,
                         start=seg_info.start_time,
                         duration=duration,
-                        channel=source.channels[0],
+                        channel=recording.channel_ids,
                         language="English",
                         speaker=seg_info.speaker,
                         gender=seg_info.gender,
                         text=seg_info.text,
                     )
                 )
     return SupervisionSet.from_segments(segments)
```

### Comparing `lhotse-1.8.0/lhotse/recipes/l2_arctic.py` & `lhotse-1.9.0/lhotse/recipes/l2_arctic.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/libricss.py` & `lhotse-1.9.0/lhotse/recipes/libricss.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from lhotse import (
     RecordingSet,
     SupervisionSegment,
     SupervisionSet,
     validate_recordings_and_supervisions,
 )
 from lhotse.audio import Recording
-from lhotse.utils import Pathlike
+from lhotse.utils import Pathlike, fastcopy
 
 # fmt: off
 # The following mapping is courtesy Zhuo Chen (Microsoft). It is not available in the original
 # LibriCSS dataset. It is useful for preparation of the data in the IHM setting, which consists
 # of 8 channels, each belonging to a different speaker. This mapping provides the correspondence
 # between the IHM channel and the speaker, which is then used in preparing the supervisions.
 SPK_TO_CHANNEL_MAP = {
@@ -137,17 +137,15 @@
     :param corpus_dir: Pathlike, the path to the extracted corpus.
     :param output_dir: Pathlike, the path where to write the manifests.
     :param type: str, the type of data to prepare ('mdm', 'sdm', 'ihm-mix', or 'ihm'). These settings
         are similar to the ones in AMI and ICSI recipes.
     :return: a Dict whose key is the dataset part, and the value is Dicts with the keys 'audio' and 'supervisions'.
 
     """
-    assert type in ["mdm", "ihm-mix", "ihm"]
-
-    manifests = {}
+    assert type in ["mdm", "sdm", "ihm-mix", "ihm"]
 
     corpus_dir = Path(corpus_dir)
     corpus_dir = (
         corpus_dir / "for_release" if corpus_dir.stem != "for_release" else corpus_dir
     )
 
     recordings = []
@@ -161,32 +159,40 @@
             audio_path = (
                 session / "clean" / "mix.wav"
                 if type == "ihm-mix"
                 else session / "clean" / "each_spk.wav"
                 if type == "ihm"
                 else session / "record" / "raw_recording.wav"
             )
-            recordings.append(
-                Recording.from_file(audio_path, recording_id=recording_id)
-            )
+            recording = Recording.from_file(audio_path, recording_id=recording_id)
+
+            if type == "sdm":
+                recordings.append(fastcopy(recording, channel_ids=[0]))
+            else:
+                recordings.append(recording)
+
             for idx, seg in enumerate(
                 parse_transcript(session / "transcription" / "meeting_info.txt")
             ):
+                if type == "ihm-mix" or type == "sdm":
+                    channel = 0
+                elif type == "ihm":
+                    channel = SPK_TO_CHANNEL_MAP[session.name][seg[2]]
+                else:
+                    channel = list(range(7))
                 segments.append(
                     SupervisionSegment(
                         id=f"{recording_id}-{idx}",
                         recording_id=recording_id,
                         start=seg[0],
                         duration=seg[1] - seg[0],
                         text=seg[4],
                         language="English",
                         speaker=seg[2],
-                        channel=SPK_TO_CHANNEL_MAP[session.name][seg[2]]
-                        if type == "ihm"
-                        else 0,
+                        channel=channel,
                     )
                 )
 
     supervisions = SupervisionSet.from_segments(segments)
     recordings = RecordingSet.from_recordings(recordings)
     validate_recordings_and_supervisions(recordings, supervisions)
```

### Comparing `lhotse-1.8.0/lhotse/recipes/librimix.py` & `lhotse-1.9.0/lhotse/recipes/librimix.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/librispeech.py` & `lhotse-1.9.0/lhotse/recipes/librispeech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/libritts.py` & `lhotse-1.9.0/lhotse/recipes/libritts.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/ljspeech.py` & `lhotse-1.9.0/lhotse/recipes/ljspeech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/magicdata.py` & `lhotse-1.9.0/lhotse/recipes/magicdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from lhotse import validate_recordings_and_supervisions
 from lhotse.audio import Recording, RecordingSet
 from lhotse.supervision import SupervisionSegment, SupervisionSet
 from lhotse.utils import Pathlike, urlretrieve_progress
 
 
 def text_normalize(line: str):
-    """
+    r"""
     Modified from https://github.com/wenet-e2e/wenet/blob/main/examples/multi_cn/s0/local/magicdata_data_prep.sh#L41
-     sed 's/！//g' | sed 's/？//g' |\
+    sed 's/！//g' | sed 's/？//g' |\
     sed 's/，//g' | sed 's/－//g' |\
     sed 's/：//g' | sed 's/；//g' |\
     sed 's/　//g' | sed 's/。//g' |\
     sed 's/`//g' | sed 's/,//g' |\
     sed 's/://g' | sed 's/?//g' |\
     sed 's/\///g' | sed 's/·//g' |\
     sed 's/\"//g' | sed 's/“//g' |\
```

### Comparing `lhotse-1.8.0/lhotse/recipes/mgb2.py` & `lhotse-1.9.0/lhotse/recipes/mgb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,16 +255,16 @@
         "|": " ",
     }
     trans_string = str.maketrans(eastern_to_western)
     return text.translate(trans_string)
 
 
 def remove_extra_space(text: str) -> str:
-    text = sub("\s+", " ", text)
-    text = sub("\s+\.\s+", ".", text)
+    text = sub(r"\s+", " ", text)
+    text = sub(r"\s+\.\s+", ".", text)
     return text
 
 
 def cleaning(text: str) -> str:
     text = remove_punctuations(text)
     text = east_to_west_num(text)
     text = remove_diacritics(text)
```

### Comparing `lhotse-1.8.0/lhotse/recipes/mls.py` & `lhotse-1.9.0/lhotse/recipes/mls.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/mobvoihotwords.py` & `lhotse-1.9.0/lhotse/recipes/mobvoihotwords.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/mtedx.py` & `lhotse-1.9.0/lhotse/recipes/mtedx.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/musan.py` & `lhotse-1.9.0/lhotse/recipes/musan.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/nsc.py` & `lhotse-1.9.0/lhotse/recipes/nsc.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/peoples_speech.py` & `lhotse-1.9.0/lhotse/recipes/peoples_speech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/primewords.py` & `lhotse-1.9.0/lhotse/recipes/primewords.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/rir_noise.py` & `lhotse-1.9.0/lhotse/recipes/rir_noise.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/spgispeech.py` & `lhotse-1.9.0/lhotse/recipes/spgispeech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/stcmds.py` & `lhotse-1.9.0/lhotse/recipes/stcmds.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/switchboard.py` & `lhotse-1.9.0/lhotse/recipes/switchboard.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/tal_asr.py` & `lhotse-1.9.0/lhotse/recipes/tal_asr.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/tal_csasr.py` & `lhotse-1.9.0/lhotse/recipes/tal_csasr.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/tedlium.py` & `lhotse-1.9.0/lhotse/recipes/tedlium.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/thchs_30.py` & `lhotse-1.9.0/lhotse/recipes/thchs_30.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/timit.py` & `lhotse-1.9.0/lhotse/recipes/timit.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/utils.py` & `lhotse-1.9.0/lhotse/recipes/utils.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/vctk.py` & `lhotse-1.9.0/lhotse/recipes/vctk.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/voxceleb.py` & `lhotse-1.9.0/lhotse/recipes/voxceleb.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/wenet_speech.py` & `lhotse-1.9.0/lhotse/recipes/wenet_speech.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/recipes/yesno.py` & `lhotse-1.9.0/lhotse/recipes/yesno.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         words = audio_path.stem.split("_")
         assert len(words) == 8
         assert set(words).union({"0", "1"}) == {"0", "1"}, f"words is: {words}"
 
         words = [word_map[w] for w in words]
         text = " ".join(words)
 
-        recording = Recording.from_file(audio_path)
+        recording = Recording.from_file(audio_path.absolute())
         recordings.append(recording)
 
         segment = SupervisionSegment(
             id=audio_path.stem,
             recording_id=audio_path.stem,
             start=0.0,
             duration=recording.duration,
```

### Comparing `lhotse-1.8.0/lhotse/serialization.py` & `lhotse-1.9.0/lhotse/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,29 +492,31 @@
     def to_file(self, path: Pathlike) -> None:
         store_manifest(self, path)
 
 
 def deserialize_item(data: dict) -> Any:
     # Figures out what type of manifest is being decoded with some heuristics
     # and returns a Lhotse manifest object rather than a raw dict.
-    from lhotse import Features, MonoCut, Recording, SupervisionSegment
+    from lhotse import Features, MonoCut, MultiCut, Recording, SupervisionSegment
     from lhotse.array import deserialize_array
     from lhotse.cut import MixedCut
 
     if "shape" in data or "array" in data:
         return deserialize_array(data)
     if "sources" in data:
         return Recording.from_dict(data)
     if "num_features" in data:
         return Features.from_dict(data)
     if "type" not in data:
         return SupervisionSegment.from_dict(data)
     cut_type = data.pop("type")
     if cut_type == "MonoCut":
         return MonoCut.from_dict(data)
+    if cut_type == "MultiCut":
+        return MultiCut.from_dict(data)
     if cut_type == "Cut":
         warnings.warn(
             "Your manifest was created with Lhotse version earlier than v0.8, when MonoCut was called Cut. "
             "Please re-generate it with Lhotse v0.8 as it might stop working in a future version "
             "(using manifest.from_file() and then manifest.to_file() should be sufficient)."
         )
         return MonoCut.from_dict(data)
```

### Comparing `lhotse-1.8.0/lhotse/supervision.py` & `lhotse-1.9.0/lhotse/supervision.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     add_durations,
     asdict_nonull,
     compute_num_samples,
     exactly_one_not_null,
     fastcopy,
     ifnone,
     index_by_id_and_check,
+    is_equal_or_contains,
     overspans,
     perturb_num_samples,
     split_manifest_lazy,
     split_sequence,
 )
 
 
@@ -47,15 +48,18 @@
 
     # Score is an optional aligner-specific measure of confidence.
     # A simple measure can be an average probability of "symbol" across
     # frames covered by the AlignmentItem.
     score: Optional[float] = None
 
     @staticmethod
-    def deserialize(data: list) -> "AlignmentItem":
+    def deserialize(data: Union[List, Dict]) -> "AlignmentItem":
+        if isinstance(data, dict):
+            # Support loading alignments stored in the format we had before Lhotse v1.8
+            return AlignmentItem(*list(data.values()))
         return AlignmentItem(*data)
 
     def serialize(self) -> list:
         return list(self)
 
     @property
     def end(self) -> Seconds:
@@ -114,15 +118,17 @@
 @dataclass
 class SupervisionSegment:
     """
     :class:`~lhotse.supervsion.SupervisionSegment` represents a time interval (segment) annotated with some
     supervision labels and/or metadata, such as the transcription, the speaker identity, the language, etc.
 
     Each supervision has unique ``id`` and always refers to a specific recording (via ``recording_id``)
-    and a specific ``channel`` (by default, 0).
+    and one or more ``channel`` (by default, 0). Note that multiple channels of the recording
+    may share the same supervision, in which case the ``channel`` field will be a list of integers.
+
     It's also characterized by the start time (relative to the beginning of a :class:`~lhotse.audio.Recording`
     or a :class:`~lhotse.cut.Cut`) and a duration, both expressed in seconds.
 
     The remaining fields are all optional, and their availability depends on specific corpora.
     Since it is difficult to predict all possible types of metadata, the ``custom`` field (a dict) can be used to
     insert types of supervisions that are not supported out of the box.
 
@@ -179,27 +185,36 @@
             ...         'phone': [
             ...             AlignmentItem(symbol='AY0', start=33.0, duration=0.6),
             ...             AlignmentItem(symbol='S', start=33.6, duration=0.4)
             ...         ]
             ...     }
             ... )
 
+        A supervision shared across multiple channels of a recording (e.g. a microphone array)::
+
+            >>> sup5 = SupervisionSegment(
+            ...     id='rec00001-sup00005', recording_id='rec00001',
+            ...     start=33.0, duration=1.0, channel=[0, 1],
+            ...     text="ice",
+            ...     speaker='Maryla Zechariah',
+            ... )
+
         Converting :class:`~lhotse.supervsion.SupervisionSegment` to a ``dict``::
 
             >>> sup0.to_dict()
             {'id': 'rec00001-sup00000', 'recording_id': 'rec00001', 'start': 0.5, 'duration': 5.0, 'channel': 0}
 
 
     """
 
     id: str
     recording_id: str
     start: Seconds
     duration: Seconds
-    channel: int = 0
+    channel: Union[int, List[int]] = 0
     text: Optional[str] = None
     language: Optional[str] = None
     speaker: Optional[str] = None
     gender: Optional[str] = None
     custom: Optional[Dict[str, Any]] = None
     alignment: Optional[Dict[str, List[AlignmentItem]]] = None
 
@@ -315,27 +330,30 @@
             self,
             id=f"{self.id}_vp{factor}" if affix_id else self.id,
             recording_id=f"{self.recording_id}_vp{factor}"
             if affix_id
             else self.recording_id,
         )
 
-    def reverb_rir(self, affix_id: bool = True) -> "SupervisionSegment":
+    def reverb_rir(
+        self, affix_id: bool = True, channel: Optional[Union[int, List[int]]] = None
+    ) -> "SupervisionSegment":
         """
         Return a ``SupervisionSegment`` with modified ids.
 
         :param affix_id: When true, we will modify the ``id`` and ``recording_id`` fields
             by affixing it with "_rvb".
         :return: a modified copy of the current ``SupervisionSegment``.
         """
 
         return fastcopy(
             self,
             id=f"{self.id}_rvb" if affix_id else self.id,
             recording_id=f"{self.recording_id}_rvb" if affix_id else self.recording_id,
+            channel=channel if channel is not None else self.channel,
         )
 
     def trim(self, end: Seconds, start: Seconds = 0) -> "SupervisionSegment":
         """
         Return an identical ``SupervisionSegment``, but ensure that ``self.start`` is not negative (in which case
         it's set to 0) and ``self.end`` does not exceed the ``end`` parameter. If a `start` is optionally
         provided, the supervision is trimmed from the left (note that start should be relative to the cut times).
@@ -665,16 +683,17 @@
         :param ctm_file: Path to output CTM file (will be created if not exists)
         :param type: Alignment type to write (default = `word`)
         """
         with open(ctm_file, "w") as f:
             for s in self:
                 if type in s.alignment:
                     for ali in s.alignment[type]:
+                        c = s.channel[0] if isinstance(s.channel, list) else s.channel
                         f.write(
-                            f"{s.recording_id} {s.channel} {ali.start:.02f} {ali.duration:.02f} {ali.symbol}\n"
+                            f"{s.recording_id} {c} {ali.start:.02f} {ali.duration:.02f} {ali.symbol}\n"
                         )
 
     def to_dicts(self) -> Iterable[dict]:
         return (s.to_dict() for s in self)
 
     def split(
         self, num_splits: int, shuffle: bool = False, drop_last: bool = False
@@ -813,15 +832,15 @@
         """
         segment_by_recording_id = self._index_by_recording_id_and_cache()
         return (
             # We only modify the offset - the duration remains the same, as we're only shifting the segment
             # relative to the Cut's start, and not truncating anything.
             segment.with_offset(-start_after) if adjust_offset else segment
             for segment in segment_by_recording_id.get(recording_id, [])
-            if (channel is None or segment.channel == channel)
+            if (channel is None or is_equal_or_contains(segment.channel, channel))
             and segment.start >= start_after - tolerance
             and (end_before is None or segment.end <= end_before + tolerance)
         )
 
     # This is a cache that significantly speeds up repeated ``find()`` queries.
     _segments_by_recording_id: Optional[Dict[str, List[SupervisionSegment]]] = None
```

### Comparing `lhotse-1.8.0/lhotse/testing/dummies.py` & `lhotse-1.9.0/lhotse/testing/dummies.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 from tempfile import NamedTemporaryFile
 from typing import Dict, List, Optional, Type, Union
 
 from lhotse import AudioSource
 from lhotse.array import Array, TemporalArray
 from lhotse.audio import Recording, RecordingSet
-from lhotse.cut import CutSet, MonoCut
+from lhotse.cut import CutSet, MonoCut, MultiCut
 from lhotse.features import Features, FeatureSet
 from lhotse.manipulation import Manifest
 from lhotse.supervision import AlignmentItem, SupervisionSegment, SupervisionSet
 from lhotse.utils import fastcopy
 
 
 @contextlib.contextmanager
@@ -55,14 +55,32 @@
         ],
         sampling_rate=16000,
         num_samples=16000,
         duration=duration,
     )
 
 
+def dummy_multi_channel_recording(
+    unique_id: int, duration: float = 1.0, channel_ids: Optional[List[int]] = None
+) -> Recording:
+    if channel_ids is None:
+        channel_ids = [0, 1]
+    return Recording(
+        id=f"dummy-multi-channel-recording-{unique_id:04d}",
+        sources=[
+            AudioSource(
+                type="command", channels=channel_ids, source='echo "dummy waveform"'
+            )
+        ],
+        sampling_rate=16000,
+        num_samples=16000,
+        duration=duration,
+    )
+
+
 def dummy_alignment(
     text: str = "irrelevant", start: float = 0.0, duration: float = 1.0
 ) -> Dict[str, List[AlignmentItem]]:
     subwords = [
         text[i : i + 3] for i in range(0, len(text), 3)
     ]  # Create subwords of 3 chars
     dur = duration / len(subwords)
@@ -73,22 +91,24 @@
     return {"subword": alignment}
 
 
 def dummy_supervision(
     unique_id: int,
     start: float = 0.0,
     duration: float = 1.0,
+    channel: Union[int, List[int]] = 0,
     text: str = "irrelevant",
     alignment: Optional[Dict[str, List[AlignmentItem]]] = dummy_alignment(),
 ) -> SupervisionSegment:
     return SupervisionSegment(
         id=f"dummy-segment-{unique_id:04d}",
         recording_id=f"dummy-recording-{unique_id:04d}",
         start=start,
         duration=duration,
+        channel=channel,
         text=text,
         speaker="irrelevant",
         language="irrelevant",
         gender="irrelevant",
         custom={"custom_field": "irrelevant"},
         alignment=alignment,
     )
@@ -109,14 +129,38 @@
         sampling_rate=16000,
         storage_type="lilcom_files",
         storage_path="test/fixtures/dummy_feats/storage",
         storage_key="dbf9a0ec-f79d-4eb8-ae83-143a6d5de64d.llc",
     )
 
 
+def dummy_multi_channel_features(
+    unique_id: int,
+    start: float = 0.0,
+    duration: float = 1.0,
+    channels: Optional[List[int]] = None,
+) -> Features:
+    if channels is None:
+        channels = [0, 1]
+    return Features(
+        recording_id=f"dummy-multi-channel-recording-{unique_id:04d}",
+        channels=channels,
+        start=start,
+        duration=duration,
+        type="fbank",
+        num_frames=100,
+        num_features=23,
+        frame_shift=0.01,
+        sampling_rate=16000,
+        storage_type="lilcom_files",
+        storage_path="test/fixtures/dummy_feats/storage",
+        storage_key="dbf9a0ec-f79d-4eb8-ae83-143a6d5de64d.llc",
+    )
+
+
 def dummy_temporal_array(start: float = 0.0) -> TemporalArray:
     return TemporalArray(
         array=Array(
             storage_type="lilcom_files",
             storage_path="test/fixtures/dummy_feats/storage",
             storage_key="dbf9a0ec-f79d-4eb8-ae83-143a6d5de64d.llc",
             shape=[100, 23],
@@ -132,21 +176,43 @@
     start: float = 0.0,
     duration: float = 1.0,
     recording: Recording = None,
     features: Features = None,
     supervisions=None,
 ):
     return MonoCut(
-        id=f"dummy-cut-{unique_id:04d}",
+        id=f"dummy-mono-cut-{unique_id:04d}",
         start=start,
         duration=duration,
         channel=0,
         recording=recording if recording else dummy_recording(unique_id),
         features=features if features else dummy_features(unique_id),
         supervisions=supervisions if supervisions is not None else [],
     )
 
 
+def dummy_multi_cut(
+    unique_id: int,
+    start: float = 0.0,
+    duration: float = 1.0,
+    recording: Recording = None,
+    features: Features = None,
+    supervisions: SupervisionSet = None,
+    channel: Optional[List[int]] = None,
+):
+    if channel is None:
+        channel = [0, 1]
+    return MultiCut(
+        id=f"dummy-multi-cut-{unique_id:04d}",
+        start=start,
+        duration=duration,
+        channel=channel,
+        recording=recording if recording else dummy_multi_channel_recording(unique_id),
+        features=features if features else dummy_multi_channel_features(unique_id),
+        supervisions=supervisions if supervisions is not None else [],
+    )
+
+
 def remove_spaces_from_segment_text(segment):
     if segment.text is None:
         return segment
     return fastcopy(segment, text=segment.text.replace(" ", ""))
```

### Comparing `lhotse-1.8.0/lhotse/testing/fixtures.py` & `lhotse-1.9.0/lhotse/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/tools/sph2pipe.py` & `lhotse-1.9.0/lhotse/tools/sph2pipe.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/utils.py` & `lhotse-1.9.0/lhotse/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import math
 import random
 import uuid
 import warnings
 from contextlib import AbstractContextManager, contextmanager
 from dataclasses import asdict, dataclass
 from decimal import ROUND_HALF_DOWN, ROUND_HALF_UP, Decimal
+from itertools import chain
 from math import ceil, isclose
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
@@ -549,14 +550,28 @@
         # We'll decrease the new_duration by the negative offset.
         new_duration = round(new_duration + new_start, ndigits=15)
         new_start = 0
 
     return round(new_start, ndigits=15), new_duration
 
 
+def merge_items_with_delimiter(
+    values: Iterable[str], prefix: str = "cat", delimiter: str = "#"
+) -> Optional[str]:
+    # e.g.
+    # values = ["1125-76840-0001", "1125-53670-0003"]
+    # return "cat#1125-76840-0001#1125-53670-0003"
+    values = list(values)
+    if len(values) == 0:
+        return None
+    if len(values) == 1:
+        return values[0]
+    return delimiter.join(chain([prefix], values))
+
+
 def index_by_id_and_check(manifests: Iterable[T]) -> Dict[str, T]:
     id2man = {}
     for m in manifests:
         assert m.id not in id2man, f"Duplicated manifest ID: {m.id}"
         id2man[m.id] = m
     return id2man
 
@@ -605,14 +620,18 @@
     return start_sample, num_samples
 
 
 def is_none_or_gt(value, threshold) -> bool:
     return value is None or value > threshold
 
 
+def is_equal_or_contains(value: Union[T, Sequence[T]], other: T) -> bool:
+    return value == other or (isinstance(value, Sequence) and other in value)
+
+
 def is_module_available(*modules: str) -> bool:
     r"""Returns if a top-level module with :attr:`name` exists *without**
     importing it. This is generally safer than try-catch block around a
     `import X`. It avoids third party libraries breaking assumptions of some of
     our tests, e.g., setting multiprocessing start method when imported
     (see librosa/#747, torchvision/#544).
 
@@ -638,14 +657,19 @@
 
 
 def ifnone(item: Optional[Any], alt_item: Any) -> Any:
     """Return ``alt_item`` if ``item is None``, otherwise ``item``."""
     return alt_item if item is None else item
 
 
+def to_list(item: Union[Any, Sequence[Any]]) -> List[Any]:
+    """Convert ``item`` to a list if it is not already a list."""
+    return item if isinstance(item, list) else [item]
+
+
 def lens_to_mask(lens: torch.IntTensor) -> torch.Tensor:
     """
     Create a 2-D mask tensor of shape (batch_size, max_length) and dtype float32
     from a 1-D tensor of integers describing the length of batch samples in another tensor.
     """
     mask = lens.new_zeros(lens.shape[0], max(lens), dtype=torch.float32)
     for i, num in enumerate(lens):
```

### Comparing `lhotse-1.8.0/lhotse/workarounds.py` & `lhotse-1.9.0/lhotse/workarounds.py`

 * *Files identical despite different names*

### Comparing `lhotse-1.8.0/lhotse/workflows/forced_alignment.py` & `lhotse-1.9.0/lhotse/workflows/forced_alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,22 @@
 
 
 def _make_discard_symbols_regex(labels: Sequence[str]) -> re.Pattern:
     return re.compile(rf"[^{' '.join(labels)}]")
 
 
 def _normalize_text(text: str, discard_symbols: re.Pattern) -> str:
+    from lhotse.utils import is_module_available
+
+    assert is_module_available(
+        "num2words"
+    ), "To align with torchaudio, please run 'pip install num2words' for number to word normalization."
+    from num2words import num2words
+
+    text = re.sub(r"(\d+)", lambda x: num2words(int(x.group(0))), text)
     return re.sub(discard_symbols, "", text.upper().replace(" ", "|"))
 
 
 def _get_trellis(
     emission: torch.Tensor, tokens: Sequence[int], blank_id: int = 0
 ) -> torch.Tensor:
     num_frame = emission.size(0)
```

### Comparing `lhotse-1.8.0/lhotse.egg-info/PKG-INFO` & `lhotse-1.9.0/lhotse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lhotse
-Version: 1.8.0
+Version: 1.9.0
 Summary: Data preparation for speech processing models training.
 Author: The Lhotse Development Team
 Author-email: pzelasko@jhu.edu
 License: Apache-2.0 License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `lhotse-1.8.0/lhotse.egg-info/SOURCES.txt` & `lhotse-1.9.0/lhotse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 lhotse/bin/modes/recipes/bvcc.py
 lhotse/bin/modes/recipes/callhome_egyptian.py
 lhotse/bin/modes/recipes/callhome_english.py
 lhotse/bin/modes/recipes/cmu_arctic.py
 lhotse/bin/modes/recipes/cmu_indic.py
 lhotse/bin/modes/recipes/cmu_kids.py
 lhotse/bin/modes/recipes/commonvoice.py
+lhotse/bin/modes/recipes/csj.py
 lhotse/bin/modes/recipes/cslu_kids.py
 lhotse/bin/modes/recipes/daily_talk.py
 lhotse/bin/modes/recipes/dihard3.py
 lhotse/bin/modes/recipes/earnings21.py
 lhotse/bin/modes/recipes/earnings22.py
 lhotse/bin/modes/recipes/eval2000.py
 lhotse/bin/modes/recipes/fisher_english.py
@@ -99,16 +100,18 @@
 lhotse/bin/modes/recipes/timit.py
 lhotse/bin/modes/recipes/vctk.py
 lhotse/bin/modes/recipes/voxceleb.py
 lhotse/bin/modes/recipes/wenet_speech.py
 lhotse/bin/modes/recipes/yesno.py
 lhotse/cut/__init__.py
 lhotse/cut/base.py
+lhotse/cut/data.py
 lhotse/cut/mixed.py
 lhotse/cut/mono.py
+lhotse/cut/multi.py
 lhotse/cut/padding.py
 lhotse/cut/set.py
 lhotse/dataset/__init__.py
 lhotse/dataset/collation.py
 lhotse/dataset/dataloading.py
 lhotse/dataset/diarization.py
 lhotse/dataset/input_strategies.py
@@ -168,14 +171,15 @@
 lhotse/recipes/bvcc.py
 lhotse/recipes/callhome_egyptian.py
 lhotse/recipes/callhome_english.py
 lhotse/recipes/cmu_arctic.py
 lhotse/recipes/cmu_indic.py
 lhotse/recipes/cmu_kids.py
 lhotse/recipes/commonvoice.py
+lhotse/recipes/csj.py
 lhotse/recipes/cslu_kids.py
 lhotse/recipes/daily_talk.py
 lhotse/recipes/dihard3.py
 lhotse/recipes/earnings21.py
 lhotse/recipes/earnings22.py
 lhotse/recipes/eval2000.py
 lhotse/recipes/fisher_english.py
```

### Comparing `lhotse-1.8.0/lhotse.egg-info/requires.txt` & `lhotse-1.9.0/lhotse.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,50 +8,50 @@
 packaging
 pyyaml>=5.3.1
 tqdm
 lilcom>=1.1.0
 
 [all]
 black==22.3.0
-coverage>=6.0.0
+coverage==6.5.0
 dill
-flake8==4.0.1
-hypothesis==5.41.2
+flake8==5.0.4
+hypothesis==6.56.0
 isort==5.10.1
 jupyterlab
 matplotlib
 numpy>=1.18.1
 orjson>=3.6.6
 pre-commit<=2.19.0,>=2.17.0
-pytest-cov==3.0.0
+pytest-cov==4.0.0
 pytest-forked==1.4.0
 pytest-xdist==2.5.0
-pytest>=5.4.3
+pytest==7.1.3
 sphinx-autodoc-typehints==1.12.0
 sphinx-click==3.0.1
 sphinx==4.2.0
 sphinx_rtd_theme
 webdataset==0.2.5
 
 [dev]
 black==22.3.0
-coverage>=6.0.0
+coverage==6.5.0
 dill
-flake8==4.0.1
-hypothesis==5.41.2
+flake8==5.0.4
+hypothesis==6.56.0
 isort==5.10.1
 jupyterlab
 matplotlib
 numpy>=1.18.1
 orjson>=3.6.6
 pre-commit<=2.19.0,>=2.17.0
-pytest-cov==3.0.0
+pytest-cov==4.0.0
 pytest-forked==1.4.0
 pytest-xdist==2.5.0
-pytest>=5.4.3
+pytest==7.1.3
 sphinx-autodoc-typehints==1.12.0
 sphinx-click==3.0.1
 sphinx==4.2.0
 sphinx_rtd_theme
 webdataset==0.2.5
 
 [dill]
@@ -71,20 +71,20 @@
 kaldi_native_io
 kaldifeat
 
 [orjson]
 orjson>=3.6.6
 
 [tests]
-pytest>=5.4.3
+pytest==7.1.3
 pytest-forked==1.4.0
 pytest-xdist==2.5.0
-pytest-cov==3.0.0
-flake8==4.0.1
-coverage>=6.0.0
-hypothesis==5.41.2
+pytest-cov==4.0.0
+flake8==5.0.4
+coverage==6.5.0
+hypothesis==6.56.0
 black==22.3.0
 isort==5.10.1
 pre-commit<=2.19.0,>=2.17.0
 
 [webdataset]
 webdataset==0.2.5
```

### Comparing `lhotse-1.8.0/setup.py` & `lhotse-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 project_root = Path(__file__).parent
 
 # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! #
 # NOTE: REMEMBER TO UPDATE THE FALLBACK VERSION IN lhotse/__init__.py WHEN RELEASING #
 # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! #
 MAJOR_VERSION = 1
-MINOR_VERSION = 8
+MINOR_VERSION = 9
 PATCH_VERSION = 0
 IS_DEV_VERSION = False  # False = public release, True = otherwise
 
 
 if sys.version_info < (3,):
     # fmt: off
     print(
@@ -176,21 +176,21 @@
             "or https://github.com/pytorch/audio#dependencies"
         )
 except ImportError:
     install_requires.extend(["torch", "torchaudio"])
 
 docs_require = (project_root / "docs" / "requirements.txt").read_text().splitlines()
 tests_require = [
-    "pytest>=5.4.3",
+    "pytest==7.1.3",
     "pytest-forked==1.4.0",
     "pytest-xdist==2.5.0",
-    "pytest-cov==3.0.0",
-    "flake8==4.0.1",
-    "coverage>=6.0.0",
-    "hypothesis==5.41.2",
+    "pytest-cov==4.0.0",
+    "flake8==5.0.4",
+    "coverage==6.5.0",
+    "hypothesis==6.56.0",
     "black==22.3.0",
     "isort==5.10.1",
     "pre-commit>=2.17.0,<=2.19.0",
 ]
 orjson_requires = ["orjson>=3.6.6"]
 webdataset_requires = ["webdataset==0.2.5"]
 dill_requires = ["dill"]
```

