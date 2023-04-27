# Comparing `tmp/glow-0.12.2.tar.gz` & `tmp/glow-0.12.3.tar.gz`

## Comparing `glow-0.12.2.tar` & `glow-0.12.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.2/examples/__init__.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.2/examples/cifar10.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.2/examples/gan.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/__init__.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/cli.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/cli.pyi
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/distributed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/py.typed
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/api/__init__.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/api/config.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/api/exporting.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/__init__.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_coro.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_import_hook.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_more.py
--rw-r--r--   0        0        0    14592 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_parallel.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_parallel.pyi
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_patch_len.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_patch_print.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_patch_scipy.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_profile.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_profile.pyi
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_reduction.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_repr.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_sizeof.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_thread_quota.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/_uuid.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/debug.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/wrap/__init__.py
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/wrap/cache.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/wrap/cache.pyi
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/wrap/concurrency.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/wrap/concurrency.pyi
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/wrap/reusable.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/core/wrap/util.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/io/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/io/_sound.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/io/_svg.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/metrics/__init__.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/metrics/base.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/metrics/confusion.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/metrics/raw.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/__init__.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/_loader.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/_sampler.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/_trainer.py
--rw-r--r--   0        0        0    13042 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/amp.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/driver.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/functional.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/optimizers.py
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/plot.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/proto.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/util.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/modules/__init__.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/modules/aggregates.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/modules/context.py
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/modules/convnets.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/modules/lazy.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/modules/simple.py
--rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/modules/transformers.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/modules/util.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/nn/modules/vision.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/transforms/__init__.py
--rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/transforms/classes.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/transforms/core.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/transforms/functional/__init__.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/transforms/functional/core.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.2/src/glow/transforms/functional/numba.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.2/test/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.2/test/run_metrics.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_api.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_batch.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_buffered.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_cli.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_iter.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_loader.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_shm.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_thread_pool.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_timed.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_timer.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.2/test/test_uuid.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.2/LICENSE
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.2/README.md
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 glow-0.12.2/pyproject.toml
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 glow-0.12.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.3/examples/__init__.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.3/examples/cifar10.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.3/examples/gan.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/__init__.py
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/cli.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/cli.pyi
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/distributed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/py.typed
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/api/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/api/config.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/api/exporting.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/__init__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_coro.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_import_hook.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_more.py
+-rw-r--r--   0        0        0    14592 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_parallel.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_parallel.pyi
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_patch_len.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_patch_print.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_patch_scipy.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_profile.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_profile.pyi
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_reduction.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_repr.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_sizeof.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_thread_quota.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/_uuid.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/debug.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/__init__.py
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/cache.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/cache.pyi
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/concurrency.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/concurrency.pyi
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/reusable.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/core/wrap/util.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/io/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/io/_sound.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/io/_svg.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/metrics/__init__.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/metrics/base.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/metrics/confusion.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/metrics/raw.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/__init__.py
+-rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/_loader.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/_sampler.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/_trainer.py
+-rw-r--r--   0        0        0    13042 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/amp.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/driver.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/functional.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/optimizers.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/plot.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/proto.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/util.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/__init__.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/aggregates.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/context.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/convnets.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/lazy.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/simple.py
+-rw-r--r--   0        0        0     8697 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/transformers.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/util.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/nn/modules/vision.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/__init__.py
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/classes.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/core.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/functional/__init__.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/functional/core.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.3/src/glow/transforms/functional/numba.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.3/test/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.3/test/run_metrics.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_api.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_batch.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_buffered.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_cli.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_iter.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_loader.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_shm.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_thread_pool.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_timed.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_timer.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.3/test/test_uuid.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.3/LICENSE
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.3/README.md
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 glow-0.12.3/pyproject.toml
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 glow-0.12.3/PKG-INFO
```

### Comparing `glow-0.12.2/examples/cifar10.py` & `glow-0.12.3/examples/cifar10.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/cli.py` & `glow-0.12.3/src/glow/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,29 +93,30 @@
 
 def _unwrap_type(tp: type) -> tuple[type, dict[str, Any]]:
     if tp is list:
         raise ValueError('Type list should be parametrized')
 
     origin = get_origin(tp)
     *args, = get_args(tp)
-    if not origin or not args:
+    if not origin or not args:  # Not a generic type
         return tp, {'type': tp}
 
-    if origin is list:
+    if origin is list:  # `List[T]`
         cls, opts = _unwrap_type(args[0])
         return cls, opts | {'nargs': argparse.ZERO_OR_MORE}
 
