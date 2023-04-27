# Comparing `tmp/GANDLF-0.0.16.dev20230425.tar.gz` & `tmp/GANDLF-0.0.16.dev20230426.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.16.dev20230425.tar", last modified: Tue Apr 25 03:12:59 2023, max compression
+gzip compressed data, was "GANDLF-0.0.16.dev20230426.tar", last modified: Wed Apr 26 03:12:50 2023, max compression
```

## Comparing `GANDLF-0.0.16.dev20230425.tar` & `GANDLF-0.0.16.dev20230426.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.742323 GANDLF-0.0.16.dev20230425/
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.706323 GANDLF-0.0.16.dev20230425/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.706323 GANDLF-0.0.16.dev20230425/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.710323 GANDLF-0.0.16.dev20230425/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.714323 GANDLF-0.0.16.dev20230425/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.714323 GANDLF-0.0.16.dev20230425/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.714323 GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.714323 GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.718323 GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.718323 GANDLF-0.0.16.dev20230425/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.718323 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.722323 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.722323 GANDLF-0.0.16.dev20230425/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.726323 GANDLF-0.0.16.dev20230425/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.726323 GANDLF-0.0.16.dev20230425/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/metrics/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.734323 GANDLF-0.0.16.dev20230425/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17212 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.738323 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24703 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.738323 GANDLF-0.0.16.dev20230425/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30645 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.738323 GANDLF-0.0.16.dev20230425/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.742323 GANDLF-0.0.16.dev20230425/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 03:12:52.000000 GANDLF-0.0.16.dev20230425/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:12:59.706323 GANDLF-0.0.16.dev20230425/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-25 03:12:59.000000 GANDLF-0.0.16.dev20230425/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-25 03:12:59.000000 GANDLF-0.0.16.dev20230425/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:12:59.000000 GANDLF-0.0.16.dev20230425/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:10:26.000000 GANDLF-0.0.16.dev20230425/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-25 03:12:59.000000 GANDLF-0.0.16.dev20230425/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 03:12:59.000000 GANDLF-0.0.16.dev20230425/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-25 03:12:59.742323 GANDLF-0.0.16.dev20230425/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 03:12:59.742323 GANDLF-0.0.16.dev20230425/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-25 03:10:19.000000 GANDLF-0.0.16.dev20230425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.392314 GANDLF-0.0.16.dev20230426/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.356313 GANDLF-0.0.16.dev20230426/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.356313 GANDLF-0.0.16.dev20230426/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.360314 GANDLF-0.0.16.dev20230426/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.360314 GANDLF-0.0.16.dev20230426/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.364313 GANDLF-0.0.16.dev20230426/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.364313 GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.364313 GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.364313 GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.368314 GANDLF-0.0.16.dev20230426/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.368314 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.372314 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.372314 GANDLF-0.0.16.dev20230426/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.372314 GANDLF-0.0.16.dev20230426/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.376314 GANDLF-0.0.16.dev20230426/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/metrics/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.380314 GANDLF-0.0.16.dev20230426/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17212 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.384314 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24703 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.388314 GANDLF-0.0.16.dev20230426/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30754 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.388314 GANDLF-0.0.16.dev20230426/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.388314 GANDLF-0.0.16.dev20230426/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 03:12:43.000000 GANDLF-0.0.16.dev20230426/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:12:50.356313 GANDLF-0.0.16.dev20230426/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-26 03:12:50.000000 GANDLF-0.0.16.dev20230426/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-26 03:12:50.000000 GANDLF-0.0.16.dev20230426/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:12:50.000000 GANDLF-0.0.16.dev20230426/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:10:23.000000 GANDLF-0.0.16.dev20230426/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-26 03:12:50.000000 GANDLF-0.0.16.dev20230426/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 03:12:50.000000 GANDLF-0.0.16.dev20230426/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-26 03:12:50.392314 GANDLF-0.0.16.dev20230426/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 03:12:50.392314 GANDLF-0.0.16.dev20230426/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-04-26 03:10:14.000000 GANDLF-0.0.16.dev20230426/setup.py
```

### Comparing `GANDLF-0.0.16.dev20230425/CODE_OF_CONDUCT.md` & `GANDLF-0.0.16.dev20230426/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/CONTRIBUTING.md` & `GANDLF-0.0.16.dev20230426/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.16.dev20230426/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/cli/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/cli/config_generator.py` & `GANDLF-0.0.16.dev20230426/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/cli/deploy.py` & `GANDLF-0.0.16.dev20230426/GANDLF/cli/deploy.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,31 +66,35 @@
         outputdir (str): The path to the output directory.
         mlcubedir (str): The path to the mlcube directory.
     """
     # Set up docker client for any future calls
     docker_client = docker.from_env()
     print("Connected to the docker service.")
 
-    mlcube_config_file = mlcubedir + "/mlcube.yaml"
+    mlcube_config_file = os.path.join(mlcubedir, "mlcube.yaml")
     assert os.path.exists(mlcubedir) and os.path.exists(
         mlcube_config_file
     ), "MLCube Directory: This does not appear to be a valid MLCube directory."
 
-    os.makedirs(outputdir + "/workspace", exist_ok=True)
-    shutil.copytree(
-        mlcubedir + "/workspace", outputdir + "/workspace", dirs_exist_ok=True
-    )
-    shutil.copyfile(config, outputdir + "/workspace/config.yml")
+    output_workspace_folder = os.path.join(outputdir, "workspace")
+    mlcube_workspace_folder = os.path.join(mlcubedir, "workspace")
+
+    os.makedirs(output_workspace_folder, exist_ok=True)
+    if os.path.exists(mlcube_workspace_folder):
+        shutil.copytree(
+            mlcube_workspace_folder, output_workspace_folder, dirs_exist_ok=True,
+        )
+    shutil.copyfile(config, os.path.join(output_workspace_folder, "config.yml"))
 
     # First grab the existing the mlcube config then modify for the embedded-model image.
     mlcube_config = None
     with open(mlcube_config_file, "r") as f:
         mlcube_config = yaml.safe_load(f)
 
-    output_mlcube_config_path = outputdir + "/mlcube.yaml"
+    output_mlcube_config_path = os.path.join(outputdir, "mlcube.yaml")
 
     old_train_output_modeldir = mlcube_config["tasks"]["train"]["parameters"][
         "outputs"
     ].pop("modeldir", None)
     mlcube_config["tasks"]["infer"]["parameters"]["inputs"].pop("modeldir", None)
     mlcube_config["tasks"]["train"]["parameters"]["inputs"].pop("config", None)
     # Currently disabled because we've decided exposing config-on-inference complicates the MLCube use case.
```

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/cli/main_run.py` & `GANDLF-0.0.16.dev20230426/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.16.dev20230426/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.16.dev20230426/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.16.dev20230426/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/cli/recover_config.py` & `GANDLF-0.0.16.dev20230426/GANDLF/cli/recover_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     pickle_location = os.path.join(modelDir, "parameters.pkl")
     assert os.path.exists(
         pickle_location
     ), "The model does not appear to have a configuration file. Please check parameters."
 
     with open(pickle_location, "rb") as handle:
         parameters = pickle.load(handle)
-        os.makedirs(os.path.dirname(outputFile), exist_ok=True)
+        os.makedirs(os.path.dirname(os.path.realpath(outputFile)), exist_ok=True)
 
         # Remove a few problematic objects from the output
         # These cannot be safe_dumped to YAML (or present other problems).
         # To avoid this, try to use primitives and don't use integers as dict keys.
         removable_entries = [
             "output_dir",
             "model_dir_embedded",
```

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.16.dev20230426/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/compute/generic.py` & `GANDLF-0.0.16.dev20230426/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.16.dev20230426/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.16.dev20230426/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/compute/step.py` & `GANDLF-0.0.16.dev20230426/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/compute/training_loop.py` & `GANDLF-0.0.16.dev20230426/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/ImagesFromDataFrame.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import os
+from pathlib import Path
 import numpy as np
 
 import torch
 import torchio
 from torchio.transforms import Pad
 import SimpleITK as sitk
 from tqdm import tqdm
 
-from GANDLF.utils import perform_sanity_check_on_subject, resize_image
+from GANDLF.utils import (
+    perform_sanity_check_on_subject,
+    resize_image,
+    get_filename_extension_sanitized,
+)
 from .preprocessing import get_transforms_for_preprocessing
 from .augmentation import global_augs_dict
 
 global_sampler_dict = {
     "uniform": torchio.data.UniformSampler,
     "uniformsampler": torchio.data.UniformSampler,
     "uniformsample": torchio.data.UniformSampler,
@@ -93,14 +98,41 @@
             # check for different resizing keys
             if key in ["resize", "resize_image", "resize_images"]:
                 if not (preprocessing[key] is None):
                     resize_images_flag = True
                     preprocessing["resize_image"] = preprocessing[key]
                     break
 
+    # helper function to save the resized images
+    def _save_resized_images(
+        resized_image, output_dir, subject_id, channel_str, loader_type, extension
+    ):
+        """
+        Helper function to save the resized images
+
+        Args:
+            resized_image (sitk.Image): The resized image.
+            output_dir (str): The output directory.
+            subject_id (str): The subject ID.
+            channel_str (str): The channel string.
+            loader_type (str): The loader type.
+            extension (str): The extension of the image.
+        """
+        # save img_resized to disk
+        save_dir_for_resized_images = os.path.join(
+            output_dir, loader_type + "_resized_images"
+        )
+        Path(save_dir_for_resized_images).mkdir(parents=True, exist_ok=True)
+        save_path = os.path.join(
+            save_dir_for_resized_images,
+            subject_id + "_" + channel_str + "_resized" + extension,
+        )
+        if not os.path.isfile(save_path):
+            sitk.WriteImage(resized_image, save_path)
+
     # iterating through the dataframe
     for patient in tqdm(
         range(num_row), desc="Constructing queue for " + loader_type + " data"
     ):
         # We need this dict for storing the meta data for each subject
         # such as different image modalities, labels, any other data
         subject_dict = {}
@@ -124,17 +156,31 @@
                 subject_dict["spacing"] = torch.Tensor(file_reader.GetSpacing())
 
             # if resize_image is requested, the perform per-image resize with appropriate interpolator
             if resize_images_flag:
                 img_resized = resize_image(
                     subject_dict[str(channel)].as_sitk(), preprocessing["resize_image"]
                 )
-                # always ensure resized image spacing is used
-                subject_dict["spacing"] = torch.Tensor(img_resized.GetSpacing())
-                subject_dict[str(channel)] = torchio.ScalarImage.from_sitk(img_resized)
+                if parameters["memory_save_mode"]:
+                    _save_resized_images(
+                        img_resized,
+                        parameters["output_dir"],
+                        subject_dict["subject_id"],
+                        str(channel),
+                        loader_type,
+                        get_filename_extension_sanitized(
+                            str(dataframe[channel][patient])
+                        ),
+                    )
+                else:
+                    # always ensure resized image spacing is used
+                    subject_dict["spacing"] = torch.Tensor(img_resized.GetSpacing())
+                    subject_dict[str(channel)] = torchio.ScalarImage.from_sitk(
+                        img_resized
+                    )
 
         # # for regression -- this logic needs to be thought through
         # if predictionHeaders:
         #     # get the mask
         #     if (subject_dict['label'] is None) and (class_list is not None):
         #         sys.exit('The \'class_list\' parameter has been defined but a label file is not present for patient: ', patient)
 
@@ -148,15 +194,27 @@
             # if resize is requested, the perform per-image resize with appropriate interpolator
             if resize_images_flag:
                 img_resized = resize_image(
                     subject_dict["label"].as_sitk(),
                     preprocessing["resize_image"],
                     sitk.sitkNearestNeighbor,
                 )
-                subject_dict["label"] = torchio.LabelMap.from_sitk(img_resized)
+                if parameters["memory_save_mode"]:
+                    _save_resized_images(
+                        img_resized,
+                        parameters["output_dir"],
+                        subject_dict["subject_id"],
+                        "label",
+                        loader_type,
+                        get_filename_extension_sanitized(
+                            str(dataframe[channel][patient])
+                        ),
+                    )
+                else:
+                    subject_dict["label"] = torchio.LabelMap.from_sitk(img_resized)
 
         else:
             subject_dict["label"] = "NA"
             subject_dict["path_to_metadata"] = str(dataframe[channel][patient])
 
         # iterating through the values to predict of the subject
         valueCounter = 0
```

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/post_process/morphology.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,7 @@
     ]
     largest_region = 0
     if len(labels_connected_sizes) > 1:
         largest_region = np.argmax(labels_connected_sizes[1:]) + 1
     seg[labels_connected != largest_region] = 0
 
     return seg
-
```

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.16.dev20230426/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.16.dev20230426/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.16.dev20230426/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.16.dev20230426/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/inference_manager.py` & `GANDLF-0.0.16.dev20230426/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/logger.py` & `GANDLF-0.0.16.dev20230426/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/losses/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/losses/hybrid.py` & `GANDLF-0.0.16.dev20230426/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/losses/regression.py` & `GANDLF-0.0.16.dev20230426/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/losses/segmentation.py` & `GANDLF-0.0.16.dev20230426/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/metrics/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/metrics/classification.py` & `GANDLF-0.0.16.dev20230426/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/metrics/generic.py` & `GANDLF-0.0.16.dev20230426/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/metrics/regression.py` & `GANDLF-0.0.16.dev20230426/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.16.dev20230426/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/MSDNet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/brain_age.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/deep_unet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/densenet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/efficientnet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/fcn.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/imagenet_unet.py`

 * *Files 8% similar despite different names*

```diff
@@ -190,25 +190,41 @@
 
     def __init__(
         self,
         parameters,
     ) -> None:
         super(ImageNet_UNet, self).__init__(parameters)
 
+        # https://github.com/qubvel/segmentation_models.pytorch/issues/745
+        import ssl
+
+        ssl._create_default_https_context = ssl._create_unverified_context
+
         decoder_use_batchnorm = False
         if parameters["model"]["norm_type"] == "batch":
             decoder_use_batchnorm = True
         decoder_use_batchnorm = parameters["model"].get(
             "decoder_use_batchnorm", decoder_use_batchnorm
         )
+
+        default_encoder_name = parameters["model"].get("encoder_name", "resnet34")
+        # MixVision Transformers only support 2D inputs with 3 channels (the channel dimension is checked in the encoder)
+        if ("mit_" in default_encoder_name) or ("timm-" in default_encoder_name):
+            assert (
+                self.n_dimensions == 2
+            ), "MixVision Transformers and TIMM models only support 2D inputs"
+
         encoder_depth = parameters["model"].get("depth", 5)
         encoder_depth = parameters["model"].get("encoder_depth", encoder_depth)
         parameters["model"]["pretrained"] = parameters["model"].get("pretrained", True)
         if parameters["model"]["pretrained"]:
             parameters["model"]["encoder_weights"] = "imagenet"
+            # special case for some encoders: https://github.com/search?q=repo%3Aqubvel%2Fsegmentation_models.pytorch%20imagenet%2B5k&type=code
+            if default_encoder_name in ["dpn68b", "dpn92", "dpn107"]:
+                parameters["model"]["encoder_weights"] = "imagenet+5k"
         else:
             parameters["model"]["encoder_weights"] = None
 
         if parameters["problem_type"] != "segmentation":
             classifier_head_parameters = {}
             classifier_head_parameters["classes"] = self.n_classes
             classifier_head_parameters["activation"] = parameters["model"][
@@ -221,20 +237,14 @@
             )
             classifier_head_parameters["pooling"] = parameters["model"].get(
                 "pooling", "avg"
             )
         else:
             classifier_head_parameters = None
 
-        default_encoder_name = parameters["model"].get("encoder_name", "resnet34")
-        if "mit_" in default_encoder_name:
-            assert (
-                self.n_dimensions == 2
-            ), "MixVision Transformers only support 2D inputs"
-
         self.model = Unet(
             encoder_name=default_encoder_name,
             encoder_weights=parameters["model"]["encoder_weights"],
             in_channels=self.n_channels,
             classes=self.n_classes,
             activation=parameters["model"]["final_layer"],
             decoder_use_batchnorm=decoder_use_batchnorm,
```

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/light_unet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/modelBase.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/resnet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/sdnet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/transunet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/uinc.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/unet.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/unetr.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/models/vgg.py` & `GANDLF-0.0.16.dev20230426/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.16.dev20230426/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/parseConfig.py` & `GANDLF-0.0.16.dev20230426/GANDLF/parseConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     "q_num_workers": 4,  # number of worker threads to use
     "num_epochs": 100,  # total number of epochs to train
     "patience": 100,  # number of epochs to wait for performance improvement
     "batch_size": 1,  # default batch size of training
     "learning_rate": 0.001,  # default learning rate
     "clip_grad": None,  # clip_gradient value
     "track_memory_usage": False,  # default memory tracking
-    "print_rgb_label_warning": True,  # default memory tracking
+    "memory_save_mode": False,  # default memory saving, if enabled, resize/resample will save files to disk
+    "print_rgb_label_warning": True,  # print rgb label warning
     "data_postprocessing": {},  # default data postprocessing
     "grid_aggregator_overlap": "crop",  # default grid aggregator overlap strategy
     "determinism": False,  # using deterministic version of computation
 }
 
 ## dictionary to define string defaults for appropriate options
 parameter_defaults_string = {
```

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.16.dev20230426/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/training_manager.py` & `GANDLF-0.0.16.dev20230426/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/utils/__init__.py` & `GANDLF-0.0.16.dev20230426/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/utils/generic.py` & `GANDLF-0.0.16.dev20230426/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.16.dev20230426/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/utils/imaging.py` & `GANDLF-0.0.16.dev20230426/GANDLF/utils/imaging.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,34 +53,32 @@
 
 
 def resize_image(input_image, output_size, interpolator=sitk.sitkLinear):
     """
     This function resizes the input image based on the output size and interpolator.
     Args:
         input_image (SimpleITK.Image): The input image to be resized.