+    # `Optional[T]` or `T | None`
     if origin in _UNION_TYPES and len(args) == 2 and _NoneType in args:
         args.remove(_NoneType)
         cls, opts = _unwrap_type(args[0])
         if opts.get('nargs') == argparse.ZERO_OR_MORE:
             return cls, opts
         return cls, opts | {'nargs': argparse.OPTIONAL}
 
-    if origin is Literal:
+    if origin is Literal:  # `Literal[x, y]`
         choices = get_args(tp)
         if len(tps := {type(c) for c in choices}) != 1:
             raise ValueError('Literal parameters should have '
                              f'the same type. Got: {tps}')
         cls, = tps
         return cls, {'type': cls, 'choices': choices}
 
@@ -192,19 +193,21 @@
         parser.add_argument(
             f'--{snake}',
             *flags,
             action=BooleanOptionalAction,
             default=fd.default,
             help=help_)
 
-    elif fd.default is not MISSING:  # Generic optional
+    # Generic optional
+    elif fd.default is not MISSING or fd.default_factory is not MISSING:
         if opts.get('nargs') == argparse.OPTIONAL:
             del opts['nargs']
+        default = fd.default_factory() if fd.default is MISSING else fd.default
         parser.add_argument(
-            f'--{snake}', *flags, **opts, default=fd.default, help=help_)
+            f'--{snake}', *flags, **opts, default=default, help=help_)
 
     elif isinstance(parser, ArgumentParser):  # Allow only for root parser
         if flags:
             raise ValueError(f'Positional-only field "{fd.name}" '
                              'should not have flag')
         parser.add_argument(snake, **opts, help=help_)
```

### Comparing `glow-0.12.2/src/glow/cli.pyi` & `glow-0.12.3/src/glow/cli.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/distributed.py` & `glow-0.12.3/src/glow/distributed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/api/config.py` & `glow-0.12.3/src/glow/api/config.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/api/exporting.py` & `glow-0.12.3/src/glow/api/exporting.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/__init__.py` & `glow-0.12.3/src/glow/core/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_coro.py` & `glow-0.12.3/src/glow/core/_coro.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_import_hook.py` & `glow-0.12.3/src/glow/core/_import_hook.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_more.py` & `glow-0.12.3/src/glow/core/_more.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_parallel.py` & `glow-0.12.3/src/glow/core/_parallel.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_parallel.pyi` & `glow-0.12.3/src/glow/core/_parallel.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_patch_len.py` & `glow-0.12.3/src/glow/core/_patch_len.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_patch_print.py` & `glow-0.12.3/src/glow/core/_patch_print.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_patch_scipy.py` & `glow-0.12.3/src/glow/core/_patch_scipy.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_profile.py` & `glow-0.12.3/src/glow/core/_profile.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_profile.pyi` & `glow-0.12.3/src/glow/core/_profile.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_reduction.py` & `glow-0.12.3/src/glow/core/_reduction.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_repr.py` & `glow-0.12.3/src/glow/core/_repr.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_sizeof.py` & `glow-0.12.3/src/glow/core/_sizeof.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_thread_quota.py` & `glow-0.12.3/src/glow/core/_thread_quota.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/_uuid.py` & `glow-0.12.3/src/glow/core/_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/debug.py` & `glow-0.12.3/src/glow/core/debug.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/wrap/cache.py` & `glow-0.12.3/src/glow/core/wrap/cache.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/wrap/cache.pyi` & `glow-0.12.3/src/glow/core/wrap/cache.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/wrap/concurrency.py` & `glow-0.12.3/src/glow/core/wrap/concurrency.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/wrap/concurrency.pyi` & `glow-0.12.3/src/glow/core/wrap/concurrency.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/wrap/reusable.py` & `glow-0.12.3/src/glow/core/wrap/reusable.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/core/wrap/util.py` & `glow-0.12.3/src/glow/core/wrap/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/io/_sound.py` & `glow-0.12.3/src/glow/io/_sound.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/io/_svg.py` & `glow-0.12.3/src/glow/io/_svg.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/metrics/__init__.py` & `glow-0.12.3/src/glow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/metrics/base.py` & `glow-0.12.3/src/glow/metrics/base.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/metrics/confusion.py` & `glow-0.12.3/src/glow/metrics/confusion.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/metrics/raw.py` & `glow-0.12.3/src/glow/metrics/raw.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/__init__.py` & `glow-0.12.3/src/glow/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/_loader.py` & `glow-0.12.3/src/glow/nn/_loader.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/_sampler.py` & `glow-0.12.3/src/glow/nn/_sampler.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/_trainer.py` & `glow-0.12.3/src/glow/nn/_trainer.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/amp.py` & `glow-0.12.3/src/glow/nn/amp.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/driver.py` & `glow-0.12.3/src/glow/nn/driver.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/functional.py` & `glow-0.12.3/src/glow/nn/functional.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/optimizers.py` & `glow-0.12.3/src/glow/nn/optimizers.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/plot.py` & `glow-0.12.3/src/glow/nn/plot.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/proto.py` & `glow-0.12.3/src/glow/nn/proto.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/util.py` & `glow-0.12.3/src/glow/nn/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/modules/__init__.py` & `glow-0.12.3/src/glow/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/modules/aggregates.py` & `glow-0.12.3/src/glow/nn/modules/aggregates.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/modules/context.py` & `glow-0.12.3/src/glow/nn/modules/context.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/modules/convnets.py` & `glow-0.12.3/src/glow/nn/modules/convnets.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/modules/lazy.py` & `glow-0.12.3/src/glow/nn/modules/lazy.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/modules/simple.py` & `glow-0.12.3/src/glow/nn/modules/simple.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/modules/transformers.py` & `glow-0.12.3/src/glow/nn/modules/transformers.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/modules/util.py` & `glow-0.12.3/src/glow/nn/modules/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/nn/modules/vision.py` & `glow-0.12.3/src/glow/nn/modules/vision.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/transforms/__init__.py` & `glow-0.12.3/src/glow/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/transforms/classes.py` & `glow-0.12.3/src/glow/transforms/classes.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/transforms/core.py` & `glow-0.12.3/src/glow/transforms/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/transforms/functional/core.py` & `glow-0.12.3/src/glow/transforms/functional/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/src/glow/transforms/functional/numba.py` & `glow-0.12.3/src/glow/transforms/functional/numba.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/run_metrics.py` & `glow-0.12.3/test/run_metrics.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_api.py` & `glow-0.12.3/test/test_api.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_batch.py` & `glow-0.12.3/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_buffered.py` & `glow-0.12.3/test/test_buffered.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_cli.py` & `glow-0.12.3/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_iter.py` & `glow-0.12.3/test/test_iter.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_loader.py` & `glow-0.12.3/test/test_loader.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_shm.py` & `glow-0.12.3/test/test_shm.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_thread_pool.py` & `glow-0.12.3/test/test_thread_pool.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_timed.py` & `glow-0.12.3/test/test_timed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/test/test_uuid.py` & `glow-0.12.3/test/test_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/LICENSE` & `glow-0.12.3/LICENSE`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/README.md` & `glow-0.12.3/README.md`

 * *Files identical despite different names*

### Comparing `glow-0.12.2/pyproject.toml` & `glow-0.12.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 only-packages = true
 
 [project]
 name = "glow"
-version = "0.12.2"
+version = "0.12.3"
 description = "Functional Python tools with a PyTorch flavour"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = []
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
@@ -61,15 +61,15 @@
     "flake8-pyi",
     "flake8-pyproject",
     "flake8-simplify",
     "isort",
     "mypy~=1.1.1",
     "pytest~=6.0",
     "ruff",
-    "yapf[pyproject]==0.32.0",
+    "yapf[pyproject]==0.33.0",
     "toml; python_version>='3.11'",  # See: https://github.com/google/yapf/pull/1040. Drop for yapf~=0.33
 ]
 dev = [
     "glow[dev-core]",
     "flake8-alphabetize",
     # "flake8-class-attributes-order",
     # "flake8-newspaper-style",
```

### Comparing `glow-0.12.2/PKG-INFO` & `glow-0.12.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glow
-Version: 0.12.2
+Version: 0.12.3
 Summary: Functional Python tools with a PyTorch flavour
 Project-URL: homepage, https://github.com/arquolo/glow
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Paul Maevskikh
@@ -59,15 +59,15 @@
 Requires-Dist: flake8-simplify; extra == 'dev-core'
 Requires-Dist: flake8~=6.0.0; extra == 'dev-core'
 Requires-Dist: isort; extra == 'dev-core'
 Requires-Dist: mypy~=1.1.1; extra == 'dev-core'
 Requires-Dist: pytest~=6.0; extra == 'dev-core'
 Requires-Dist: ruff; extra == 'dev-core'
 Requires-Dist: toml; python_version >= '3.11' and extra == 'dev-core'
-Requires-Dist: yapf[pyproject]==0.32.0; extra == 'dev-core'
+Requires-Dist: yapf[pyproject]==0.33.0; extra == 'dev-core'
 Provides-Extra: dev-wemake
 Requires-Dist: glow[dev-core]; extra == 'dev-wemake'
 Requires-Dist: wemake-python-styleguide~=0.15.0; extra == 'dev-wemake'
 Provides-Extra: io
 Requires-Dist: sounddevice; extra == 'io'
 Requires-Dist: soundfile; extra == 'io'
 Provides-Extra: memprof
```