-        output_size (numpy.array | list): The output size to resample input_image to.
+        output_size (Union[numpy.ndarray, list, tuple]): The output size to resample input_image to.
         interpolator (SimpleITK.sitkInterpolator): The desired interpolator.
     Returns:
         SimpleITK.Image: The output image after resizing.
     """
     output_size_parsed = None
     inputSize = input_image.GetSize()
     inputSpacing = np.array(input_image.GetSpacing())
     outputSpacing = np.array(inputSpacing)
 
+    output_size_parsed = output_size
     if isinstance(output_size, dict):
         if "resize" in output_size:
             output_size_parsed = output_size["resize"]
-    elif isinstance(output_size, list) or isinstance(output_size, np.array):
-        output_size_parsed = output_size
 
-    if len(output_size_parsed) != len(inputSpacing):
-        sys.exit(
-            "The output size dimension is inconsistent with the input dataset, please check parameters."
-        )
+    assert len(output_size_parsed) == len(
+        inputSpacing
+    ), "The output size dimension is inconsistent with the input dataset, please check parameters."
 
     for i, n in enumerate(output_size_parsed):
         outputSpacing[i] = outputSpacing[i] * (inputSize[i] / n)
 
     return resample_image(
         input_image,
         outputSpacing,
@@ -130,33 +128,39 @@
 
     import copy
 
     list_for_comparison = copy.deepcopy(parameters["headers"]["channelHeaders"])
     if parameters["headers"]["labelHeader"] is not None:
         list_for_comparison.append("label")
 
+    def _get_itkimage_or_filereader(subject_str_key):
+        """
+        Helper function to get the itk image or file reader from the subject.
+
+        Args:
+            subject_str_key (Union[str, sitk.Image]): The subject string key.
+
+        Returns:
+            Union[sitk.ImageFileReader, sitk.Image]: The itk image or file reader.
+        """
+        if subject_str_key["path"] != "":
+            file_reader = sitk.ImageFileReader()
+            file_reader.SetFileName(subject_str_key["path"])
+            file_reader.ReadImageInformation()
+            return file_reader
+        else:
+            # this case is required if any tensor/imaging operation has been applied in dataloader
+            file_reader = subject_str_key.as_sitk()
+
     if len(list_for_comparison) > 1:
         for key in list_for_comparison:
             if file_reader_base is None:
-                if subject[str(key)]["path"] != "":
-                    file_reader_base = sitk.ImageFileReader()
-                    file_reader_base.SetFileName(subject[str(key)]["path"])
-                    file_reader_base.ReadImageInformation()
-                else:
-                    # this case is required if any tensor/imaging operation has been applied in dataloader
-                    file_reader_base = subject[str(key)].as_sitk()
+                file_reader_base = _get_itkimage_or_filereader(subject[str(key)])
             else:
-                if subject[str(key)]["path"] != "":
-                    # in this case, file_reader_base is ready
-                    file_reader_current = sitk.ImageFileReader()
-                    file_reader_current.SetFileName(subject[str(key)]["path"])
-                    file_reader_current.ReadImageInformation()
-                else:
-                    # this case is required if any tensor/imaging operation has been applied in dataloader
-                    file_reader_current = subject[str(key)].as_sitk()
+                file_reader_current = _get_itkimage_or_filereader(subject[str(key)])
 
                 # this check needs to be absolute
                 if (
                     file_reader_base.GetDimension()
                     != file_reader_current.GetDimension()
                 ):
                     raise ValueError(
```

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/utils/modelbase.py` & `GANDLF-0.0.16.dev20230426/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/utils/modelio.py` & `GANDLF-0.0.16.dev20230426/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.16.dev20230426/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/utils/tensor.py` & `GANDLF-0.0.16.dev20230426/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF/utils/write_parse.py` & `GANDLF-0.0.16.dev20230426/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.16.dev20230426/GANDLF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.16.dev20230425
+Version: 0.0.16.dev20230426
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230425 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230426 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.16.dev20230425/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.16.dev20230426/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/HISTORY.md` & `GANDLF-0.0.16.dev20230426/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 - Added ability to save `initial` and `latest` models in addition to `best`
 - Added ability to specify testing data csv in main cli
 - Normalized surface dice has been added
 - Added dedicated script to perform post-training model optimization
 - Added CI and documentation for OpenFL integration
 - Added getting started guide
 - Added documentation for all loss functions and updated guideline
+- Added ability to save resized images instead of loading them directly
 
 ## 0.0.15
 - Updated `setup.py` for `python>=3.8`
 - `stride_size` is now handled internally for histology data
 - Probability maps are now saved overlaid with original WSI
 - Added ability to print model size and summary at run-time
 - Improved error checking added for WSI inference
```

### Comparing `GANDLF-0.0.16.dev20230425/LICENSE` & `GANDLF-0.0.16.dev20230426/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/PKG-INFO` & `GANDLF-0.0.16.dev20230426/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.16.dev20230425
+Version: 0.0.16.dev20230426
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230425 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.16.dev20230426 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.16.dev20230425/README.md` & `GANDLF-0.0.16.dev20230426/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/SECURITY.md` & `GANDLF-0.0.16.dev20230426/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_anonymizer` & `GANDLF-0.0.16.dev20230426/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_collectStats` & `GANDLF-0.0.16.dev20230426/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_configGenerator` & `GANDLF-0.0.16.dev20230426/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_constructCSV` & `GANDLF-0.0.16.dev20230426/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_deploy` & `GANDLF-0.0.16.dev20230426/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_optimizeModel` & `GANDLF-0.0.16.dev20230426/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_patchMiner` & `GANDLF-0.0.16.dev20230426/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_preprocess` & `GANDLF-0.0.16.dev20230426/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_recoverConfig` & `GANDLF-0.0.16.dev20230426/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_run` & `GANDLF-0.0.16.dev20230426/gandlf_run`

 * *Files 2% similar despite different names*

```diff
@@ -133,10 +133,10 @@
             args.train,
             args.device,
             args.resume,
             args.reset,
             args.outputdir,
         )
     except Exception as e:
-        sys.exit("Error in GANDLF run:", e)
+        sys.exit("ERROR: " + str(e))
 
     print("Finished.")
```

### Comparing `GANDLF-0.0.16.dev20230425/gandlf_verifyInstall` & `GANDLF-0.0.16.dev20230426/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.16.dev20230425/setup.py` & `GANDLF-0.0.16.dev20230426/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     "numpy==1.22.0",
     "scipy",
     "SimpleITK!=2.0.*",
     "SimpleITK!=2.2.1",  # https://github.com/mlcommons/GaNDLF/issues/536
     "torchvision",
     "tqdm",
     "torchio==0.18.75",
-    "pandas",
+    "pandas<2.0.0",
     "scikit-learn>=0.23.2",
     "scikit-image>=0.19.1",
     "setuptools",
     "seaborn",
     "pyyaml",
     "tiffslide",
     "matplotlib",
```

